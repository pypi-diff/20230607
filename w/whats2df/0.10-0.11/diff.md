# Comparing `tmp/whats2df-0.10.tar.gz` & `tmp/whats2df-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whats2df-0.10.tar", last modified: Tue Jun  6 17:44:31 2023, max compression
+gzip compressed data, was "whats2df-0.11.tar", last modified: Wed Jun  7 00:22:17 2023, max compression
```

## Comparing `whats2df-0.10.tar` & `whats2df-0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 17:44:31.534259 whats2df-0.10/
--rw-rw-rw-   0        0        0     1148 2023-06-06 17:44:20.000000 whats2df-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      125 2023-06-06 17:44:19.000000 whats2df-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2601 2023-06-06 17:44:31.534259 whats2df-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1941 2023-06-06 17:35:22.000000 whats2df-0.10/README.md
--rw-rw-rw-   0        0        0       85 2023-06-06 17:44:31.535256 whats2df-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1542 2023-06-06 17:44:30.000000 whats2df-0.10/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:44:31.530271 whats2df-0.10/whats2df/
--rw-rw-rw-   0        0        0     1941 2023-06-06 17:35:22.000000 whats2df-0.10/whats2df/README.MD
--rw-rw-rw-   0        0        0      970 2023-06-06 17:44:02.000000 whats2df-0.10/whats2df/__init__.py
--rw-rw-rw-   0        0        0      106 2023-06-06 17:44:30.000000 whats2df-0.10/whats2df/requirements.txt
--rw-rw-rw-   0        0        0    44043 2023-06-06 17:44:30.000000 whats2df-0.10/whats2df/thirdparty.json
--rw-rw-rw-   0        0        0    22842 2023-06-06 17:03:25.000000 whats2df-0.10/whats2df/whats2df.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:44:31.533262 whats2df-0.10/whats2df.egg-info/
--rw-rw-rw-   0        0        0     2601 2023-06-06 17:44:31.000000 whats2df-0.10/whats2df.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-06-06 17:44:31.000000 whats2df-0.10/whats2df.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 17:44:31.000000 whats2df-0.10/whats2df.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-06-06 17:44:31.000000 whats2df-0.10/whats2df.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 17:44:31.000000 whats2df-0.10/whats2df.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 00:22:17.665870 whats2df-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-06-07 00:22:03.000000 whats2df-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      125 2023-06-07 00:21:58.000000 whats2df-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2799 2023-06-07 00:22:17.665870 whats2df-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2141 2023-06-07 00:21:34.000000 whats2df-0.11/README.md
+-rw-rw-rw-   0        0        0       85 2023-06-07 00:22:17.666867 whats2df-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1542 2023-06-07 00:22:16.000000 whats2df-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 00:22:17.661880 whats2df-0.11/whats2df/
+-rw-rw-rw-   0        0        0     2141 2023-06-07 00:21:34.000000 whats2df-0.11/whats2df/README.MD
+-rw-rw-rw-   0        0        0      970 2023-06-06 17:44:02.000000 whats2df-0.11/whats2df/__init__.py
+-rw-rw-rw-   0        0        0      106 2023-06-07 00:22:16.000000 whats2df-0.11/whats2df/requirements.txt
+-rw-rw-rw-   0        0        0    44043 2023-06-07 00:22:16.000000 whats2df-0.11/whats2df/thirdparty.json
+-rw-rw-rw-   0        0        0    22842 2023-06-06 17:03:25.000000 whats2df-0.11/whats2df/whats2df.py
+drwxrwxrwx   0        0        0        0 2023-06-07 00:22:17.664873 whats2df-0.11/whats2df.egg-info/
+-rw-rw-rw-   0        0        0     2799 2023-06-07 00:22:17.000000 whats2df-0.11/whats2df.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-06-07 00:22:17.000000 whats2df-0.11/whats2df.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 00:22:17.000000 whats2df-0.11/whats2df.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-06-07 00:22:17.000000 whats2df-0.11/whats2df.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 00:22:17.000000 whats2df-0.11/whats2df.egg-info/top_level.txt
```

### Comparing `whats2df-0.10/LICENSE.rst` & `whats2df-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `whats2df-0.10/PKG-INFO` & `whats2df-0.11/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whats2df
-Version: 0.10
+Version: 0.11
 Summary: Whatsapp to Pandas DataFrame (csv/xlsx/pkl) Doesn't require root access!
 Home-page: https://github.com/hansalemaos/whats2df
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: whatsapp,pandas,DataFrame,convert
 Classifier: Development Status :: 4 - Beta
@@ -16,14 +16,19 @@
 License-File: LICENSE.rst
 
 
 # Finding certain messages in your WhatsApp message is sometimes hard, but Pandas makes it easier. Doesn't require root access!
 
 #### Tested against Google Pixel 6 / Windows 10 / Python 3.10
 
+### Tutorial (Brazilian Portuguese)
+
+[![YT](https://i.ytimg.com/vi/KG_xC2TmbDo/maxresdefault.jpg)](https://www.youtube.com/watch?v=KG_xC2TmbDo)
+[https://www.youtube.com/watch?v=KG_xC2TmbDo]()
+
 ```python
 pip install whats2df
 
 # This is the updated version of https://github.com/hansalemaos/a_pandas_ex_whatsapp_to_df
 ```
 
 ## Follow these steps if you want to avoid rooting your cell phone:
```

