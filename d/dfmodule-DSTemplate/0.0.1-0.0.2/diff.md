# Comparing `tmp/dfmodule_DSTemplate-0.0.1.tar.gz` & `tmp/dfmodule_DSTemplate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule_DSTemplate-0.0.1.tar", last modified: Wed Jun  7 02:43:58 2023, max compression
+gzip compressed data, was "dfmodule_DSTemplate-0.0.2.tar", last modified: Wed Jun  7 03:00:23 2023, max compression
```

## Comparing `dfmodule_DSTemplate-0.0.1.tar` & `dfmodule_DSTemplate-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 02:43:58.486492 dfmodule_DSTemplate-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-07 02:43:58.475495 dfmodule_DSTemplate-0.0.1/DS/
--rw-rw-rw-   0        0        0       55 2023-06-07 02:43:47.000000 dfmodule_DSTemplate-0.0.1/DS/__init__.py
--rw-rw-rw-   0        0        0      563 2023-06-07 02:43:58.486492 dfmodule_DSTemplate-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 02:36:22.000000 dfmodule_DSTemplate-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 02:43:58.485492 dfmodule_DSTemplate-0.0.1/dfmodule_DSTemplate.egg-info/
--rw-rw-rw-   0        0        0      563 2023-06-07 02:43:58.000000 dfmodule_DSTemplate-0.0.1/dfmodule_DSTemplate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-06-07 02:43:58.000000 dfmodule_DSTemplate-0.0.1/dfmodule_DSTemplate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 02:43:58.000000 dfmodule_DSTemplate-0.0.1/dfmodule_DSTemplate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-07 02:43:58.000000 dfmodule_DSTemplate-0.0.1/dfmodule_DSTemplate.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        3 2023-06-07 02:43:58.000000 dfmodule_DSTemplate-0.0.1/dfmodule_DSTemplate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 02:43:58.486492 dfmodule_DSTemplate-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-06-07 02:42:30.000000 dfmodule_DSTemplate-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:00:23.774487 dfmodule_DSTemplate-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-07 03:00:23.763438 dfmodule_DSTemplate-0.0.2/DS/
+-rw-rw-rw-   0        0        0     2420 2023-06-07 02:59:27.000000 dfmodule_DSTemplate-0.0.2/DS/Get_by_dates.py
+-rw-rw-rw-   0        0        0       55 2023-06-07 02:50:58.000000 dfmodule_DSTemplate-0.0.2/DS/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-06-07 03:00:23.773450 dfmodule_DSTemplate-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 02:36:22.000000 dfmodule_DSTemplate-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 03:00:23.772449 dfmodule_DSTemplate-0.0.2/dfmodule_DSTemplate.egg-info/
+-rw-rw-rw-   0        0        0      563 2023-06-07 03:00:23.000000 dfmodule_DSTemplate-0.0.2/dfmodule_DSTemplate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-06-07 03:00:23.000000 dfmodule_DSTemplate-0.0.2/dfmodule_DSTemplate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 03:00:23.000000 dfmodule_DSTemplate-0.0.2/dfmodule_DSTemplate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-07 02:43:58.000000 dfmodule_DSTemplate-0.0.2/dfmodule_DSTemplate.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       36 2023-06-07 03:00:23.000000 dfmodule_DSTemplate-0.0.2/dfmodule_DSTemplate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2023-06-07 03:00:23.000000 dfmodule_DSTemplate-0.0.2/dfmodule_DSTemplate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 03:00:23.774487 dfmodule_DSTemplate-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      847 2023-06-07 02:59:58.000000 dfmodule_DSTemplate-0.0.2/setup.py
```

### Comparing `dfmodule_DSTemplate-0.0.1/PKG-INFO` & `dfmodule_DSTemplate-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfmodule_DSTemplate
-Version: 0.0.1
+Version: 0.0.2
 Summary: dfmodule for DE -> DS code transition
 Home-page: https://github.com/Data-Flower/dfmodule_DSTemplate
 Author: SG, JH
 Author-email: rimmoyee@example.com
 Keywords: dfmodule_DS, dfmodule, dfmodule_DSTemplate
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dfmodule_DSTemplate-0.0.1/dfmodule_DSTemplate.egg-info/PKG-INFO` & `dfmodule_DSTemplate-0.0.2/dfmodule_DSTemplate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfmodule-DSTemplate
-Version: 0.0.1
+Version: 0.0.2
 Summary: dfmodule for DE -> DS code transition
 Home-page: https://github.com/Data-Flower/dfmodule_DSTemplate
 Author: SG, JH
 Author-email: rimmoyee@example.com
 Keywords: dfmodule_DS, dfmodule, dfmodule_DSTemplate
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dfmodule_DSTemplate-0.0.1/setup.py` & `dfmodule_DSTemplate-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dfmodule_DSTemplate",
-    version="0.0.1",
+    version="0.0.2",
     description="dfmodule for DE -> DS code transition",
     author="SG, JH",
     author_email="rimmoyee@example.com",
     url="https://github.com/Data-Flower/dfmodule_DSTemplate",
-    install_requires=[],
+    install_requires=['boto3', 'pandas', 'python-dotenv', 'requests'],
     packages=find_packages(exclude=['tests*']),
     keywords=['dfmodule_DS, dfmodule, dfmodule_DSTemplate'],
     python_requires='>=3.6',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
```

