# Comparing `tmp/sk_calculator-0.1.0.tar.gz` & `tmp/sk_calculator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sk_calculator-0.1.0.tar", last modified: Wed Jun  7 17:05:38 2023, max compression
+gzip compressed data, was "sk_calculator-1.0.2.tar", last modified: Wed Jun  7 17:45:57 2023, max compression
```

## Comparing `sk_calculator-0.1.0.tar` & `sk_calculator-1.0.2.tar`

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
+drwxrwxrwx   0        0        0        0 2023-06-07 17:45:57.113712 sk_calculator-1.0.2/
+-rw-rw-rw-   0        0        0     1055 2023-06-07 13:28:37.000000 sk_calculator-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     7592 2023-06-07 17:45:57.109716 sk_calculator-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7117 2023-06-07 17:11:13.000000 sk_calculator-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 17:45:57.113712 sk_calculator-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      928 2023-06-07 17:37:23.000000 sk_calculator-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:45:56.791038 sk_calculator-1.0.2/sk_calculator/
+-rw-rw-rw-   0        0        0     3517 2023-06-07 17:08:43.000000 sk_calculator-1.0.2/sk_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:45:56.910912 sk_calculator-1.0.2/sk_calculator/controller/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.2/sk_calculator/controller/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-06-05 15:11:16.000000 sk_calculator-1.0.2/sk_calculator/controller/base.py
+-rw-rw-rw-   0        0        0     1181 2023-06-07 17:26:18.000000 sk_calculator-1.0.2/sk_calculator/controller/bracket.py
+-rw-rw-rw-   0        0        0      701 2023-06-07 17:26:14.000000 sk_calculator-1.0.2/sk_calculator/controller/default.py
+-rw-rw-rw-   0        0        0      853 2023-06-07 17:26:10.000000 sk_calculator-1.0.2/sk_calculator/controller/error.py
+-rw-rw-rw-   0        0        0     5099 2023-06-07 17:25:55.000000 sk_calculator-1.0.2/sk_calculator/controller/function.py
+-rw-rw-rw-   0        0        0     1098 2023-06-07 17:25:17.000000 sk_calculator-1.0.2/sk_calculator/controller/process.py
+-rw-rw-rw-   0        0        0      849 2023-06-07 17:24:58.000000 sk_calculator-1.0.2/sk_calculator/controller/recorder.py
+-rw-rw-rw-   0        0        0     3314 2023-06-07 17:24:50.000000 sk_calculator-1.0.2/sk_calculator/controller/validation.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:45:56.943915 sk_calculator-1.0.2/sk_calculator/function/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.2/sk_calculator/function/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-06-07 17:27:06.000000 sk_calculator-1.0.2/sk_calculator/function/abs.py
+-rw-rw-rw-   0        0        0      712 2023-06-07 17:27:01.000000 sk_calculator-1.0.2/sk_calculator/function/default.py
+-rw-rw-rw-   0        0        0      681 2023-06-07 17:26:55.000000 sk_calculator-1.0.2/sk_calculator/function/exp.py
+-rw-rw-rw-   0        0        0      841 2023-06-07 17:26:50.000000 sk_calculator-1.0.2/sk_calculator/function/ln.py
+-rw-rw-rw-   0        0        0     1103 2023-06-07 17:26:45.000000 sk_calculator-1.0.2/sk_calculator/function/log.py
+-rw-rw-rw-   0        0        0      703 2023-06-07 17:26:41.000000 sk_calculator-1.0.2/sk_calculator/function/sqrt.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:45:57.015715 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/__init__.py
+-rw-rw-rw-   0        0        0      775 2023-06-07 17:27:56.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/cos.py
+-rw-rw-rw-   0        0        0     1041 2023-06-07 17:27:46.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/cosec.py
+-rw-rw-rw-   0        0        0     1067 2023-06-07 17:27:40.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/cot.py
+-rw-rw-rw-   0        0        0     1070 2023-06-07 17:27:35.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/sec.py
+-rw-rw-rw-   0        0        0      784 2023-06-07 17:27:28.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/sin.py
+-rw-rw-rw-   0        0        0     1061 2023-06-07 17:27:23.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/tan.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:45:57.059715 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/__init__.py
+-rw-rw-rw-   0        0        0      828 2023-06-07 17:28:38.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/acos.py
+-rw-rw-rw-   0        0        0      826 2023-06-07 17:28:34.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/acosec.py
+-rw-rw-rw-   0        0        0      820 2023-06-07 17:28:30.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/acot.py
+-rw-rw-rw-   0        0        0      822 2023-06-07 17:28:23.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/asec.py
+-rw-rw-rw-   0        0        0      830 2023-06-07 17:28:18.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/asin.py
+-rw-rw-rw-   0        0        0      642 2023-06-07 17:28:13.000000 sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/atan.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:45:57.101715 sk_calculator-1.0.2/sk_calculator/operations/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:11:16.000000 sk_calculator-1.0.2/sk_calculator/operations/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-07 17:29:25.000000 sk_calculator-1.0.2/sk_calculator/operations/addition.py
+-rw-rw-rw-   0        0        0      899 2023-06-07 17:29:40.000000 sk_calculator-1.0.2/sk_calculator/operations/bracket.py
+-rw-rw-rw-   0        0        0     1309 2023-06-07 17:29:18.000000 sk_calculator-1.0.2/sk_calculator/operations/division.py
+-rw-rw-rw-   0        0        0      976 2023-06-07 17:29:15.000000 sk_calculator-1.0.2/sk_calculator/operations/mod.py
+-rw-rw-rw-   0        0        0     1143 2023-06-07 17:29:10.000000 sk_calculator-1.0.2/sk_calculator/operations/multiplication.py
+-rw-rw-rw-   0        0        0      979 2023-06-07 17:29:06.000000 sk_calculator-1.0.2/sk_calculator/operations/power.py
+-rw-rw-rw-   0        0        0     1148 2023-06-07 17:29:01.000000 sk_calculator-1.0.2/sk_calculator/operations/substraction.py
+-rw-rw-rw-   0        0        0     1057 2023-06-07 17:28:56.000000 sk_calculator-1.0.2/sk_calculator/operations/unary.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:45:56.831910 sk_calculator-1.0.2/sk_calculator.egg-info/
+-rw-rw-rw-   0        0        0     7592 2023-06-07 17:45:56.000000 sk_calculator-1.0.2/sk_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1973 2023-06-07 17:45:56.000000 sk_calculator-1.0.2/sk_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 17:45:56.000000 sk_calculator-1.0.2/sk_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-07 17:45:56.000000 sk_calculator-1.0.2/sk_calculator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-06-07 17:45:56.000000 sk_calculator-1.0.2/sk_calculator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 17:45:56.000000 sk_calculator-1.0.2/sk_calculator.egg-info/top_level.txt
```

