# Comparing `tmp/SmoobuExtractorFormatter-1.1.0.tar.gz` & `tmp/SmoobuExtractorFormatter-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.1.0.tar", last modified: Wed Jun  7 14:05:49 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.1.1.tar", last modified: Wed Jun  7 14:19:45 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.1.0.tar` & `SmoobuExtractorFormatter-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:05:49.068178 SmoobuExtractorFormatter-1.1.0/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-07 14:05:49.067178 SmoobuExtractorFormatter-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 14:05:49.040916 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0     8924 2023-06-07 14:04:40.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:05:49.065178 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-07 14:05:48.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-07 14:05:48.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:05:48.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-07 14:05:48.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-07 14:05:48.000000 SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 14:05:49.069187 SmoobuExtractorFormatter-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-07 14:04:56.000000 SmoobuExtractorFormatter-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:19:45.445477 SmoobuExtractorFormatter-1.1.1/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-07 14:19:45.444478 SmoobuExtractorFormatter-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 14:19:45.422477 SmoobuExtractorFormatter-1.1.1/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.1/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0     8961 2023-06-07 14:19:21.000000 SmoobuExtractorFormatter-1.1.1/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:19:45.441478 SmoobuExtractorFormatter-1.1.1/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-07 14:19:45.000000 SmoobuExtractorFormatter-1.1.1/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-07 14:19:45.000000 SmoobuExtractorFormatter-1.1.1/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:19:45.000000 SmoobuExtractorFormatter-1.1.1/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-07 14:19:45.000000 SmoobuExtractorFormatter-1.1.1/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-07 14:19:45.000000 SmoobuExtractorFormatter-1.1.1/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 14:19:45.445477 SmoobuExtractorFormatter-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-07 14:19:32.000000 SmoobuExtractorFormatter-1.1.1/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.1.0/LICENSE.txt` & `SmoobuExtractorFormatter-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.1.0/PKG-INFO` & `SmoobuExtractorFormatter-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.1.0
+Version: 1.1.1
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.1.1/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
                 
             else :
                 del bookings['frais_menage_']
                 
                 
                 
             # merging every columns into one : taxe de sejour
+            bookings['taxe_sejour_'] = 0.0 
             
             bookings['taxe_sejour_'] = bookings['taxe_sejour'].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
             
             lens2 = bookings['taxe_sejour_'].apply(len_value)
             
             if lens2[lens2 == 2].shape[0] == 0:
                 del bookings['taxe_sejour']
@@ -269,16 +270,16 @@
                 bookings = bookings.round(2) # pour eviter des erreurs d'arrondis
                 
                 bookings['Added-Taxes'] = np.where(bookings['taxe_sejour_'] == bookings['delta'],True,False)
                 bookings['Equals-Prices'] = np.where(bookings['total-price'] == bookings['payé-voyageur_calculated'],True,False)
         
                             
                 del bookings['delta']
-            except (KeyError) as KeyError:
-                print(KeyError)
+            except KeyError as error:
+                print(error)
                 print("\nThere is a problem with the columns : total-price and payé-voyageur_calculated\n")
 
             # newly formated data to excel
             bookings = bookings.round(2)
             bookings.to_excel( path_output +"/Smoobu_"+file_name.split("/")[-1] + ".xlsx", index = False)
             
             print("\nSmoobu file created \n")
```

### Comparing `SmoobuExtractorFormatter-1.1.0/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.1.1/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.1.0
+Version: 1.1.1
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.1.0/setup.py` & `SmoobuExtractorFormatter-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.1.0',
+    version='1.1.1',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

