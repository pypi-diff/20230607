# Comparing `tmp/junit-to-md-py-0.1.1.tar.gz` & `tmp/junit-to-md-py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junit-to-md-py-0.1.1.tar", last modified: Wed Jun  7 10:29:58 2023, max compression
+gzip compressed data, was "junit-to-md-py-0.2.0.tar", last modified: Wed Jun  7 11:59:48 2023, max compression
```

## Comparing `junit-to-md-py-0.1.1.tar` & `junit-to-md-py-0.2.0.tar`

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
+drwxrwxrwx   0        0        0        0 2023-06-07 11:59:48.420435 junit-to-md-py-0.2.0/
+-rw-rw-rw-   0        0        0      706 2023-06-07 11:59:48.419434 junit-to-md-py-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-06-07 11:58:44.000000 junit-to-md-py-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-07 11:59:48.392432 junit-to-md-py-0.2.0/junit_to_md/
+-rw-rw-rw-   0        0        0       37 2023-06-07 11:42:31.000000 junit-to-md-py-0.2.0/junit_to_md/__init__.py
+-rw-rw-rw-   0        0        0     1083 2023-06-07 11:42:55.000000 junit-to-md-py-0.2.0/junit_to_md/junit_to_md.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:59:48.416453 junit-to-md-py-0.2.0/junit_to_md_py.egg-info/
+-rw-rw-rw-   0        0        0      706 2023-06-07 11:59:48.000000 junit-to-md-py-0.2.0/junit_to_md_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-07 11:59:48.000000 junit-to-md-py-0.2.0/junit_to_md_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 11:59:48.000000 junit-to-md-py-0.2.0/junit_to_md_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-07 11:59:48.000000 junit-to-md-py-0.2.0/junit_to_md_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-07 11:59:48.000000 junit-to-md-py-0.2.0/junit_to_md_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 11:59:48.421435 junit-to-md-py-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      521 2023-06-07 11:59:16.000000 junit-to-md-py-0.2.0/setup.py
```

### Comparing `junit-to-md-py-0.1.1/script/junit_to_md.py` & `junit-to-md-py-0.2.0/junit_to_md/junit_to_md.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-#!/usr/bin/env python3
 import sys
 from lxml import etree
 import xml.etree.ElementTree as ET
 
 
 def junit_to_md(user_input: str):
-
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

### Comparing `junit-to-md-py-0.1.1/setup.py` & `junit-to-md-py-0.2.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 setup(
     name="junit-to-md-py",
-    version="0.1.1",
+    version="0.2.0",
     author="srydz_catalogicsoftware",
     author_email="srydz@catalogicsoftware.com",
     description="Python script which converts junit xml file/text into the markdown representation",
-    long_description=open("README.md").read(),
-    url='https://github.com/catalogicsoftware/dpx-utils-junit-to-md',
-    license='MIT',
-    packages=["script"],
+    long_description=open("README.rst", encoding="utf-8").read(),
+    url="https://github.com/catalogicsoftware/dpx-utils-junit-to-md",
+    license="MIT",
+    packages=["junit_to_md"],
     install_requires=[
         "lxml",
     ],
 )
```

