# Comparing `tmp/junit-to-md-py-0.1.3.tar.gz` & `tmp/junit-to-md-py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junit-to-md-py-0.1.3.tar", last modified: Wed Jun  7 10:50:55 2023, max compression
+gzip compressed data, was "junit-to-md-py-0.1.4.tar", last modified: Wed Jun  7 11:14:36 2023, max compression
```

## Comparing `junit-to-md-py-0.1.3.tar` & `junit-to-md-py-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 10:50:55.487427 junit-to-md-py-0.1.3/
--rw-rw-rw-   0        0        0      741 2023-06-07 10:50:55.486426 junit-to-md-py-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-06-06 17:40:29.000000 junit-to-md-py-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 10:50:55.462423 junit-to-md-py-0.1.3/junit_to_md/
--rw-rw-rw-   0        0        0       36 2023-06-07 10:48:32.000000 junit-to-md-py-0.1.3/junit_to_md/__init__.py
--rw-rw-rw-   0        0        0     1106 2023-06-07 10:49:10.000000 junit-to-md-py-0.1.3/junit_to_md/junit_to_md.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:50:55.483428 junit-to-md-py-0.1.3/junit_to_md_py.egg-info/
--rw-rw-rw-   0        0        0      741 2023-06-07 10:50:55.000000 junit-to-md-py-0.1.3/junit_to_md_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-07 10:50:55.000000 junit-to-md-py-0.1.3/junit_to_md_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 10:50:55.000000 junit-to-md-py-0.1.3/junit_to_md_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-07 10:50:55.000000 junit-to-md-py-0.1.3/junit_to_md_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 10:50:55.000000 junit-to-md-py-0.1.3/junit_to_md_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 10:50:55.487427 junit-to-md-py-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-06-07 10:50:43.000000 junit-to-md-py-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:14:36.988444 junit-to-md-py-0.1.4/
+-rw-rw-rw-   0        0        0      741 2023-06-07 11:14:36.987443 junit-to-md-py-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-06-06 17:40:29.000000 junit-to-md-py-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 11:14:36.962448 junit-to-md-py-0.1.4/junit_to_md/
+-rw-rw-rw-   0        0        0       36 2023-06-07 11:10:34.000000 junit-to-md-py-0.1.4/junit_to_md/__init__.py
+-rw-rw-rw-   0        0        0     1085 2023-06-07 11:14:12.000000 junit-to-md-py-0.1.4/junit_to_md/junit_to_md.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:14:36.985445 junit-to-md-py-0.1.4/junit_to_md_py.egg-info/
+-rw-rw-rw-   0        0        0      741 2023-06-07 11:14:36.000000 junit-to-md-py-0.1.4/junit_to_md_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-07 11:14:36.000000 junit-to-md-py-0.1.4/junit_to_md_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 11:14:36.000000 junit-to-md-py-0.1.4/junit_to_md_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-07 11:14:36.000000 junit-to-md-py-0.1.4/junit_to_md_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-07 11:14:36.000000 junit-to-md-py-0.1.4/junit_to_md_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 11:14:36.989444 junit-to-md-py-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-06-07 11:14:16.000000 junit-to-md-py-0.1.4/setup.py
```

### Comparing `junit-to-md-py-0.1.3/PKG-INFO` & `junit-to-md-py-0.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 # Python script which converts junit xml file/text into the markdown representation
```

### Comparing `junit-to-md-py-0.1.3/junit_to_md/junit_to_md.py` & `junit-to-md-py-0.1.4/junit_to_md/junit_to_md.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-#!/usr/bin/env python3
 import sys
 from lxml import etree
 import xml.etree.ElementTree as ET
 
 
 def junit_to_md(user_input: str):
 
     failedTestDetails = []
     allTests = []
 
     try:
         xmlDoc = etree.parse(user_input)
     except ET.ParseError:
-        print("Error: junit file parse error.")
+        print("Error parsing the text from file.")
         sys.exit(1)
 
     suites = xmlDoc.xpath("//testsuite")
     for suite in suites:
         tests = suite.xpath(".//testcase")
         for test in tests:
             allTests.append(test)
```

### Comparing `junit-to-md-py-0.1.3/junit_to_md_py.egg-info/PKG-INFO` & `junit-to-md-py-0.1.4/junit_to_md_py.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 # Python script which converts junit xml file/text into the markdown representation
```

### Comparing `junit-to-md-py-0.1.3/setup.py` & `junit-to-md-py-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="junit-to-md-py",
-    version="0.1.3",
+    version="0.1.4",
     author="srydz_catalogicsoftware",
     author_email="srydz@catalogicsoftware.com",
     description="Python script which converts junit xml file/text into the markdown representation",
     long_description=open("README.md").read(),
     url='https://github.com/catalogicsoftware/dpx-utils-junit-to-md',
     license='MIT',
     packages=["junit_to_md"],
```

