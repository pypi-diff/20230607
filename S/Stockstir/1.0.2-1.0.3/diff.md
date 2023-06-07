# Comparing `tmp/stockstir-1.0.2.tar.gz` & `tmp/stockstir-1.0.3.tar.gz`

## Comparing `stockstir-1.0.2.tar` & `stockstir-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 stockstir-1.0.2/.DS_Store
--rw-r--r--   0        0        0    14876 2020-02-02 00:00:00.000000 stockstir-1.0.2/Documentation.md
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/code structure.rst
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/conf.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/credits.rst
--rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/function use.rst
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/index.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/installation.rst
--rw-r--r--   0        0        0   135557 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/img/stockstirlogo.jpeg
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 stockstir-1.0.2/src/Stockstir/__init__.py
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 stockstir-1.0.2/src/Stockstir/stockstir.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 stockstir-1.0.2/tests/README(GithubVersion).md
--rw-r--r--   0        0        0   135557 2020-02-02 00:00:00.000000 stockstir-1.0.2/tests/stockstir-logo.jpg
--rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 stockstir-1.0.2/tests/stockstir.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 stockstir-1.0.2/tests/tests.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 stockstir-1.0.2/LICENSE
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 stockstir-1.0.2/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 stockstir-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 stockstir-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 stockstir-1.0.3/.DS_Store
+-rw-r--r--   0        0        0    14876 2020-02-02 00:00:00.000000 stockstir-1.0.3/Documentation.md
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 stockstir-1.0.3/docs/code structure.rst
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 stockstir-1.0.3/docs/conf.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 stockstir-1.0.3/docs/credits.rst
+-rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 stockstir-1.0.3/docs/function use.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 stockstir-1.0.3/docs/index.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 stockstir-1.0.3/docs/installation.rst
+-rw-r--r--   0        0        0   135557 2020-02-02 00:00:00.000000 stockstir-1.0.3/docs/img/stockstirlogo.jpeg
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 stockstir-1.0.3/src/Stockstir/__init__.py
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 stockstir-1.0.3/src/Stockstir/stockstir.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 stockstir-1.0.3/tests/README(GithubVersion).md
+-rw-r--r--   0        0        0   135557 2020-02-02 00:00:00.000000 stockstir-1.0.3/tests/stockstir-logo.jpg
+-rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 stockstir-1.0.3/tests/stockstir.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 stockstir-1.0.3/tests/tests.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 stockstir-1.0.3/LICENSE
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 stockstir-1.0.3/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 stockstir-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 stockstir-1.0.3/PKG-INFO
```

### Comparing `stockstir-1.0.2/.DS_Store` & `stockstir-1.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/Documentation.md` & `stockstir-1.0.3/Documentation.md`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/docs/code structure.rst` & `stockstir-1.0.3/docs/code structure.rst`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/docs/conf.py` & `stockstir-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/docs/credits.rst` & `stockstir-1.0.3/docs/credits.rst`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/docs/function use.rst` & `stockstir-1.0.3/docs/function use.rst`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/docs/index.rst` & `stockstir-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/docs/img/stockstirlogo.jpeg` & `stockstir-1.0.3/docs/img/stockstirlogo.jpeg`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/src/Stockstir/stockstir.py` & `stockstir-1.0.3/src/Stockstir/stockstir.py`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/tests/README(GithubVersion).md` & `stockstir-1.0.3/tests/README(GithubVersion).md`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/tests/stockstir-logo.jpg` & `stockstir-1.0.3/tests/stockstir-logo.jpg`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/tests/stockstir.py` & `stockstir-1.0.3/tests/stockstir.py`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/LICENSE` & `stockstir-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.2/README.md` & `stockstir-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 Instantly and easily gather stock data in real time of any company in any of your python scripts
 
 ![stockstir-logo](https://user-images.githubusercontent.com/116693779/227736659-b39d549e-ccfd-4bef-851e-228f5bb6ac02.jpg)
 
 <p align="center">
 	<img src="https://img.shields.io/badge/License-MIT-brightgreen"
 		height="23">
-	<img src="https://img.shields.io/badge/Version-Latest-brightgreen"
-		height="23">
 	<img src="https://img.shields.io/badge/Creator-PatzEdi-brightgreen"
 		height="23">
+	<img src="https://readthedocs.org/projects/stockstir/badge/?version=latest"
+		height="23">
+	<img src="https://img.shields.io/badge/Version-Latest-brightgreen"
+		height="23">
 </p>
 
 ## **Important Note:**
 
 **The full documentation for this library is now hosted on readthedocs.org! [ReadtheDocs Documentation](https://stockstir.readthedocs.io/en/latest/index.html) file under the project files. Take a look to explore the features of Stockstir and how to use them, as well as getting to know how Stockstir works in a detailed way.**
 
 ## **Made with Python, made with passion: Stockstir is a way to gather stock data from any Python script in an easy and quick way.** 
 ____________________________________________________________________________
-## **CHANGELOG: 1.0.2**
+## **CHANGELOG: 1.0.3**
 - Added documentation to readthedocs.org. Now, the documentation is much easier to access and read through!
 
 ## **Usage**
 
 Installation:
 ```
 pip install Stockstir