### Comparing `sk_calculator-0.1.0/LICENSE.txt` & `sk_calculator-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/PKG-INFO` & `sk_calculator-1.0.2/sk_calculator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sk_calculator
-Version: 0.1.0
+Name: sk-calculator
+Version: 1.0.2
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

### Comparing `sk_calculator-0.1.0/README.md` & `sk_calculator-1.0.2/README.md`

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

### Comparing `sk_calculator-0.1.0/setup.py` & `sk_calculator-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sk_calculator',
-    version='0.1.0',
+    version='1.0.2',
     description='A simple calculator program',
     author='gkibria',
     long_description=long_description,
     long_description_content_type="text/markdown",  # Specify the content type as Markdown
     author_email='gkibria121@gmail.com',
     packages=find_packages(),
     install_requires=['regex'],
```

### Comparing `sk_calculator-0.1.0/sk_calculator/__init__.py` & `sk_calculator-1.0.2/sk_calculator/__init__.py`

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

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/base.py` & `sk_calculator-1.0.2/sk_calculator/controller/base.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/bracket.py` & `sk_calculator-1.0.2/sk_calculator/controller/bracket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..controller.base import IOperation
+from sk_calculator.controller.base import IOperation
 import re
 class Brackets(IOperation):
 
 
     def evaluate(self,expression):
 
         self.expression = expression
```

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/default.py` & `sk_calculator-1.0.2/sk_calculator/controller/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..controller.base import IOperation
+from sk_calculator.controller.base import IOperation
 import re
 class Default(IOperation):
 
     def evaluate(self,exp):
         try:
             exp = float(exp)
