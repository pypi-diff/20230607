# Comparing `tmp/sk_calculator-0.1.0.tar.gz` & `tmp/sk_calculator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sk_calculator-0.1.0.tar", last modified: Wed Jun  7 17:05:38 2023, max compression
+gzip compressed data, was "sk_calculator-1.0.1.tar", last modified: Wed Jun  7 17:12:17 2023, max compression
```

## Comparing `sk_calculator-0.1.0.tar` & `sk_calculator-1.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 17:05:38.530552 sk_calculator-0.1.0/
--rw-rw-rw-   0        0        0     1055 2023-06-07 13:28:37.000000 sk_calculator-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     7534 2023-06-07 17:05:38.530552 sk_calculator-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7059 2023-06-07 13:56:25.000000 sk_calculator-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 17:05:38.530552 sk_calculator-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-06-07 17:05:33.000000 sk_calculator-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:05:38.280566 sk_calculator-0.1.0/sk_calculator/
--rw-rw-rw-   0        0        0     3810 2023-06-07 16:42:47.000000 sk_calculator-0.1.0/sk_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:05:38.358675 sk_calculator-0.1.0/sk_calculator/controller/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-0.1.0/sk_calculator/controller/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-06-05 15:11:16.000000 sk_calculator-0.1.0/sk_calculator/controller/base.py
--rw-rw-rw-   0        0        0     1169 2023-06-07 06:11:55.000000 sk_calculator-0.1.0/sk_calculator/controller/bracket.py
--rw-rw-rw-   0        0        0      689 2023-06-07 06:12:04.000000 sk_calculator-0.1.0/sk_calculator/controller/default.py
--rw-rw-rw-   0        0        0      841 2023-06-07 06:08:13.000000 sk_calculator-0.1.0/sk_calculator/controller/error.py
--rw-rw-rw-   0        0        0     4859 2023-06-07 06:08:03.000000 sk_calculator-0.1.0/sk_calculator/controller/function.py
--rw-rw-rw-   0        0        0     1038 2023-06-07 06:10:42.000000 sk_calculator-0.1.0/sk_calculator/controller/process.py
--rw-rw-rw-   0        0        0      837 2023-06-07 06:16:00.000000 sk_calculator-0.1.0/sk_calculator/controller/recorder.py
--rw-rw-rw-   0        0        0     3170 2023-06-07 05:57:35.000000 sk_calculator-0.1.0/sk_calculator/controller/validation.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:05:38.436802 sk_calculator-0.1.0/sk_calculator/function/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-0.1.0/sk_calculator/function/__init__.py
--rw-rw-rw-   0        0        0      651 2023-06-07 06:07:12.000000 sk_calculator-0.1.0/sk_calculator/function/abs.py
--rw-rw-rw-   0        0        0      700 2023-06-07 06:07:43.000000 sk_calculator-0.1.0/sk_calculator/function/default.py
--rw-rw-rw-   0        0        0      669 2023-06-07 06:07:23.000000 sk_calculator-0.1.0/sk_calculator/function/exp.py
--rw-rw-rw-   0        0        0      829 2023-06-07 06:07:35.000000 sk_calculator-0.1.0/sk_calculator/function/ln.py
--rw-rw-rw-   0        0        0     1091 2023-06-07 06:07:29.000000 sk_calculator-0.1.0/sk_calculator/function/log.py
--rw-rw-rw-   0        0        0      691 2023-06-07 06:07:03.000000 sk_calculator-0.1.0/sk_calculator/function/sqrt.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:05:38.452428 sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/__init__.py
--rw-rw-rw-   0        0        0      764 2023-06-07 06:04:47.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/cos.py
--rw-rw-rw-   0        0        0     1030 2023-06-07 06:05:03.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/cosec.py
--rw-rw-rw-   0        0        0     1056 2023-06-07 06:05:15.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/cot.py
--rw-rw-rw-   0        0        0     1059 2023-06-07 06:05:08.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/sec.py
--rw-rw-rw-   0        0        0      773 2023-06-07 06:03:41.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/sin.py
--rw-rw-rw-   0        0        0     1050 2023-06-07 06:04:57.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/tan.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:05:38.499299 sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/__init__.py
--rw-rw-rw-   0        0        0      817 2023-06-07 06:05:28.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/acos.py
--rw-rw-rw-   0        0        0      815 2023-06-07 06:06:20.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/acosec.py
--rw-rw-rw-   0        0        0      809 2023-06-07 06:06:32.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/acot.py
--rw-rw-rw-   0        0        0      811 2023-06-07 06:06:26.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/asec.py
--rw-rw-rw-   0        0        0      819 2023-06-07 06:05:23.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/asin.py
--rw-rw-rw-   0        0        0      631 2023-06-07 06:06:15.000000 sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/atan.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:05:38.530552 sk_calculator-0.1.0/sk_calculator/operations/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-0.1.0/sk_calculator/operations/__init__.py
--rw-rw-rw-   0        0        0     1150 2023-06-07 06:12:39.000000 sk_calculator-0.1.0/sk_calculator/operations/addition.py
--rw-rw-rw-   0        0        0      885 2023-06-05 15:11:16.000000 sk_calculator-0.1.0/sk_calculator/operations/bracket.py
--rw-rw-rw-   0        0        0     1297 2023-06-07 06:13:00.000000 sk_calculator-0.1.0/sk_calculator/operations/division.py
--rw-rw-rw-   0        0        0      964 2023-06-07 06:13:11.000000 sk_calculator-0.1.0/sk_calculator/operations/mod.py
--rw-rw-rw-   0        0        0     1131 2023-06-07 06:12:54.000000 sk_calculator-0.1.0/sk_calculator/operations/multiplication.py
--rw-rw-rw-   0        0        0      967 2023-06-07 06:13:05.000000 sk_calculator-0.1.0/sk_calculator/operations/power.py
--rw-rw-rw-   0        0        0     1136 2023-06-07 06:12:45.000000 sk_calculator-0.1.0/sk_calculator/operations/substraction.py
--rw-rw-rw-   0        0        0     1045 2023-06-07 06:12:17.000000 sk_calculator-0.1.0/sk_calculator/operations/unary.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:05:38.327429 sk_calculator-0.1.0/sk_calculator.egg-info/
--rw-rw-rw-   0        0        0     7534 2023-06-07 17:05:37.000000 sk_calculator-0.1.0/sk_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1973 2023-06-07 17:05:38.000000 sk_calculator-0.1.0/sk_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 17:05:37.000000 sk_calculator-0.1.0/sk_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-07 17:05:37.000000 sk_calculator-0.1.0/sk_calculator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-06-07 17:05:37.000000 sk_calculator-0.1.0/sk_calculator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 17:05:37.000000 sk_calculator-0.1.0/sk_calculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 17:12:17.550366 sk_calculator-1.0.1/
+-rw-rw-rw-   0        0        0     1055 2023-06-07 13:28:37.000000 sk_calculator-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     7592 2023-06-07 17:12:17.550366 sk_calculator-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7117 2023-06-07 17:11:13.000000 sk_calculator-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 17:12:17.550366 sk_calculator-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      928 2023-06-07 17:10:06.000000 sk_calculator-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:12:17.284740 sk_calculator-1.0.1/sk_calculator/
+-rw-rw-rw-   0        0        0     3517 2023-06-07 17:08:43.000000 sk_calculator-1.0.1/sk_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:12:17.378491 sk_calculator-1.0.1/sk_calculator/controller/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.1/sk_calculator/controller/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-06-05 15:11:16.000000 sk_calculator-1.0.1/sk_calculator/controller/base.py
+-rw-rw-rw-   0        0        0     1169 2023-06-07 06:11:55.000000 sk_calculator-1.0.1/sk_calculator/controller/bracket.py
+-rw-rw-rw-   0        0        0      689 2023-06-07 06:12:04.000000 sk_calculator-1.0.1/sk_calculator/controller/default.py
+-rw-rw-rw-   0        0        0      841 2023-06-07 06:08:13.000000 sk_calculator-1.0.1/sk_calculator/controller/error.py
+-rw-rw-rw-   0        0        0     4859 2023-06-07 06:08:03.000000 sk_calculator-1.0.1/sk_calculator/controller/function.py
+-rw-rw-rw-   0        0        0     1038 2023-06-07 06:10:42.000000 sk_calculator-1.0.1/sk_calculator/controller/process.py
+-rw-rw-rw-   0        0        0      837 2023-06-07 06:16:00.000000 sk_calculator-1.0.1/sk_calculator/controller/recorder.py
+-rw-rw-rw-   0        0        0     3170 2023-06-07 05:57:35.000000 sk_calculator-1.0.1/sk_calculator/controller/validation.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:12:17.409739 sk_calculator-1.0.1/sk_calculator/function/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.1/sk_calculator/function/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-06-07 06:07:12.000000 sk_calculator-1.0.1/sk_calculator/function/abs.py
+-rw-rw-rw-   0        0        0      700 2023-06-07 06:07:43.000000 sk_calculator-1.0.1/sk_calculator/function/default.py
+-rw-rw-rw-   0        0        0      669 2023-06-07 06:07:23.000000 sk_calculator-1.0.1/sk_calculator/function/exp.py
+-rw-rw-rw-   0        0        0      829 2023-06-07 06:07:35.000000 sk_calculator-1.0.1/sk_calculator/function/ln.py
+-rw-rw-rw-   0        0        0     1091 2023-06-07 06:07:29.000000 sk_calculator-1.0.1/sk_calculator/function/log.py
+-rw-rw-rw-   0        0        0      691 2023-06-07 06:07:03.000000 sk_calculator-1.0.1/sk_calculator/function/sqrt.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:12:17.472240 sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/__init__.py
+-rw-rw-rw-   0        0        0      764 2023-06-07 06:04:47.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/cos.py
+-rw-rw-rw-   0        0        0     1030 2023-06-07 06:05:03.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/cosec.py
+-rw-rw-rw-   0        0        0     1056 2023-06-07 06:05:15.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/cot.py
+-rw-rw-rw-   0        0        0     1059 2023-06-07 06:05:08.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/sec.py
+-rw-rw-rw-   0        0        0      773 2023-06-07 06:03:41.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/sin.py
+-rw-rw-rw-   0        0        0     1050 2023-06-07 06:04:57.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/tan.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:12:17.503491 sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-06-07 06:05:28.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/acos.py
+-rw-rw-rw-   0        0        0      815 2023-06-07 06:06:20.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/acosec.py
+-rw-rw-rw-   0        0        0      809 2023-06-07 06:06:32.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/acot.py
+-rw-rw-rw-   0        0        0      811 2023-06-07 06:06:26.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/asec.py
+-rw-rw-rw-   0        0        0      819 2023-06-07 06:05:23.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/asin.py
+-rw-rw-rw-   0        0        0      631 2023-06-07 06:06:15.000000 sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/atan.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:12:17.550366 sk_calculator-1.0.1/sk_calculator/operations/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.1/sk_calculator/operations/__init__.py
+-rw-rw-rw-   0        0        0     1150 2023-06-07 06:12:39.000000 sk_calculator-1.0.1/sk_calculator/operations/addition.py
+-rw-rw-rw-   0        0        0      885 2023-06-05 15:11:16.000000 sk_calculator-1.0.1/sk_calculator/operations/bracket.py
+-rw-rw-rw-   0        0        0     1297 2023-06-07 06:13:00.000000 sk_calculator-1.0.1/sk_calculator/operations/division.py
+-rw-rw-rw-   0        0        0      964 2023-06-07 06:13:11.000000 sk_calculator-1.0.1/sk_calculator/operations/mod.py
+-rw-rw-rw-   0        0        0     1131 2023-06-07 06:12:54.000000 sk_calculator-1.0.1/sk_calculator/operations/multiplication.py
+-rw-rw-rw-   0        0        0      967 2023-06-07 06:13:05.000000 sk_calculator-1.0.1/sk_calculator/operations/power.py
+-rw-rw-rw-   0        0        0     1136 2023-06-07 06:12:45.000000 sk_calculator-1.0.1/sk_calculator/operations/substraction.py
+-rw-rw-rw-   0        0        0     1045 2023-06-07 06:12:17.000000 sk_calculator-1.0.1/sk_calculator/operations/unary.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:12:17.331614 sk_calculator-1.0.1/sk_calculator.egg-info/
+-rw-rw-rw-   0        0        0     7592 2023-06-07 17:12:17.000000 sk_calculator-1.0.1/sk_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1973 2023-06-07 17:12:17.000000 sk_calculator-1.0.1/sk_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 17:12:17.000000 sk_calculator-1.0.1/sk_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-07 17:12:17.000000 sk_calculator-1.0.1/sk_calculator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-06-07 17:12:17.000000 sk_calculator-1.0.1/sk_calculator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 17:12:17.000000 sk_calculator-1.0.1/sk_calculator.egg-info/top_level.txt
```

### Comparing `sk_calculator-0.1.0/LICENSE.txt` & `sk_calculator-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/PKG-INFO` & `sk_calculator-1.0.1/sk_calculator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sk_calculator
-Version: 0.1.0
+Name: sk-calculator
+Version: 1.0.1
 Summary: A simple calculator program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,calculator,python calculator,gk calculator,advanced calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,24 +21,28 @@
 - Unary operators: positive and negative signs
 - Evaluation of expressions inside brackets
 - Trigonometric functions: sin, cos, tan, cosec, sec, and cot
 - Inverse trigonometric functions: asin, acos, atan
 
 ## Getting Started
 
