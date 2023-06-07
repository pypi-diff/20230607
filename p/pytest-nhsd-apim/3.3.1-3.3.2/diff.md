# Comparing `tmp/pytest-nhsd-apim-3.3.1.tar.gz` & `tmp/pytest-nhsd-apim-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-nhsd-apim-3.3.1.tar", last modified: Mon Mar  6 16:41:02 2023, max compression
+gzip compressed data, was "pytest-nhsd-apim-3.3.2.tar", last modified: Wed Jun  7 12:54:22 2023, max compression
```

## Comparing `pytest-nhsd-apim-3.3.1.tar` & `pytest-nhsd-apim-3.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:41:02.140924 pytest-nhsd-apim-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-03-06 16:41:02.140924 pytest-nhsd-apim-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-06 16:41:02.140924 pytest-nhsd-apim-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:41:02.128924 pytest-nhsd-apim-3.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:41:02.136924 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57430 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/apigee_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)    18675 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/apigee_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/auth_journey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20107 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/identity_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/nhsd_apim_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/pytest_nhsd_apim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/token_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:41:02.136924 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-03-06 16:41:02.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-06 16:41:02.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 16:41:02.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-06 16:41:02.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-06 16:41:02.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-06 16:41:02.000000 pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:41:02.140924 pytest-nhsd-apim-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/tests/test_apigee_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-06 16:40:15.000000 pytest-nhsd-apim-3.3.1/tests/test_nhsd_apim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:22.479457 pytest-nhsd-apim-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-07 12:54:22.479457 pytest-nhsd-apim-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 12:54:22.479457 pytest-nhsd-apim-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:22.475458 pytest-nhsd-apim-3.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:22.479457 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57430 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/apigee_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18675 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/apigee_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/auth_journey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/identity_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/nhsd_apim_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/pytest_nhsd_apim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/token_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:22.479457 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-07 12:54:22.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-07 12:54:22.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:54:22.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 12:54:22.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-07 12:54:22.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 12:54:22.000000 pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:54:22.479457 pytest-nhsd-apim-3.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/tests/test_apigee_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-07 12:53:51.000000 pytest-nhsd-apim-3.3.2/tests/test_nhsd_apim.py
```

### Comparing `pytest-nhsd-apim-3.3.1/PKG-INFO` & `pytest-nhsd-apim-3.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytest-nhsd-apim
-Version: 3.3.1
+Version: 3.3.2
 Summary: Pytest plugin accessing NHSDigital's APIM proxies
 Home-page: https://github.com/NHSDigital/pytest-nhsd-apim
-Author: Ben Strutt
-Author-email: ben.strutt1@nhs.net
-Maintainer: Ben Strutt
-Maintainer-email: ben.strutt1@nhs.net
+Author: Adrian Ciobanita
+Author-email: adrian.ciobanita1@nhs.net
+Maintainer: Alex Carrie
+Maintainer-email: alexander.carrie1@nhs.net
 License: MIT
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # pytest-nhsd-apim
```

### Comparing `pytest-nhsd-apim-3.3.1/README.md` & `pytest-nhsd-apim-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/pyproject.toml` & `pytest-nhsd-apim-3.3.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pytest-nhsd-apim"
-version = "3.3.1"
+version = "3.3.2"
 description = "Pytest plugin accessing NHSDigital's APIM proxies"
-authors = ["Ben Strutt <ben.strutt1@nhs.net>", "Adrian Ciobanita <adrian.ciobanita1@nhs.net>", "Alex Carrie <alexander.carrie1@nhs.net>", "Lucas Fantini <lucas.fantini@nhs.net>"]
-maintainers = ["Ben Strutt <ben.strutt1@nhs.net>", "Alex Carrie <alexander.carrie1@nhs.net>"]
+authors = ["Adrian Ciobanita <adrian.ciobanita1@nhs.net>", "Alex Carrie <alexander.carrie1@nhs.net>", "Lucas Fantini <lucas.fantini@nhs.net>"]
+maintainers = ["Alex Carrie <alexander.carrie1@nhs.net>", "Alex Hawdon <alex.hawdon1@nhs.net"]
 readme = "README.md"
 repository = "https://github.com/NHSDigital/pytest-nhsd-apim"
 classifiers = ["Framework :: Pytest"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 Authlib = "^0.15.5"
```

### Comparing `pytest-nhsd-apim-3.3.1/setup.py` & `pytest-nhsd-apim-3.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/apigee_apis.py` & `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/apigee_apis.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/apigee_edge.py` & `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/apigee_edge.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/auth_journey.py` & `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/auth_journey.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/config.py` & `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/config.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/identity_service.py` & `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/identity_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         "Api-producers",  # just in case u want to get a cheeky token for proxygen ;)
     ]
 
     @property
     def keycloak_url(self):
         prefix = "https://"
         host = "identity.ptl.api.platform.nhs.uk"
-        path = f"/auth/realms/{self.realm}/protocol/openid-connect"
+        path = f"/realms/{self.realm}/protocol/openid-connect"
         return f"{prefix}{host}{path}"
 
 
 class KeycloakUserConfig(KeycloakConfig):
     client_id: str
     client_secret: str
     redirect_uri: HttpUrl = "https://example.org"
```

### Comparing `pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/log.py` & `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/log.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/nhsd_apim_authorization.py` & `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/nhsd_apim_authorization.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/pytest_nhsd_apim.py` & `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/pytest_nhsd_apim.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/secrets.py` & `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/secrets.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim/token_cache.py` & `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim/token_cache.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim.egg-info/PKG-INFO` & `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytest-nhsd-apim
-Version: 3.3.1
+Version: 3.3.2
 Summary: Pytest plugin accessing NHSDigital's APIM proxies
 Home-page: https://github.com/NHSDigital/pytest-nhsd-apim
-Author: Ben Strutt
-Author-email: ben.strutt1@nhs.net
-Maintainer: Ben Strutt
-Maintainer-email: ben.strutt1@nhs.net
+Author: Adrian Ciobanita
+Author-email: adrian.ciobanita1@nhs.net
+Maintainer: Alex Carrie
+Maintainer-email: alexander.carrie1@nhs.net
 License: MIT
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # pytest-nhsd-apim
```

### Comparing `pytest-nhsd-apim-3.3.1/src/pytest_nhsd_apim.egg-info/SOURCES.txt` & `pytest-nhsd-apim-3.3.2/src/pytest_nhsd_apim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/tests/test_apigee_apis.py` & `pytest-nhsd-apim-3.3.2/tests/test_apigee_apis.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/tests/test_examples.py` & `pytest-nhsd-apim-3.3.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.1/tests/test_nhsd_apim.py` & `pytest-nhsd-apim-3.3.2/tests/test_nhsd_apim.py`

 * *Files identical despite different names*