```

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/error.py` & `sk_calculator-1.0.2/sk_calculator/controller/error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..controller.base import IErrorHandler
+from sk_calculator.controller.base import IErrorHandler
 
 class ErrorHandle(IErrorHandler):
 
     def __init__(self):
 
 
         self.errors = {}
```

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/function.py` & `sk_calculator-1.0.2/sk_calculator/controller/function.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from ..controller.base import IOperation
+from sk_calculator.controller.base import IOperation
 import re
 import regex
 import math
 
-from ..function.trigonometric_function.sin import Sin
-from ..function.trigonometric_function.cos import Cos
-from ..function.trigonometric_function.tan import Tan
-from ..function.trigonometric_function.cosec import Cosec
-from ..function.trigonometric_function.sec import Sec
-from ..function.trigonometric_function.cot import Cot
-from ..function.trigonometric_inverse_function.asin import Asin
-from ..function.trigonometric_inverse_function.acos import Acos
-from ..function.trigonometric_inverse_function.atan import Atan
-from ..function.trigonometric_inverse_function.acosec import Acosec
-from ..function.trigonometric_inverse_function.asec import Asec
-from ..function.trigonometric_inverse_function.acot import Acot
-from ..function.sqrt import Sqrt
-from ..function.abs import Abs
-from ..function.exp import Exp
-from ..function.log import Log
-from ..function.ln import Ln
-from ..function.default import Default
-from ..controller.error import ErrorHandle
+from sk_calculator.function.trigonometric_function.sin import Sin
+from sk_calculator.function.trigonometric_function.cos import Cos
+from sk_calculator.function.trigonometric_function.tan import Tan
+from sk_calculator.function.trigonometric_function.cosec import Cosec
+from sk_calculator.function.trigonometric_function.sec import Sec
+from sk_calculator.function.trigonometric_function.cot import Cot
+from sk_calculator.function.trigonometric_inverse_function.asin import Asin
+from sk_calculator.function.trigonometric_inverse_function.acos import Acos
+from sk_calculator.function.trigonometric_inverse_function.atan import Atan
+from sk_calculator.function.trigonometric_inverse_function.acosec import Acosec
+from sk_calculator.function.trigonometric_inverse_function.asec import Asec
+from sk_calculator.function.trigonometric_inverse_function.acot import Acot
+from sk_calculator.function.sqrt import Sqrt
+from sk_calculator.function.abs import Abs
+from sk_calculator.function.exp import Exp
+from sk_calculator.function.log import Log
+from sk_calculator.function.ln import Ln
+from sk_calculator.function.default import Default
+from sk_calculator.controller.error import ErrorHandle
 
 class FunctionHandler(IOperation):
 
     def __init__(self):
 
         self.sin = Sin()
         self.cos = Cos()
```

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/process.py` & `sk_calculator-1.0.2/sk_calculator/controller/process.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from ..controller.base import IOperation
+from sk_calculator.controller.base import IOperation
 
-from ..process.pi import Pi
-from ..process.e import E
-from ..process.space import Space
-from ..process.default import Default
+from sk_calculator.process.pi import Pi
+from sk_calculator.process.e import E
+from sk_calculator.process.space import Space
+from sk_calculator.process.default import Default
 
 class Process(IOperation):
 
     def __init__(self):
 
         self.pi = Pi()
         self.e = E()
```

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/recorder.py` & `sk_calculator-1.0.2/sk_calculator/controller/recorder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..controller.base import IRecorder
+from sk_calculator.controller.base import IRecorder
 
 class Recorder(IRecorder):
 
     def __init__(self):
 
         self.index = 0
