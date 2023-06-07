# Comparing `tmp/venomics-client-0.1.0.tar.gz` & `tmp/venomics-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venomics-client-0.1.0.tar", last modified: Wed Jun  7 07:58:49 2023, max compression
+gzip compressed data, was "venomics-client-0.1.1.tar", last modified: Wed Jun  7 08:04:09 2023, max compression
```

## Comparing `venomics-client-0.1.0.tar` & `venomics-client-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-07 07:58:49.048443 venomics-client-0.1.0/
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)     1064 2023-06-07 04:08:03.000000 venomics-client-0.1.0/LICENSE
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     6522 2023-06-07 07:58:49.048523 venomics-client-0.1.0/PKG-INFO
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)     5503 2023-06-07 07:58:46.000000 venomics-client-0.1.0/README.md
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     1201 2023-06-07 07:58:49.048863 venomics-client-0.1.0/setup.cfg
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)       69 2023-06-07 05:31:57.000000 venomics-client-0.1.0/setup.py
-drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-07 07:58:49.047597 venomics-client-0.1.0/venomics_client/
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)      118 2023-06-07 07:41:07.000000 venomics-client-0.1.0/venomics_client/__init__.py
--rw-rw-r--   0 mnechepurenko   (501) staff       (20)     6994 2023-06-07 07:41:07.000000 venomics-client-0.1.0/venomics_client/client.py
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     4426 2023-06-07 07:41:07.000000 venomics-client-0.1.0/venomics_client/date_ranges.py
-drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-07 07:58:49.048328 venomics-client-0.1.0/venomics_client.egg-info/
--rw-r--r--   0 mnechepurenko   (501) staff       (20)     6522 2023-06-07 07:58:49.000000 venomics-client-0.1.0/venomics_client.egg-info/PKG-INFO
--rw-r--r--   0 mnechepurenko   (501) staff       (20)      353 2023-06-07 07:58:49.000000 venomics-client-0.1.0/venomics_client.egg-info/SOURCES.txt
--rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-07 07:58:49.000000 venomics-client-0.1.0/venomics_client.egg-info/dependency_links.txt
--rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-07 07:54:13.000000 venomics-client-0.1.0/venomics_client.egg-info/not-zip-safe
--rw-r--r--   0 mnechepurenko   (501) staff       (20)       90 2023-06-07 07:58:49.000000 venomics-client-0.1.0/venomics_client.egg-info/requires.txt
--rw-r--r--   0 mnechepurenko   (501) staff       (20)       16 2023-06-07 07:58:49.000000 venomics-client-0.1.0/venomics_client.egg-info/top_level.txt
+drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-07 08:04:09.290562 venomics-client-0.1.1/
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)     1064 2023-06-07 04:08:03.000000 venomics-client-0.1.1/LICENSE
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)     6423 2023-06-07 08:04:09.290640 venomics-client-0.1.1/PKG-INFO
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)     5404 2023-06-07 08:03:56.000000 venomics-client-0.1.1/README.md
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)     1201 2023-06-07 08:04:09.290934 venomics-client-0.1.1/setup.cfg
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)       69 2023-06-07 05:31:57.000000 venomics-client-0.1.1/setup.py
+drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-07 08:04:09.289659 venomics-client-0.1.1/venomics_client/
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)      118 2023-06-07 07:41:07.000000 venomics-client-0.1.1/venomics_client/__init__.py
+-rw-rw-r--   0 mnechepurenko   (501) staff       (20)     6994 2023-06-07 07:41:07.000000 venomics-client-0.1.1/venomics_client/client.py
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)     4426 2023-06-07 07:41:07.000000 venomics-client-0.1.1/venomics_client/date_ranges.py
+drwxr-xr-x   0 mnechepurenko   (501) staff       (20)        0 2023-06-07 08:04:09.290457 venomics-client-0.1.1/venomics_client.egg-info/
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)     6423 2023-06-07 08:04:09.000000 venomics-client-0.1.1/venomics_client.egg-info/PKG-INFO
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)      353 2023-06-07 08:04:09.000000 venomics-client-0.1.1/venomics_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-07 08:04:09.000000 venomics-client-0.1.1/venomics_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)        1 2023-06-07 07:54:13.000000 venomics-client-0.1.1/venomics_client.egg-info/not-zip-safe
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)       90 2023-06-07 08:04:09.000000 venomics-client-0.1.1/venomics_client.egg-info/requires.txt
+-rw-r--r--   0 mnechepurenko   (501) staff       (20)       16 2023-06-07 08:04:09.000000 venomics-client-0.1.1/venomics_client.egg-info/top_level.txt
```

### Comparing `venomics-client-0.1.0/LICENSE` & `venomics-client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `venomics-client-0.1.0/PKG-INFO` & `venomics-client-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venomics-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Venomics API Client
 Home-page: https://www.venomics.xyz/
 Author: maksymds
 Author-email: redoubt@devnull.ae
 License: MIT
 Project-URL: Github, https://github.com/Venomics/venomics-api-client
 Project-URL: Documentation, https://www.vebnomics.xyz/
@@ -26,15 +26,14 @@
 License-File: LICENSE
 
 # Venomics-API-Client
 
 [![PyPI version fury.io](https://badge.fury.io/py/venomics-client.svg)](https://pypi.org/project/venomics-client/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/venomics-client.svg)](https://pypi.python.org/pypi/venomics-client/)
 [![PyPI license](https://img.shields.io/pypi/l/venomics-client.svg)](https://pypi.python.org/pypi/venomics-client/)
-[![Downloads](https://pepy.tech/badge/venomics-client)](https://pepy.tech/project/venomics-client)
 
 The official API client and utilities to manage a Venomics instance written in Python.
 
 - [INSTALLATION](#installation)
 - [EXAMPLE SCRIPTS](#example-scripts)
```

