# Comparing `tmp/chaind-0.3.2.tar.gz` & `tmp/chaind-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaind-0.3.2.tar", last modified: Mon Nov 14 08:13:58 2022, max compression
+gzip compressed data, was "dist/chaind-0.4.0.tar", last modified: Wed Jun  7 09:16:23 2023, max compression
```

## Comparing `chaind-0.3.2.tar` & `chaind-0.4.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:13:58.893294 chaind-0.3.2/
--rw-r--r--   0 lash      (1000) lash      (1000)      959 2022-11-14 07:37:49.000000 chaind-0.3.2/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:32:58.000000 chaind-0.3.2/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      111 2022-11-14 07:35:56.000000 chaind-0.3.2/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      754 2022-11-14 08:13:58.893294 chaind-0.3.2/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      866 2022-11-14 07:35:04.000000 chaind-0.3.2/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1621 2022-11-14 07:35:41.000000 chaind-0.3.2/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:13:58.889960 chaind-0.3.2/chaind/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:13:58.893294 chaind-0.3.2/chaind/adapters/
--rw-r--r--   0 lash      (1000) lash      (1000)      921 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/adapters/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5198 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/adapters/fs.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:13:58.893294 chaind-0.3.2/chaind/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      666 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)      290 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/cli/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      725 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/cli/config.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:13:58.893294 chaind-0.3.2/chaind/data/
--rw-r--r--   0 lash      (1000) lash      (1000)      132 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/data/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:13:58.893294 chaind-0.3.2/chaind/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       56 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/data/config/config.ini
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:13:58.893294 chaind-0.3.2/chaind/data/config/syncer/
--rw-r--r--   0 lash      (1000) lash      (1000)       62 2021-07-20 14:57:40.000000 chaind-0.3.2/chaind/data/config/syncer/config.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       17 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/data/config/token.ini
--rw-r--r--   0 lash      (1000) lash      (1000)      887 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/dispatch.py
--rw-r--r--   0 lash      (1000) lash      (1000)      928 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/driver.py
--rw-r--r--   0 lash      (1000) lash      (1000)      317 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4151 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/filter.py
--rw-r--r--   0 lash      (1000) lash      (1000)      778 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/lock.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3664 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/session.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3812 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/settings.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:13:58.893294 chaind-0.3.2/chaind/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)     1129 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/unittest/common.py
--rw-r--r--   0 lash      (1000) lash      (1000)      796 2022-10-13 11:40:08.000000 chaind-0.3.2/chaind/unittest/fs.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:13:58.893294 chaind-0.3.2/chaind.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      754 2022-11-14 08:13:58.000000 chaind-0.3.2/chaind.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      663 2022-11-14 08:13:58.000000 chaind-0.3.2/chaind.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2022-11-14 08:13:58.000000 chaind-0.3.2/chaind.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      317 2022-11-14 08:13:58.000000 chaind-0.3.2/chaind.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        7 2022-11-14 08:13:58.000000 chaind-0.3.2/chaind.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       93 2022-10-13 11:40:08.000000 chaind-0.3.2/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      806 2022-11-14 08:13:58.893294 chaind-0.3.2/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      745 2021-06-03 10:04:22.000000 chaind-0.3.2/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-06-03 10:04:33.000000 chaind-0.3.2/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-07 09:16:23.883323 chaind-0.4.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1008 2023-06-07 09:15:39.000000 chaind-0.4.0/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:32:58.000000 chaind-0.4.0/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      111 2022-11-14 07:35:56.000000 chaind-0.4.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      686 2023-06-07 09:16:23.883323 chaind-0.4.0/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      866 2022-11-14 07:35:04.000000 chaind-0.4.0/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1621 2022-11-14 07:35:41.000000 chaind-0.4.0/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-07 09:16:23.879990 chaind-0.4.0/chaind/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-07 09:16:23.879990 chaind-0.4.0/chaind/adapters/
+-rw-r--r--   0 lash      (1000) lash      (1000)      921 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/adapters/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5198 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/adapters/fs.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-07 09:16:23.879990 chaind-0.4.0/chaind/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      666 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      290 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/cli/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      725 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/cli/config.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-07 09:16:23.883323 chaind-0.4.0/chaind/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)      132 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/data/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-07 09:16:23.883323 chaind-0.4.0/chaind/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       56 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/data/config/config.ini
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-07 09:16:23.883323 chaind-0.4.0/chaind/data/config/syncer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       62 2021-07-20 14:57:40.000000 chaind-0.4.0/chaind/data/config/syncer/config.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       17 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/data/config/token.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)      887 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/dispatch.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      928 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/driver.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      317 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4151 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/filter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      778 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/lock.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3664 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/session.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3812 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/settings.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-07 09:16:23.883323 chaind-0.4.0/chaind/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1129 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/unittest/common.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      796 2022-10-13 11:40:08.000000 chaind-0.4.0/chaind/unittest/fs.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-07 09:16:23.879990 chaind-0.4.0/chaind.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      686 2023-06-07 09:16:23.000000 chaind-0.4.0/chaind.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      680 2023-06-07 09:16:23.000000 chaind-0.4.0/chaind.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-07 09:16:23.000000 chaind-0.4.0/chaind.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      320 2023-06-07 09:16:23.000000 chaind-0.4.0/chaind.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-06-07 09:16:23.000000 chaind-0.4.0/chaind.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       94 2023-06-07 08:52:13.000000 chaind-0.4.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      738 2023-06-07 09:16:23.883323 chaind-0.4.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      745 2021-06-03 10:04:22.000000 chaind-0.4.0/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-06-03 10:04:33.000000 chaind-0.4.0/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-07 09:16:23.883323 chaind-0.4.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2721 2022-10-13 11:40:08.000000 chaind-0.4.0/tests/test_fs.py
```

### Comparing `chaind-0.3.2/CHANGELOG` & `chaind-0.4.0/CHANGELOG`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+- 0.4.0
+	* Upgrade dependencies (chainlib 0.4.x)
 - 0.3.1
 	* Change license to AGPL3 and copyright waived to public domain
 - 0.3.0
 	* Implement on chainlib 0.3.0
 - 0.2.12
 	* Breaking upgrade of chainlib.
 	* Implement generic block and tx.
```