```

### Comparing `sk_calculator-0.1.0/sk_calculator/controller/validation.py` & `sk_calculator-1.0.2/sk_calculator/controller/validation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from ..controller.base import IOperation
+from sk_calculator.controller.base import IOperation
 import re
 import math
-from ..validations.default import Default
-from ..validations.type_check import Typechecker
-from ..validations.division_check import DivsionErrorChecker
-from ..validations.parentheses_check import ParenthesesErrorChecker
-from ..validations.function_check import FunctionErrorChecker
-from ..validations.operator_check import OperatorErrorChecker
-from ..validations.keyword_check import KeywordChecker
-from ..validations.completion_check import CompletionErrorChecker
-from ..validations.key_check import UnsupportedKeyCheck
-from ..validations.constant_check import ConstantChecker
-from ..validations.number_check import NumberChecker
+from sk_calculator.validations.default import Default
+from sk_calculator.validations.type_check import Typechecker
+from sk_calculator.validations.division_check import DivsionErrorChecker
+from sk_calculator.validations.parentheses_check import ParenthesesErrorChecker
+from sk_calculator.validations.function_check import FunctionErrorChecker
+from sk_calculator.validations.operator_check import OperatorErrorChecker
+from sk_calculator.validations.keyword_check import KeywordChecker
+from sk_calculator.validations.completion_check import CompletionErrorChecker
+from sk_calculator.validations.key_check import UnsupportedKeyCheck
+from sk_calculator.validations.constant_check import ConstantChecker
+from sk_calculator.validations.number_check import NumberChecker
 
 class Validation(IOperation):
 
     def __init__(self):
         self.default = Default()
 
         self.type_check = Typechecker()
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/abs.py` & `sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/atan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-from ..controller.base import IFunction
-class Abs(IFunction):
+from sk_calculator.controller.base import IFunction
+import math
+class Atan(IFunction):
 
-    def evaluate(self,match):
-        if match[0] == 'abs':
-
-            try:
-                value = abs(float(match[1]))
-            except ValueError:
-                return self.error_handler.set_error("Math Error : Invalid type")
-            return round(value,9)
 
+    def evaluate(self,match):
+        if match[0] == 'atan':
+            atan = math.atan
+            radian =float(match[1])
+            value = atan(radian)
+            deg = math.degrees(value)
+            return round(deg,9)
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
+
+
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
+
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/default.py` & `sk_calculator-1.0.2/sk_calculator/function/abs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-from ..controller.base import IFunction
-import re
-class Default(IFunction):
-
-    def evaluate(self,exp):
-
-        if  ' ' in exp or exp == '':
-            return exp
-        try:
-            exp = float(exp)
-        except TypeError:
-            if (len(exp[0])!=1):
-                match = exp
-                error = 'Invalid Function Error : '+ match[0]+'()'
-                return self.error_handler.set_error(error)
-            error = 'Undefined Variable Error : ' + exp[0]
-            return self.error_handler.set_error(error)
+from sk_calculator.controller.base import IFunction
+class Abs(IFunction):
 
-        return exp
+    def evaluate(self,match):
+        if match[0] == 'abs':
 
-    def set_successor(self):
-        pass
+            try:
+                value = abs(float(match[1]))
+            except ValueError:
+                return self.error_handler.set_error("Math Error : Invalid type")
+            return round(value,9)
+
+        if(self.error_handler.get_error()):
+            return self.error_handler.get_error()
+
+        return self.successor.evaluate(match)
+    def set_successor(self,successor):
+
+        self.successor  = successor
 
     def set_error_handler(self,handler):