### Comparing `venomics-client-0.1.0/README.md` & `venomics-client-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Venomics-API-Client
 
 [![PyPI version fury.io](https://badge.fury.io/py/venomics-client.svg)](https://pypi.org/project/venomics-client/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/venomics-client.svg)](https://pypi.python.org/pypi/venomics-client/)
 [![PyPI license](https://img.shields.io/pypi/l/venomics-client.svg)](https://pypi.python.org/pypi/venomics-client/)
-[![Downloads](https://pepy.tech/badge/venomics-client)](https://pepy.tech/project/venomics-client)
 
 The official API client and utilities to manage a Venomics instance written in Python.
 
 - [INSTALLATION](#installation)
 - [EXAMPLE SCRIPTS](#example-scripts)
```

### Comparing `venomics-client-0.1.0/setup.cfg` & `venomics-client-0.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = venomics-client
-version = 0.1.0
+version = 0.1.1
 description = Venomics API Client
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.venomics.xyz/
 keywords = Venomics, redoubt, API
 license = MIT
 classifiers =
```

### Comparing `venomics-client-0.1.0/venomics_client/client.py` & `venomics-client-0.1.1/venomics_client/client.py`

 * *Files identical despite different names*

### Comparing `venomics-client-0.1.0/venomics_client/date_ranges.py` & `venomics-client-0.1.1/venomics_client/date_ranges.py`

 * *Files identical despite different names*

### Comparing `venomics-client-0.1.0/venomics_client.egg-info/PKG-INFO` & `venomics-client-0.1.1/venomics_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venomics-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Venomics API Client
 Home-page: https://www.venomics.xyz/
 Author: maksymds
 Author-email: redoubt@devnull.ae
 License: MIT
 Project-URL: Github, https://github.com/Venomics/venomics-api-client
 Project-URL: Documentation, https://www.vebnomics.xyz/
@@ -26,15 +26,14 @@
 License-File: LICENSE
 
 # Venomics-API-Client
 
 [![PyPI version fury.io](https://badge.fury.io/py/venomics-client.svg)](https://pypi.org/project/venomics-client/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/venomics-client.svg)](https://pypi.python.org/pypi/venomics-client/)
 [![PyPI license](https://img.shields.io/pypi/l/venomics-client.svg)](https://pypi.python.org/pypi/venomics-client/)
-[![Downloads](https://pepy.tech/badge/venomics-client)](https://pepy.tech/project/venomics-client)
 
 The official API client and utilities to manage a Venomics instance written in Python.
 
 - [INSTALLATION](#installation)
 - [EXAMPLE SCRIPTS](#example-scripts)
```

