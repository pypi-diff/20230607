# Comparing `tmp/pyem_st_artifacts-1.0.1.post1.tar.gz` & `tmp/pyem_st_artifacts-1.0.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyem_st_artifacts-1.0.1.post1.tar", last modified: Wed Jun  7 13:45:56 2023, max compression
+gzip compressed data, was "dist\pyem_st_artifacts-1.0.1.post2.tar", last modified: Wed Jun  7 13:59:52 2023, max compression
```

## Comparing `pyem_st_artifacts-1.0.1.post1.tar` & `pyem_st_artifacts-1.0.1.post2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 13:45:56.000000 pyem_st_artifacts-1.0.1.post1/
--rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyem_st_artifacts-1.0.1.post1/LICENSE
--rw-rw-rw-   0        0        0     9709 2023-06-07 13:45:56.000000 pyem_st_artifacts-1.0.1.post1/PKG-INFO
--rw-rw-rw-   0        0        0     9155 2023-06-07 12:28:29.000000 pyem_st_artifacts-1.0.1.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 13:45:56.000000 pyem_st_artifacts-1.0.1.post1/em_st_artifacts/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post1/em_st_artifacts/__init__.py
--rw-rw-rw-   0        0        0    23950 2023-06-07 09:59:08.000000 pyem_st_artifacts-1.0.1.post1/em_st_artifacts/em_st_artifactslib.py
--rw-rw-rw-   0        0        0     3448 2023-06-07 13:09:40.000000 pyem_st_artifacts-1.0.1.post1/em_st_artifacts/sample.py
-drwxrwxrwx   0        0        0        0 2023-06-07 13:45:56.000000 pyem_st_artifacts-1.0.1.post1/pyem_st_artifacts.egg-info/
--rw-rw-rw-   0        0        0     9709 2023-06-07 13:45:56.000000 pyem_st_artifacts-1.0.1.post1/pyem_st_artifacts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-07 13:45:56.000000 pyem_st_artifacts-1.0.1.post1/pyem_st_artifacts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 13:45:56.000000 pyem_st_artifacts-1.0.1.post1/pyem_st_artifacts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-07 13:45:56.000000 pyem_st_artifacts-1.0.1.post1/pyem_st_artifacts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 13:45:56.000000 pyem_st_artifacts-1.0.1.post1/setup.cfg
--rw-rw-rw-   0        0        0     1264 2023-06-07 13:45:49.000000 pyem_st_artifacts-1.0.1.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/
+-rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyem_st_artifacts-1.0.1.post2/LICENSE
+-rw-rw-rw-   0        0        0     9709 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/PKG-INFO
+-rw-rw-rw-   0        0        0     9155 2023-06-07 12:28:29.000000 pyem_st_artifacts-1.0.1.post2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/__init__.py
+-rw-rw-rw-   0        0        0    23950 2023-06-07 09:59:08.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/emotional_math.py
+-rw-rw-rw-   0        0        0     3448 2023-06-07 13:09:40.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/sample.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/utils/__init__.py
+-rw-rw-rw-   0        0        0      944 2023-06-06 14:04:47.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/utils/lib_settings.py
+-rw-rw-rw-   0        0        0      655 2023-06-06 13:59:02.000000 pyem_st_artifacts-1.0.1.post2/em_st_artifacts/utils/support_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/pyem_st_artifacts.egg-info/
+-rw-rw-rw-   0        0        0     9709 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/pyem_st_artifacts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/pyem_st_artifacts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/pyem_st_artifacts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/pyem_st_artifacts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 13:59:52.000000 pyem_st_artifacts-1.0.1.post2/setup.cfg
+-rw-rw-rw-   0        0        0     1357 2023-06-07 13:59:45.000000 pyem_st_artifacts-1.0.1.post2/setup.py
```

### Comparing `pyem_st_artifacts-1.0.1.post1/LICENSE` & `pyem_st_artifacts-1.0.1.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post1/PKG-INFO` & `pyem_st_artifacts-1.0.1.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyem_st_artifacts
-Version: 1.0.1.post1
+Version: 1.0.1.post2
 Summary: Python wrapper for Emotions library
 Home-page: https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python
 Author: Brainbit Inc.
 Author-email: support@brainbit.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyem_st_artifacts-1.0.1.post1/README.md` & `pyem_st_artifacts-1.0.1.post2/README.md`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post1/em_st_artifacts/em_st_artifactslib.py` & `pyem_st_artifacts-1.0.1.post2/em_st_artifacts/emotional_math.py`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post1/em_st_artifacts/sample.py` & `pyem_st_artifacts-1.0.1.post2/em_st_artifacts/sample.py`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post1/pyem_st_artifacts.egg-info/PKG-INFO` & `pyem_st_artifacts-1.0.1.post2/pyem_st_artifacts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyem-st-artifacts
-Version: 1.0.1.post1
+Version: 1.0.1.post2
 Summary: Python wrapper for Emotions library
 Home-page: https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python
 Author: Brainbit Inc.
 Author-email: support@brainbit.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyem_st_artifacts-1.0.1.post1/setup.py` & `pyem_st_artifacts-1.0.1.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pyem_st_artifacts',
-    version='1.0.1.post1',
+    version='1.0.1.post2',
     py_modules=[
-        'em_st_artifacts.em_st_artifactslib'],
+        'em_st_artifacts.emotional_math',
+        'em_st_artifacts.utils.lib_settings',
+        'em_st_artifacts.utils.support_classes'],
     packages=['em_st_artifacts'],
     url='https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python',
     license='MIT',
     author='Brainbit Inc.',
     author_email='support@brainbit.com',
     description='Python wrapper for Emotions library',
     long_description=long_description,
```

