# Comparing `tmp/formalmath-0.0.3.tar.gz` & `tmp/formalmath-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formalmath-0.0.3.tar", last modified: Wed Jun  7 05:32:14 2023, max compression
+gzip compressed data, was "formalmath-0.0.4.tar", last modified: Wed Jun  7 05:37:03 2023, max compression
```

## Comparing `formalmath-0.0.3.tar` & `formalmath-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 05:32:14.011114 formalmath-0.0.3/
--rw-rw-rw-   0        0        0     1647 2023-06-07 05:32:14.010114 formalmath-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2023-06-07 05:31:44.000000 formalmath-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 05:32:14.008114 formalmath-0.0.3/formalmath/
--rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.3/formalmath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:32:14.010114 formalmath-0.0.3/formalmath/setmm/
--rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.3/formalmath/setmm/__init__.py
--rw-rw-rw-   0        0        0     5539 2023-06-07 05:14:32.000000 formalmath-0.0.3/formalmath/setmm/basic_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:32:14.009114 formalmath-0.0.3/formalmath.egg-info/
--rw-rw-rw-   0        0        0     1647 2023-06-07 05:32:13.000000 formalmath-0.0.3/formalmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-07 05:32:13.000000 formalmath-0.0.3/formalmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 05:32:13.000000 formalmath-0.0.3/formalmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-07 05:32:13.000000 formalmath-0.0.3/formalmath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 05:32:14.011114 formalmath-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-06-07 05:32:05.000000 formalmath-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:37:03.346152 formalmath-0.0.4/
+-rw-rw-rw-   0        0        0     1695 2023-06-07 05:37:03.346152 formalmath-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1249 2023-06-07 05:34:30.000000 formalmath-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 05:37:03.344153 formalmath-0.0.4/formalmath/
+-rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.4/formalmath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:37:03.346152 formalmath-0.0.4/formalmath/setmm/
+-rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.4/formalmath/setmm/__init__.py
+-rw-rw-rw-   0        0        0     5539 2023-06-07 05:14:32.000000 formalmath-0.0.4/formalmath/setmm/basic_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:37:03.345152 formalmath-0.0.4/formalmath.egg-info/
+-rw-rw-rw-   0        0        0     1695 2023-06-07 05:37:03.000000 formalmath-0.0.4/formalmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-07 05:37:03.000000 formalmath-0.0.4/formalmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 05:37:03.000000 formalmath-0.0.4/formalmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 05:37:03.000000 formalmath-0.0.4/formalmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 05:37:03.346152 formalmath-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-06-07 05:36:45.000000 formalmath-0.0.4/setup.py
```

### Comparing `formalmath-0.0.3/PKG-INFO` & `formalmath-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formalmath
-Version: 0.0.3
+Version: 0.0.4
 Summary: a python port of formal mathematics proof verifier.
 Home-page: https://github.com/lixiang90/formalmath.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,22 +25,22 @@
 
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath import setmm
-test1 = MObject("x1")
-test2 = MObject("y1")
-# test3 = MObject("x1")
+test1 = setmm.MObject("x1")
+test2 = setmm.MObject("y1")
+# test3 = setmm.MObject("x1")
 print(test1) # output: MObject("x1")
-test3 = MObject.find_MObject_by_label("y1")
+test3 = setmm.MObject.find_MObject_by_label("y1")
 print(test3) # output: MObject("y1")
 
-lp = Constant("\\left(")
-rp = Constant("\\right)")
-# lp2 = Constant("\\left(")
+lp = setmm.Constant("\\left(")
+rp = setmm.Constant("\\right)")
+# lp2 = setmm.Constant("\\left(")
 print(lp) # output: Constant("\left(")
-testConst = Constant.find_MObject_by_label("\\right)")
+testConst = setmm.Constant.find_MObject_by_label("\\right)")
 print(testConst) # output: Constant("\right)")
 ```
```

### Comparing `formalmath-0.0.3/README.md` & `formalmath-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath import setmm
-test1 = MObject("x1")
-test2 = MObject("y1")
-# test3 = MObject("x1")
+test1 = setmm.MObject("x1")
+test2 = setmm.MObject("y1")
+# test3 = setmm.MObject("x1")
 print(test1) # output: MObject("x1")
-test3 = MObject.find_MObject_by_label("y1")
+test3 = setmm.MObject.find_MObject_by_label("y1")
 print(test3) # output: MObject("y1")
 
-lp = Constant("\\left(")
-rp = Constant("\\right)")
-# lp2 = Constant("\\left(")
+lp = setmm.Constant("\\left(")
+rp = setmm.Constant("\\right)")
+# lp2 = setmm.Constant("\\left(")
 print(lp) # output: Constant("\left(")
-testConst = Constant.find_MObject_by_label("\\right)")
+testConst = setmm.Constant.find_MObject_by_label("\\right)")
 print(testConst) # output: Constant("\right)")
 ```
```

### Comparing `formalmath-0.0.3/formalmath/setmm/basic_classes.py` & `formalmath-0.0.4/formalmath/setmm/basic_classes.py`

 * *Files identical despite different names*

### Comparing `formalmath-0.0.3/formalmath.egg-info/PKG-INFO` & `formalmath-0.0.4/formalmath.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formalmath
-Version: 0.0.3
+Version: 0.0.4
 Summary: a python port of formal mathematics proof verifier.
 Home-page: https://github.com/lixiang90/formalmath.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,22 +25,22 @@
 
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath import setmm
-test1 = MObject("x1")
-test2 = MObject("y1")
-# test3 = MObject("x1")
+test1 = setmm.MObject("x1")
+test2 = setmm.MObject("y1")
+# test3 = setmm.MObject("x1")
 print(test1) # output: MObject("x1")
-test3 = MObject.find_MObject_by_label("y1")
+test3 = setmm.MObject.find_MObject_by_label("y1")
 print(test3) # output: MObject("y1")
 
-lp = Constant("\\left(")
-rp = Constant("\\right)")
-# lp2 = Constant("\\left(")
+lp = setmm.Constant("\\left(")
+rp = setmm.Constant("\\right)")
+# lp2 = setmm.Constant("\\left(")
 print(lp) # output: Constant("\left(")
-testConst = Constant.find_MObject_by_label("\\right)")
+testConst = setmm.Constant.find_MObject_by_label("\\right)")
 print(testConst) # output: Constant("\right)")
 ```
```

### Comparing `formalmath-0.0.3/setup.py` & `formalmath-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="formalmath",  # Replace with your own username
-    version="0.0.3",
+    version="0.0.4",
     author="lixiang90",
     author_email="lixiang90@github.com",
     description="a python port of formal mathematics proof verifier.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lixiang90/formalmath.git",
     packages=setuptools.find_packages(),
```

