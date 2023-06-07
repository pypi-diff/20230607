# Comparing `tmp/defillamaAPI-0.0.1.tar.gz` & `tmp/defillamaAPI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defillamaAPI-0.0.1.tar", last modified: Tue May 30 15:45:58 2023, max compression
+gzip compressed data, was "defillamaAPI-0.0.2.tar", last modified: Wed Jun  7 13:38:31 2023, max compression
```

## Comparing `defillamaAPI-0.0.1.tar` & `defillamaAPI-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 15:45:58.945272 defillamaAPI-0.0.1/
--rw-rw-rw-   0        0        0      895 2023-05-30 15:45:58.944308 defillamaAPI-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-05-30 15:41:07.000000 defillamaAPI-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 15:45:58.928318 defillamaAPI-0.0.1/defillamaAPI/
--rw-rw-rw-   0        0        0       36 2023-05-30 15:31:20.000000 defillamaAPI-0.0.1/defillamaAPI/__init__.py
--rw-rw-rw-   0        0        0      294 2023-05-30 15:42:52.000000 defillamaAPI-0.0.1/defillamaAPI/__version__.py
--rw-rw-rw-   0        0        0     8514 2023-05-30 06:23:10.000000 defillamaAPI-0.0.1/defillamaAPI/defillamaAPI.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:45:58.942283 defillamaAPI-0.0.1/defillamaAPI.egg-info/
--rw-rw-rw-   0        0        0      895 2023-05-30 15:45:58.000000 defillamaAPI-0.0.1/defillamaAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-30 15:45:58.000000 defillamaAPI-0.0.1/defillamaAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 15:45:58.000000 defillamaAPI-0.0.1/defillamaAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-30 15:45:58.000000 defillamaAPI-0.0.1/defillamaAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-30 15:45:58.000000 defillamaAPI-0.0.1/defillamaAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      596 2023-05-30 15:41:34.000000 defillamaAPI-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 15:45:58.945272 defillamaAPI-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      944 2023-05-30 15:42:21.000000 defillamaAPI-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:38:31.285631 defillamaAPI-0.0.2/
+-rw-rw-rw-   0        0        0     1212 2023-06-07 13:38:31.284647 defillamaAPI-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2023-06-07 13:18:47.000000 defillamaAPI-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 13:38:31.273479 defillamaAPI-0.0.2/defillamaAPI/
+-rw-rw-rw-   0        0        0       36 2023-05-30 15:31:20.000000 defillamaAPI-0.0.2/defillamaAPI/__init__.py
+-rw-rw-rw-   0        0        0      294 2023-06-07 13:38:17.000000 defillamaAPI-0.0.2/defillamaAPI/__version__.py
+-rw-rw-rw-   0        0        0    20000 2023-06-07 13:18:31.000000 defillamaAPI-0.0.2/defillamaAPI/defillamaAPI.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:38:31.283633 defillamaAPI-0.0.2/defillamaAPI.egg-info/
+-rw-rw-rw-   0        0        0     1212 2023-06-07 13:38:31.000000 defillamaAPI-0.0.2/defillamaAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-06-07 13:38:31.000000 defillamaAPI-0.0.2/defillamaAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 13:38:31.000000 defillamaAPI-0.0.2/defillamaAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-07 13:38:31.000000 defillamaAPI-0.0.2/defillamaAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-07 13:38:31.000000 defillamaAPI-0.0.2/defillamaAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      596 2023-06-07 13:38:07.000000 defillamaAPI-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 13:38:31.285631 defillamaAPI-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      944 2023-05-30 15:42:21.000000 defillamaAPI-0.0.2/setup.py
```

### Comparing `defillamaAPI-0.0.1/PKG-INFO` & `defillamaAPI-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defillamaAPI
-Version: 0.0.1
+Version: 0.0.2
 Summary: defillama API Module
 Home-page: https://github.com/jafark92/defillamaAPI
 Author: Jafar Sadiq
 Author-email: Jafar Sadiq <jsadiqk92@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/jafark92/defillamaAPI
 Project-URL: Bug Tracker, https://github.com/jafark92/defillamaAPI/issues
@@ -12,13 +12,36 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # defillamaAPI
 Under Development
-API Collection of DefiLlama - Unofficial
+API Collection of DefiLlama (https://defillama.com/docs/api) - Unofficial
+
+### Installation:
+
+use pip to install:
+
+``` 
+pip install defillamaAPI
+```
+
+### Example usage:
+
+```
+from defillamaAPI import TVL
+
+# initialize TVL api client
+defillama_tvl = TVL()
+
+# Get all protocols data
+response = defillama_tvl.get_protocols()
+
+```
+
+-------
 
 Task ToDo
 -> Add remaining endpoints
 -> User can select if he wants pandas dataframe or just response json
 -> Test with other versions of python ( Although used only requests and time module with no fancy methods)
```

### Comparing `defillamaAPI-0.0.1/defillamaAPI.egg-info/PKG-INFO` & `defillamaAPI-0.0.2/defillamaAPI.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defillamaAPI
-Version: 0.0.1
+Version: 0.0.2
 Summary: defillama API Module
 Home-page: https://github.com/jafark92/defillamaAPI
 Author: Jafar Sadiq
 Author-email: Jafar Sadiq <jsadiqk92@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/jafark92/defillamaAPI
 Project-URL: Bug Tracker, https://github.com/jafark92/defillamaAPI/issues
@@ -12,13 +12,36 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # defillamaAPI
 Under Development
-API Collection of DefiLlama - Unofficial
+API Collection of DefiLlama (https://defillama.com/docs/api) - Unofficial
+
+### Installation:
+
+use pip to install:
+
+``` 
+pip install defillamaAPI
+```
+
+### Example usage:
+
+```
+from defillamaAPI import TVL
+
+# initialize TVL api client
+defillama_tvl = TVL()
+
+# Get all protocols data
+response = defillama_tvl.get_protocols()
+
+```
+
+-------
 
 Task ToDo
 -> Add remaining endpoints
 -> User can select if he wants pandas dataframe or just response json
 -> Test with other versions of python ( Although used only requests and time module with no fancy methods)
```

### Comparing `defillamaAPI-0.0.1/pyproject.toml` & `defillamaAPI-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "defillamaAPI"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jafar Sadiq", email="jsadiqk92@gmail.com" },
 ]
 description = "defillama API Module"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `defillamaAPI-0.0.1/setup.py` & `defillamaAPI-0.0.2/setup.py`

 * *Files identical despite different names*

