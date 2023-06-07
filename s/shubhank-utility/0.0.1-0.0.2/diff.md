# Comparing `tmp/shubhank_utility-0.0.1.tar.gz` & `tmp/shubhank_utility-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shubhank_utility-0.0.1.tar", last modified: Wed Jun  7 20:53:45 2023, max compression
+gzip compressed data, was "shubhank_utility-0.0.2.tar", last modified: Wed Jun  7 21:01:12 2023, max compression
```

## Comparing `shubhank_utility-0.0.1.tar` & `shubhank_utility-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 20:53:45.728230 shubhank_utility-0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-06-07 18:58:17.000000 shubhank_utility-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1165 2023-06-07 20:53:45.728230 shubhank_utility-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-06-07 18:58:17.000000 shubhank_utility-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-06-07 20:53:45.730452 shubhank_utility-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1606 2023-06-07 20:53:33.000000 shubhank_utility-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 20:53:45.705364 shubhank_utility-0.0.1/shubhank_utility/
--rw-rw-rw-   0        0        0      950 2023-06-07 20:34:41.000000 shubhank_utility-0.0.1/shubhank_utility/__init__.py
--rw-rw-rw-   0        0        0     5497 2023-06-07 19:57:35.000000 shubhank_utility-0.0.1/shubhank_utility/database.py
--rw-rw-rw-   0        0        0     1166 2023-06-07 20:03:59.000000 shubhank_utility-0.0.1/shubhank_utility/fuzzy_match.py
--rw-rw-rw-   0        0        0     2943 2023-06-07 20:34:37.000000 shubhank_utility-0.0.1/shubhank_utility/pdf_download.py
--rw-rw-rw-   0        0        0     5596 2023-06-07 20:31:33.000000 shubhank_utility-0.0.1/shubhank_utility/utility.py
-drwxrwxrwx   0        0        0        0 2023-06-07 20:53:45.725963 shubhank_utility-0.0.1/shubhank_utility.egg-info/
--rw-rw-rw-   0        0        0     1165 2023-06-07 20:53:45.000000 shubhank_utility-0.0.1/shubhank_utility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-06-07 20:53:45.000000 shubhank_utility-0.0.1/shubhank_utility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 20:53:45.000000 shubhank_utility-0.0.1/shubhank_utility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-06-07 20:53:45.000000 shubhank_utility-0.0.1/shubhank_utility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-07 20:53:45.000000 shubhank_utility-0.0.1/shubhank_utility.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 21:01:12.424158 shubhank_utility-0.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-06-07 18:58:17.000000 shubhank_utility-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1165 2023-06-07 21:01:12.424158 shubhank_utility-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-06-07 18:58:17.000000 shubhank_utility-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-07 21:01:12.427229 shubhank_utility-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1636 2023-06-07 21:01:05.000000 shubhank_utility-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:01:12.395401 shubhank_utility-0.0.2/shubhank_utility/
+-rw-rw-rw-   0        0        0      950 2023-06-07 20:59:32.000000 shubhank_utility-0.0.2/shubhank_utility/__init__.py
+-rw-rw-rw-   0        0        0     5497 2023-06-07 19:57:35.000000 shubhank_utility-0.0.2/shubhank_utility/database.py
+-rw-rw-rw-   0        0        0     1166 2023-06-07 20:03:59.000000 shubhank_utility-0.0.2/shubhank_utility/fuzzy_match.py
+-rw-rw-rw-   0        0        0     2943 2023-06-07 20:34:37.000000 shubhank_utility-0.0.2/shubhank_utility/pdf_download.py
+-rw-rw-rw-   0        0        0     5596 2023-06-07 20:31:33.000000 shubhank_utility-0.0.2/shubhank_utility/utility.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:01:12.422288 shubhank_utility-0.0.2/shubhank_utility.egg-info/
+-rw-rw-rw-   0        0        0     1165 2023-06-07 21:01:12.000000 shubhank_utility-0.0.2/shubhank_utility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2023-06-07 21:01:12.000000 shubhank_utility-0.0.2/shubhank_utility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 21:01:12.000000 shubhank_utility-0.0.2/shubhank_utility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-06-07 21:01:12.000000 shubhank_utility-0.0.2/shubhank_utility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-07 21:01:12.000000 shubhank_utility-0.0.2/shubhank_utility.egg-info/top_level.txt
```

### Comparing `shubhank_utility-0.0.1/LICENSE` & `shubhank_utility-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shubhank_utility-0.0.1/PKG-INFO` & `shubhank_utility-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shubhank_utility
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for personal work
 Home-page: https://github.com/ShubhankSinghal/shubhank-utility