-        self.error_handler = handler
+        self.error_handler = handler
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/exp.py` & `sk_calculator-1.0.2/sk_calculator/function/exp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
 class Exp(IFunction):
 
     def evaluate(self,match):
         if match[0] == 'exp':
 
             try:
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/ln.py` & `sk_calculator-1.0.2/sk_calculator/function/ln.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
 import regex
 class Ln(IFunction):
 
     def evaluate(self,match):
         if match[0]=='ln' :
             try:
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/log.py` & `sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/cos.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,27 @@
-from ..controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
-import regex
-class Log(IFunction):
+class Cos(IFunction):
 
-    def evaluate(self,match):
-        if 'log' in match[0]:
-            base_pattern = '[a-zA-Z]+(\d+)'
-            base = regex.search(base_pattern,match[0])
-            try:
-                if match[0]=='log':
-                    value = math.log10(float(match[1]))
-                elif 'log' in match[0]:
-                    value = math.log(float(match[1]),float(base[1]))
-
-            except ValueError:
-
-                if (float(match[1])==0):
-                    return self.error_handler.set_error("Math Error: logarithm of zero")
-
-                return self.error_handler.set_error("Math Error: logarithm of a negative number")
-            return round(value,9)
 
+    def evaluate(self,match):
+        if match[0] == 'cos':
+            cos = math.cos
+            deg = math.radians(float(match[1]))
+            if match[2]=='degree':
+                deg = math.radians(float(match[1]))
+            if match[2] == 'radians':
+                deg = float(match[1])
+            value = cos(deg)
+            return  round(value,9)
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
+
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
+
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/sqrt.py` & `sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/acot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-from ..controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
-class Sqrt(IFunction):
+class Acot(IFunction):
 
-    def evaluate(self,match):
-        if match[0] == 'sqrt':
 
+    def evaluate(self,match):
+        if match[0] == 'acot':
             try:
-                value = math.sqrt(float(match[1]))
+                atan = math.atan
+                deg = float(match[1])
+                value = atan(1/deg)
+                degr = math.degrees(value)
+                return round(degr,9)
             except ValueError:
