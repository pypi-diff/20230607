# Comparing `tmp/forevd-0.1.6.tar.gz` & `tmp/forevd-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forevd-0.1.6.tar", max compression
+gzip compressed data, was "forevd-0.1.7.tar", max compression
```

## Comparing `forevd-0.1.6.tar` & `forevd-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-01 11:18:49.906961 forevd-0.1.6/LICENSE
--rw-r--r--   0        0        0     4063 2023-06-01 11:18:49.906961 forevd-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/__init__.py
--rw-r--r--   0        0        0     5214 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/__main__.py
--rw-r--r--   0        0        0     1543 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/apache/__init__.py
--rw-r--r--   0        0        0     4461 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/apache/httpd.conf
--rw-r--r--   0        0        0      216 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/app.py
--rw-r--r--   0        0        0        0 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/resources/logging/__init__.py
--rw-r--r--   0        0        0      387 2023-06-01 11:18:49.906961 forevd-0.1.6/forevd/resources/logging/cli.conf
--rw-r--r--   0        0        0      884 2023-06-01 11:18:49.906961 forevd-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4768 1970-01-01 00:00:00.000000 forevd-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-06 22:07:52.728894 forevd-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4065 2023-06-06 22:07:52.732894 forevd-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/__init__.py
+-rw-r--r--   0        0        0     5879 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/__main__.py
+-rw-r--r--   0        0        0     1543 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/apache/__init__.py
+-rw-r--r--   0        0        0     4779 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/apache/httpd.conf
+-rw-r--r--   0        0        0      216 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/app.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/resources/logging/__init__.py
+-rw-r--r--   0        0        0      387 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/resources/logging/cli.conf
+-rw-r--r--   0        0        0      884 2023-06-06 22:07:52.732894 forevd-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4770 1970-01-01 00:00:00.000000 forevd-0.1.7/PKG-INFO
```

### Comparing `forevd-0.1.6/LICENSE` & `forevd-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `forevd-0.1.6/README.md` & `forevd-0.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 format of the file is a dictionary of locations, or endpoints, and their correspondign data.
 
 #### Example
 
 The following adds LDAP group **and** static user authorization to `/`
 
 ```yaml
-/:
+- path: /
   authz:
     join_type: "any"
     ldap:
       url: "ldaps://127.0.0.1/DC=foo,DC=example,DC=com"
       bind-dn: "foo"
       bind-pw: "{{ LDAP_BINDID_PASSWORD }}"
       groups:
@@ -103,16 +103,16 @@
 CacheTTL: 600
 OpCacheEntries: 1024
 OpCacheTTL: 600
 ```
 
 ## Mutual TLS
 
-The following command provides termination of mTLS on `/` and redirects connections to a backend at
-`http://localhost:8081`
+The following command provides termination of mTLS on `/` and passes connections to a backend at
+`http://0.0.0.0:8080`
 
 ```
 forevd --debug --listen 0.0.0.0:8080 \
     --ca-cert $PWD/../certs/ca/ca-cert.pem
     --cert $PWD/../certs/server.crt
     --cert-key $PWD/../certs/server.key
     --backend http://localhost:8081
```

### Comparing `forevd-0.1.6/forevd/__main__.py` & `forevd-0.1.7/forevd/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,35 +25,53 @@
     cli.init_logging("forevd.resources.logging", "cli.conf")
 
     if debug:
         logging.getLogger().setLevel(logging.DEBUG)
         logging.getLogger("forevd").setLevel(logging.DEBUG)
 
 
+def _get_loc_by_path(locations, path):
+    for config in locations:
+        if "path" not in config:
+            raise click.UsageError("Locations must contain a path")
+        if config["path"] == path:
+            return config
+
+    return None
+
+
 def _nomalize_locations(
     locations: dict, backend: str, location: str, mtls: bool, http_methods: list
 ):
     if not locations:
-        locations = {}
+        locations = []
 
-    endpoints = list(locations.keys())
-    if location:
-        endpoints.insert(0, location)
+    endpoints = [conf["path"] for conf in locations]
+
+    missing_cli_loc = False
+    if location and location not in endpoints:
+        endpoints.append(location)
+        missing_cli_loc = True
     _LOGGER.debug(f"endpoints: {endpoints}")
 
     for endpoint in endpoints:
-        config = locations[endpoint]
+        config = _get_loc_by_path(locations, endpoint)
+        if not config:
+            config = {"path": endpoint}
+
         if "backend" not in config:
             config["backend"] = backend
         if "mtls" not in config:
             config["mtls"] = mtls
         if "http_methods" not in config:
             config["http_methods"] = http_methods
 