-//
+Install by command
+```
+pip install sk_calculator
+```
+
 
 ## Usage
 
 To evaluate an arithmetic expression, create an instance of the `Calculator` class and call the `evaluate` method, passing the expression as a string parameter. The method will return the result of the evaluation.
 
 Here's an example:
 
 ```python
-from calculator import Calculator
+from sk_calculator import Calculator
 
 # Create an instance of the Calculator class
 calculator = Calculator()
 
 # Evaluate an arithmetic expression
 result = calculator.evaluate('2 + 3 * 4')
 print(result)  # Output: 14
```

### Comparing `sk_calculator-0.1.0/README.md` & `sk_calculator-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,28 @@
 - Unary operators: positive and negative signs
 - Evaluation of expressions inside brackets
 - Trigonometric functions: sin, cos, tan, cosec, sec, and cot
 - Inverse trigonometric functions: asin, acos, atan
 
 ## Getting Started
 
-//
+Install by command
+```
+pip install sk_calculator
+```
+
 
 ## Usage
 
 To evaluate an arithmetic expression, create an instance of the `Calculator` class and call the `evaluate` method, passing the expression as a string parameter. The method will return the result of the evaluation.
 
 Here's an example:
 
 ```python
-from calculator import Calculator
+from sk_calculator import Calculator
 
 # Create an instance of the Calculator class
 calculator = Calculator()
 
 # Evaluate an arithmetic expression
 result = calculator.evaluate('2 + 3 * 4')
 print(result)  # Output: 14
```

