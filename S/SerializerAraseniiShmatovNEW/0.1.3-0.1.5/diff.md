# Comparing `tmp/SerializerAraseniiShmatovNEW-0.1.3.tar.gz` & `tmp/SerializerAraseniiShmatovNEW-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SerializerAraseniiShmatovNEW-0.1.3.tar", last modified: Tue Jun  6 23:09:32 2023, max compression
+gzip compressed data, was "SerializerAraseniiShmatovNEW-0.1.5.tar", last modified: Tue Jun  6 23:12:36 2023, max compression
```

## Comparing `SerializerAraseniiShmatovNEW-0.1.3.tar` & `SerializerAraseniiShmatovNEW-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:09:32.288505 SerializerAraseniiShmatovNEW-0.1.3/
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      727 2023-06-06 23:09:32.288505 SerializerAraseniiShmatovNEW-0.1.3/PKG-INFO
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       38 2023-05-10 18:19:58.000000 SerializerAraseniiShmatovNEW-0.1.3/README.md
-drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:09:32.288505 SerializerAraseniiShmatovNEW-0.1.3/SerializerAraseniiShmatovNEW.egg-info/
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      727 2023-06-06 23:09:32.000000 SerializerAraseniiShmatovNEW-0.1.3/SerializerAraseniiShmatovNEW.egg-info/PKG-INFO
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      481 2023-06-06 23:09:32.000000 SerializerAraseniiShmatovNEW-0.1.3/SerializerAraseniiShmatovNEW.egg-info/SOURCES.txt
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)        1 2023-06-06 23:09:32.000000 SerializerAraseniiShmatovNEW-0.1.3/SerializerAraseniiShmatovNEW.egg-info/dependency_links.txt
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)        6 2023-06-06 23:09:32.000000 SerializerAraseniiShmatovNEW-0.1.3/SerializerAraseniiShmatovNEW.egg-info/requires.txt
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       18 2023-06-06 23:09:32.000000 SerializerAraseniiShmatovNEW-0.1.3/SerializerAraseniiShmatovNEW.egg-info/top_level.txt
-drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:09:32.288505 SerializerAraseniiShmatovNEW-0.1.3/SerilizerShmatovA/
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      409 2023-05-10 19:32:29.000000 SerializerAraseniiShmatovNEW-0.1.3/SerilizerShmatovA/Creator.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     3151 2023-05-10 19:28:51.000000 SerializerAraseniiShmatovNEW-0.1.3/SerilizerShmatovA/JSONSerializer.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     3268 2023-05-10 19:32:13.000000 SerializerAraseniiShmatovNEW-0.1.3/SerilizerShmatovA/XMLSerializator.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      120 2023-05-10 19:27:47.000000 SerializerAraseniiShmatovNEW-0.1.3/SerilizerShmatovA/__init__.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      554 2023-05-10 18:20:03.000000 SerializerAraseniiShmatovNEW-0.1.3/SerilizerShmatovA/constans.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)    12095 2023-06-06 23:07:20.000000 SerializerAraseniiShmatovNEW-0.1.3/SerilizerShmatovA/serializer_functions.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       38 2023-06-06 23:09:32.288505 SerializerAraseniiShmatovNEW-0.1.3/setup.cfg
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     1246 2023-06-06 23:09:27.000000 SerializerAraseniiShmatovNEW-0.1.3/setup.py
+drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:12:36.425678 SerializerAraseniiShmatovNEW-0.1.5/
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      727 2023-06-06 23:12:36.425678 SerializerAraseniiShmatovNEW-0.1.5/PKG-INFO
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       38 2023-05-10 18:19:58.000000 SerializerAraseniiShmatovNEW-0.1.5/README.md
+drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:12:36.425678 SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      727 2023-06-06 23:12:36.000000 SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/PKG-INFO
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      481 2023-06-06 23:12:36.000000 SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/SOURCES.txt
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)        1 2023-06-06 23:12:36.000000 SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/dependency_links.txt
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)        6 2023-06-06 23:12:36.000000 SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/requires.txt
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       18 2023-06-06 23:12:36.000000 SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/top_level.txt
+drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:12:36.425678 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      409 2023-05-10 19:32:29.000000 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/Creator.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     3151 2023-05-10 19:28:51.000000 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/JSONSerializer.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     3268 2023-05-10 19:32:13.000000 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/XMLSerializator.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      120 2023-05-10 19:27:47.000000 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/__init__.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      554 2023-05-10 18:20:03.000000 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/constans.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)    12094 2023-06-06 23:11:49.000000 SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/serializer_functions.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       38 2023-06-06 23:12:36.425678 SerializerAraseniiShmatovNEW-0.1.5/setup.cfg
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     1246 2023-06-06 23:12:30.000000 SerializerAraseniiShmatovNEW-0.1.5/setup.py
```

### Comparing `SerializerAraseniiShmatovNEW-0.1.3/PKG-INFO` & `SerializerAraseniiShmatovNEW-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SerializerAraseniiShmatovNEW
-Version: 0.1.3
+Version: 0.1.5
 Summary: Demo library
 Home-page: UNKNOWN
 Author: Shmatov Arsenii
 Author-email: shmatovarsenii09@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `SerializerAraseniiShmatovNEW-0.1.3/SerializerAraseniiShmatovNEW.egg-info/PKG-INFO` & `SerializerAraseniiShmatovNEW-0.1.5/SerializerAraseniiShmatovNEW.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SerializerAraseniiShmatovNEW
-Version: 0.1.3
+Version: 0.1.5
 Summary: Demo library
 Home-page: UNKNOWN
 Author: Shmatov Arsenii
 Author-email: shmatovarsenii09@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `SerializerAraseniiShmatovNEW-0.1.3/SerilizerShmatovA/JSONSerializer.py` & `SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/JSONSerializer.py`

 * *Files identical despite different names*

### Comparing `SerializerAraseniiShmatovNEW-0.1.3/SerilizerShmatovA/XMLSerializator.py` & `SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/XMLSerializator.py`

 * *Files identical despite different names*

### Comparing `SerializerAraseniiShmatovNEW-0.1.3/SerilizerShmatovA/constans.py` & `SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/constans.py`

 * *Files identical despite different names*

### Comparing `SerializerAraseniiShmatovNEW-0.1.3/SerilizerShmatovA/serializer_functions.py` & `SerializerAraseniiShmatovNEW-0.1.5/SerilizerShmatovA/serializer_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                               "value" : {"type" : "function",
                                          "value": ser_func(member[1].__func__, obj)}}
         elif (isinstance(obj.__dict__[member[0]], property)):
             ser[member[0]] = {"type" : "property",
                               "value" : {"type" : "function",
                                          "value": ser_func(member[1].__func__, obj)}}
         elif (inspect.ismethod(member[1])):
-            ser[member[0]] = ser_func(member[1].__func__, obj)
+            ser[member[0]] = ser_func(member[1].__doc__, obj)
             
         elif inspect.isfunction(member[1]):
             ser[member[0]] = {"type" : "function", "value": ser_func(member[1], obj)}
         else:
             #print(member[0])
             #k = input()
             #if(k == "e"):
```

### Comparing `SerializerAraseniiShmatovNEW-0.1.3/setup.py` & `SerializerAraseniiShmatovNEW-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="SerializerAraseniiShmatovNEW",
-    version="0.1.3",
+    version="0.1.5",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Shmatov Arsenii",
     author_email="shmatovarsenii09@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
```

