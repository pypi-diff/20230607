# Comparing `tmp/SerializerAraseniiShmatovNEW-0.1.5.tar.gz` & `tmp/SerializerAraseniiShmatovNEW-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SerializerAraseniiShmatovNEW-0.1.5.tar", last modified: Tue Jun  6 23:12:36 2023, max compression
+gzip compressed data, was "SerializerAraseniiShmatovNEW-0.1.7.tar", last modified: Tue Jun  6 23:15:03 2023, max compression
```

## Comparing `SerializerAraseniiShmatovNEW-0.1.5.tar` & `SerializerAraseniiShmatovNEW-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:12:36.425678 SerializerAraseniiShmatovNEW-0.1.5/
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      727 2023-06-06 23:12:36.425678 SerializerAraseniiShmatovNEW-0.1.5/PKG-INFO
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       38 2023-05-10 18:19:58.000000 SerializerAraseniiShmatovNEW-0.1.5/README.md
-drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:12:36.425678 SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      727 2023-06-06 23:12:36.000000 SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/PKG-INFO
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      481 2023-06-06 23:12:36.000000 SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/SOURCES.txt
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)        1 2023-06-06 23:12:36.000000 SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/dependency_links.txt
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)        6 2023-06-06 23:12:36.000000 SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/requires.txt
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       18 2023-06-06 23:12:36.000000 SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/top_level.txt
-drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:12:36.425678 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      409 2023-05-10 19:32:29.000000 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/Creator.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     3151 2023-05-10 19:28:51.000000 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/JSONSerializer.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     3268 2023-05-10 19:32:13.000000 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/XMLSerializator.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      120 2023-05-10 19:27:47.000000 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/__init__.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      554 2023-05-10 18:20:03.000000 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/constans.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)    12094 2023-06-06 23:11:49.000000 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/serializer_functions.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       38 2023-06-06 23:12:36.425678 SerializerAraseniiShmatovNEW-0.1.5/setup.cfg
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     1246 2023-06-06 23:12:30.000000 SerializerAraseniiShmatovNEW-0.1.5/setup.py
+drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:15:03.414358 SerializerAraseniiShmatovNEW-0.1.7/
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      727 2023-06-06 23:15:03.414358 SerializerAraseniiShmatovNEW-0.1.7/PKG-INFO
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       38 2023-05-10 18:19:58.000000 SerializerAraseniiShmatovNEW-0.1.7/README.md
+drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:15:03.414358 SerializerAraseniiShmatovNEW-0.1.7/SerializerAraseniiShmatovNEW.egg-info/
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      727 2023-06-06 23:15:03.000000 SerializerAraseniiShmatovNEW-0.1.7/SerializerAraseniiShmatovNEW.egg-info/PKG-INFO
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      481 2023-06-06 23:15:03.000000 SerializerAraseniiShmatovNEW-0.1.7/SerializerAraseniiShmatovNEW.egg-info/SOURCES.txt
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)        1 2023-06-06 23:15:03.000000 SerializerAraseniiShmatovNEW-0.1.7/SerializerAraseniiShmatovNEW.egg-info/dependency_links.txt
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)        6 2023-06-06 23:15:03.000000 SerializerAraseniiShmatovNEW-0.1.7/SerializerAraseniiShmatovNEW.egg-info/requires.txt
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       18 2023-06-06 23:15:03.000000 SerializerAraseniiShmatovNEW-0.1.7/SerializerAraseniiShmatovNEW.egg-info/top_level.txt
+drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:15:03.414358 SerializerAraseniiShmatovNEW-0.1.7/SerilizerShmatovA/
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      409 2023-05-10 19:32:29.000000 SerializerAraseniiShmatovNEW-0.1.7/SerilizerShmatovA/Creator.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     3151 2023-05-10 19:28:51.000000 SerializerAraseniiShmatovNEW-0.1.7/SerilizerShmatovA/JSONSerializer.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     3268 2023-05-10 19:32:13.000000 SerializerAraseniiShmatovNEW-0.1.7/SerilizerShmatovA/XMLSerializator.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      120 2023-05-10 19:27:47.000000 SerializerAraseniiShmatovNEW-0.1.7/SerilizerShmatovA/__init__.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      554 2023-05-10 18:20:03.000000 SerializerAraseniiShmatovNEW-0.1.7/SerilizerShmatovA/constans.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)    12094 2023-06-06 23:14:16.000000 SerializerAraseniiShmatovNEW-0.1.7/SerilizerShmatovA/serializer_functions.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       38 2023-06-06 23:15:03.414358 SerializerAraseniiShmatovNEW-0.1.7/setup.cfg
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     1246 2023-06-06 23:15:00.000000 SerializerAraseniiShmatovNEW-0.1.7/setup.py
```

### Comparing `SerializerAraseniiShmatovNEW-0.1.5/PKG-INFO` & `SerializerAraseniiShmatovNEW-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SerializerAraseniiShmatovNEW
-Version: 0.1.5
+Version: 0.1.7
 Summary: Demo library
 Home-page: UNKNOWN
 Author: Shmatov Arsenii
 Author-email: shmatovarsenii09@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/PKG-INFO` & `SerializerAraseniiShmatovNEW-0.1.7/SerializerAraseniiShmatovNEW.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SerializerAraseniiShmatovNEW
-Version: 0.1.5
+Version: 0.1.7
 Summary: Demo library
 Home-page: UNKNOWN
 Author: Shmatov Arsenii
 Author-email: shmatovarsenii09@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/JSONSerializer.py` & `SerializerAraseniiShmatovNEW-0.1.7/SerilizerShmatovA/JSONSerializer.py`

 * *Files identical despite different names*

### Comparing `SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/XMLSerializator.py` & `SerializerAraseniiShmatovNEW-0.1.7/SerilizerShmatovA/XMLSerializator.py`

 * *Files identical despite different names*

### Comparing `SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/constans.py` & `SerializerAraseniiShmatovNEW-0.1.7/SerilizerShmatovA/constans.py`

 * *Files identical despite different names*

### Comparing `SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/serializer_functions.py` & `SerializerAraseniiShmatovNEW-0.1.7/SerilizerShmatovA/serializer_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,17 +135,17 @@
         elif (isinstance(obj.__dict__[member[0]], classmethod)):
             ser[member[0]] = {"type" : "classmethod",
                               "value" : {"type" : "function",
                                          "value": ser_func(member[1].__func__, obj)}}
         elif (isinstance(obj.__dict__[member[0]], property)):
             ser[member[0]] = {"type" : "property",
                               "value" : {"type" : "function",
-                                         "value": ser_func(member[1].__func__, obj)}}
+                                         "value": ser_func(member[1].__doc__, obj)}}
         elif (inspect.ismethod(member[1])):
-            ser[member[0]] = ser_func(member[1].__doc__, obj)
+            ser[member[0]] = ser_func(member[1].__func__, obj)
             
         elif inspect.isfunction(member[1]):
             ser[member[0]] = {"type" : "function", "value": ser_func(member[1], obj)}
         else:
             #print(member[0])
             #k = input()
             #if(k == "e"):
```

### Comparing `SerializerAraseniiShmatovNEW-0.1.5/setup.py` & `SerializerAraseniiShmatovNEW-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="SerializerAraseniiShmatovNEW",
-    version="0.1.5",
+    version="0.1.7",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Shmatov Arsenii",
     author_email="shmatovarsenii09@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
```