### Comparing `sk_calculator-0.1.0/setup.py` & `sk_calculator-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sk_calculator',
-    version='0.1.0',
+    version='1.0.1',
     description='A simple calculator program',
     author='gkibria',
     long_description=long_description,
     long_description_content_type="text/markdown",  # Specify the content type as Markdown
     author_email='gkibria121@gmail.com',
     packages=find_packages(),
     install_requires=['regex'],
```

### Comparing `sk_calculator-0.1.0/sk_calculator/__init__.py` & `sk_calculator-1.0.1/sk_calculator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,85 +10,82 @@
 from .operations.substraction import Substraction
 from .operations.multiplication import Multiplication
 from .operations.division import Division
 from .operations.power import Power
 from .operations.mod import Mod
 
 
-def main():
-    class Calculator:
 
+class Calculator:
 
-        def __init__(self):
 
+    def __init__(self):
 
-            self.error_handle = ErrorHandle()
-            self.default  =Default()
-            self.division = Division()
-            self.power = Power()
-            self.mod = Mod()
-            self.multiplication = Multiplication()
-            self.substraction = Substraction()
-            self.addition = Addition()
-            self.unary = Unary()
-            self.bracket = Brackets()
-            self.validation = Validation()
-            self.process = Process()
-            self.function = FunctionHandler()
-            self.recorder = Recorder()
-
-            ## set successor
-            self.power.set_successor (self.default)
-            self.mod.set_successor (self.power)
-            self.division.set_successor (self.mod)
-            self.multiplication.set_successor (self.division)
-            self.substraction.set_successor ( self.multiplication)
-            self.addition.set_successor ( self.substraction)
-            self.unary.set_successor(self.addition)
-            self.bracket.set_successor(self.unary)
-            self.function.set_successor (self.bracket)
-            self.process.set_successor (self.function)
-            self.validation.set_successor (self.process)
-
-            ## set error handler
-            self.division.set_error_handler (self.error_handle)
-            self.multiplication.set_error_handler (self.error_handle)
-            self.substraction.set_error_handler ( self.error_handle)
-            self.addition.set_error_handler (self.error_handle)
-            self.unary.set_error_handler(self.error_handle)
-            self.bracket.set_error_handler(self.error_handle)
-            self.validation.set_error_handler (self.error_handle)
-            self.default.set_error_handler(self.error_handle)
-            self.power.set_error_handler(self.error_handle)
-            self.function.set_error_handler(self.error_handle)
-            self.process.set_error_handler(self.error_handle)
-            self.mod.set_error_handler(self.error_handle)
-
-            ## set Recorder
-
-            self.division.set_recorder (self.recorder)
-            self.multiplication.set_recorder (self.recorder)
-            self.substraction.set_recorder ( self.recorder)
-            self.addition.set_recorder (self.recorder)
-            self.unary.set_recorder(self.recorder)
-            self.bracket.set_recorder(self.recorder)
-            self.validation.set_recorder (self.recorder)
-            self.default.set_recorder(self.recorder)
-            self.power.set_recorder(self.recorder)
-            self.mod.set_recorder(self.recorder)
-            self.function.set_recorder(self.recorder)
-            self.process.set_recorder(self.recorder)
-
-
-
-        def evaluate(self,expression):
-
-            self.error_handle.set_expression(expression)
-            self.recorder.set_expression(expression)
-            self.expression =  self.validation.evaluate(expression)
-            self.recorder.record(expression,self.expression,self.__class__.__name__)
-            return self.expression
 
