# Comparing `tmp/SmoobuExtractorFormatter-1.1.6.tar.gz` & `tmp/SmoobuExtractorFormatter-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.1.6.tar", last modified: Wed Jun  7 15:39:16 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.1.7.tar", last modified: Wed Jun  7 15:41:44 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.1.6.tar` & `SmoobuExtractorFormatter-1.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 15:39:16.902564 SmoobuExtractorFormatter-1.1.6/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-07 15:39:16.901561 SmoobuExtractorFormatter-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 15:39:16.881502 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0     8260 2023-06-07 15:30:21.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:39:16.899508 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-07 15:39:16.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-07 15:39:16.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 15:39:16.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-07 15:39:16.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-07 15:39:16.000000 SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 15:39:16.903562 SmoobuExtractorFormatter-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-07 15:39:07.000000 SmoobuExtractorFormatter-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:41:44.376097 SmoobuExtractorFormatter-1.1.7/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-07 15:41:44.375098 SmoobuExtractorFormatter-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 15:41:44.353023 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0     8243 2023-06-07 15:41:24.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:41:44.374095 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-07 15:41:44.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-07 15:41:44.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 15:41:44.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-07 15:41:44.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-07 15:41:44.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 15:41:44.377097 SmoobuExtractorFormatter-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-07 15:41:29.000000 SmoobuExtractorFormatter-1.1.7/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.1.6/LICENSE.txt` & `SmoobuExtractorFormatter-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.1.6/PKG-INFO` & `SmoobuExtractorFormatter-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.1.6
+Version: 1.1.7
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,19 +243,17 @@
                     bookings = bookings.round(2)  # to avoid rounding errors
                     bookings['Added-Taxes'] = np.where(bookings['taxe_sejour_'] == bookings['delta'], True, False)
                     bookings['Equals-Prices'] = np.where(bookings['total-price'] == bookings['payé-voyageur_calculated'], True, False)
 
                     del bookings['delta']
                 except KeyError as error:
                     _, _, tb = sys.exc_info()
-                    line_number = traceback.extract_tb(tb)[-1][1]
-                
-                    
-            print(f"Error occurred on line {line_number}: {error}")
-            print("\nThere is a problem with the columns: total-price and payé-voyageur_calculated\n")
+                    line_number = traceback.extract_tb(tb)[-1][1]       
+                    print(f"Error occurred on line {line_number}: {error}")
+                    print("\nThere is a problem with the columns: total-price and payé-voyageur_calculated\n")
 
             # newly formated data to excel
             bookings = bookings.round(2)
             bookings.to_excel( path_output +"/Smoobu_"+file_name.split("/")[-1] + ".xlsx", index = False)
             
             print("\nSmoobu file created \n")
             for file in os.listdir():
```

### Comparing `SmoobuExtractorFormatter-1.1.6/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.1.6
+Version: 1.1.7
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.1.6/setup.py` & `SmoobuExtractorFormatter-1.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.1.6',
+    version='1.1.7',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