### Comparing `whats2df-0.10/README.md` & `whats2df-0.11/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Finding certain messages in your WhatsApp message is sometimes hard, but Pandas makes it easier. Doesn't require root access!
 
 #### Tested against Google Pixel 6 / Windows 10 / Python 3.10
 
+### Tutorial (Brazilian Portuguese)
+
+[![YT](https://i.ytimg.com/vi/KG_xC2TmbDo/maxresdefault.jpg)](https://www.youtube.com/watch?v=KG_xC2TmbDo)
+[https://www.youtube.com/watch?v=KG_xC2TmbDo]()
+
 ```python
 pip install whats2df
 
 # This is the updated version of https://github.com/hansalemaos/a_pandas_ex_whatsapp_to_df
 ```
 
 ## Follow these steps if you want to avoid rooting your cell phone:
@@ -34,8 +39,8 @@
 
 ## CLI 
 
 ```
 # adjust the path to "whats2df.py"
 
 python C:\ProgramData\anaconda3\envs\nu\Lib\site-packages\whats2df\whats2df.py --decryptkey e2c412cea3b0a662e47a2062fffa0db7cf7cca093636abf5bca6e701a6fae3bc --encrypted_db C:\Users\hansc\Desktop\msgstore.db.crypt15 --decrypted_db C:\Users\hansc\Desktop\msgstore.db --output_df C:\Users\hansc\Desktop\msgstore.pkl --download_sql_dll 1
-```
+```
```

### Comparing `whats2df-0.10/setup.py` & `whats2df-0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Whatsapp to Pandas DataFrame (csv/xlsx/pkl) Doesn't require root access!'''
 
 # Setting up
 setup(
     name="whats2df",
     version=VERSION,
     license='MIT',
```

### Comparing `whats2df-0.10/whats2df/README.MD` & `whats2df-0.11/whats2df/README.MD`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Finding certain messages in your WhatsApp message is sometimes hard, but Pandas makes it easier. Doesn't require root access!
 
 #### Tested against Google Pixel 6 / Windows 10 / Python 3.10
 
+### Tutorial (Brazilian Portuguese)
+
+[![YT](https://i.ytimg.com/vi/KG_xC2TmbDo/maxresdefault.jpg)](https://www.youtube.com/watch?v=KG_xC2TmbDo)
+[https://www.youtube.com/watch?v=KG_xC2TmbDo]()
+
 ```python
 pip install whats2df
 
 # This is the updated version of https://github.com/hansalemaos/a_pandas_ex_whatsapp_to_df
 ```
 
 ## Follow these steps if you want to avoid rooting your cell phone:
@@ -34,8 +39,8 @@
 
 ## CLI 
 
 ```
 # adjust the path to "whats2df.py"
 
 python C:\ProgramData\anaconda3\envs\nu\Lib\site-packages\whats2df\whats2df.py --decryptkey e2c412cea3b0a662e47a2062fffa0db7cf7cca093636abf5bca6e701a6fae3bc --encrypted_db C:\Users\hansc\Desktop\msgstore.db.crypt15 --decrypted_db C:\Users\hansc\Desktop\msgstore.db --output_df C:\Users\hansc\Desktop\msgstore.pkl --download_sql_dll 1
-```
+```
```

### Comparing `whats2df-0.10/whats2df/__init__.py` & `whats2df-0.11/whats2df/__init__.py`

 * *Files identical despite different names*

### Comparing `whats2df-0.10/whats2df/thirdparty.json` & `whats2df-0.11/whats2df/thirdparty.json`

 * *Files identical despite different names*

### Comparing `whats2df-0.10/whats2df/whats2df.py` & `whats2df-0.11/whats2df/whats2df.py`

 * *Files identical despite different names*

### Comparing `whats2df-0.10/whats2df.egg-info/PKG-INFO` & `whats2df-0.11/whats2df.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whats2df
-Version: 0.10
+Version: 0.11
 Summary: Whatsapp to Pandas DataFrame (csv/xlsx/pkl) Doesn't require root access!
 Home-page: https://github.com/hansalemaos/whats2df
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: whatsapp,pandas,DataFrame,convert
 Classifier: Development Status :: 4 - Beta
@@ -16,14 +16,19 @@
 License-File: LICENSE.rst
 
 
 # Finding certain messages in your WhatsApp message is sometimes hard, but Pandas makes it easier. Doesn't require root access!
 
 #### Tested against Google Pixel 6 / Windows 10 / Python 3.10
 
+### Tutorial (Brazilian Portuguese)
+
+[![YT](https://i.ytimg.com/vi/KG_xC2TmbDo/maxresdefault.jpg)](https://www.youtube.com/watch?v=KG_xC2TmbDo)
+[https://www.youtube.com/watch?v=KG_xC2TmbDo]()
+
 ```python
 pip install whats2df
 
 # This is the updated version of https://github.com/hansalemaos/a_pandas_ex_whatsapp_to_df
 ```
 
 ## Follow these steps if you want to avoid rooting your cell phone:
```

