# Comparing `tmp/stockstir-1.0.1.tar.gz` & `tmp/stockstir-1.0.2.tar.gz`

## Comparing `stockstir-1.0.1.tar` & `stockstir-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,19 @@
--rw-r--r--   0        0        0    14876 2020-02-02 00:00:00.000000 stockstir-1.0.1/Documentation.md
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 stockstir-1.0.1/src/Stockstir/__init__.py
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 stockstir-1.0.1/src/Stockstir/stockstir.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 stockstir-1.0.1/tests/README(GithubVersion).md
--rw-r--r--   0        0        0   135557 2020-02-02 00:00:00.000000 stockstir-1.0.1/tests/stockstir-logo.jpg
--rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 stockstir-1.0.1/tests/stockstir.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 stockstir-1.0.1/tests/tests.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 stockstir-1.0.1/LICENSE
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 stockstir-1.0.1/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 stockstir-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 stockstir-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 stockstir-1.0.2/.DS_Store
+-rw-r--r--   0        0        0    14876 2020-02-02 00:00:00.000000 stockstir-1.0.2/Documentation.md
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/code structure.rst
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/credits.rst
+-rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/function use.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/index.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/installation.rst
+-rw-r--r--   0        0        0   135557 2020-02-02 00:00:00.000000 stockstir-1.0.2/docs/img/stockstirlogo.jpeg
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 stockstir-1.0.2/src/Stockstir/__init__.py
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 stockstir-1.0.2/src/Stockstir/stockstir.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 stockstir-1.0.2/tests/README(GithubVersion).md
+-rw-r--r--   0        0        0   135557 2020-02-02 00:00:00.000000 stockstir-1.0.2/tests/stockstir-logo.jpg
+-rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 stockstir-1.0.2/tests/stockstir.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 stockstir-1.0.2/tests/tests.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 stockstir-1.0.2/LICENSE
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 stockstir-1.0.2/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 stockstir-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 stockstir-1.0.2/PKG-INFO
```

### Comparing `stockstir-1.0.1/Documentation.md` & `stockstir-1.0.2/Documentation.md`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.1/src/Stockstir/stockstir.py` & `stockstir-1.0.2/src/Stockstir/stockstir.py`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.1/tests/README(GithubVersion).md` & `stockstir-1.0.2/tests/README(GithubVersion).md`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.1/tests/stockstir-logo.jpg` & `stockstir-1.0.2/docs/img/stockstirlogo.jpeg`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.1/tests/stockstir.py` & `stockstir-1.0.2/tests/stockstir.py`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.1/LICENSE` & `stockstir-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stockstir-1.0.1/README.md` & `stockstir-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # Stockstir
 Instantly and easily gather stock data in real time of any company in any of your python scripts
 
 ![stockstir-logo](https://user-images.githubusercontent.com/116693779/227736659-b39d549e-ccfd-4bef-851e-228f5bb6ac02.jpg)
 
-
 <p align="center">
 	<img src="https://img.shields.io/badge/License-MIT-brightgreen"
 		height="23">
-	<img src="https://img.shields.io/badge/Creator-PatzEdi-brightgreen"
-		height="23">
 	<img src="https://img.shields.io/badge/Version-Latest-brightgreen"
 		height="23">
+	<img src="https://img.shields.io/badge/Creator-PatzEdi-brightgreen"
+		height="23">
 </p>
 
 ## **Important Note:**
-The full documentation for this tool is under the Documentation.md file under the project files. Take a look to explore the features of Stockstir and how to use them, as well as getting to know how Stockstir works in a detailed way.
+
+**The full documentation for this library is now hosted on readthedocs.org! [ReadtheDocs Documentation](https://stockstir.readthedocs.io/en/latest/index.html) file under the project files. Take a look to explore the features of Stockstir and how to use them, as well as getting to know how Stockstir works in a detailed way.**
 
 ## **Made with Python, made with passion: Stockstir is a way to gather stock data from any Python script in an easy and quick way.** 
 ____________________________________________________________________________
-## **CHANGELOG: 1.0.0**
-- Fixed bug where any stock value greater than 999.99 would give type errors.
+## **CHANGELOG: 1.0.2**
+- Added documentation to readthedocs.org. Now, the documentation is much easier to access and read through!
 
 ## **Usage**
 
 Installation:
 ```
 pip install Stockstir
 ```
@@ -32,15 +32,15 @@
 ```
 import Stockstir
 ```
 Simple example to gather stock data from any website:
 ```
 Stockstir.Tools.getSinglePrice("ticker/stockSymbol")
 ```
-Since this library has many more features (too many to explain here in a neat way), you can take a look at the Documentation.md file under the project files.
+Since this library has many more features (too many to explain here in a neat way), you can take a look at the [Documentation](https://stockstir.readthedocs.io/en/latest/index.html) file under the project files.
 
 ## **Features**
 - Instantly gather stock prices from any company in real time.
 - Includes a single price gathering tool to get the price of any company once.
 - Includes a multi data gathering tool which has features like anti ban, random user agents, delay for each request, and of course how much data to gather.  
 - Useful tools such as getting the trend of the gathered data determining whether the stock price went up, down, or stayed neutral throughout that time period.
 - Ability to return the time spent in the total process of gathering the data. This can be useful in order to analyze data and comparing it to the time spent overall. Not only that, but getting the trend also comes with an optional option to get the change between the first and the last value of the gathered data.
@@ -58,19 +58,19 @@
 ## **How?**
 - Using many useful libraries (credits below), I was able to get what I needed to make a library like this one. 
 - The way it works is very interesting. I basically gathered the source code of the webpage of CNBC and added to the url of "https://www.cnbc.com/quotes/" the ticker/stock symbol. I made a request to that URL, got the source code, and created a regex pattern that suited the website CNBC. I figured out that the regex pattern I used was universal for any company and its source at CNBC. Using the regex, I could instantly find the value of the price. So overall, this script basically sends a request to CNBC and analyzes the source in order to gather the price.
 ____________________________________________________________________________
 ## **User notice**
 - Please be aware that using a rotating IP address (for example a VPN with a rotating IP) could help you not get banned from the website CNBC when making a lot of requests. If you want to use the multi data gathering tool, you can use the anti ban function to try to avoid getting banned from the website and being recognized as a potential "bot" making automatic requests.
 - This project is still a work in progress. Adding new features is very easy, but so far I have started with it simple. 
-- Please note that the README file briefly goes into the details of how the project works. If you want more in depth details of what each and every function and parameter does, take a look at the Documentation.md file in the project files.
+- Please note that the README file briefly goes into the details of how the project works. If you want more in depth details of what each and every function and parameter does, take a look at the [Documentation](https://stockstir.readthedocs.io/en/latest/index.html) file in the project files.
 ____________________________________________________________________________
 ## **Services used (Credits):**
 - [Requests module](https://requests.readthedocs.io/en/latest/)
 - [URLLib module](https://docs.python.org/3/library/urllib.html)
 - [Re module](https://docs.python.org/3/library/re.html)
 - [Time module](https://docs.python.org/3/library/time.html)
 - [Random module](https://docs.python.org/3/library/random.html)
 
 ____________________________________________________________________________
 ## **Make sure to leave a star!**
-- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful in order to gather the stock data you need.
+- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful in order to gather the stock data you need.
```

