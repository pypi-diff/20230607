# Comparing `tmp/pikanetwork.py-0.0.2.tar.gz` & `tmp/pikanetwork.py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikanetwork.py-0.0.2.tar", last modified: Wed Jun  7 12:48:27 2023, max compression
+gzip compressed data, was "pikanetwork.py-0.0.3.tar", last modified: Wed Jun  7 12:58:44 2023, max compression
```

## Comparing `pikanetwork.py-0.0.2.tar` & `pikanetwork.py-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 12:48:27.254301 pikanetwork.py-0.0.2/
--rw-rw-rw-   0        0        0     1070 2023-06-07 11:42:00.000000 pikanetwork.py-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1776 2023-06-07 12:48:27.252293 pikanetwork.py-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1531 2023-06-07 11:49:13.000000 pikanetwork.py-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 12:48:27.241297 pikanetwork.py-0.0.2/pikanetwork/
--rw-rw-rw-   0        0        0      311 2023-06-07 11:26:13.000000 pikanetwork.py-0.0.2/pikanetwork/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-07 11:49:13.000000 pikanetwork.py-0.0.2/pikanetwork/api.py
--rw-rw-rw-   0        0        0     2481 2023-06-07 11:27:56.000000 pikanetwork.py-0.0.2/pikanetwork/builders.py
--rw-rw-rw-   0        0        0     1747 2023-06-07 10:59:44.000000 pikanetwork.py-0.0.2/pikanetwork/models.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:48:27.249293 pikanetwork.py-0.0.2/pikanetwork.py.egg-info/
--rw-rw-rw-   0        0        0     1776 2023-06-07 12:48:27.000000 pikanetwork.py-0.0.2/pikanetwork.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-07 12:48:27.000000 pikanetwork.py-0.0.2/pikanetwork.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 12:48:27.000000 pikanetwork.py-0.0.2/pikanetwork.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 12:48:27.000000 pikanetwork.py-0.0.2/pikanetwork.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 12:48:27.256297 pikanetwork.py-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      478 2023-06-07 12:47:45.000000 pikanetwork.py-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:58:44.008229 pikanetwork.py-0.0.3/
+-rw-rw-rw-   0        0        0     1070 2023-06-07 11:42:00.000000 pikanetwork.py-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2464 2023-06-07 12:58:44.007229 pikanetwork.py-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1531 2023-06-07 11:49:13.000000 pikanetwork.py-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 12:58:43.985621 pikanetwork.py-0.0.3/pikanetwork/
+-rw-rw-rw-   0        0        0      311 2023-06-07 12:54:25.000000 pikanetwork.py-0.0.3/pikanetwork/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-07 11:49:13.000000 pikanetwork.py-0.0.3/pikanetwork/api.py
+-rw-rw-rw-   0        0        0     2481 2023-06-07 11:27:56.000000 pikanetwork.py-0.0.3/pikanetwork/builders.py
+-rw-rw-rw-   0        0        0     1747 2023-06-07 10:59:44.000000 pikanetwork.py-0.0.3/pikanetwork/models.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:58:44.003229 pikanetwork.py-0.0.3/pikanetwork.py.egg-info/
+-rw-rw-rw-   0        0        0     2464 2023-06-07 12:58:43.000000 pikanetwork.py-0.0.3/pikanetwork.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-06-07 12:58:43.000000 pikanetwork.py-0.0.3/pikanetwork.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 12:58:43.000000 pikanetwork.py-0.0.3/pikanetwork.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 12:58:43.000000 pikanetwork.py-0.0.3/pikanetwork.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-07 12:58:43.000000 pikanetwork.py-0.0.3/pikanetwork.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 12:58:44.008229 pikanetwork.py-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2182 2023-06-07 12:58:41.000000 pikanetwork.py-0.0.3/setup.py
```

### Comparing `pikanetwork.py-0.0.2/LICENSE` & `pikanetwork.py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pikanetwork.py-0.0.2/PKG-INFO` & `pikanetwork.py-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: pikanetwork.py
-Version: 0.0.2
-Summary: An api wrapper for pikanetwork
-Home-page: https://github.com/LetsChill/pikanetwork.py
-Author: LetsChill
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pikanetwork.py
 
 A unique api wrapper for pikanetwork.
 
 It provides ready-to-use objects from the api to python for optimization and durability of data.
 
 It also makes accessing data an easy thing to do.
@@ -37,8 +28,8 @@
 
 Copyright (c) 2023 LetsChill.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pikanetwork.py-0.0.2/pikanetwork/api.py` & `pikanetwork.py-0.0.3/pikanetwork/api.py`

 * *Files identical despite different names*

### Comparing `pikanetwork.py-0.0.2/pikanetwork/builders.py` & `pikanetwork.py-0.0.3/pikanetwork/builders.py`

 * *Files identical despite different names*

### Comparing `pikanetwork.py-0.0.2/pikanetwork/models.py` & `pikanetwork.py-0.0.3/pikanetwork/models.py`

 * *Files identical despite different names*