-if __name__ == '__main__':
+        self.error_handle = ErrorHandle()
+        self.default  =Default()
+        self.division = Division()
+        self.power = Power()
+        self.mod = Mod()
+        self.multiplication = Multiplication()
+        self.substraction = Substraction()
+        self.addition = Addition()
+        self.unary = Unary()
+        self.bracket = Brackets()
+        self.validation = Validation()
+        self.process = Process()
+        self.function = FunctionHandler()
+        self.recorder = Recorder()
+
+        ## set successor
+        self.power.set_successor (self.default)
+        self.mod.set_successor (self.power)
+        self.division.set_successor (self.mod)
+        self.multiplication.set_successor (self.division)
+        self.substraction.set_successor ( self.multiplication)
+        self.addition.set_successor ( self.substraction)
+        self.unary.set_successor(self.addition)
+        self.bracket.set_successor(self.unary)
+        self.function.set_successor (self.bracket)
+        self.process.set_successor (self.function)
+        self.validation.set_successor (self.process)
+
+        ## set error handler
+        self.division.set_error_handler (self.error_handle)
+        self.multiplication.set_error_handler (self.error_handle)
+        self.substraction.set_error_handler ( self.error_handle)
+        self.addition.set_error_handler (self.error_handle)
+        self.unary.set_error_handler(self.error_handle)
+        self.bracket.set_error_handler(self.error_handle)
+        self.validation.set_error_handler (self.error_handle)
+        self.default.set_error_handler(self.error_handle)
+        self.power.set_error_handler(self.error_handle)
+        self.function.set_error_handler(self.error_handle)
+        self.process.set_error_handler(self.error_handle)
+        self.mod.set_error_handler(self.error_handle)
+
+        ## set Recorder
+
+        self.division.set_recorder (self.recorder)
+        self.multiplication.set_recorder (self.recorder)
+        self.substraction.set_recorder ( self.recorder)
+        self.addition.set_recorder (self.recorder)
+        self.unary.set_recorder(self.recorder)
+        self.bracket.set_recorder(self.recorder)
+        self.validation.set_recorder (self.recorder)
+        self.default.set_recorder(self.recorder)
+        self.power.set_recorder(self.recorder)
+        self.mod.set_recorder(self.recorder)
+        self.function.set_recorder(self.recorder)
+        self.process.set_recorder(self.recorder)
+
+
+
+    def evaluate(self,expression):
+
+        self.error_handle.set_expression(expression)
+        self.recorder.set_expression(expression)
+        self.expression =  self.validation.evaluate(expression)
+        self.recorder.record(expression,self.expression,self.__class__.__name__)
+        return self.expression
 
