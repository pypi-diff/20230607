# Comparing `tmp/zillow-api-s-1.0.0.tar.gz` & `tmp/zillow-api-s-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillow-api-s-1.0.0.tar", last modified: Wed Jun  7 09:22:08 2023, max compression
+gzip compressed data, was "zillow-api-s-1.0.1.tar", last modified: Wed Jun  7 09:27:52 2023, max compression
```

## Comparing `zillow-api-s-1.0.0.tar` & `zillow-api-s-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 techvice   (501) staff       (20)        0 2023-06-07 09:22:08.767203 zillow-api-s-1.0.0/
--rw-r--r--   0 techvice   (501) staff       (20)     1071 2023-06-06 21:19:34.000000 zillow-api-s-1.0.0/LICENSE
--rw-r--r--   0 techvice   (501) staff       (20)     6119 2023-06-07 09:22:08.767027 zillow-api-s-1.0.0/PKG-INFO
--rw-r--r--   0 techvice   (501) staff       (20)     5268 2023-06-06 21:39:08.000000 zillow-api-s-1.0.0/README.md
--rw-r--r--   0 techvice   (501) staff       (20)       38 2023-06-07 09:22:08.767237 zillow-api-s-1.0.0/setup.cfg
--rw-r--r--   0 techvice   (501) staff       (20)     1244 2023-06-07 09:20:17.000000 zillow-api-s-1.0.0/setup.py
-drwxr-xr-x   0 techvice   (501) staff       (20)        0 2023-06-07 09:22:08.765850 zillow-api-s-1.0.0/zillow_api/
--rw-r--r--   0 techvice   (501) staff       (20)       65 2023-06-06 21:19:34.000000 zillow-api-s-1.0.0/zillow_api/__init__.py
--rw-r--r--   0 techvice   (501) staff       (20)       22 2023-06-06 21:19:34.000000 zillow-api-s-1.0.0/zillow_api/__version__.py
--rw-r--r--   0 techvice   (501) staff       (20)     2449 2023-06-06 21:37:32.000000 zillow-api-s-1.0.0/zillow_api/client.py
--rw-r--r--   0 techvice   (501) staff       (20)      152 2023-06-06 21:19:34.000000 zillow-api-s-1.0.0/zillow_api/default_headers.py
-drwxr-xr-x   0 techvice   (501) staff       (20)        0 2023-06-07 09:22:08.766767 zillow-api-s-1.0.0/zillow_api_s.egg-info/
--rw-r--r--   0 techvice   (501) staff       (20)     6119 2023-06-07 09:22:08.000000 zillow-api-s-1.0.0/zillow_api_s.egg-info/PKG-INFO
--rw-r--r--   0 techvice   (501) staff       (20)      305 2023-06-07 09:22:08.000000 zillow-api-s-1.0.0/zillow_api_s.egg-info/SOURCES.txt
--rw-r--r--   0 techvice   (501) staff       (20)        1 2023-06-07 09:22:08.000000 zillow-api-s-1.0.0/zillow_api_s.egg-info/dependency_links.txt
--rw-r--r--   0 techvice   (501) staff       (20)        9 2023-06-07 09:22:08.000000 zillow-api-s-1.0.0/zillow_api_s.egg-info/requires.txt
--rw-r--r--   0 techvice   (501) staff       (20)       11 2023-06-07 09:22:08.000000 zillow-api-s-1.0.0/zillow_api_s.egg-info/top_level.txt
+drwxr-xr-x   0 techvice   (501) staff       (20)        0 2023-06-07 09:27:52.071303 zillow-api-s-1.0.1/
+-rw-r--r--   0 techvice   (501) staff       (20)     1071 2023-06-06 21:19:34.000000 zillow-api-s-1.0.1/LICENSE
+-rw-r--r--   0 techvice   (501) staff       (20)     6121 2023-06-07 09:27:52.071143 zillow-api-s-1.0.1/PKG-INFO
+-rw-r--r--   0 techvice   (501) staff       (20)     5270 2023-06-07 09:26:47.000000 zillow-api-s-1.0.1/README.md
+-rw-r--r--   0 techvice   (501) staff       (20)       38 2023-06-07 09:27:52.071357 zillow-api-s-1.0.1/setup.cfg
+-rw-r--r--   0 techvice   (501) staff       (20)     1244 2023-06-07 09:20:17.000000 zillow-api-s-1.0.1/setup.py
+drwxr-xr-x   0 techvice   (501) staff       (20)        0 2023-06-07 09:27:52.069855 zillow-api-s-1.0.1/zillow_api/
+-rw-r--r--   0 techvice   (501) staff       (20)       65 2023-06-06 21:19:34.000000 zillow-api-s-1.0.1/zillow_api/__init__.py
+-rw-r--r--   0 techvice   (501) staff       (20)       22 2023-06-07 09:27:18.000000 zillow-api-s-1.0.1/zillow_api/__version__.py
+-rw-r--r--   0 techvice   (501) staff       (20)     2449 2023-06-06 21:37:32.000000 zillow-api-s-1.0.1/zillow_api/client.py
+-rw-r--r--   0 techvice   (501) staff       (20)      152 2023-06-06 21:19:34.000000 zillow-api-s-1.0.1/zillow_api/default_headers.py
+drwxr-xr-x   0 techvice   (501) staff       (20)        0 2023-06-07 09:27:52.070894 zillow-api-s-1.0.1/zillow_api_s.egg-info/
+-rw-r--r--   0 techvice   (501) staff       (20)     6121 2023-06-07 09:27:52.000000 zillow-api-s-1.0.1/zillow_api_s.egg-info/PKG-INFO
+-rw-r--r--   0 techvice   (501) staff       (20)      305 2023-06-07 09:27:52.000000 zillow-api-s-1.0.1/zillow_api_s.egg-info/SOURCES.txt
+-rw-r--r--   0 techvice   (501) staff       (20)        1 2023-06-07 09:27:52.000000 zillow-api-s-1.0.1/zillow_api_s.egg-info/dependency_links.txt
+-rw-r--r--   0 techvice   (501) staff       (20)        9 2023-06-07 09:27:52.000000 zillow-api-s-1.0.1/zillow_api_s.egg-info/requires.txt
+-rw-r--r--   0 techvice   (501) staff       (20)       11 2023-06-07 09:27:52.000000 zillow-api-s-1.0.1/zillow_api_s.egg-info/top_level.txt
```

### Comparing `zillow-api-s-1.0.0/LICENSE` & `zillow-api-s-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zillow-api-s-1.0.0/PKG-INFO` & `zillow-api-s-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillow-api-s
-Version: 1.0.0
+Version: 1.0.1
 Summary: Real-Time Zillow API
 Home-page: https://github.com/Scrapeit-Cloud/zillow-api-python
 Author: Roman Milyushkevich
 Author-email: roman@scrape-it.cloud
 Maintainer: Roman Milyushkevich
 Maintainer-email: roman@scrape-it.cloud
 License: MIT
