# Comparing `tmp/SmoobuExtractorFormatter-1.0.9.tar.gz` & `tmp/SmoobuExtractorFormatter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.0.9.tar", last modified: Tue Jun  6 23:31:20 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.1.0.tar", last modified: Wed Jun  7 14:05:49 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.0.9.tar` & `SmoobuExtractorFormatter-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 23:31:20.395887 SmoobuExtractorFormatter-1.0.9/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.0.9/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-06 23:31:20.394887 SmoobuExtractorFormatter-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.0.9/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 23:31:20.358456 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0     8545 2023-06-06 23:30:50.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-06 23:31:20.390690 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-06 23:31:20.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-06 23:31:20.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 23:31:20.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-06 23:31:20.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-06 23:31:20.000000 SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 23:31:20.396882 SmoobuExtractorFormatter-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-06 23:31:05.000000 SmoobuExtractorFormatter-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:05:49.068178 SmoobuExtractorFormatter-1.1.0/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-07 14:05:49.067178 SmoobuExtractorFormatter-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 14:05:49.040916 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0     8924 2023-06-07 14:04:40.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:05:49.065178 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-07 14:05:48.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-07 14:05:48.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:05:48.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-07 14:05:48.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-07 14:05:48.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 14:05:49.069187 SmoobuExtractorFormatter-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-07 14:04:56.000000 SmoobuExtractorFormatter-1.1.0/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.0.9/LICENSE.txt` & `SmoobuExtractorFormatter-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.0.9/PKG-INFO` & `SmoobuExtractorFormatter-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.0.9
+Version: 1.1.0
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,26 +71,34 @@
 	"reservation-id": "reservation-id",
 
 	"reservation-num": "reservation-num",
 
 	"created_at": "created_at",
 
 	"modified_at": "modified_at",
+ 
+    "taxe_sejour.1" : name_taxe,
+    
+    'Taxe de séjour ( seulement si réservation via Booking.com ) <-> addon' : name_taxe,
 
 	"basePrice": "basePrice",
 
 	"Commission <-> commission": "commission",
 
 	"frais de ménage <-> channelCustom": name_menage,
 
 	"taxe de séjour <-> channelCustom": name_taxe,
 
 	"Cleaning fee <-> cleaningFee": name_menage,
 
 	"Airbnb Collected Tax <-> channelCustom": name_taxe,
+ 
+    "taxe_sejour.2" : name_taxe,
+    
+    'Check Out 14H <-> addon' : 'addon',
 
 	"supplément serviettes <-> channelCustom": "supp_serviettes",
 
 	"TVA <-> channelCustom": "TVA",
 
 	"frais de linge de lit <-> channelCustom": "frais_linge_lit",
 
@@ -108,14 +116,15 @@
 
 	"frais d'entretien ménager <-> channelCustom": name_menage
 }
 
 
 
 
+
 class SmoobuOutput:
     
     """
     Changes the format of the excel (or the json) given by the scrapping tool
     of the Smoobu application 
     
     :param file: the excel file or the json file to be changed
@@ -228,14 +237,18 @@
                 del bookings['supp_serviettes']
             except :
                 pass
             try :
                 del bookings['supp_animaux'] # pas compris dans le prix 
             except : 
                 pass
+            try : 
+                del bookings['addon']
+            except :
+                pass
 
             
             
             # new column
             
             payé_voyageur_calculated = ['basePrice','frais_menage_','taxe_sejour_','frais_gestion','frais_electricite','frais_linge_serviettes']
             
@@ -256,15 +269,16 @@
                 bookings = bookings.round(2) # pour eviter des erreurs d'arrondis
                 
                 bookings['Added-Taxes'] = np.where(bookings['taxe_sejour_'] == bookings['delta'],True,False)
                 bookings['Equals-Prices'] = np.where(bookings['total-price'] == bookings['payé-voyageur_calculated'],True,False)
         
                             
                 del bookings['delta']
-            except : 
+            except (KeyError) as KeyError:
+                print(KeyError)
                 print("\nThere is a problem with the columns : total-price and payé-voyageur_calculated\n")
 
             # newly formated data to excel
             bookings = bookings.round(2)
             bookings.to_excel( path_output +"/Smoobu_"+file_name.split("/")[-1] + ".xlsx", index = False)
             
             print("\nSmoobu file created \n")
```

### Comparing `SmoobuExtractorFormatter-1.0.9/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.0.9
+Version: 1.1.0
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.0.9/setup.py` & `SmoobuExtractorFormatter-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.0.9',
+    version='1.1.0',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

