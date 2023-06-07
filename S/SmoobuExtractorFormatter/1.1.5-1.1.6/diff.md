# Comparing `tmp/SmoobuExtractorFormatter-1.1.5.tar.gz` & `tmp/SmoobuExtractorFormatter-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.1.5.tar", last modified: Wed Jun  7 15:18:37 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.1.6.tar", last modified: Wed Jun  7 15:39:16 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.1.5.tar` & `SmoobuExtractorFormatter-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 15:18:37.357884 SmoobuExtractorFormatter-1.1.5/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-07 15:18:37.357884 SmoobuExtractorFormatter-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 15:18:37.337918 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0     8492 2023-06-07 15:18:04.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:18:37.354883 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-07 15:18:37.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-07 15:18:37.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 15:18:37.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-07 15:18:37.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-07 15:18:37.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 15:18:37.358885 SmoobuExtractorFormatter-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-07 15:18:28.000000 SmoobuExtractorFormatter-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:39:16.902564 SmoobuExtractorFormatter-1.1.6/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-07 15:39:16.901561 SmoobuExtractorFormatter-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 15:39:16.881502 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0     8260 2023-06-07 15:30:21.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:39:16.899508 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-07 15:39:16.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-07 15:39:16.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 15:39:16.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-07 15:39:16.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-07 15:39:16.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 15:39:16.903562 SmoobuExtractorFormatter-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-07 15:39:07.000000 SmoobuExtractorFormatter-1.1.6/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.1.5/LICENSE.txt` & `SmoobuExtractorFormatter-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.1.5/PKG-INFO` & `SmoobuExtractorFormatter-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.1.5
+Version: 1.1.6
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 import pandas as pd
 import numpy as np
+import sys
+import traceback
 
 name_menage = "frais_menage"
 name_taxe = "taxe_sejour"
 
 
 SEJOUR_MOTS = ["Séjour", "Résidence", "Visite", "Escale", "Vacances", "Voyage","Tourisme"]
 SEJOUR_WORDS = ["Stay", "Sojourn", "Visit", "Residence", "Stopover", "Vacation", "Trip",'Tourism']
@@ -186,88 +188,74 @@
             else :
                 del bookings['frais_menage_']
                 
                 
                 
             # merging every columns into one : taxe de sejour
 
-            bookings['taxe_sejour_'] = bookings['taxe_sejour'].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
-            lens2 = bookings['taxe_sejour_'].apply(len_value)
+                bookings['taxe_sejour_'] = bookings['taxe_sejour'].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                lens2 = bookings['taxe_sejour_'].apply(len_value)
 
