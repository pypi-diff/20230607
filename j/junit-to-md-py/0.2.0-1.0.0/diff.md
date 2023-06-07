# Comparing `tmp/junit-to-md-py-0.2.0.tar.gz` & `tmp/junit-to-md-py-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junit-to-md-py-0.2.0.tar", last modified: Wed Jun  7 11:59:48 2023, max compression
+gzip compressed data, was "junit-to-md-py-1.0.0.tar", last modified: Wed Jun  7 18:15:07 2023, max compression
```

## Comparing `junit-to-md-py-0.2.0.tar` & `junit-to-md-py-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 11:59:48.420435 junit-to-md-py-0.2.0/
--rw-rw-rw-   0        0        0      706 2023-06-07 11:59:48.419434 junit-to-md-py-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-06-07 11:58:44.000000 junit-to-md-py-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-07 11:59:48.392432 junit-to-md-py-0.2.0/junit_to_md/
--rw-rw-rw-   0        0        0       37 2023-06-07 11:42:31.000000 junit-to-md-py-0.2.0/junit_to_md/__init__.py
--rw-rw-rw-   0        0        0     1083 2023-06-07 11:42:55.000000 junit-to-md-py-0.2.0/junit_to_md/junit_to_md.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:59:48.416453 junit-to-md-py-0.2.0/junit_to_md_py.egg-info/
--rw-rw-rw-   0        0        0      706 2023-06-07 11:59:48.000000 junit-to-md-py-0.2.0/junit_to_md_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-06-07 11:59:48.000000 junit-to-md-py-0.2.0/junit_to_md_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 11:59:48.000000 junit-to-md-py-0.2.0/junit_to_md_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-07 11:59:48.000000 junit-to-md-py-0.2.0/junit_to_md_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 11:59:48.000000 junit-to-md-py-0.2.0/junit_to_md_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 11:59:48.421435 junit-to-md-py-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      521 2023-06-07 11:59:16.000000 junit-to-md-py-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:15:07.837024 junit-to-md-py-1.0.0/
+-rw-rw-rw-   0        0        0      617 2023-06-07 18:15:07.837024 junit-to-md-py-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-06-07 18:12:45.000000 junit-to-md-py-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-07 18:15:07.802607 junit-to-md-py-1.0.0/junit_to_md/
+-rw-rw-rw-   0        0        0       37 2023-06-07 11:42:31.000000 junit-to-md-py-1.0.0/junit_to_md/__init__.py
+-rw-rw-rw-   0        0        0     1010 2023-06-07 18:09:23.000000 junit-to-md-py-1.0.0/junit_to_md/junit_to_md.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:15:07.833022 junit-to-md-py-1.0.0/junit_to_md_py.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-06-07 18:15:07.000000 junit-to-md-py-1.0.0/junit_to_md_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-07 18:15:07.000000 junit-to-md-py-1.0.0/junit_to_md_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 18:15:07.000000 junit-to-md-py-1.0.0/junit_to_md_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-07 18:15:07.000000 junit-to-md-py-1.0.0/junit_to_md_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-07 18:15:07.000000 junit-to-md-py-1.0.0/junit_to_md_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 18:15:07.837024 junit-to-md-py-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      521 2023-06-07 18:12:30.000000 junit-to-md-py-1.0.0/setup.py
```

### Comparing `junit-to-md-py-0.2.0/PKG-INFO` & `junit-to-md-py-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 0.2.0
+Version: 1.0.0
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 Python script which converts junit xml file/text into the markdown representation
@@ -14,12 +14,7 @@
 ~~~~~~~~~~~~~
 
 ::
 
    from junit_to_md import junit_to_md
 
    junit_to_md(open("sample_junitOutput.xml", "r"))
-
-Sample output
-~~~~~~~~~~~~~
-
-You can see see sample output at **sample_output.md**
```

### Comparing `junit-to-md-py-0.2.0/junit_to_md_py.egg-info/PKG-INFO` & `junit-to-md-py-1.0.0/junit_to_md_py.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 0.2.0
+Version: 1.0.0
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 Python script which converts junit xml file/text into the markdown representation
@@ -14,12 +14,7 @@
 ~~~~~~~~~~~~~
 
 ::
 
    from junit_to_md import junit_to_md
 
    junit_to_md(open("sample_junitOutput.xml", "r"))
-
-Sample output
-~~~~~~~~~~~~~
-
-You can see see sample output at **sample_output.md**
```

### Comparing `junit-to-md-py-0.2.0/setup.py` & `junit-to-md-py-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="junit-to-md-py",
-    version="0.2.0",
+    version="1.0.0",
     author="srydz_catalogicsoftware",
     author_email="srydz@catalogicsoftware.com",
     description="Python script which converts junit xml file/text into the markdown representation",
     long_description=open("README.rst", encoding="utf-8").read(),
     url="https://github.com/catalogicsoftware/dpx-utils-junit-to-md",
     license="MIT",
     packages=["junit_to_md"],
```