### Comparing `chaind-0.3.2/LICENSE` & `chaind-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/PKG-INFO` & `chaind-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: chaind
-Version: 0.3.2
+Version: 0.4.0
 Summary: Base package for chain queue service
-Home-page: https://git.defalsify.org/chaind.eth
+Home-page: https://git.defalsify.org/chaind
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
-License: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+License: AGPLv3+
 Keywords: blockchain,cryptocurrency,dlt
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: postgres
 Provides-Extra: sqlite
 License-File: LICENSE
```

### Comparing `chaind-0.3.2/WAIVER` & `chaind-0.4.0/WAIVER`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/WAIVER.asc` & `chaind-0.4.0/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/adapters/base.py` & `chaind-0.4.0/chaind/adapters/base.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/adapters/fs.py` & `chaind-0.4.0/chaind/adapters/fs.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/cli/arg.py` & `chaind-0.4.0/chaind/cli/arg.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/cli/config.py` & `chaind-0.4.0/chaind/cli/config.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/dispatch.py` & `chaind-0.4.0/chaind/dispatch.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/driver.py` & `chaind-0.4.0/chaind/driver.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/filter.py` & `chaind-0.4.0/chaind/filter.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/lock.py` & `chaind-0.4.0/chaind/lock.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/session.py` & `chaind-0.4.0/chaind/session.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/settings.py` & `chaind-0.4.0/chaind/settings.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/setup.py` & `chaind-0.4.0/chaind/setup.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/unittest/common.py` & `chaind-0.4.0/chaind/unittest/common.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind/unittest/fs.py` & `chaind-0.4.0/chaind/unittest/fs.py`

 * *Files identical despite different names*

### Comparing `chaind-0.3.2/chaind.egg-info/PKG-INFO` & `chaind-0.4.0/chaind.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: chaind
-Version: 0.3.2
+Version: 0.4.0
 Summary: Base package for chain queue service
-Home-page: https://git.defalsify.org/chaind.eth
+Home-page: https://git.defalsify.org/chaind
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
-License: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+License: AGPLv3+
 Keywords: blockchain,cryptocurrency,dlt
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: postgres
 Provides-Extra: sqlite
 License-File: LICENSE
```

### Comparing `chaind-0.3.2/chaind.egg-info/SOURCES.txt` & `chaind-0.4.0/chaind.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -26,8 +26,9 @@
 chaind/cli/base.py
 chaind/cli/config.py
 chaind/data/__init__.py
 chaind/data/config/config.ini
 chaind/data/config/token.ini
 chaind/data/config/syncer/config.ini
 chaind/unittest/common.py
-chaind/unittest/fs.py
+chaind/unittest/fs.py
+tests/test_fs.py
```

### Comparing `chaind-0.3.2/setup.cfg` & `chaind-0.4.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [metadata]
 name = chaind
-version = 0.3.2
+version = 0.4.0
 description = Base package for chain queue service
 author = Louis Holbrook
 author_email = dev@holbrook.no
-url = https://git.defalsify.org/chaind.eth
+url = https://git.defalsify.org/chaind
 keywords = 
 	blockchain
 	cryptocurrency
 	dlt
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 	Topic :: Internet
-license = OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+license = AGPLv3+
 licence_files = 
 	LICENSE
 
 [options]
-python_requires = >= 3.7
+python_requires = >= 3.8
 include_package_data = True
 packages = 
 	chaind
 	chaind.adapters
 	chaind.unittest
 	chaind.data
 	chaind.cli
```

### Comparing `chaind-0.3.2/setup.py` & `chaind-0.4.0/setup.py`

 * *Files identical despite different names*