### Comparing `stockstir-1.0.1/pyproject.toml` & `stockstir-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Stockstir"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
 	{ name="PatzEdi", email="edwardferrari717@gmail.com" },
 ]
 description = "Instantly and easily gather stock data in real time of any company in any of your python scripts"
 readme = "README.md"
 keywords = ["stocks", "stockmanagement", "stockdata", "stockmarkettool"]
 requires-python = ">=3.9"
```

### Comparing `stockstir-1.0.1/PKG-INFO` & `stockstir-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Stockstir
-Version: 1.0.1
+Version: 1.0.2
 Summary: Instantly and easily gather stock data in real time of any company in any of your python scripts
 Project-URL: Homepage, https://github.com/PatzEdi
 Project-URL: Repository, https://github.com/PatzEdi/Stockstir
 Project-URL: Bug Tracker, https://github.com/PatzEdi/Stockstir/issues
 Author-email: PatzEdi <edwardferrari717@gmail.com>
 License-File: LICENSE
 Keywords: stockdata,stockmanagement,stockmarkettool,stocks
@@ -15,31 +15,31 @@
 Description-Content-Type: text/markdown
 
 # Stockstir
 Instantly and easily gather stock data in real time of any company in any of your python scripts
 
 ![stockstir-logo](https://user-images.githubusercontent.com/116693779/227736659-b39d549e-ccfd-4bef-851e-228f5bb6ac02.jpg)
 
-
 <p align="center">
 	<img src="https://img.shields.io/badge/License-MIT-brightgreen"
 		height="23">
-	<img src="https://img.shields.io/badge/Creator-PatzEdi-brightgreen"
-		height="23">
 	<img src="https://img.shields.io/badge/Version-Latest-brightgreen"
 		height="23">
+	<img src="https://img.shields.io/badge/Creator-PatzEdi-brightgreen"
+		height="23">
 </p>
 
 ## **Important Note:**
-The full documentation for this tool is under the Documentation.md file under the project files. Take a look to explore the features of Stockstir and how to use them, as well as getting to know how Stockstir works in a detailed way.
+
+**The full documentation for this library is now hosted on readthedocs.org! [ReadtheDocs Documentation](https://stockstir.readthedocs.io/en/latest/index.html) file under the project files. Take a look to explore the features of Stockstir and how to use them, as well as getting to know how Stockstir works in a detailed way.**
 
 ## **Made with Python, made with passion: Stockstir is a way to gather stock data from any Python script in an easy and quick way.** 
 ____________________________________________________________________________
-## **CHANGELOG: 1.0.0**
-- Fixed bug where any stock value greater than 999.99 would give type errors.
+## **CHANGELOG: 1.0.2**
+- Added documentation to readthedocs.org. Now, the documentation is much easier to access and read through!
 
 ## **Usage**
 
 Installation:
 ```
 pip install Stockstir
 ```
@@ -48,15 +48,15 @@
 ```
 import Stockstir
 ```
 Simple example to gather stock data from any website:
 ```
 Stockstir.Tools.getSinglePrice("ticker/stockSymbol")
 ```
-Since this library has many more features (too many to explain here in a neat way), you can take a look at the Documentation.md file under the project files.
+Since this library has many more features (too many to explain here in a neat way), you can take a look at the [Documentation](https://stockstir.readthedocs.io/en/latest/index.html) file under the project files.
 
 ## **Features**
 - Instantly gather stock prices from any company in real time.
 - Includes a single price gathering tool to get the price of any company once.
 - Includes a multi data gathering tool which has features like anti ban, random user agents, delay for each request, and of course how much data to gather.  
 - Useful tools such as getting the trend of the gathered data determining whether the stock price went up, down, or stayed neutral throughout that time period.
 - Ability to return the time spent in the total process of gathering the data. This can be useful in order to analyze data and comparing it to the time spent overall. Not only that, but getting the trend also comes with an optional option to get the change between the first and the last value of the gathered data.
@@ -74,19 +74,19 @@
 ## **How?**
 - Using many useful libraries (credits below), I was able to get what I needed to make a library like this one. 
 - The way it works is very interesting. I basically gathered the source code of the webpage of CNBC and added to the url of "https://www.cnbc.com/quotes/" the ticker/stock symbol. I made a request to that URL, got the source code, and created a regex pattern that suited the website CNBC. I figured out that the regex pattern I used was universal for any company and its source at CNBC. Using the regex, I could instantly find the value of the price. So overall, this script basically sends a request to CNBC and analyzes the source in order to gather the price.
 ____________________________________________________________________________
 ## **User notice**
 - Please be aware that using a rotating IP address (for example a VPN with a rotating IP) could help you not get banned from the website CNBC when making a lot of requests. If you want to use the multi data gathering tool, you can use the anti ban function to try to avoid getting banned from the website and being recognized as a potential "bot" making automatic requests.
 - This project is still a work in progress. Adding new features is very easy, but so far I have started with it simple. 
-- Please note that the README file briefly goes into the details of how the project works. If you want more in depth details of what each and every function and parameter does, take a look at the Documentation.md file in the project files.
+- Please note that the README file briefly goes into the details of how the project works. If you want more in depth details of what each and every function and parameter does, take a look at the [Documentation](https://stockstir.readthedocs.io/en/latest/index.html) file in the project files.
 ____________________________________________________________________________
 ## **Services used (Credits):**
 - [Requests module](https://requests.readthedocs.io/en/latest/)
 - [URLLib module](https://docs.python.org/3/library/urllib.html)
 - [Re module](https://docs.python.org/3/library/re.html)
 - [Time module](https://docs.python.org/3/library/time.html)
 - [Random module](https://docs.python.org/3/library/random.html)
 
 ____________________________________________________________________________
 ## **Make sure to leave a star!**
-- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful in order to gather the stock data you need.
+- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful in order to gather the stock data you need.
```