@@ -27,15 +27,15 @@
 
 Using the Zillow data API, you can collect up-to-date real estate data without worrying about blockings, rotating proxies, and other difficulties you might encounter in the development process.
 
 It makes it easy to get data such as a full address, coordinates (longitude and latitude), price, property description, and many other data characterizing the features of the property, such as the number of bedrooms and bathrooms.
 
 ## Install
 
-`pip install zillow_api`
+`pip install zillow-api-s`
 
 ## API Key
 
 To use the Zillow API, you need an API key. You can get an API key and some credits for free by signing up on the [Scrape-It.Cloud](https://scrape-it.cloud/).
 
 ## Using
```

### Comparing `zillow-api-s-1.0.0/README.md` & `zillow-api-s-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Using the Zillow data API, you can collect up-to-date real estate data without worrying about blockings, rotating proxies, and other difficulties you might encounter in the development process.
 
 It makes it easy to get data such as a full address, coordinates (longitude and latitude), price, property description, and many other data characterizing the features of the property, such as the number of bedrooms and bathrooms.
 
 ## Install
 
-`pip install zillow_api`
+`pip install zillow-api-s`
 
 ## API Key
 
 To use the Zillow API, you need an API key. You can get an API key and some credits for free by signing up on the [Scrape-It.Cloud](https://scrape-it.cloud/).
 
 ## Using
```

### Comparing `zillow-api-s-1.0.0/setup.py` & `zillow-api-s-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `zillow-api-s-1.0.0/zillow_api/client.py` & `zillow-api-s-1.0.1/zillow_api/client.py`

 * *Files identical despite different names*

### Comparing `zillow-api-s-1.0.0/zillow_api_s.egg-info/PKG-INFO` & `zillow-api-s-1.0.1/zillow_api_s.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillow-api-s
-Version: 1.0.0
+Version: 1.0.1
 Summary: Real-Time Zillow API
 Home-page: https://github.com/Scrapeit-Cloud/zillow-api-python
 Author: Roman Milyushkevich
 Author-email: roman@scrape-it.cloud
 Maintainer: Roman Milyushkevich
 Maintainer-email: roman@scrape-it.cloud
 License: MIT
@@ -27,15 +27,15 @@
 
 Using the Zillow data API, you can collect up-to-date real estate data without worrying about blockings, rotating proxies, and other difficulties you might encounter in the development process.
 
 It makes it easy to get data such as a full address, coordinates (longitude and latitude), price, property description, and many other data characterizing the features of the property, such as the number of bedrooms and bathrooms.
 
 ## Install
 
-`pip install zillow_api`
+`pip install zillow-api-s`
 
 ## API Key
 
 To use the Zillow API, you need an API key. You can get an API key and some credits for free by signing up on the [Scrape-It.Cloud](https://scrape-it.cloud/).
 
 ## Using
```

