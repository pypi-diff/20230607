# Comparing `tmp/SmoobuExtractorFormatter-1.1.2.tar.gz` & `tmp/SmoobuExtractorFormatter-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.1.2.tar", last modified: Wed Jun  7 14:33:37 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.1.3.tar", last modified: Wed Jun  7 14:46:49 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.1.2.tar` & `SmoobuExtractorFormatter-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:33:37.625139 SmoobuExtractorFormatter-1.1.2/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-07 14:33:37.624141 SmoobuExtractorFormatter-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 14:33:37.599137 SmoobuExtractorFormatter-1.1.2/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.2/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0     8988 2023-06-07 14:32:17.000000 SmoobuExtractorFormatter-1.1.2/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:33:37.621140 SmoobuExtractorFormatter-1.1.2/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-07 14:33:37.000000 SmoobuExtractorFormatter-1.1.2/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-07 14:33:37.000000 SmoobuExtractorFormatter-1.1.2/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:33:37.000000 SmoobuExtractorFormatter-1.1.2/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-07 14:33:37.000000 SmoobuExtractorFormatter-1.1.2/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-07 14:33:37.000000 SmoobuExtractorFormatter-1.1.2/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 14:33:37.625139 SmoobuExtractorFormatter-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-07 14:33:29.000000 SmoobuExtractorFormatter-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:46:49.777115 SmoobuExtractorFormatter-1.1.3/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-07 14:46:49.776115 SmoobuExtractorFormatter-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 14:46:49.753115 SmoobuExtractorFormatter-1.1.3/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.3/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0     9281 2023-06-07 14:45:47.000000 SmoobuExtractorFormatter-1.1.3/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:46:49.772116 SmoobuExtractorFormatter-1.1.3/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-07 14:46:49.000000 SmoobuExtractorFormatter-1.1.3/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-07 14:46:49.000000 SmoobuExtractorFormatter-1.1.3/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:46:49.000000 SmoobuExtractorFormatter-1.1.3/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-07 14:46:49.000000 SmoobuExtractorFormatter-1.1.3/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-07 14:46:49.000000 SmoobuExtractorFormatter-1.1.3/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 14:46:49.778121 SmoobuExtractorFormatter-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-07 14:46:38.000000 SmoobuExtractorFormatter-1.1.3/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.1.2/LICENSE.txt` & `SmoobuExtractorFormatter-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.1.2/PKG-INFO` & `SmoobuExtractorFormatter-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.1.2
+Version: 1.1.3
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.1.2/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.1.3/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,24 +198,31 @@
                 del bookings['frais_menage_']
                 
                 
                 
             # merging every columns into one : taxe de sejour
             bookings['taxe_sejour_'] = 0.0 
             
-            bookings['taxe_sejour_'] = bookings['taxe_sejour'].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+            #bookings['taxe_sejour_'] = bookings['taxe_sejour'].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
             
-            lens2 = bookings['taxe_sejour_'].apply(len_value)
+            taxes = ['taxe_sejour','taxe_sejour.1','taxe_sejour.2','taxe_sejour.3']
+            
+            for tax in taxes :
+                bookings['taxe_sejour_'] = bookings[tax].fillna(0.0)
+                del bookings[tax]
+            
+            '''lens2 = bookings['taxe_sejour_'].apply(len_value)
             
             if lens2[lens2 == 2].shape[0] == 0:
                 del bookings['taxe_sejour']
                 bookings['taxe_sejour_'] = bookings['taxe_sejour_'].apply(one_value)
                 bookings['taxe_sejour_'] = bookings['taxe_sejour_'].explode()
             else :
-                del bookings['taxe_sejour_']
+                del bookings['taxe_sejour_']'''
+                
                 
 
             # sum of all the fees into the cleaning fee 
             
             
             bookings['frais_menage_'] = bookings['frais_menage_'].fillna(0.0) 
             
@@ -247,15 +254,15 @@
             except :
                 pass
 
             
             
             # new column
             
-            payé_voyageur_calculated = ['basePrice','frais_menage_','taxe_sejour_','frais_gestion','frais_electricite','frais_linge_serviettes']
+            payé_voyageur_calculated = ['basePrice','frais_menage_','taxe_sejour_','frais_gestion','frais_electricite','frais_linge_serviettes','frais_gestion_2']
             
             bookings['payé-voyageur_calculated'] = 0.0
             
             
             for frais in payé_voyageur_calculated :
                 if frais in columns :
                     bookings['payé-voyageur_calculated'] += bookings[frais].fillna(0.0)
```

### Comparing `SmoobuExtractorFormatter-1.1.2/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.1.3/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.1.2
+Version: 1.1.3
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.1.2/setup.py` & `SmoobuExtractorFormatter-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.1.2',
+    version='1.1.3',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

