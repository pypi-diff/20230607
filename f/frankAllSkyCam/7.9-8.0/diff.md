# Comparing `tmp/frankAllSkyCam-7.9.tar.gz` & `tmp/frankAllSkyCam-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-7.9.tar", last modified: Wed Jun  7 12:46:05 2023, max compression
+gzip compressed data, was "frankAllSkyCam-8.0.tar", last modified: Wed Jun  7 19:02:55 2023, max compression
```

## Comparing `frankAllSkyCam-7.9.tar` & `frankAllSkyCam-8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 12:46:05.336249 frankAllSkyCam-7.9/
--rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-06-07 12:46:05.336249 frankAllSkyCam-7.9/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 12:46:05.336249 frankAllSkyCam-7.9/frankAllSkyCam/
--rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-06-07 12:42:20.509821 frankAllSkyCam-7.9/frankAllSkyCam/__init__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     5427 2023-06-07 12:39:31.306876 frankAllSkyCam-7.9/frankAllSkyCam/__main__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1033 2023-06-07 12:39:31.298876 frankAllSkyCam-7.9/frankAllSkyCam/allskycamdelete.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3421 2023-06-07 12:39:31.302876 frankAllSkyCam-7.9/frankAllSkyCam/config.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3491 2023-06-07 12:39:31.302876 frankAllSkyCam-7.9/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2431 2023-06-07 12:39:31.302876 frankAllSkyCam-7.9/frankAllSkyCam/drawtext.py
--rw-r-xr--   0 pi        (1000) pi        (1000)     1156 2023-06-07 12:39:31.302876 frankAllSkyCam-7.9/frankAllSkyCam/exposurecalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3758 2023-06-07 12:39:31.302876 frankAllSkyCam-7.9/frankAllSkyCam/fileManager.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2823 2023-06-07 12:39:31.302876 frankAllSkyCam-7.9/frankAllSkyCam/getextdata.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     9426 2023-06-07 12:39:31.306876 frankAllSkyCam-7.9/frankAllSkyCam/imageHeader.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-06-07 12:39:31.306876 frankAllSkyCam-7.9/frankAllSkyCam/index.py
--rw-r--r--   0 pi        (1000) pi        (1000)      233 2023-06-07 12:39:31.306876 frankAllSkyCam-7.9/frankAllSkyCam/sqmexp.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)    16497 2023-06-07 12:39:31.306876 frankAllSkyCam-7.9/frankAllSkyCam/sqmreader.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3082 2023-06-07 12:39:31.310876 frankAllSkyCam-7.9/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-06-07 12:39:31.310876 frankAllSkyCam-7.9/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-06-05 20:12:48.501031 frankAllSkyCam-7.9/frankAllSkyCam/test_suncalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     4433 2023-06-07 12:39:31.310876 frankAllSkyCam-7.9/frankAllSkyCam/timelapse.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1593 2023-06-07 12:39:31.310876 frankAllSkyCam-7.9/frankAllSkyCam/watchDog.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-7.9/setup.cfg
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1067 2023-06-07 12:41:14.390249 frankAllSkyCam-7.9/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 19:02:55.576105 frankAllSkyCam-8.0/
+-rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-06-07 19:02:55.576105 frankAllSkyCam-8.0/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 19:02:55.576105 frankAllSkyCam-8.0/frankAllSkyCam/
+-rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-06-07 19:01:56.984643 frankAllSkyCam-8.0/frankAllSkyCam/__init__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     5427 2023-06-07 12:39:31.306876 frankAllSkyCam-8.0/frankAllSkyCam/__main__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1033 2023-06-07 12:39:31.298876 frankAllSkyCam-8.0/frankAllSkyCam/allskycamdelete.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3421 2023-06-07 12:39:31.302876 frankAllSkyCam-8.0/frankAllSkyCam/config.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3491 2023-06-07 12:39:31.302876 frankAllSkyCam-8.0/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2431 2023-06-07 12:39:31.302876 frankAllSkyCam-8.0/frankAllSkyCam/drawtext.py
+-rw-r-xr--   0 pi        (1000) pi        (1000)     1156 2023-06-07 12:39:31.302876 frankAllSkyCam-8.0/frankAllSkyCam/exposurecalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3758 2023-06-07 12:39:31.302876 frankAllSkyCam-8.0/frankAllSkyCam/fileManager.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2823 2023-06-07 12:39:31.302876 frankAllSkyCam-8.0/frankAllSkyCam/getextdata.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     9426 2023-06-07 12:39:31.306876 frankAllSkyCam-8.0/frankAllSkyCam/imageHeader.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-06-07 12:39:31.306876 frankAllSkyCam-8.0/frankAllSkyCam/index.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      233 2023-06-07 12:39:31.306876 frankAllSkyCam-8.0/frankAllSkyCam/sqmexp.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)    16497 2023-06-07 12:39:31.306876 frankAllSkyCam-8.0/frankAllSkyCam/sqmreader.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3082 2023-06-07 12:39:31.310876 frankAllSkyCam-8.0/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-06-07 12:39:31.310876 frankAllSkyCam-8.0/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-06-05 20:12:48.501031 frankAllSkyCam-8.0/frankAllSkyCam/test_suncalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4433 2023-06-07 12:39:31.310876 frankAllSkyCam-8.0/frankAllSkyCam/timelapse.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1593 2023-06-07 12:39:31.310876 frankAllSkyCam-8.0/frankAllSkyCam/watchDog.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-8.0/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1067 2023-06-07 19:00:16.097564 frankAllSkyCam-8.0/setup.py
```

### Comparing `frankAllSkyCam-7.9/PKG-INFO` & `frankAllSkyCam-8.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: frankAllSkyCam
-Version: 7.9
+Version: 8.0
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/7.9.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.0.tar.gz
 Description: UNKNOWN
 Keywords: AllSkyCamera,Astronomy,AllSky
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/__main__.py` & `frankAllSkyCam-8.0/frankAllSkyCam/__main__.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-8.0/frankAllSkyCam/allskycamdelete.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/config.py` & `frankAllSkyCam-8.0/frankAllSkyCam/config.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/crontab.py` & `frankAllSkyCam-8.0/frankAllSkyCam/crontab.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-8.0/frankAllSkyCam/drawtext.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/exposurecalc.py` & `frankAllSkyCam-8.0/frankAllSkyCam/exposurecalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-8.0/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/getextdata.py` & `frankAllSkyCam-8.0/frankAllSkyCam/getextdata.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-8.0/frankAllSkyCam/imageHeader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/sqmreader.py` & `frankAllSkyCam-8.0/frankAllSkyCam/sqmreader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/startrail.py` & `frankAllSkyCam-8.0/frankAllSkyCam/startrail.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-8.0/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-8.0/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-8.0/frankAllSkyCam/timelapse.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-8.0/frankAllSkyCam/watchDog.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.9/setup.py` & `frankAllSkyCam-8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'frankAllSkyCam',
   packages = ['frankAllSkyCam'],
-  version = '7.9',
+  version = '8.0',
   license='MIT',
   description = 'AllSkyCamera with Raspberry Pi and Pi HQ Camera ',
   author = 'Francesco Sferlazza',
   author_email = 'sferlazza@gmail.com',
   url = 'https://github.com/sferlix/frankAllSkyCam',
-  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/7.9.tar.gz',
+  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.0.tar.gz',
   keywords = ['AllSkyCamera', 'Astronomy', 'AllSky'],
   install_requires=[
           'pytz',
           'numpy',
           'pandas',
       ],
   classifiers=[
```