-    main()
```

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/base.py` & `sk_calculator-1.0.1/sk_calculator/controller/base.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/bracket.py` & `sk_calculator-1.0.1/sk_calculator/controller/bracket.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/default.py` & `sk_calculator-1.0.1/sk_calculator/controller/default.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/error.py` & `sk_calculator-1.0.1/sk_calculator/controller/error.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/function.py` & `sk_calculator-1.0.1/sk_calculator/controller/function.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/process.py` & `sk_calculator-1.0.1/sk_calculator/controller/process.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/recorder.py` & `sk_calculator-1.0.1/sk_calculator/controller/recorder.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/validation.py` & `sk_calculator-1.0.1/sk_calculator/controller/validation.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/abs.py` & `sk_calculator-1.0.1/sk_calculator/function/abs.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/default.py` & `sk_calculator-1.0.1/sk_calculator/function/default.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/exp.py` & `sk_calculator-1.0.1/sk_calculator/function/exp.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/ln.py` & `sk_calculator-1.0.1/sk_calculator/function/ln.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/log.py` & `sk_calculator-1.0.1/sk_calculator/function/log.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/sqrt.py` & `sk_calculator-1.0.1/sk_calculator/function/sqrt.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/cos.py` & `sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/cos.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/cosec.py` & `sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/cosec.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/cot.py` & `sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/cot.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/sec.py` & `sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/sec.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/sin.py` & `sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/sin.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/tan.py` & `sk_calculator-1.0.1/sk_calculator/function/trigonometric_function/tan.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/acos.py` & `sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/acos.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/acosec.py` & `sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/acosec.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/acot.py` & `sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/acot.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/asec.py` & `sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/asec.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/asin.py` & `sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/asin.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/atan.py` & `sk_calculator-1.0.1/sk_calculator/function/trigonometric_inverse_function/atan.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/addition.py` & `sk_calculator-1.0.1/sk_calculator/operations/addition.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/bracket.py` & `sk_calculator-1.0.1/sk_calculator/operations/bracket.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/division.py` & `sk_calculator-1.0.1/sk_calculator/operations/division.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/mod.py` & `sk_calculator-1.0.1/sk_calculator/operations/mod.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/multiplication.py` & `sk_calculator-1.0.1/sk_calculator/operations/multiplication.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/power.py` & `sk_calculator-1.0.1/sk_calculator/operations/power.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/substraction.py` & `sk_calculator-1.0.1/sk_calculator/operations/substraction.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/unary.py` & `sk_calculator-1.0.1/sk_calculator/operations/unary.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator.egg-info/PKG-INFO` & `sk_calculator-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sk-calculator
-Version: 0.1.0
+Name: sk_calculator
+Version: 1.0.1
 Summary: A simple calculator program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,calculator,python calculator,gk calculator,advanced calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,24 +21,28 @@
 - Unary operators: positive and negative signs
 - Evaluation of expressions inside brackets
 - Trigonometric functions: sin, cos, tan, cosec, sec, and cot
 - Inverse trigonometric functions: asin, acos, atan
 
 ## Getting Started
 
-//
+Install by command
+```
+pip install sk_calculator
+```
+
 
 ## Usage
 
 To evaluate an arithmetic expression, create an instance of the `Calculator` class and call the `evaluate` method, passing the expression as a string parameter. The method will return the result of the evaluation.
 
 Here's an example:
 
 ```python
-from calculator import Calculator
+from sk_calculator import Calculator
 
 # Create an instance of the Calculator class
 calculator = Calculator()
 
 # Evaluate an arithmetic expression
 result = calculator.evaluate('2 + 3 * 4')
 print(result)  # Output: 14
```

### Comparing `sk_calculator-0.1.0/sk_calculator.egg-info/SOURCES.txt` & `sk_calculator-1.0.1/sk_calculator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

