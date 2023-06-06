# Comparing `tmp/SmoobuExtractorFormatter-1.0.7.tar.gz` & `tmp/SmoobuExtractorFormatter-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.0.7.tar", last modified: Tue Jun  6 23:20:16 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.0.8.tar", last modified: Tue Jun  6 23:28:49 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.0.7.tar` & `SmoobuExtractorFormatter-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 23:20:16.915904 SmoobuExtractorFormatter-1.0.7/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.0.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-06 23:20:16.914901 SmoobuExtractorFormatter-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.0.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 23:20:16.870216 SmoobuExtractorFormatter-1.0.7/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.0.7/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0     8399 2023-06-06 23:12:45.000000 SmoobuExtractorFormatter-1.0.7/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-06 23:20:16.910780 SmoobuExtractorFormatter-1.0.7/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-06 23:20:16.000000 SmoobuExtractorFormatter-1.0.7/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-06 23:20:16.000000 SmoobuExtractorFormatter-1.0.7/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 23:20:16.000000 SmoobuExtractorFormatter-1.0.7/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-06 23:20:16.000000 SmoobuExtractorFormatter-1.0.7/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-06 23:20:16.000000 SmoobuExtractorFormatter-1.0.7/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 23:20:16.916898 SmoobuExtractorFormatter-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-06 23:12:50.000000 SmoobuExtractorFormatter-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:28:49.778495 SmoobuExtractorFormatter-1.0.8/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.0.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-06 23:28:49.777499 SmoobuExtractorFormatter-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.0.8/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 23:28:49.729804 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0     8392 2023-06-06 23:28:43.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:28:49.774497 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-06 23:28:49.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-06 23:28:49.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 23:28:49.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-06 23:28:49.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-06 23:28:49.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 23:28:49.779498 SmoobuExtractorFormatter-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-06 23:28:37.000000 SmoobuExtractorFormatter-1.0.8/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.0.7/LICENSE.txt` & `SmoobuExtractorFormatter-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.0.7/PKG-INFO` & `SmoobuExtractorFormatter-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.0.7
+Version: 1.0.8
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.0.7/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             
             bookings = pd.read_excel(self.file)
             #bookings.rename(columns = table, inplace = True)
             
             columns = bookings.columns 
             dict = {}
 
-            bookings.rename(columns = table,axis=1, inplace = True)
+            bookings.rename(columns = table, inplace = True)
             
             columns_exist = {}
             columns_notexist = []
             
             for name in table.keys():
                 if name in columns :
                     columns_exist[name] = True
```

### Comparing `SmoobuExtractorFormatter-1.0.7/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.0.7
+Version: 1.0.8
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.0.7/setup.py` & `SmoobuExtractorFormatter-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.0.7',
+    version='1.0.8',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