-            if lens2[lens2 == 2].shape[0] == 0:
-                del bookings['taxe_sejour']
-                bookings['taxe_sejour_'] = bookings['taxe_sejour_'].apply(one_value)
-                bookings['taxe_sejour_'] = bookings['taxe_sejour_'].explode()
-            else:
-                del bookings['taxe_sejour_']
-                
-
-            # sum of all the fees into the cleaning fee 
-            
-            
-            bookings['frais_menage_'] = bookings['frais_menage_'].fillna(0.0) 
-            
-            
-            frais_linge_serviettes = ['frais_linge_lit']
-            bookings['frais_linge_serviettes'] = 0.0
-            
-            for frais in frais_linge_serviettes :
-                if frais in columns :
-                    bookings['frais_linge_serviettes'] += bookings['frais'].fillna(0.0) 
-            
-            
-            
-            try :
-                del bookings['frais_linge_lit']
-            except :
-                pass
-            try :
-                del bookings['supp_serviettes']
-                del bookings['supp_linen']
-            except :
-                pass
-            try :
-                del bookings['supp_animaux'] # pas compris dans le prix 
-            except : 
-                pass
-            try : 
-                del bookings['addon']
-            except :
-                pass
-
-            
-            
-            # new column
-            
-            payé_voyageur_calculated = ['basePrice','frais_menage_','taxe_sejour_','frais_gestion','frais_linge_serviettes','frais_gestion_2']
-            
-            bookings['payé-voyageur_calculated'] = 0.0
-            
-            
-            for frais in payé_voyageur_calculated :
-                if frais in columns :
-                    bookings['payé-voyageur_calculated'] += bookings[frais].fillna(0.0)
-            
-            #bookings['payé-voyageur_calculated'] = bookings['basePrice'].fillna(0.0) + bookings['frais_menage_'].fillna(0.0) + bookings['taxe_sejour_'].fillna(0.0) + bookings['frais_gestion'].fillna(0.0) + bookings['frais_electricite'].fillna(0.0) +   bookings['frais_linge_serviettes'].fillna(0.0)
-
-            
-
-            try : 
-                bookings['delta'] = (abs(bookings['total-price'] - bookings['payé-voyageur_calculated']))
-                
-                bookings = bookings.round(2) # pour eviter des erreurs d'arrondis
+                if lens2[lens2 == 2].shape[0] == 0:
+                    del bookings['taxe_sejour']
+                    bookings['taxe_sejour_'] = bookings['taxe_sejour_'].apply(one_value)
+                    bookings['taxe_sejour_'] = bookings['taxe_sejour_'].explode()
+                else:
+                    del bookings['taxe_sejour_']
+
+                # Sum of all the fees into the cleaning fee
+                bookings['frais_menage_'] = bookings['frais_menage_'].fillna(0.0)
+
+                frais_linge_serviettes = ['frais_linge_lit']
+                bookings['frais_linge_serviettes'] = 0.0
+
+                for frais in frais_linge_serviettes:
+                    if frais in columns:
+                        bookings['frais_linge_serviettes'] += bookings['frais'].fillna(0.0)
+
+                try:
+                    del bookings['frais_linge_lit']
+                except:
+                    pass
+                try:
+                    del bookings['supp_serviettes']
+                    del bookings['supp_linen']
+                except:
+                    pass
+                try:
+                    del bookings['supp_animaux']  # not included in the price
+                except:
+                    pass
+                try:
+                    del bookings['addon']
+                except:
+                    pass
+
+                # New column
+                payé_voyageur_calculated = ['basePrice', 'frais_menage_', 'taxe_sejour_', 'frais_gestion', 'frais_linge_serviettes', 'frais_gestion_2']
+                bookings['payé-voyageur_calculated'] = 0.0
+
+                for frais in payé_voyageur_calculated:
+                    if frais in columns:
+                        bookings['payé-voyageur_calculated'] += bookings[frais].fillna(0.0)
+
+                try:
+                    bookings['delta'] = (abs(bookings['total-price'] - bookings['payé-voyageur_calculated']))
+                    bookings = bookings.round(2)  # to avoid rounding errors
+                    bookings['Added-Taxes'] = np.where(bookings['taxe_sejour_'] == bookings['delta'], True, False)
+                    bookings['Equals-Prices'] = np.where(bookings['total-price'] == bookings['payé-voyageur_calculated'], True, False)
+
+                    del bookings['delta']
+                except KeyError as error:
+                    _, _, tb = sys.exc_info()
+                    line_number = traceback.extract_tb(tb)[-1][1]
                 
-                bookings['Added-Taxes'] = np.where(bookings['taxe_sejour_'] == bookings['delta'],True,False)
-                bookings['Equals-Prices'] = np.where(bookings['total-price'] == bookings['payé-voyageur_calculated'],True,False)
-        
-                            
-                del bookings['delta']
-            except KeyError as error:
-                print(error)
-                print("\nThere is a problem with the columns : total-price and payé-voyageur_calculated\n")
+                    
+            print(f"Error occurred on line {line_number}: {error}")
+            print("\nThere is a problem with the columns: total-price and payé-voyageur_calculated\n")
 
             # newly formated data to excel
             bookings = bookings.round(2)
             bookings.to_excel( path_output +"/Smoobu_"+file_name.split("/")[-1] + ".xlsx", index = False)
             
             print("\nSmoobu file created \n")
             for file in os.listdir():
```

### Comparing `SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.1.5
+Version: 1.1.6
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.1.5/setup.py` & `SmoobuExtractorFormatter-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.1.5',
+    version='1.1.6',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

