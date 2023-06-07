# Comparing `tmp/perun.proxy.utils-1.2.0.tar.gz` & `tmp/perun.proxy.utils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.proxy.utils-1.2.0.tar", last modified: Tue Jun  6 15:17:46 2023, max compression
+gzip compressed data, was "perun.proxy.utils-1.3.0.tar", last modified: Wed Jun  7 05:35:58 2023, max compression
```

## Comparing `perun.proxy.utils-1.2.0.tar` & `perun.proxy.utils-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:46.812100 perun.proxy.utils-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-06-05 07:54:03.000000 perun.proxy.utils-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-06 15:17:46.812100 perun.proxy.utils-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2273 2023-06-05 07:54:03.000000 perun.proxy.utils-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:46.708098 perun.proxy.utils-1.2.0/perun/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:46.708098 perun.proxy.utils-1.2.0/perun/proxy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:46.744098 perun.proxy.utils-1.2.0/perun/proxy/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 07:54:03.000000 perun.proxy.utils-1.2.0/perun/proxy/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-06-05 07:54:03.000000 perun.proxy.utils-1.2.0/perun/proxy/utils/metadata_expiration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:46.812100 perun.proxy.utils-1.2.0/perun/proxy/utils/nagios/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 07:54:03.000000 perun.proxy.utils-1.2.0/perun/proxy/utils/nagios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      709 2023-06-06 15:09:34.000000 perun.proxy.utils-1.2.0/perun/proxy/utils/nagios/check_custom_command.py
--rw-rw-rw-   0 root         (0) root         (0)    72133 2023-06-05 07:54:03.000000 perun.proxy.utils-1.2.0/perun/proxy/utils/nagios/check_mongodb.py
--rw-rw-rw-   0 root         (0) root         (0)     1758 2023-06-06 15:06:39.000000 perun.proxy.utils-1.2.0/perun/proxy/utils/nagios/check_rpc_status.py
--rwxrwxrwx   0 root         (0) root         (0)    18134 2023-06-05 07:54:03.000000 perun.proxy.utils-1.2.0/perun/proxy/utils/nagios/check_saml.py
--rw-rw-rw-   0 root         (0) root         (0)     3193 2023-06-05 07:54:03.000000 perun.proxy.utils-1.2.0/perun/proxy/utils/nagios/check_user_logins.py
--rwxrwxrwx   0 root         (0) root         (0)     2322 2023-06-05 07:54:03.000000 perun.proxy.utils-1.2.0/perun/proxy/utils/print_docker_versions.py
--rw-rw-rw-   0 root         (0) root         (0)     3038 2023-06-05 07:54:03.000000 perun.proxy.utils-1.2.0/perun/proxy/utils/run_version_script.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-05 07:54:03.000000 perun.proxy.utils-1.2.0/perun/proxy/utils/separate_oidc_logs.py
--rwxrwxrwx   0 root         (0) root         (0)     2238 2023-06-05 07:54:03.000000 perun.proxy.utils-1.2.0/perun/proxy/utils/separate_ssp_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:46.744098 perun.proxy.utils-1.2.0/perun.proxy.utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-06 15:17:46.000000 perun.proxy.utils-1.2.0/perun.proxy.utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      731 2023-06-06 15:17:46.000000 perun.proxy.utils-1.2.0/perun.proxy.utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 15:17:46.000000 perun.proxy.utils-1.2.0/perun.proxy.utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-06-06 15:17:46.000000 perun.proxy.utils-1.2.0/perun.proxy.utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-06 15:17:46.000000 perun.proxy.utils-1.2.0/perun.proxy.utils.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-06 15:17:46.812100 perun.proxy.utils-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-06-06 15:06:39.000000 perun.proxy.utils-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 05:35:58.356145 perun.proxy.utils-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-06-05 07:53:45.000000 perun.proxy.utils-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-07 05:35:58.356145 perun.proxy.utils-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2273 2023-06-05 07:53:45.000000 perun.proxy.utils-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 05:35:58.240142 perun.proxy.utils-1.3.0/perun/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 05:35:58.240142 perun.proxy.utils-1.3.0/perun/proxy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 05:35:58.296144 perun.proxy.utils-1.3.0/perun/proxy/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 07:53:45.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-06-05 07:53:45.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/metadata_expiration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 05:35:58.352145 perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 07:53:45.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-06-07 05:08:08.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/check_custom_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     2436 2023-06-07 05:08:08.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/check_ldap.py
+-rw-rw-rw-   0 root         (0) root         (0)    72133 2023-06-05 07:53:45.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/check_mongodb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1758 2023-06-06 15:06:34.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/check_rpc_status.py
+-rwxrwxrwx   0 root         (0) root         (0)    18134 2023-06-05 07:53:45.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/check_saml.py
+-rw-rw-rw-   0 root         (0) root         (0)     3193 2023-06-05 07:53:45.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/check_user_logins.py
+-rwxrwxrwx   0 root         (0) root         (0)     2322 2023-06-05 07:53:45.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/print_docker_versions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3038 2023-06-05 07:53:45.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/run_version_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-05 07:53:45.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/separate_oidc_logs.py
+-rwxrwxrwx   0 root         (0) root         (0)     2238 2023-06-05 07:53:45.000000 perun.proxy.utils-1.3.0/perun/proxy/utils/separate_ssp_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 05:35:58.260143 perun.proxy.utils-1.3.0/perun.proxy.utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-07 05:35:58.000000 perun.proxy.utils-1.3.0/perun.proxy.utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      770 2023-06-07 05:35:58.000000 perun.proxy.utils-1.3.0/perun.proxy.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 05:35:58.000000 perun.proxy.utils-1.3.0/perun.proxy.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-07 05:35:58.000000 perun.proxy.utils-1.3.0/perun.proxy.utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-07 05:35:58.000000 perun.proxy.utils-1.3.0/perun.proxy.utils.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-07 05:35:58.356145 perun.proxy.utils-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-06-07 05:08:08.000000 perun.proxy.utils-1.3.0/setup.py
```

### Comparing `perun.proxy.utils-1.2.0/LICENSE` & `perun.proxy.utils-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.2.0/README.md` & `perun.proxy.utils-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.2.0/perun/proxy/utils/nagios/check_custom_command.py` & `perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/check_custom_command.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.2.0/perun/proxy/utils/nagios/check_mongodb.py` & `perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/check_mongodb.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.2.0/perun/proxy/utils/nagios/check_rpc_status.py` & `perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/check_rpc_status.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.2.0/perun/proxy/utils/nagios/check_saml.py` & `perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/check_saml.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.2.0/perun/proxy/utils/nagios/check_user_logins.py` & `perun.proxy.utils-1.3.0/perun/proxy/utils/nagios/check_user_logins.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.2.0/perun/proxy/utils/print_docker_versions.py` & `perun.proxy.utils-1.3.0/perun/proxy/utils/print_docker_versions.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.2.0/perun/proxy/utils/run_version_script.py` & `perun.proxy.utils-1.3.0/perun/proxy/utils/run_version_script.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.2.0/perun/proxy/utils/separate_oidc_logs.py` & `perun.proxy.utils-1.3.0/perun/proxy/utils/separate_oidc_logs.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.2.0/perun/proxy/utils/separate_ssp_logs.py` & `perun.proxy.utils-1.3.0/perun/proxy/utils/separate_ssp_logs.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.2.0/perun.proxy.utils.egg-info/SOURCES.txt` & `perun.proxy.utils-1.3.0/perun.proxy.utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,11 +11,12 @@
 perun/proxy/utils/metadata_expiration.py
 perun/proxy/utils/print_docker_versions.py
 perun/proxy/utils/run_version_script.py
 perun/proxy/utils/separate_oidc_logs.py
 perun/proxy/utils/separate_ssp_logs.py
 perun/proxy/utils/nagios/__init__.py
 perun/proxy/utils/nagios/check_custom_command.py
+perun/proxy/utils/nagios/check_ldap.py
 perun/proxy/utils/nagios/check_mongodb.py
 perun/proxy/utils/nagios/check_rpc_status.py
 perun/proxy/utils/nagios/check_saml.py
 perun/proxy/utils/nagios/check_user_logins.py
```

### Comparing `perun.proxy.utils-1.2.0/setup.py` & `perun.proxy.utils-1.3.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,9 +10,10 @@
     install_requires=[
         "setuptools",
         "pymongo~=4.3",
         "asyncssh~=2.13",
         "docker~=6.0",
         "beautifulsoup4~=4.12",
         "requests~=2.31",
+        "ldap3~=2.9.1",
     ],
 )
```

