# Comparing `tmp/pymangaj-0.1.7.tar.gz` & `tmp/pymangaj-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymangaj-0.1.7.tar", last modified: Thu Jun  1 00:31:01 2023, max compression
+gzip compressed data, was "pymangaj-0.1.8.tar", last modified: Tue Jun  6 23:34:11 2023, max compression
```

## Comparing `pymangaj-0.1.7.tar` & `pymangaj-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 00:31:01.117208 pymangaj-0.1.7/
--rw-rw-rw-   0        0        0     1106 2023-05-02 22:15:56.000000 pymangaj-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     2208 2023-06-01 00:31:01.117208 pymangaj-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1533 2023-06-01 00:19:06.000000 pymangaj-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 00:31:01.087209 pymangaj-0.1.7/pymangaj/
--rw-rw-rw-   0        0        0       41 2023-05-30 04:12:41.000000 pymangaj-0.1.7/pymangaj/__init__.py
--rw-rw-rw-   0        0        0     2927 2023-06-01 00:19:10.000000 pymangaj-0.1.7/pymangaj/chapmanganato.py
--rw-rw-rw-   0        0        0     3324 2023-06-01 00:17:11.000000 pymangaj-0.1.7/pymangaj/mangalivre.py
--rw-rw-rw-   0        0        0     1665 2023-05-30 01:42:44.000000 pymangaj-0.1.7/pymangaj/muitomanga.py
--rw-rw-rw-   0        0        0     1177 2023-06-01 00:17:43.000000 pymangaj-0.1.7/pymangaj/pymangaj.py
-drwxrwxrwx   0        0        0        0 2023-06-01 00:31:01.115207 pymangaj-0.1.7/pymangaj.egg-info/
--rw-rw-rw-   0        0        0     2208 2023-06-01 00:31:00.000000 pymangaj-0.1.7/pymangaj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-06-01 00:31:00.000000 pymangaj-0.1.7/pymangaj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 00:31:00.000000 pymangaj-0.1.7/pymangaj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 00:31:00.000000 pymangaj-0.1.7/pymangaj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 00:31:01.117208 pymangaj-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      868 2023-06-01 00:27:48.000000 pymangaj-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:34:11.690978 pymangaj-0.1.8/
+-rw-rw-rw-   0        0        0     1106 2023-05-02 22:15:56.000000 pymangaj-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     3703 2023-06-06 23:34:11.688981 pymangaj-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1606 2023-06-06 23:29:50.000000 pymangaj-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 23:34:11.672977 pymangaj-0.1.8/pymangaj/
+-rw-rw-rw-   0        0        0       41 2023-05-30 04:12:41.000000 pymangaj-0.1.8/pymangaj/__init__.py
+-rw-rw-rw-   0        0        0     2927 2023-06-06 23:28:25.000000 pymangaj-0.1.8/pymangaj/chapmanganato.py
+-rw-rw-rw-   0        0        0     3324 2023-06-01 00:17:11.000000 pymangaj-0.1.8/pymangaj/mangalivre.py
+-rw-rw-rw-   0        0        0     1665 2023-05-30 01:42:44.000000 pymangaj-0.1.8/pymangaj/muitomanga.py
+-rw-rw-rw-   0        0        0     1177 2023-06-06 23:28:25.000000 pymangaj-0.1.8/pymangaj/pymangaj.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:34:11.686974 pymangaj-0.1.8/pymangaj.egg-info/
+-rw-rw-rw-   0        0        0     3703 2023-06-06 23:34:11.000000 pymangaj-0.1.8/pymangaj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-06-06 23:34:11.000000 pymangaj-0.1.8/pymangaj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 23:34:11.000000 pymangaj-0.1.8/pymangaj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-06 23:34:11.000000 pymangaj-0.1.8/pymangaj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 23:34:11.000000 pymangaj-0.1.8/pymangaj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1013 2023-06-06 23:31:39.000000 pymangaj-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 23:34:11.690978 pymangaj-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-06-06 23:28:25.000000 pymangaj-0.1.8/setup.py
```

### Comparing `pymangaj-0.1.7/LICENSE` & `pymangaj-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.7/README.md` & `pymangaj-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -37,7 +37,11 @@
 ## Contribution
 
 Contributions to pymangaj are welcome! If you have any bug reports, feature requests, or suggestions, please open an issue on the [GitHub repository](https://github.com/jjeanjacques10/pymangaj).
 
 ## Authors
 
 - [@jjeanjacques10](https://github.com/jjeanjacques10)
+
+## Contributors
+
+- [@fabiobarkoski](https://github.com/fabiobarkoski)
```

### Comparing `pymangaj-0.1.7/pymangaj/chapmanganato.py` & `pymangaj-0.1.8/pymangaj/chapmanganato.py`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.7/pymangaj/mangalivre.py` & `pymangaj-0.1.8/pymangaj/mangalivre.py`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.7/pymangaj/muitomanga.py` & `pymangaj-0.1.8/pymangaj/muitomanga.py`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.7/pymangaj/pymangaj.py` & `pymangaj-0.1.8/pymangaj/pymangaj.py`

 * *Files identical despite different names*

