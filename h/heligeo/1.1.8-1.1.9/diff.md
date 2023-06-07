# Comparing `tmp/heligeo-1.1.8.tar.gz` & `tmp/heligeo-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heligeo-1.1.8.tar", last modified: Wed Mar 29 07:35:22 2023, max compression
+gzip compressed data, was "heligeo-1.1.9.tar", last modified: Wed Jun  7 06:36:37 2023, max compression
```

## Comparing `heligeo-1.1.8.tar` & `heligeo-1.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 07:35:22.494897 heligeo-1.1.8/
--rw-rw-rw-   0        0        0     1084 2023-03-29 03:44:12.000000 heligeo-1.1.8/LICENSE
--rw-rw-rw-   0        0        0    33632 2023-03-29 07:35:22.494897 heligeo-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    33149 2023-03-29 03:44:12.000000 heligeo-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 07:35:22.485865 heligeo-1.1.8/heligeo/
--rw-rw-rw-   0        0        0      133 2021-11-22 08:38:50.000000 heligeo-1.1.8/heligeo/__init__.py
--rw-rw-rw-   0        0        0   153934 2023-03-29 06:01:59.000000 heligeo-1.1.8/heligeo/main.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:35:22.492848 heligeo-1.1.8/heligeo.egg-info/
--rw-rw-rw-   0        0        0    33632 2023-03-29 07:35:21.000000 heligeo-1.1.8/heligeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-03-29 07:35:21.000000 heligeo-1.1.8/heligeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 07:35:21.000000 heligeo-1.1.8/heligeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-03-29 07:35:21.000000 heligeo-1.1.8/heligeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-29 07:35:21.000000 heligeo-1.1.8/heligeo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-29 07:35:22.494897 heligeo-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-03-29 07:23:06.000000 heligeo-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:36:37.916615 heligeo-1.1.9/
+-rw-rw-rw-   0        0        0     1084 2023-03-29 03:44:12.000000 heligeo-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0    33632 2023-06-07 06:36:37.915618 heligeo-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    33149 2023-03-29 03:44:12.000000 heligeo-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 06:36:37.899660 heligeo-1.1.9/heligeo/
+-rw-rw-rw-   0        0        0      133 2021-11-22 08:38:50.000000 heligeo-1.1.9/heligeo/__init__.py
+-rw-rw-rw-   0        0        0   153934 2023-03-29 06:01:59.000000 heligeo-1.1.9/heligeo/main.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:36:37.914620 heligeo-1.1.9/heligeo.egg-info/
+-rw-rw-rw-   0        0        0    33632 2023-06-07 06:36:37.000000 heligeo-1.1.9/heligeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-06-07 06:36:37.000000 heligeo-1.1.9/heligeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 06:36:37.000000 heligeo-1.1.9/heligeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-06-07 06:36:37.000000 heligeo-1.1.9/heligeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-07 06:36:37.000000 heligeo-1.1.9/heligeo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 06:36:37.916615 heligeo-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-06-07 06:21:52.000000 heligeo-1.1.9/setup.py
```

### Comparing `heligeo-1.1.8/LICENSE` & `heligeo-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `heligeo-1.1.8/PKG-INFO` & `heligeo-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heligeo
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python client for requests to heligeo API services
 Author: Heliware
 Author-email:  rajan@heliware.co.in
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `heligeo-1.1.8/README.md` & `heligeo-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `heligeo-1.1.8/heligeo/main.py` & `heligeo-1.1.9/heligeo/main.py`

 * *Files identical despite different names*

### Comparing `heligeo-1.1.8/heligeo.egg-info/PKG-INFO` & `heligeo-1.1.9/heligeo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heligeo
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python client for requests to heligeo API services
 Author: Heliware
 Author-email:  rajan@heliware.co.in
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `heligeo-1.1.8/setup.py` & `heligeo-1.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="heligeo",
-    version="1.1.8",
+    version="1.1.9",
     description="Python client for requests to heligeo API services",
     long_description=README,
     long_description_content_type="text/markdown",
 
     author="Heliware",
     author_email=" rajan@heliware.co.in",
     license="MIT",
```