-                return self.error_handler.set_error("Math Error: Square Root Of A Negative Number")
-            return round(value,9)
-
+                self.error_handler.set_error(f'Math Error : Math Domain Error at {match[0]}({match[1]})')
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
+
+
+
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
+
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/cos.py` & `sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/sin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-from ...controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
-class Cos(IFunction):
+
+
+class Sin(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'cos':
-            cos = math.cos
+        if match[0] == 'sin':
+            sin = math.sin
             deg = math.radians(float(match[1]))
             if match[2]=='degree':
                 deg = math.radians(float(match[1]))
             if match[2] == 'radians':
                 deg = float(match[1])
-            value = cos(deg)
-            return  round(value,9)
+
+            value = sin(deg)
+            return round(value,9)
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
 
+
+
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/cosec.py` & `sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/sec.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from ...controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
-class Cosec(IFunction):
+class Sec(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'cosec':
+        if match[0] == 'sec':
             n =float(match[1]) /  90
             if match[2] == 'radians':
                 n = float(match[1])/(math.pi/2)
-            if n%2 == 0:
+            if n%2 != 0 and n.is_integer() and n%2 >= 1 :
                 return self.error_handler.set_error(f'Math Error: {match[0]}({match[1]}) is undefined')
-            sin = math.sin
+            cos = math.cos
             deg = math.radians(float(match[1]))
             if match[2]=='degree':
                 deg = math.radians(float(match[1]))
             if match[2] == 'radians':
                 deg = float(match[1])
-            value = 1/sin(deg)
+            value = 1/cos(deg)
             return round(value,9)
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/cot.py` & `sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/cot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
 class Cot(IFunction):
 
 
     def evaluate(self,match):
         if match[0] == 'cot':
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/sec.py` & `sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/tan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-from ...controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
-class Sec(IFunction):
+class Tan(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'sec':
+        if match[0] == 'tan':
             n =float(match[1]) /  90
             if match[2] == 'radians':
                 n = float(match[1])/(math.pi/2)
-            if n%2 != 0 and n.is_integer() and n%2 >= 1 :
+            if n%2 != 0 and n.is_integer() and n>=1:
                 return self.error_handler.set_error(f'Math Error: {match[0]}({match[1]}) is undefined')
-            cos = math.cos
+            tan = math.tan
             deg = math.radians(float(match[1]))
             if match[2]=='degree':
                 deg = math.radians(float(match[1]))
             if match[2] == 'radians':
                 deg = float(match[1])
-            value = 1/cos(deg)
+            value = tan(deg)
             return round(value,9)
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
 
 
-
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/sin.py` & `sk_calculator-1.0.2/sk_calculator/function/sqrt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,23 @@
-from ...controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
-
-
-class Sin(IFunction):
-
+class Sqrt(IFunction):
 
     def evaluate(self,match):
-        if match[0] == 'sin':
-            sin = math.sin
-            deg = math.radians(float(match[1]))
-            if match[2]=='degree':
-                deg = math.radians(float(match[1]))
-            if match[2] == 'radians':
-                deg = float(match[1])
+        if match[0] == 'sqrt':
 
-            value = sin(deg)
+            try:
+                value = math.sqrt(float(match[1]))
+            except ValueError:
+                return self.error_handler.set_error("Math Error: Square Root Of A Negative Number")
             return round(value,9)
+
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
-
-
-
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
-
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_function/tan.py` & `sk_calculator-1.0.2/sk_calculator/function/trigonometric_function/cosec.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from ...controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
-class Tan(IFunction):
+class Cosec(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'tan':
+        if match[0] == 'cosec':
             n =float(match[1]) /  90
             if match[2] == 'radians':
                 n = float(match[1])/(math.pi/2)
-            if n%2 != 0 and n.is_integer() and n>=1:
+            if n%2 == 0:
                 return self.error_handler.set_error(f'Math Error: {match[0]}({match[1]}) is undefined')
-            tan = math.tan
+            sin = math.sin
             deg = math.radians(float(match[1]))
             if match[2]=='degree':
                 deg = math.radians(float(match[1]))
             if match[2] == 'radians':
                 deg = float(match[1])
-            value = tan(deg)
+            value = 1/sin(deg)
             return round(value,9)
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
 
 
+
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/acos.py` & `sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/acos.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
 
 
 class Acos(IFunction):
 
 
     def evaluate(self,match):
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/acosec.py` & `sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/asin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-from ...controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
-class Acosec(IFunction):
+
+
+class Asin(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'acosec':
+        if match[0] == 'asin':
             try:
                 asin = math.asin
-                rad = float(match[1])
-                value = asin(1/rad)
-                value = math.degrees(value)
-                return round(value,9)
+                radians = float(match[1])
+                value = asin(radians)
+                deg = math.degrees(value)
+                return round(deg,9)
             except ValueError:
                 self.error_handler.set_error(f'Math Error : Math Domain Error at {match[0]}({match[1]})')
+
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/acot.py` & `sk_calculator-1.0.2/sk_calculator/function/trigonometric_inverse_function/asec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from ...controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
-class Acot(IFunction):
+class Asec(IFunction):
 
 
     def evaluate(self,match):
-        if match[0] == 'acot':
+        if match[0] == 'asec':
             try:
-                atan = math.atan
+                acos = math.acos
                 deg = float(match[1])
-                value = atan(1/deg)
-                degr = math.degrees(value)
-                return round(degr,9)
+                value = acos(1/deg)
+                value = math.degrees(value)
+                return round(value,9)
             except ValueError:
                 self.error_handler.set_error(f'Math Error : Math Domain Error at {match[0]}({match[1]})')
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/asec.py` & `sk_calculator-1.0.2/sk_calculator/operations/bracket.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-from ...controller.base import IFunction
-import math
-class Asec(IFunction):
-
-
-    def evaluate(self,match):
-        if match[0] == 'asec':
-            try:
-                acos = math.acos
-                deg = float(match[1])
-                value = acos(1/deg)
-                value = math.degrees(value)
-                return round(value,9)
-            except ValueError:
-                self.error_handler.set_error(f'Math Error : Math Domain Error at {match[0]}({match[1]})')
-        if(self.error_handler.get_error()):
-            return self.error_handler.get_error()
+from sk_calculator.controller.base import IOperation
+import re
+class Brackets(IOperation):
 
-        return self.successor.evaluate(match)
 
+    def evaluate(self,expression):
 
+        brackets = r'\([^()]+\)'
+        matches = re.findall(brackets,expression)
+
+
+
+        if matches:
+            while matches:
+                for match in matches:
+                    exp =match.replace('(','').replace(')','')
+                    evl = self.successor.evaluate(exp)
+                    expression = expression.replace(match,str(evl))
+                brackets = r'\([^()]+\)'
+                matches = re.findall(brackets,str(expression))
 
-    def set_successor(self,successor):
 
+        return self.successor.evaluate(expression)
+
+
+    def set_successor(self,successor):
         self.successor  = successor
 
     def set_error_handler(self,handler):
-        self.error_handler = handler
+        self.handler = handler
+    def set_recorder(self,recorder):
 
+            self.recorder = recorder
```

### Comparing `sk_calculator-0.1.0/sk_calculator/function/trigonometric_inverse_function/asin.py` & `sk_calculator-1.0.2/sk_calculator/function/log.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from ...controller.base import IFunction
+from sk_calculator.controller.base import IFunction
 import math
-
-
-class Asin(IFunction):
-
+import regex
+class Log(IFunction):
 
     def evaluate(self,match):
-        if match[0] == 'asin':
+        if 'log' in match[0]:
+            base_pattern = '[a-zA-Z]+(\d+)'
+            base = regex.search(base_pattern,match[0])
             try:
-                asin = math.asin
-                radians = float(match[1])
-                value = asin(radians)
-                deg = math.degrees(value)
-                return round(deg,9)
+                if match[0]=='log':
+                    value = math.log10(float(match[1]))
+                elif 'log' in match[0]:
+                    value = math.log(float(match[1]),float(base[1]))
+
             except ValueError:
-                self.error_handler.set_error(f'Math Error : Math Domain Error at {match[0]}({match[1]})')
+
+                if (float(match[1])==0):
+                    return self.error_handler.set_error("Math Error: logarithm of zero")
+
+                return self.error_handler.set_error("Math Error: logarithm of a negative number")
+            return round(value,9)
 
         if(self.error_handler.get_error()):
             return self.error_handler.get_error()
 
         return self.successor.evaluate(match)
-
-
-
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
         self.error_handler = handler
-
```

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/addition.py` & `sk_calculator-1.0.2/sk_calculator/operations/substraction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-from ..controller.base import IOperation
+from sk_calculator.controller.base import IOperation
 import re
-class Addition(IOperation):
+class Substraction(IOperation):
+
 
 
     def evaluate(self,expression):
 
-        add_pattern = r'(?<=\d)[+]'
+        sub_pattern = r'(?<=\d)-'
 
-        match = re.search(add_pattern,expression)
+        match = re.search(sub_pattern,expression)
 
         if match:
 
-            exp_list = re.split(add_pattern,expression)
+            exp_list = re.split(sub_pattern,expression)
+
             num_list = []
+
             for exp in exp_list:
                 num_list.append(self.successor.evaluate(exp))
             total =num_list[0]
 
-            if(self.error_handler.get_error()):
+            if(self.handler.get_error()):
 
-                return self.error_handler.get_error()
+                return self.handler.get_error()
 
             for num in num_list[1:]:
+                total = total - float(num)
 
-                total = total + float(num)
-                self.expression = str(total)
+            self.expression = str(total)
             if (self.expression != expression):
                 self.recorder.record(expression,self.expression,self.__class__.__name__)
             return total
 
         return self.successor.evaluate(expression)
 
     def set_successor(self,successor):
 
         self.successor  = successor
 
     def set_error_handler(self,handler):
-        self.error_handler = handler
+        self.handler = handler
+
     def set_recorder(self,recorder):
 
-            self.recorder = recorder
+            self.recorder = recorder
```

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/bracket.py` & `sk_calculator-1.0.2/sk_calculator/operations/addition.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,42 @@
-from controller.base import IOperation
+from sk_calculator.controller.base import IOperation
 import re
-class Brackets(IOperation):
+class Addition(IOperation):
 
 
     def evaluate(self,expression):
 
-        brackets = r'\([^()]+\)'
-        matches = re.findall(brackets,expression)
+        add_pattern = r'(?<=\d)[+]'
 
+        match = re.search(add_pattern,expression)
 
+        if match:
 
-        if matches:
-            while matches:
-                for match in matches:
-                    exp =match.replace('(','').replace(')','')
-                    evl = self.successor.evaluate(exp)
-                    expression = expression.replace(match,str(evl))
-                brackets = r'\([^()]+\)'
-                matches = re.findall(brackets,str(expression))
+            exp_list = re.split(add_pattern,expression)
+            num_list = []
+            for exp in exp_list:
+                num_list.append(self.successor.evaluate(exp))
+            total =num_list[0]
 
+            if(self.error_handler.get_error()):
 
-        return self.successor.evaluate(expression)
+                return self.error_handler.get_error()
+
+            for num in num_list[1:]:
 
+                total = total + float(num)
+                self.expression = str(total)
+            if (self.expression != expression):
+                self.recorder.record(expression,self.expression,self.__class__.__name__)
+            return total
+
+        return self.successor.evaluate(expression)
 
     def set_successor(self,successor):
+
         self.successor  = successor
 
     def set_error_handler(self,handler):
-        self.handler = handler
+        self.error_handler = handler
     def set_recorder(self,recorder):
 
-            self.recorder = recorder
+            self.recorder = recorder
```

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/division.py` & `sk_calculator-1.0.2/sk_calculator/operations/division.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..controller.base import IOperation
+from sk_calculator.controller.base import IOperation
 import re
 class Division(IOperation):
 
 
     def evaluate(self,expression):
 
         divide_pattern = r'(?<=\d)[/]'
```

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/mod.py` & `sk_calculator-1.0.2/sk_calculator/operations/mod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..controller.base import IOperation
+from sk_calculator.controller.base import IOperation
 import math
 import re
 class Mod(IOperation):
 
 
     def evaluate(self,expression):
```

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/multiplication.py` & `sk_calculator-1.0.2/sk_calculator/operations/multiplication.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..controller.base import IOperation
+from sk_calculator.controller.base import IOperation
 import re
 class Multiplication(IOperation):
 
 
     def evaluate(self,expression):
 
         mul_pattern = r'(?<=\d)[*]'
```

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/power.py` & `sk_calculator-1.0.2/sk_calculator/operations/power.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..controller.base import IOperation
+from sk_calculator.controller.base import IOperation
 import math
 import re
 class Power(IOperation):
 
 
     def evaluate(self,expression):
```

### Comparing `sk_calculator-0.1.0/sk_calculator/operations/unary.py` & `sk_calculator-1.0.2/sk_calculator/operations/unary.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..controller.base import IOperation
+from sk_calculator.controller.base import IOperation
 import re
 class Unary(IOperation):
 
 
 
     def evaluate(self,expression):
```

### Comparing `sk_calculator-0.1.0/sk_calculator.egg-info/PKG-INFO` & `sk_calculator-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sk-calculator
-Version: 0.1.0
+Name: sk_calculator
+Version: 1.0.2
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

### Comparing `sk_calculator-0.1.0/sk_calculator.egg-info/SOURCES.txt` & `sk_calculator-1.0.2/sk_calculator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

