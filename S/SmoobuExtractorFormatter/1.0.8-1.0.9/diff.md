# Comparing `tmp/SmoobuExtractorFormatter-1.0.8.tar.gz` & `tmp/SmoobuExtractorFormatter-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.0.8.tar", last modified: Tue Jun  6 23:28:49 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.0.9.tar", last modified: Tue Jun  6 23:31:20 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.0.8.tar` & `SmoobuExtractorFormatter-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 23:28:49.778495 SmoobuExtractorFormatter-1.0.8/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.0.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-06 23:28:49.777499 SmoobuExtractorFormatter-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.0.8/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 23:28:49.729804 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0     8392 2023-06-06 23:28:43.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-06 23:28:49.774497 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-06 23:28:49.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-06 23:28:49.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 23:28:49.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-06 23:28:49.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-06 23:28:49.000000 SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 23:28:49.779498 SmoobuExtractorFormatter-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-06 23:28:37.000000 SmoobuExtractorFormatter-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:31:20.395887 SmoobuExtractorFormatter-1.0.9/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.0.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-06 23:31:20.394887 SmoobuExtractorFormatter-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 23:31:20.358456 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0     8545 2023-06-06 23:30:50.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:31:20.390690 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-06 23:31:20.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-06 23:31:20.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 23:31:20.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-06 23:31:20.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-06 23:31:20.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 23:31:20.396882 SmoobuExtractorFormatter-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-06 23:31:05.000000 SmoobuExtractorFormatter-1.0.9/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.0.8/LICENSE.txt` & `SmoobuExtractorFormatter-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.0.8/PKG-INFO` & `SmoobuExtractorFormatter-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,17 @@
                 
 
             # sum of all the fees into the cleaning fee 
             
             
             bookings['frais_menage_'] = bookings['frais_menage_'].fillna(0.0) 
             
+            
             frais_linge_serviettes = ['frais_linge_lit','supp_serviettes']
+            bookings['frais_linge_serviettes'] = 0.0
             
             for frais in frais_linge_serviettes :
                 if frais in columns :
                     bookings['frais_linge_serviettes'] += bookings['frais'].fillna(0.0) 
             
             
             bookings['frais_menage_'].replace(0,np.nan,inplace = True)
@@ -233,14 +235,17 @@
 
             
             
             # new column
             
             payé_voyageur_calculated = ['basePrice','frais_menage_','taxe_sejour_','frais_gestion','frais_electricite','frais_linge_serviettes']
             
+            bookings['payé-voyageur_calculated'] = 0.0
+            
+            
             for frais in payé_voyageur_calculated :
                 if frais in columns :
                     bookings['payé-voyageur_calculated'] += bookings[frais].fillna(0.0)
             
             #bookings['payé-voyageur_calculated'] = bookings['basePrice'].fillna(0.0) + bookings['frais_menage_'].fillna(0.0) + bookings['taxe_sejour_'].fillna(0.0) + bookings['frais_gestion'].fillna(0.0) + bookings['frais_electricite'].fillna(0.0) +   bookings['frais_linge_serviettes'].fillna(0.0)
```

### Comparing `SmoobuExtractorFormatter-1.0.8/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.0.8/setup.py` & `SmoobuExtractorFormatter-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.0.8',
+    version='1.0.9',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