-Download-URL: https://github.com/ShubhankSinghal/shubhank-utility/archive/refs/tags/0.0.1.tar.gz
+Download-URL: https://github.com/ShubhankSinghal/shubhank-utility/archive/refs/tags/0.0.2.tar.gz
 Author: Shubhank Singhal
 Author-email: shubhank.singhal98@gmail.com
 License: MIT
 Keywords: SHUBHANK,SHUBHANKSINGHAL
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shubhank_utility-0.0.1/setup.py` & `shubhank_utility-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # from setuptools import setup
 from distutils.core import setup
 
 setup(
     name='shubhank_utility',
     packages=['shubhank_utility'],
-    version='0.0.1',
+    version='0.0.2',
     license='MIT',
     description='A Python package for personal work',
     author='Shubhank Singhal',
     author_email='shubhank.singhal98@gmail.com',
     url='https://github.com/ShubhankSinghal/shubhank-utility',
-    download_url='https://github.com/ShubhankSinghal/shubhank-utility/archive/refs/tags/0.0.1.tar.gz',
+    download_url='https://github.com/ShubhankSinghal/shubhank-utility/archive/refs/tags/0.0.2.tar.gz',
     keywords=['SHUBHANK', 'SHUBHANKSINGHAL'],
     install_requires = [
         'pymongo',
         'requests',
         'tldextract',
         'fuzzywuzzy',
         "bs4",
         "beautifulsoup4",
         "html5lib",
         "lxml",
         "pymssql",
         "python-Levenshtein",
         "pandas",
         "numpy",
-        "nltk"
+        "nltk",
+        "country-converter"
     ],
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 2',
```

### Comparing `shubhank_utility-0.0.1/shubhank_utility/__init__.py` & `shubhank_utility-0.0.2/shubhank_utility/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 shubhank_utility.
 """
 
-_version_ = "0.0.1"
+_version_ = "0.0.2"
 _author_ = 'Shubhank Singhal'
 _credits_ = 'Shubhank Singhal'
 
 
 import os
 import re
 import ast
```

### Comparing `shubhank_utility-0.0.1/shubhank_utility/database.py` & `shubhank_utility-0.0.2/shubhank_utility/database.py`

 * *Files identical despite different names*

### Comparing `shubhank_utility-0.0.1/shubhank_utility/fuzzy_match.py` & `shubhank_utility-0.0.2/shubhank_utility/fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `shubhank_utility-0.0.1/shubhank_utility/pdf_download.py` & `shubhank_utility-0.0.2/shubhank_utility/pdf_download.py`

 * *Files identical despite different names*

### Comparing `shubhank_utility-0.0.1/shubhank_utility/utility.py` & `shubhank_utility-0.0.2/shubhank_utility/utility.py`

 * *Files identical despite different names*

### Comparing `shubhank_utility-0.0.1/shubhank_utility.egg-info/PKG-INFO` & `shubhank_utility-0.0.2/shubhank_utility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shubhank-utility
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for personal work
 Home-page: https://github.com/ShubhankSinghal/shubhank-utility
-Download-URL: https://github.com/ShubhankSinghal/shubhank-utility/archive/refs/tags/0.0.1.tar.gz
+Download-URL: https://github.com/ShubhankSinghal/shubhank-utility/archive/refs/tags/0.0.2.tar.gz
 Author: Shubhank Singhal
 Author-email: shubhank.singhal98@gmail.com
 License: MIT
 Keywords: SHUBHANK,SHUBHANKSINGHAL
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