-        locations[endpoint] = config
+        if missing_cli_loc:
+            locations.append(config)
+
     _LOGGER.debug(f"locations: {locations}")
 
     return locations
 
 
 @click.command()
 @click.option(
@@ -112,14 +130,19 @@
 )
 @click.option(
     "--http-methods",
     help="Restrict HTTP method calls for the supplied list ",
     type=cli.StrList,
 )
 @click.option(
+    "--httpd-include",
+    help="Add your own config from a file into the generated httpd.conf",
+    type=cli.FromJsonOrYaml(),
+)
+@click.option(
     "--ldap",
     help="Provide the LDAP config in a JSON or YAML string or file",
     type=cli.FromJsonOrYaml(),
 )
 @click.option(
     "--listen",
     help="The IP/hostname and port to listen on",
@@ -167,14 +190,15 @@
     cert,
     cert_key,
     cmd,
     debug,
     err_log,
     do_exec,
     http_methods,
+    httpd_include,
     ldap,
     listen,
     location,
     locations,
     mtls,
     oidc,
     server_name,
@@ -191,14 +215,15 @@
 
     config = {
         "err_log": err_log,
         "access_log": access_log,
         "ca_cert": ca_cert,
         "cert": cert,
         "cert_key": cert_key,
+        "httpd_include": httpd_include,
         "debug": debug,
         "ldap": ldap,
         "locations": _nomalize_locations(locations, backend, location, mtls, http_methods),
         "listen": listen,
         "oidc": oidc,
         "server_name": server_name,
     }
```

### Comparing `forevd-0.1.6/forevd/apache/__init__.py` & `forevd-0.1.7/forevd/apache/__init__.py`

 * *Files identical despite different names*

### Comparing `forevd-0.1.6/forevd/apache/httpd.conf` & `forevd-0.1.7/forevd/apache/httpd.conf`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 LoadModule ssl_module modules/mod_ssl.so
 LoadModule socache_shmcb_module modules/mod_socache_shmcb.so
 {% endif %}
 {% if oidc -%}
 LoadModule authz_user_module modules/mod_authz_user.so
 LoadModule auth_openidc_module modules/mod_auth_openidc.so
 {% endif %}
+{% if httpd_include -%}
+{{ httpd_include }}
+{% endif %}
 
 ServerName {{ server_name }}
 Listen {{ listen }}
 
 UseCanonicalName On
 
 Timeout 10
@@ -79,16 +82,16 @@
 
 {% if ldap -%}
 {% for key, value in ldap.items()  -%}
 LDAP{{ key }} {{ value }}
 {% endfor %}
 {% endif -%}
 
-{% for path in locations -%}
-{% set location = locations[path] -%}
+{% for location in locations -%}
+{% set path = location["path"] -%}
 {% set authz = location.get("authz", {}) -%}
 
 {# Setup the required users #}
 {% if authz -%}
     {% set authz_required_users = [] -%}
     {% if "users" in authz -%}
         {% set users = authz["users"]|join(" ") -%}
@@ -111,15 +114,19 @@
         {% do authz_required_users.insert(0, "<RequireAll>") %}
         {% do authz_required_users.append("</RequireAll>") %}
     {% endif -%}
 
     {% set required_users = authz_required_users|join("\n       ") -%}
 {% endif %}
 
-<Location "{{ path }}">
+<Location{% if "match" in location %}Match{% endif %} "{{ path }}">
+    {% if "include" in location -%}
+    {{ location["include"] }}
+    {% endif -%}
+
     ProxyPass {{ location["backend"] }}
     ProxyPassReverse {{ location["backend"] }}
 
     {% if "mtls" in location %}
     SSLOptions +StdEnvVars
     SSLUserName SSL_CLIENT_S_DN_CN
     SSLVerifyCLient {{ location["mtls"] }}
@@ -127,14 +134,15 @@
     RequestHeader set X-Remote-User %{SSL_CLIENT_S_DN_CN}e
     RequestHeader set X-SSL-certificate "%{SSL_CLIENT_CERT}s" "expr=-n %{SSL_CLIENT_CERT}"
     {% endif %}
 
     {% if oidc -%}
     AuthType openid-connect
     RequestHeader set X-Remote-User %{REMOTE_USER}s "expr=-n %{REMOTE_USER}"
+    RequestHeader set Authorization "Bearer %{OIDC_access_token}e" env=OIDC_access_token
     {% endif %}
 
     {% if "ldap" in location["authz"] -%}
     AuthLDAPURL {{ location["authz"]["ldap"]["url"] }}
     AuthLDAPBindDN {{ location["authz"]["ldap"]["bind-dn"] }}
     AuthLDAPBindPassword {{ location["authz"]["ldap"]["bind-pw"] }}
     {% endif %}
@@ -142,9 +150,9 @@
     {% if not location["http_methods"] %}
     {{ required_users }}
     {% else -%}
     <Limit {{ location["http_methods"]|join(" ") }}>
         {{ required_users }}
     </Limit>
     {% endif %}
-</Location>
+</Location{% if "match" in location %}Match{% endif %}>
 {% endfor %}
```

### Comparing `forevd-0.1.6/pyproject.toml` & `forevd-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "forevd"
-version = "0.1.6"
-description = "Forward and reverse proxy using nginx or apache"
+version = "0.1.7"
+description = "Forward and reverse proxy using apache or nginx"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Jinja2 = "^3.1.2"
```

### Comparing `forevd-0.1.6/PKG-INFO` & `forevd-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: forevd
-Version: 0.1.6
-Summary: Forward and reverse proxy using nginx or apache
+Version: 0.1.7
+Summary: Forward and reverse proxy using apache or nginx
 License: LICENSE
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -67,15 +67,15 @@
 format of the file is a dictionary of locations, or endpoints, and their correspondign data.
 
 #### Example
 
 The following adds LDAP group **and** static user authorization to `/`
 
 ```yaml
-/:
+- path: /
   authz:
     join_type: "any"
     ldap:
       url: "ldaps://127.0.0.1/DC=foo,DC=example,DC=com"
       bind-dn: "foo"
       bind-pw: "{{ LDAP_BINDID_PASSWORD }}"
       groups:
@@ -123,16 +123,16 @@
 CacheTTL: 600
 OpCacheEntries: 1024
 OpCacheTTL: 600
 ```
 
 ## Mutual TLS
 
-The following command provides termination of mTLS on `/` and redirects connections to a backend at
-`http://localhost:8081`
+The following command provides termination of mTLS on `/` and passes connections to a backend at
+`http://0.0.0.0:8080`
 
 ```
 forevd --debug --listen 0.0.0.0:8080 \
     --ca-cert $PWD/../certs/ca/ca-cert.pem
     --cert $PWD/../certs/server.crt
     --cert-key $PWD/../certs/server.key
     --backend http://localhost:8081
```

