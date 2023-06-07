# Comparing `tmp/formalmath-0.0.1.tar.gz` & `tmp/formalmath-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formalmath-0.0.1.tar", last modified: Tue Jun  6 03:21:40 2023, max compression
+gzip compressed data, was "formalmath-0.0.2.tar", last modified: Wed Jun  7 05:24:45 2023, max compression
```

## Comparing `formalmath-0.0.1.tar` & `formalmath-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 03:21:40.589889 formalmath-0.0.1/
--rw-rw-rw-   0        0        0     1111 2023-06-06 03:21:40.589889 formalmath-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      660 2023-06-06 03:12:49.000000 formalmath-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 03:21:40.586888 formalmath-0.0.1/formalmath/
--rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.1/formalmath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:21:40.588888 formalmath-0.0.1/formalmath/setmm/
--rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.1/formalmath/setmm/__init__.py
--rw-rw-rw-   0        0        0     3998 2023-06-06 03:00:00.000000 formalmath-0.0.1/formalmath/setmm/basic_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:21:40.588888 formalmath-0.0.1/formalmath.egg-info/
--rw-rw-rw-   0        0        0     1111 2023-06-06 03:21:40.000000 formalmath-0.0.1/formalmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-06 03:21:40.000000 formalmath-0.0.1/formalmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 03:21:40.000000 formalmath-0.0.1/formalmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 03:21:40.000000 formalmath-0.0.1/formalmath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 03:21:40.589889 formalmath-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-06-06 03:21:27.000000 formalmath-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:24:45.046319 formalmath-0.0.2/
+-rw-rw-rw-   0        0        0     1452 2023-06-07 05:24:45.046319 formalmath-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2023-06-07 05:24:20.000000 formalmath-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 05:24:45.043319 formalmath-0.0.2/formalmath/
+-rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.2/formalmath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:24:45.046319 formalmath-0.0.2/formalmath/setmm/
+-rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.2/formalmath/setmm/__init__.py
+-rw-rw-rw-   0        0        0     5539 2023-06-07 05:14:32.000000 formalmath-0.0.2/formalmath/setmm/basic_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:24:45.045319 formalmath-0.0.2/formalmath.egg-info/
+-rw-rw-rw-   0        0        0     1452 2023-06-07 05:24:45.000000 formalmath-0.0.2/formalmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-07 05:24:45.000000 formalmath-0.0.2/formalmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 05:24:45.000000 formalmath-0.0.2/formalmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 05:24:45.000000 formalmath-0.0.2/formalmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 05:24:45.046319 formalmath-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-06-07 05:18:14.000000 formalmath-0.0.2/setup.py
```

### Comparing `formalmath-0.0.1/setup.py` & `formalmath-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="formalmath",  # Replace with your own username
-    version="0.0.1",
+    version="0.0.2",
     author="lixiang90",
     author_email="lixiang90@github.com",
-    description="a python version of a formal mathematics proof verifier.",
+    description="a python port of formal mathematics proof verifier.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lixiang90/formalmath.git",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

