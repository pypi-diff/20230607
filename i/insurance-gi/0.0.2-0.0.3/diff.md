# Comparing `tmp/insurance_gi-0.0.2.tar.gz` & `tmp/insurance_gi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insurance_gi-0.0.2.tar", last modified: Mon Jun  5 16:28:42 2023, max compression
+gzip compressed data, was "insurance_gi-0.0.3.tar", last modified: Wed Jun  7 13:39:11 2023, max compression
```

## Comparing `insurance_gi-0.0.2.tar` & `insurance_gi-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:28:42.088824 insurance_gi-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 16:28:32.000000 insurance_gi-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 16:28:32.000000 insurance_gi-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-05 16:28:42.088824 insurance_gi-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-05 16:28:32.000000 insurance_gi-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:28:42.088824 insurance_gi-0.0.2/insurance_gi/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 16:28:32.000000 insurance_gi-0.0.2/insurance_gi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-05 16:28:32.000000 insurance_gi-0.0.2/insurance_gi/claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-05 16:28:32.000000 insurance_gi-0.0.2/insurance_gi/decrements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-05 16:28:32.000000 insurance_gi-0.0.2/insurance_gi/financials.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-06-05 16:28:32.000000 insurance_gi-0.0.2/insurance_gi/renewals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:28:42.088824 insurance_gi-0.0.2/insurance_gi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-05 16:28:42.000000 insurance_gi-0.0.2/insurance_gi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-05 16:28:42.000000 insurance_gi-0.0.2/insurance_gi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:28:42.000000 insurance_gi-0.0.2/insurance_gi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 16:28:42.000000 insurance_gi-0.0.2/insurance_gi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 16:28:42.000000 insurance_gi-0.0.2/insurance_gi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 16:28:32.000000 insurance_gi-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:28:42.088824 insurance_gi-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-05 16:28:32.000000 insurance_gi-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:39:11.103315 insurance_gi-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-07 13:38:59.000000 insurance_gi-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-07 13:38:59.000000 insurance_gi-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-07 13:39:11.103315 insurance_gi-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-07 13:38:59.000000 insurance_gi-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:39:11.103315 insurance_gi-0.0.3/insurance_gi/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-07 13:38:59.000000 insurance_gi-0.0.3/insurance_gi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-07 13:38:59.000000 insurance_gi-0.0.3/insurance_gi/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-07 13:38:59.000000 insurance_gi-0.0.3/insurance_gi/decrements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-07 13:38:59.000000 insurance_gi-0.0.3/insurance_gi/financials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-06-07 13:38:59.000000 insurance_gi-0.0.3/insurance_gi/renewals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:39:11.103315 insurance_gi-0.0.3/insurance_gi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-07 13:39:11.000000 insurance_gi-0.0.3/insurance_gi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-07 13:39:11.000000 insurance_gi-0.0.3/insurance_gi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:39:11.000000 insurance_gi-0.0.3/insurance_gi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 13:39:11.000000 insurance_gi-0.0.3/insurance_gi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 13:39:11.000000 insurance_gi-0.0.3/insurance_gi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 13:38:59.000000 insurance_gi-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:39:11.103315 insurance_gi-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-07 13:38:59.000000 insurance_gi-0.0.3/setup.py
```

### Comparing `insurance_gi-0.0.2/LICENSE` & `insurance_gi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `insurance_gi-0.0.2/PKG-INFO` & `insurance_gi-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insurance_gi
-Version: 0.0.2
+Version: 0.0.3
 Summary: GI projection tools
 Home-page: https://github.com/pdavidsonFIA/insurance_gi
 Author: Peter Davidson
 Author-email: peterjd41@gmail.com
 Project-URL: Bug Tracker, https://github.com/pdavidsonFIA/insurance_gi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `insurance_gi-0.0.2/insurance_gi/decrements.py` & `insurance_gi-0.0.3/insurance_gi/decrements.py`

 * *Files identical despite different names*

### Comparing `insurance_gi-0.0.2/insurance_gi/financials.py` & `insurance_gi-0.0.3/insurance_gi/financials.py`

 * *Files identical despite different names*

### Comparing `insurance_gi-0.0.2/insurance_gi/renewals.py` & `insurance_gi-0.0.3/insurance_gi/renewals.py`

 * *Files identical despite different names*

### Comparing `insurance_gi-0.0.2/insurance_gi.egg-info/PKG-INFO` & `insurance_gi-0.0.3/insurance_gi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insurance-gi
-Version: 0.0.2
+Version: 0.0.3
 Summary: GI projection tools
 Home-page: https://github.com/pdavidsonFIA/insurance_gi
 Author: Peter Davidson
 Author-email: peterjd41@gmail.com
 Project-URL: Bug Tracker, https://github.com/pdavidsonFIA/insurance_gi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `insurance_gi-0.0.2/setup.py` & `insurance_gi-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as f:
     dependencies = f.read().splitlines()
 
 setuptools.setup(
     name="insurance_gi",
-    version="0.0.2",
+    version="0.0.3",
     author="Peter Davidson",
     author_email="peterjd41@gmail.com",
     description="GI projection tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pdavidsonFIA/insurance_gi",
     project_urls={
```

