# Comparing `tmp/junit-to-md-py-0.1.0.tar.gz` & `tmp/junit-to-md-py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junit-to-md-py-0.1.0.tar", last modified: Wed Jun  7 10:17:12 2023, max compression
+gzip compressed data, was "junit-to-md-py-0.1.1.tar", last modified: Wed Jun  7 10:29:58 2023, max compression
```

## Comparing `junit-to-md-py-0.1.0.tar` & `junit-to-md-py-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 10:17:12.031180 junit-to-md-py-0.1.0/
--rw-rw-rw-   0        0        0      741 2023-06-07 10:17:12.030182 junit-to-md-py-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-06-06 17:40:29.000000 junit-to-md-py-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 10:17:12.004562 junit-to-md-py-0.1.0/junit_to_md/
--rw-rw-rw-   0        0        0       36 2023-06-07 10:07:50.000000 junit-to-md-py-0.1.0/junit_to_md/__init__.py
--rw-rw-rw-   0        0        0     1146 2023-06-07 10:07:23.000000 junit-to-md-py-0.1.0/junit_to_md/main.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:17:12.028178 junit-to-md-py-0.1.0/junit_to_md_py.egg-info/
--rw-rw-rw-   0        0        0      741 2023-06-07 10:17:11.000000 junit-to-md-py-0.1.0/junit_to_md_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-07 10:17:11.000000 junit-to-md-py-0.1.0/junit_to_md_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 10:17:11.000000 junit-to-md-py-0.1.0/junit_to_md_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-07 10:17:11.000000 junit-to-md-py-0.1.0/junit_to_md_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 10:17:11.000000 junit-to-md-py-0.1.0/junit_to_md_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 10:17:12.032149 junit-to-md-py-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-06-07 10:16:24.000000 junit-to-md-py-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 10:29:58.346338 junit-to-md-py-0.1.1/
+-rw-rw-rw-   0        0        0      741 2023-06-07 10:29:58.346338 junit-to-md-py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-06-06 17:40:29.000000 junit-to-md-py-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 10:29:58.337341 junit-to-md-py-0.1.1/junit_to_md_py.egg-info/
+-rw-rw-rw-   0        0        0      741 2023-06-07 10:29:58.000000 junit-to-md-py-0.1.1/junit_to_md_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-07 10:29:58.000000 junit-to-md-py-0.1.1/junit_to_md_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 10:29:58.000000 junit-to-md-py-0.1.1/junit_to_md_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-07 10:29:58.000000 junit-to-md-py-0.1.1/junit_to_md_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-07 10:29:58.000000 junit-to-md-py-0.1.1/junit_to_md_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 10:29:58.343339 junit-to-md-py-0.1.1/script/
+-rw-rw-rw-   0        0        0       36 2023-06-07 10:29:18.000000 junit-to-md-py-0.1.1/script/__init__.py
+-rw-rw-rw-   0        0        0     1106 2023-06-07 10:25:55.000000 junit-to-md-py-0.1.1/script/junit_to_md.py
+-rw-rw-rw-   0        0        0       42 2023-06-07 10:29:58.347339 junit-to-md-py-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      512 2023-06-07 10:29:32.000000 junit-to-md-py-0.1.1/setup.py
```

### Comparing `junit-to-md-py-0.1.0/PKG-INFO` & `junit-to-md-py-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 # Python script which converts junit xml file/text into the markdown representation
```

### Comparing `junit-to-md-py-0.1.0/junit_to_md/main.py` & `junit-to-md-py-0.1.1/script/junit_to_md.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #!/usr/bin/env python3
 import sys
 from lxml import etree
+import xml.etree.ElementTree as ET
 
 
-def main(user_input: str):
-
-    if len(sys.argv) < 2:
-        print("Error: junit file text argument is missing.")
-        print('Usage: python main.py "some text"')
-        sys.exit(1)
-
-    user_input = sys.argv[1]
+def junit_to_md(user_input: str):
 
     failedTestDetails = []
     allTests = []
 
-    xmlDoc = etree.parse(user_input)
+    try:
+        xmlDoc = etree.parse(user_input)
+    except ET.ParseError:
+        print("Error: junit file parse error.")
+        sys.exit(1)
+
     suites = xmlDoc.xpath("//testsuite")
     for suite in suites:
         tests = suite.xpath(".//testcase")
         for test in tests:
             allTests.append(test)
             failures = test.xpath(".//failure")
             for failure in failures:
```

### Comparing `junit-to-md-py-0.1.0/junit_to_md_py.egg-info/PKG-INFO` & `junit-to-md-py-0.1.1/junit_to_md_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 # Python script which converts junit xml file/text into the markdown representation
```

### Comparing `junit-to-md-py-0.1.0/setup.py` & `junit-to-md-py-0.1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="junit-to-md-py",
-    version="0.1.0",
+    version="0.1.1",
     author="srydz_catalogicsoftware",
     author_email="srydz@catalogicsoftware.com",
     description="Python script which converts junit xml file/text into the markdown representation",
     long_description=open("README.md").read(),
     url='https://github.com/catalogicsoftware/dpx-utils-junit-to-md',
     license='MIT',
-    packages=["junit_to_md"],
+    packages=["script"],
     install_requires=[
         "lxml",
     ],
-    
 )
```

