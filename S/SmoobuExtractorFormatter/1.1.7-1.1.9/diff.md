# Comparing `tmp/SmoobuExtractorFormatter-1.1.7.tar.gz` & `tmp/SmoobuExtractorFormatter-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.1.7.tar", last modified: Wed Jun  7 15:41:44 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.1.9.tar", last modified: Wed Jun  7 16:26:55 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.1.7.tar` & `SmoobuExtractorFormatter-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 15:41:44.376097 SmoobuExtractorFormatter-1.1.7/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-07 15:41:44.375098 SmoobuExtractorFormatter-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 15:41:44.353023 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0     8243 2023-06-07 15:41:24.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:41:44.374095 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-07 15:41:44.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-07 15:41:44.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 15:41:44.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-07 15:41:44.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-07 15:41:44.000000 SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 15:41:44.377097 SmoobuExtractorFormatter-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-07 15:41:29.000000 SmoobuExtractorFormatter-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:26:55.511251 SmoobuExtractorFormatter-1.1.9/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.1.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-07 16:26:55.510237 SmoobuExtractorFormatter-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.1.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 16:26:55.474384 SmoobuExtractorFormatter-1.1.9/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.1.9/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0     8071 2023-06-07 16:26:26.000000 SmoobuExtractorFormatter-1.1.9/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:26:55.507234 SmoobuExtractorFormatter-1.1.9/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-07 16:26:55.000000 SmoobuExtractorFormatter-1.1.9/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-07 16:26:55.000000 SmoobuExtractorFormatter-1.1.9/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 16:26:55.000000 SmoobuExtractorFormatter-1.1.9/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-07 16:26:55.000000 SmoobuExtractorFormatter-1.1.9/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-07 16:26:55.000000 SmoobuExtractorFormatter-1.1.9/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 16:26:55.512235 SmoobuExtractorFormatter-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-07 16:26:42.000000 SmoobuExtractorFormatter-1.1.9/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.1.7/LICENSE.txt` & `SmoobuExtractorFormatter-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.1.7/PKG-INFO` & `SmoobuExtractorFormatter-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.1.7
+Version: 1.1.9
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.1.9/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,82 +129,76 @@
     def __init__(self,file):
         self.file = file
         
         
     def format_allBookings(self,path_output = "./",table = TAB_INITIAL):
         
         def len_value(x):
-            return len(x)
+                return len(x)
 
         def one_value(x):
-            if len(x) == 1:
                 return x[0]
-            else:
-                return x
         
         
         file_name,file_extension = os.path.splitext(self.file)
     
 
         if(file_extension == ".xlsx"):
-            
-            bookings = pd.read_excel(self.file)
-            #bookings.rename(columns = table, inplace = True)
-            
-            columns = bookings.columns 
-            dict = {}
+                
+                bookings = pd.read_excel(self.file)
+                #bookings.rename(columns = table, inplace = True)
+                
+                columns = bookings.columns 
+                dict = {}
 
-            bookings.rename(columns = table, inplace = True)
-            
-            columns_exist = {}
-            columns_notexist = []
-            
-            for name in table.keys():
-                if name in columns :
-                    columns_exist[name] = True
-                else :
-                    columns_exist[name] = False
-                    columns_notexist.append(name)
-            
-            
-            number_menage = bookings['frais_menage'].shape[0]
-            number_sejour = bookings['taxe_sejour'].shape[0]
-            
-            
-            
-            
-            # merging every columns into one : frais de menage
-            
-            bookings['frais_menage_'] = bookings['frais_menage'].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
-            
+                bookings.rename(columns = table, inplace = True)
+                
+                columns_exist = {}
+                columns_notexist = []
+                
+                for name in table.keys():
+                    if name in columns :
+                        columns_exist[name] = True
+                    else :
+                        columns_exist[name] = False
+                        columns_notexist.append(name)
+                
+                
+                number_menage = bookings['frais_menage'].shape[0]
+                number_sejour = bookings['taxe_sejour'].shape[0]
+                
+                
+                
+                
+                # merging every columns into one : frais de menage
+                
+                bookings['frais_menage_'] = bookings['frais_menage'].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                
 
-            lens = bookings['frais_menage_'].apply(len_value)
-            
-            if lens[lens == 2].shape[0] == 0:
-            
+                lens = bookings['frais_menage_'].apply(len_value)
+                
                 del bookings['frais_menage']
+                
                 bookings['frais_menage_'] = bookings['frais_menage_'].apply(one_value)
-                bookings['frais_menage_' ] = bookings['frais_menage_'].explode()
+
                 
-            else :
-                del bookings['frais_menage_']
                 
                 
                 
-            # merging every columns into one : taxe de sejour
-
+                # merging every columns into one : taxe de sejour
+            
+            
+                print(bookings['taxe_sejour'].head())
                 bookings['taxe_sejour_'] = bookings['taxe_sejour'].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
                 lens2 = bookings['taxe_sejour_'].apply(len_value)
+                
+                del bookings['taxe_sejour']
+                
+                bookings['taxe_sejour_'] = bookings['taxe_sejour_'].apply(one_value)
 
-                if lens2[lens2 == 2].shape[0] == 0:
-                    del bookings['taxe_sejour']
-                    bookings['taxe_sejour_'] = bookings['taxe_sejour_'].apply(one_value)
-                    bookings['taxe_sejour_'] = bookings['taxe_sejour_'].explode()
-                else:
-                    del bookings['taxe_sejour_']
 
                 # Sum of all the fees into the cleaning fee
                 bookings['frais_menage_'] = bookings['frais_menage_'].fillna(0.0)
 
                 frais_linge_serviettes = ['frais_linge_lit']
                 bookings['frais_linge_serviettes'] = 0.0
 
@@ -247,31 +241,31 @@
                     del bookings['delta']
                 except KeyError as error:
                     _, _, tb = sys.exc_info()
                     line_number = traceback.extract_tb(tb)[-1][1]       
                     print(f"Error occurred on line {line_number}: {error}")
                     print("\nThere is a problem with the columns: total-price and payé-voyageur_calculated\n")
 
-            # newly formated data to excel
-            bookings = bookings.round(2)
-            bookings.to_excel( path_output +"/Smoobu_"+file_name.split("/")[-1] + ".xlsx", index = False)
-            
-            print("\nSmoobu file created \n")
-            for file in os.listdir():
-                if file == "Smoobu_"+file_name.split("/")[-1] + ".xlsx":
-                    file_path = os.path.join(os.getcwd(), file)
-                    print("File path:", file_path)
-                    break
-            return bookings
-    
+                # newly formated data to excel
+                bookings = bookings.round(2)
+                bookings.to_excel( path_output +"/Smoobu_"+file_name.split("/")[-1] + ".xlsx", index = False)
+                
+                print("\nSmoobu file created \n")
+                for file in os.listdir():
+                    if file == "Smoobu_"+file_name.split("/")[-1] + ".xlsx":
+                        file_path = os.path.join(os.getcwd(), file)
+                        print("File path:", file_path)
+                        break
+                return bookings
     
-        else:
-            print("Le fichier n'est pas au format excel")
-            return None
         
+        else:
+                print("Le fichier n'est pas au format excel")
+                return None
+
```

### Comparing `SmoobuExtractorFormatter-1.1.7/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.1.9/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.1.7
+Version: 1.1.9
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.1.7/setup.py` & `SmoobuExtractorFormatter-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.1.7',
+    version='1.1.9',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

