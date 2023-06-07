# Comparing `tmp/formalmath-0.0.2.tar.gz` & `tmp/formalmath-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formalmath-0.0.2.tar", last modified: Wed Jun  7 05:24:45 2023, max compression
+gzip compressed data, was "formalmath-0.0.3.tar", last modified: Wed Jun  7 05:32:14 2023, max compression
```

## Comparing `formalmath-0.0.2.tar` & `formalmath-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 05:24:45.046319 formalmath-0.0.2/
--rw-rw-rw-   0        0        0     1452 2023-06-07 05:24:45.046319 formalmath-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2023-06-07 05:24:20.000000 formalmath-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 05:24:45.043319 formalmath-0.0.2/formalmath/
--rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.2/formalmath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:24:45.046319 formalmath-0.0.2/formalmath/setmm/
--rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.2/formalmath/setmm/__init__.py
--rw-rw-rw-   0        0        0     5539 2023-06-07 05:14:32.000000 formalmath-0.0.2/formalmath/setmm/basic_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:24:45.045319 formalmath-0.0.2/formalmath.egg-info/
--rw-rw-rw-   0        0        0     1452 2023-06-07 05:24:45.000000 formalmath-0.0.2/formalmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-07 05:24:45.000000 formalmath-0.0.2/formalmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 05:24:45.000000 formalmath-0.0.2/formalmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-07 05:24:45.000000 formalmath-0.0.2/formalmath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 05:24:45.046319 formalmath-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-06-07 05:18:14.000000 formalmath-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:32:14.011114 formalmath-0.0.3/
+-rw-rw-rw-   0        0        0     1647 2023-06-07 05:32:14.010114 formalmath-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2023-06-07 05:31:44.000000 formalmath-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 05:32:14.008114 formalmath-0.0.3/formalmath/
+-rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.3/formalmath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:32:14.010114 formalmath-0.0.3/formalmath/setmm/
+-rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.3/formalmath/setmm/__init__.py
+-rw-rw-rw-   0        0        0     5539 2023-06-07 05:14:32.000000 formalmath-0.0.3/formalmath/setmm/basic_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-07 05:32:14.009114 formalmath-0.0.3/formalmath.egg-info/
+-rw-rw-rw-   0        0        0     1647 2023-06-07 05:32:13.000000 formalmath-0.0.3/formalmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-07 05:32:13.000000 formalmath-0.0.3/formalmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 05:32:13.000000 formalmath-0.0.3/formalmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 05:32:13.000000 formalmath-0.0.3/formalmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 05:32:14.011114 formalmath-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-06-07 05:32:05.000000 formalmath-0.0.3/setup.py
```

### Comparing `formalmath-0.0.2/PKG-INFO` & `formalmath-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formalmath
-Version: 0.0.2
+Version: 0.0.3
 Summary: a python port of formal mathematics proof verifier.
 Home-page: https://github.com/lixiang90/formalmath.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,19 +15,19 @@
 
 A formal mathematics package.
 
 ## setmm
 
 A port for [metamath](https://us.metamath.org) and `set.mm`. The language `metamath` is a math proof verifying language. And, `set.mm` is its main database of theorems, based on the classical ZFC axiom system.
 
-`MObject` is the basic class. Any `MObject` have a label. Some of them have short_code or metamath_code.
+`MObject` is the basic class. Any `MObject` have a label. Some of them have short_code or metamath_code. The label system is unique (if you create a new MObject with the same label with existing one, the program will raise ValueError). So does the short_code and metamath_code.
 
  `Constant` is the class of constants, corresponding to $c statements in metamath.
 
-The port of other concepts in metamath and set.mm
+The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath import setmm
 test1 = MObject("x1")
 test2 = MObject("y1")
```

### Comparing `formalmath-0.0.2/README.md` & `formalmath-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 A formal mathematics package.
 
 ## setmm
 
 A port for [metamath](https://us.metamath.org) and `set.mm`. The language `metamath` is a math proof verifying language. And, `set.mm` is its main database of theorems, based on the classical ZFC axiom system.
 
-`MObject` is the basic class. Any `MObject` have a label. Some of them have short_code or metamath_code.
+`MObject` is the basic class. Any `MObject` have a label. Some of them have short_code or metamath_code. The label system is unique (if you create a new MObject with the same label with existing one, the program will raise ValueError). So does the short_code and metamath_code.
 
  `Constant` is the class of constants, corresponding to $c statements in metamath.
 
-The port of other concepts in metamath and set.mm
+The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath import setmm
 test1 = MObject("x1")
 test2 = MObject("y1")
```

### Comparing `formalmath-0.0.2/formalmath/setmm/basic_classes.py` & `formalmath-0.0.3/formalmath/setmm/basic_classes.py`

 * *Files identical despite different names*

### Comparing `formalmath-0.0.2/formalmath.egg-info/PKG-INFO` & `formalmath-0.0.3/formalmath.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formalmath
-Version: 0.0.2
+Version: 0.0.3
 Summary: a python port of formal mathematics proof verifier.
 Home-page: https://github.com/lixiang90/formalmath.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,19 +15,19 @@
 
 A formal mathematics package.
 
 ## setmm
 
 A port for [metamath](https://us.metamath.org) and `set.mm`. The language `metamath` is a math proof verifying language. And, `set.mm` is its main database of theorems, based on the classical ZFC axiom system.
 
-`MObject` is the basic class. Any `MObject` have a label. Some of them have short_code or metamath_code.
+`MObject` is the basic class. Any `MObject` have a label. Some of them have short_code or metamath_code. The label system is unique (if you create a new MObject with the same label with existing one, the program will raise ValueError). So does the short_code and metamath_code.
 
  `Constant` is the class of constants, corresponding to $c statements in metamath.
 
-The port of other concepts in metamath and set.mm
+The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath import setmm
 test1 = MObject("x1")
 test2 = MObject("y1")
```

### Comparing `formalmath-0.0.2/setup.py` & `formalmath-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="formalmath",  # Replace with your own username
-    version="0.0.2",
+    version="0.0.3",
     author="lixiang90",
     author_email="lixiang90@github.com",
     description="a python port of formal mathematics proof verifier.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lixiang90/formalmath.git",
     packages=setuptools.find_packages(),
```

