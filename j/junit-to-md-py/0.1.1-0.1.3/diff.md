# Comparing `tmp/junit-to-md-py-0.1.1.tar.gz` & `tmp/junit-to-md-py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junit-to-md-py-0.1.1.tar", last modified: Wed Jun  7 10:29:58 2023, max compression
+gzip compressed data, was "junit-to-md-py-0.1.3.tar", last modified: Wed Jun  7 10:50:55 2023, max compression
```

## Comparing `junit-to-md-py-0.1.1.tar` & `junit-to-md-py-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 10:29:58.346338 junit-to-md-py-0.1.1/
--rw-rw-rw-   0        0        0      741 2023-06-07 10:29:58.346338 junit-to-md-py-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-06-06 17:40:29.000000 junit-to-md-py-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 10:29:58.337341 junit-to-md-py-0.1.1/junit_to_md_py.egg-info/
--rw-rw-rw-   0        0        0      741 2023-06-07 10:29:58.000000 junit-to-md-py-0.1.1/junit_to_md_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-06-07 10:29:58.000000 junit-to-md-py-0.1.1/junit_to_md_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 10:29:58.000000 junit-to-md-py-0.1.1/junit_to_md_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-07 10:29:58.000000 junit-to-md-py-0.1.1/junit_to_md_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-07 10:29:58.000000 junit-to-md-py-0.1.1/junit_to_md_py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 10:29:58.343339 junit-to-md-py-0.1.1/script/
--rw-rw-rw-   0        0        0       36 2023-06-07 10:29:18.000000 junit-to-md-py-0.1.1/script/__init__.py
--rw-rw-rw-   0        0        0     1106 2023-06-07 10:25:55.000000 junit-to-md-py-0.1.1/script/junit_to_md.py
--rw-rw-rw-   0        0        0       42 2023-06-07 10:29:58.347339 junit-to-md-py-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-06-07 10:29:32.000000 junit-to-md-py-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 10:50:55.487427 junit-to-md-py-0.1.3/
+-rw-rw-rw-   0        0        0      741 2023-06-07 10:50:55.486426 junit-to-md-py-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-06-06 17:40:29.000000 junit-to-md-py-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 10:50:55.462423 junit-to-md-py-0.1.3/junit_to_md/
+-rw-rw-rw-   0        0        0       36 2023-06-07 10:48:32.000000 junit-to-md-py-0.1.3/junit_to_md/__init__.py
+-rw-rw-rw-   0        0        0     1106 2023-06-07 10:49:10.000000 junit-to-md-py-0.1.3/junit_to_md/junit_to_md.py
+drwxrwxrwx   0        0        0        0 2023-06-07 10:50:55.483428 junit-to-md-py-0.1.3/junit_to_md_py.egg-info/
+-rw-rw-rw-   0        0        0      741 2023-06-07 10:50:55.000000 junit-to-md-py-0.1.3/junit_to_md_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-07 10:50:55.000000 junit-to-md-py-0.1.3/junit_to_md_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 10:50:55.000000 junit-to-md-py-0.1.3/junit_to_md_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-07 10:50:55.000000 junit-to-md-py-0.1.3/junit_to_md_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-07 10:50:55.000000 junit-to-md-py-0.1.3/junit_to_md_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 10:50:55.487427 junit-to-md-py-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-06-07 10:50:43.000000 junit-to-md-py-0.1.3/setup.py
```

### Comparing `junit-to-md-py-0.1.1/PKG-INFO` & `junit-to-md-py-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 0.1.1
+Version: 0.1.3
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 # Python script which converts junit xml file/text into the markdown representation
```

### Comparing `junit-to-md-py-0.1.1/junit_to_md_py.egg-info/PKG-INFO` & `junit-to-md-py-0.1.3/junit_to_md_py.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 0.1.1
+Version: 0.1.3
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 # Python script which converts junit xml file/text into the markdown representation
```

### Comparing `junit-to-md-py-0.1.1/script/junit_to_md.py` & `junit-to-md-py-0.1.3/junit_to_md/junit_to_md.py`

 * *Files identical despite different names*

### Comparing `junit-to-md-py-0.1.1/setup.py` & `junit-to-md-py-0.1.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="junit-to-md-py",
-    version="0.1.1",
+    version="0.1.3",
     author="srydz_catalogicsoftware",
     author_email="srydz@catalogicsoftware.com",
     description="Python script which converts junit xml file/text into the markdown representation",
     long_description=open("README.md").read(),
     url='https://github.com/catalogicsoftware/dpx-utils-junit-to-md',
     license='MIT',
-    packages=["script"],
+    packages=["junit_to_md"],
     install_requires=[
         "lxml",
     ],
 )
```

