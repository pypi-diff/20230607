# Comparing `tmp/py-geth-3.9.0.tar.gz` & `tmp/py-geth-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-geth-3.9.0.tar", last modified: Wed Aug 24 20:06:57 2022, max compression
+gzip compressed data, was "py-geth-3.9.1.tar", last modified: Wed Aug 24 21:00:19 2022, max compression
```

## Comparing `py-geth-3.9.0.tar` & `py-geth-3.9.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2022-08-24 20:06:57.987802 py-geth-3.9.0/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1080 2022-08-24 16:53:40.000000 py-geth-3.9.0/LICENSE
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      189 2022-08-24 16:53:40.000000 py-geth-3.9.0/MANIFEST.in
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7444 2022-08-24 20:06:57.983802 py-geth-3.9.0/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6619 2022-08-24 19:58:52.000000 py-geth-3.9.0/README.md
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2022-08-24 20:06:57.979802 py-geth-3.9.0/geth/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      440 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4285 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/accounts.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4036 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/chain.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       30 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/default_blockchain_password
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1016 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/exceptions.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      412 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/genesis.json
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    14165 2022-08-24 19:58:52.000000 py-geth-3.9.0/geth/install.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      999 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/main.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4697 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/mixins.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7589 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/process.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2105 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/reset.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2022-08-24 20:06:57.983802 py-geth-3.9.0/geth/utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/utils/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1349 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/utils/dag.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1340 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/utils/encoding.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1465 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/utils/filesystem.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1298 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/utils/networking.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1620 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/utils/proc.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      219 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/utils/thread.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1758 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/utils/timeout.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     8739 2022-08-24 16:53:40.000000 py-geth-3.9.0/geth/wrapper.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2022-08-24 20:06:57.983802 py-geth-3.9.0/py_geth.egg-info/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7444 2022-08-24 20:06:57.000000 py-geth-3.9.0/py_geth.egg-info/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      606 2022-08-24 20:06:57.000000 py-geth-3.9.0/py_geth.egg-info/SOURCES.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2022-08-24 20:06:57.000000 py-geth-3.9.0/py_geth.egg-info/dependency_links.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2022-08-24 20:06:57.000000 py-geth-3.9.0/py_geth.egg-info/not-zip-safe
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      263 2022-08-24 20:06:57.000000 py-geth-3.9.0/py_geth.egg-info/requires.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        5 2022-08-24 20:06:57.000000 py-geth-3.9.0/py_geth.egg-info/top_level.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2022-08-24 20:06:57.987802 py-geth-3.9.0/setup.cfg
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1749 2022-08-24 20:06:51.000000 py-geth-3.9.0/setup.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2022-08-24 21:00:19.306515 py-geth-3.9.1/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1080 2022-08-24 16:53:40.000000 py-geth-3.9.1/LICENSE
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      189 2022-08-24 16:53:40.000000 py-geth-3.9.1/MANIFEST.in
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7444 2022-08-24 21:00:19.306515 py-geth-3.9.1/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6619 2022-08-24 19:58:52.000000 py-geth-3.9.1/README.md
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2022-08-24 21:00:19.302515 py-geth-3.9.1/geth/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      440 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4285 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/accounts.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4036 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/chain.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       30 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/default_blockchain_password
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1016 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/exceptions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      412 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/genesis.json
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    14165 2022-08-24 19:58:52.000000 py-geth-3.9.1/geth/install.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      999 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/main.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4697 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/mixins.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7589 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/process.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2105 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/reset.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2022-08-24 21:00:19.302515 py-geth-3.9.1/geth/utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/utils/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1349 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/utils/dag.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1340 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/utils/encoding.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1465 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/utils/filesystem.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1298 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/utils/networking.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1620 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/utils/proc.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      219 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/utils/thread.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1758 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/utils/timeout.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     8739 2022-08-24 16:53:40.000000 py-geth-3.9.1/geth/wrapper.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2022-08-24 21:00:19.306515 py-geth-3.9.1/py_geth.egg-info/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7444 2022-08-24 21:00:18.000000 py-geth-3.9.1/py_geth.egg-info/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      606 2022-08-24 21:00:18.000000 py-geth-3.9.1/py_geth.egg-info/SOURCES.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2022-08-24 21:00:18.000000 py-geth-3.9.1/py_geth.egg-info/dependency_links.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2022-08-24 21:00:18.000000 py-geth-3.9.1/py_geth.egg-info/not-zip-safe
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      263 2022-08-24 21:00:18.000000 py-geth-3.9.1/py_geth.egg-info/requires.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        5 2022-08-24 21:00:18.000000 py-geth-3.9.1/py_geth.egg-info/top_level.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2022-08-24 21:00:19.306515 py-geth-3.9.1/setup.cfg
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1749 2022-08-24 21:00:13.000000 py-geth-3.9.1/setup.py
```

### Comparing `py-geth-3.9.0/LICENSE` & `py-geth-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/PKG-INFO` & `py-geth-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-geth
-Version: 3.9.0
+Version: 3.9.1
 Summary: Run Go-Ethereum as a subprocess
 Home-page: https://github.com/ethereum/py-geth
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum go-ethereum geth
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `py-geth-3.9.0/README.md` & `py-geth-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/accounts.py` & `py-geth-3.9.1/geth/accounts.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/chain.py` & `py-geth-3.9.1/geth/chain.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/exceptions.py` & `py-geth-3.9.1/geth/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/install.py` & `py-geth-3.9.1/geth/install.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/main.py` & `py-geth-3.9.1/geth/main.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/mixins.py` & `py-geth-3.9.1/geth/mixins.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/process.py` & `py-geth-3.9.1/geth/process.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/reset.py` & `py-geth-3.9.1/geth/reset.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/utils/dag.py` & `py-geth-3.9.1/geth/utils/dag.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/utils/encoding.py` & `py-geth-3.9.1/geth/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/utils/filesystem.py` & `py-geth-3.9.1/geth/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/utils/networking.py` & `py-geth-3.9.1/geth/utils/networking.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/utils/proc.py` & `py-geth-3.9.1/geth/utils/proc.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/utils/timeout.py` & `py-geth-3.9.1/geth/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/geth/wrapper.py` & `py-geth-3.9.1/geth/wrapper.py`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/py_geth.egg-info/PKG-INFO` & `py-geth-3.9.1/py_geth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-geth
-Version: 3.9.0
+Version: 3.9.1
 Summary: Run Go-Ethereum as a subprocess
 Home-page: https://github.com/ethereum/py-geth
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum go-ethereum geth
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `py-geth-3.9.0/py_geth.egg-info/SOURCES.txt` & `py-geth-3.9.1/py_geth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-geth-3.9.0/setup.py` & `py-geth-3.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 with open('./README.md') as readme:
     long_description = readme.read()
 
 setup(
     name='py-geth',
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version='3.9.0',
+    version='3.9.1',
     description="""Run Go-Ethereum as a subprocess""",
     long_description_content_type='text/markdown',
     long_description=long_description,
     author='Piper Merriam',
     author_email='pipermerriam@gmail.com',
     url='https://github.com/ethereum/py-geth',
     include_package_data=True,
```

