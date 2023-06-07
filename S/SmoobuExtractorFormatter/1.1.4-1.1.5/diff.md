# Comparing `tmp/SmoobuExtractorFormatter-1.1.4.tar.gz` & `tmp/SmoobuExtractorFormatter-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.1.4.tar", last modified: Wed Jun  7 14:51:52 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.1.5.tar", last modified: Wed Jun  7 15:18:37 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.1.4.tar` & `SmoobuExtractorFormatter-1.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:51:52.157178 SmoobuExtractorFormatter-1.1.4/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-07 14:51:52.156177 SmoobuExtractorFormatter-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 14:51:52.136006 SmoobuExtractorFormatter-1.1.4/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.4/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0     8922 2023-06-07 14:51:32.000000 SmoobuExtractorFormatter-1.1.4/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:51:52.154179 SmoobuExtractorFormatter-1.1.4/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-07 14:51:52.000000 SmoobuExtractorFormatter-1.1.4/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-07 14:51:52.000000 SmoobuExtractorFormatter-1.1.4/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:51:52.000000 SmoobuExtractorFormatter-1.1.4/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-07 14:51:52.000000 SmoobuExtractorFormatter-1.1.4/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-07 14:51:52.000000 SmoobuExtractorFormatter-1.1.4/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 14:51:52.157178 SmoobuExtractorFormatter-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-07 14:51:39.000000 SmoobuExtractorFormatter-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:18:37.357884 SmoobuExtractorFormatter-1.1.5/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-07 15:18:37.357884 SmoobuExtractorFormatter-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 15:18:37.337918 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0     8492 2023-06-07 15:18:04.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:18:37.354883 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-07 15:18:37.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-07 15:18:37.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 15:18:37.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-07 15:18:37.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-07 15:18:37.000000 SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 15:18:37.358885 SmoobuExtractorFormatter-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-07 15:18:28.000000 SmoobuExtractorFormatter-1.1.5/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.1.4/LICENSE.txt` & `SmoobuExtractorFormatter-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.1.4/PKG-INFO` & `SmoobuExtractorFormatter-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.1.4
+Version: 1.1.5
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.1.4/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,16 +42,14 @@
 
 	"check-in": "check-in",
 
 	"check-out": "check-out",
 
 	"price": "total-price",
 
-	"commission-included": "commission-included",
-
 	"guest-app-url": "guest-app-url",
 
 	"is-blocked-booking": "is-blocked-booking",
 
 	"guestId": "guest_id",
 
 	"apartment_id": "apartment_id",
@@ -88,37 +86,28 @@
 
 	"Cleaning fee <-> cleaningFee": name_menage,
 
 	"Airbnb Collected Tax <-> channelCustom": name_taxe,
     
     'Check Out 14H <-> addon' : 'addon',
 
-	"supplément serviettes <-> channelCustom": "supp_serviettes",
-
 	"TVA <-> channelCustom": "TVA",
 
 	"frais de linge de lit <-> channelCustom": "frais_linge_lit",
 
 	"Frais de nettoyage <-> cleaningFee": name_menage,
 
 	"Taxe de séjour <-> addon": name_taxe,
  
-    "'PASS_THROUGH_LINEN_FEE <-> channelCustom'": "supp_linen",
-
 	"[Sejournez à Troyes] Frais de gestion <-> addon": "frais_gestion", # à voir
     
     'Frais de gestion <-> addon' : "frais_gestion_2",
 
-	"Total Paid Amount <-> channelCustom": "Total", # à voir
-
 	"PASS_THROUGH_PET_FEE <-> channelCustom": "supp_animaux",
 
-	"frais de consommation d'électricité <-> channelCustom": "frais_electricite",
-
-	"frais d'entretien ménager <-> channelCustom": name_menage
 }
 
 
 
 
 
 class SmoobuOutput:
@@ -214,15 +203,15 @@
 
             # sum of all the fees into the cleaning fee 
             
             
             bookings['frais_menage_'] = bookings['frais_menage_'].fillna(0.0) 
             
             
-            frais_linge_serviettes = ['frais_linge_lit','supp_serviettes']
+            frais_linge_serviettes = ['frais_linge_lit']
             bookings['frais_linge_serviettes'] = 0.0
             
             for frais in frais_linge_serviettes :
                 if frais in columns :
                     bookings['frais_linge_serviettes'] += bookings['frais'].fillna(0.0) 
             
             
@@ -245,15 +234,15 @@
             except :
                 pass
 
             
             
             # new column
             
-            payé_voyageur_calculated = ['basePrice','frais_menage_','taxe_sejour_','frais_gestion','frais_electricite','frais_linge_serviettes','frais_gestion_2']
+            payé_voyageur_calculated = ['basePrice','frais_menage_','taxe_sejour_','frais_gestion','frais_linge_serviettes','frais_gestion_2']
             
             bookings['payé-voyageur_calculated'] = 0.0
             
             
             for frais in payé_voyageur_calculated :
                 if frais in columns :
                     bookings['payé-voyageur_calculated'] += bookings[frais].fillna(0.0)
```

### Comparing `SmoobuExtractorFormatter-1.1.4/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.1.5/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.1.4
+Version: 1.1.5
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.1.4/setup.py` & `SmoobuExtractorFormatter-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.1.4',
+    version='1.1.5',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