```

### Comparing `stockstir-1.0.2/pyproject.toml` & `stockstir-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Stockstir"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
 	{ name="PatzEdi", email="edwardferrari717@gmail.com" },
 ]
 description = "Instantly and easily gather stock data in real time of any company in any of your python scripts"
 readme = "README.md"
 keywords = ["stocks", "stockmanagement", "stockdata", "stockmarkettool"]
 requires-python = ">=3.9"
```

### Comparing `stockstir-1.0.2/PKG-INFO` & `stockstir-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Stockstir
-Version: 1.0.2
+Version: 1.0.3
 Summary: Instantly and easily gather stock data in real time of any company in any of your python scripts
 Project-URL: Homepage, https://github.com/PatzEdi
 Project-URL: Repository, https://github.com/PatzEdi/Stockstir
 Project-URL: Bug Tracker, https://github.com/PatzEdi/Stockstir/issues
 Author-email: PatzEdi <edwardferrari717@gmail.com>
 License-File: LICENSE
 Keywords: stockdata,stockmanagement,stockmarkettool,stocks
@@ -18,27 +18,29 @@
 Instantly and easily gather stock data in real time of any company in any of your python scripts
 
 ![stockstir-logo](https://user-images.githubusercontent.com/116693779/227736659-b39d549e-ccfd-4bef-851e-228f5bb6ac02.jpg)
 
 <p align="center">
 	<img src="https://img.shields.io/badge/License-MIT-brightgreen"
 		height="23">
-	<img src="https://img.shields.io/badge/Version-Latest-brightgreen"
-		height="23">
 	<img src="https://img.shields.io/badge/Creator-PatzEdi-brightgreen"
 		height="23">
+	<img src="https://readthedocs.org/projects/stockstir/badge/?version=latest"
+		height="23">
+	<img src="https://img.shields.io/badge/Version-Latest-brightgreen"
+		height="23">
 </p>
 
 ## **Important Note:**
 
 **The full documentation for this library is now hosted on readthedocs.org! [ReadtheDocs Documentation](https://stockstir.readthedocs.io/en/latest/index.html) file under the project files. Take a look to explore the features of Stockstir and how to use them, as well as getting to know how Stockstir works in a detailed way.**
 
 ## **Made with Python, made with passion: Stockstir is a way to gather stock data from any Python script in an easy and quick way.** 
 ____________________________________________________________________________
-## **CHANGELOG: 1.0.2**
+## **CHANGELOG: 1.0.3**
 - Added documentation to readthedocs.org. Now, the documentation is much easier to access and read through!
 
 ## **Usage**
 
 Installation:
 ```
 pip install Stockstir
```

