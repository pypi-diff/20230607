# Comparing `tmp/cosmoplots-0.2.0.tar.gz` & `tmp/cosmoplots-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmoplots-0.2.0.tar", max compression
+gzip compressed data, was "cosmoplots-0.2.1.tar", max compression
```

## Comparing `cosmoplots-0.2.0.tar` & `cosmoplots-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1076 2023-05-11 11:59:16.709257 cosmoplots-0.2.0/LICENSE
--rw-r--r--   0        0        0     3463 2023-05-11 11:59:16.709257 cosmoplots-0.2.0/README.md
--rw-r--r--   0        0        0       92 2023-05-11 11:59:16.713257 cosmoplots-0.2.0/cosmoplots/__init__.py
--rw-r--r--   0        0        0     1874 2023-05-11 11:59:16.713257 cosmoplots-0.2.0/cosmoplots/axes.py
--rw-r--r--   0        0        0     2723 2023-05-11 11:59:29.221358 cosmoplots-0.2.0/cosmoplots/colors.py
--rw-r--r--   0        0        0     5516 2023-05-11 11:59:16.713257 cosmoplots-0.2.0/cosmoplots/figure_defs.py
--rw-r--r--   0        0        0      485 2023-05-11 11:59:29.221358 cosmoplots-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4170 1970-01-01 00:00:00.000000 cosmoplots-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-07 12:54:21.676025 cosmoplots-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3463 2023-06-07 12:54:21.676025 cosmoplots-0.2.1/README.md
+-rw-r--r--   0        0        0      145 2023-06-07 12:54:38.512259 cosmoplots-0.2.1/cosmoplots/__init__.py
+-rw-r--r--   0        0        0     1874 2023-06-07 12:54:21.676025 cosmoplots-0.2.1/cosmoplots/axes.py
+-rw-r--r--   0        0        0     2723 2023-06-07 12:54:21.676025 cosmoplots-0.2.1/cosmoplots/colors.py
+-rw-r--r--   0        0        0     5516 2023-06-07 12:54:21.676025 cosmoplots-0.2.1/cosmoplots/figure_defs.py
+-rw-r--r--   0        0        0      515 2023-06-07 12:54:38.516259 cosmoplots-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 cosmoplots-0.2.1/PKG-INFO
```

### Comparing `cosmoplots-0.2.0/LICENSE` & `cosmoplots-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.2.0/README.md` & `cosmoplots-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.2.0/cosmoplots/axes.py` & `cosmoplots-0.2.1/cosmoplots/axes.py`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.2.0/cosmoplots/colors.py` & `cosmoplots-0.2.1/cosmoplots/colors.py`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.2.0/cosmoplots/figure_defs.py` & `cosmoplots-0.2.1/cosmoplots/figure_defs.py`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.2.0/PKG-INFO` & `cosmoplots-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cosmoplots
-Version: 0.2.0
+Version: 0.2.1
 Summary: Routines to get a sane default configuration for production quality plots.
 Home-page: https://github.com/uit-cosmo/cosmoplots
 License: MIT
 Author: gregordecristoforo
 Author-email: gregor.decristoforo@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0)
 Requires-Dist: matplotlib (>=3.3.2)
 Requires-Dist: numpy (>=1.15.0)
 Description-Content-Type: text/markdown
 
 # cosmoplots
 
 Routines to get a sane default configuration for production quality plots. Used by complex systems modelling group at UiT.
```

