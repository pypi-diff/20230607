# Comparing `tmp/SerializerAraseniiShmatovNEW-0.1.1.tar.gz` & `tmp/SerializerAraseniiShmatovNEW-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SerializerAraseniiShmatovNEW-0.1.1.tar", last modified: Tue Jun  6 22:57:50 2023, max compression
+gzip compressed data, was "SerializerAraseniiShmatovNEW-0.1.2.tar", last modified: Tue Jun  6 23:05:23 2023, max compression
```

## Comparing `SerializerAraseniiShmatovNEW-0.1.1.tar` & `SerializerAraseniiShmatovNEW-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 22:57:50.840099 SerializerAraseniiShmatovNEW-0.1.1/
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      727 2023-06-06 22:57:50.840099 SerializerAraseniiShmatovNEW-0.1.1/PKG-INFO
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       38 2023-05-10 18:19:58.000000 SerializerAraseniiShmatovNEW-0.1.1/README.md
-drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 22:57:50.836099 SerializerAraseniiShmatovNEW-0.1.1/SerializerAraseniiShmatovNEW.egg-info/
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      727 2023-06-06 22:57:50.000000 SerializerAraseniiShmatovNEW-0.1.1/SerializerAraseniiShmatovNEW.egg-info/PKG-INFO
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      481 2023-06-06 22:57:50.000000 SerializerAraseniiShmatovNEW-0.1.1/SerializerAraseniiShmatovNEW.egg-info/SOURCES.txt
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)        1 2023-06-06 22:57:50.000000 SerializerAraseniiShmatovNEW-0.1.1/SerializerAraseniiShmatovNEW.egg-info/dependency_links.txt
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)        6 2023-06-06 22:57:50.000000 SerializerAraseniiShmatovNEW-0.1.1/SerializerAraseniiShmatovNEW.egg-info/requires.txt
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       18 2023-06-06 22:57:50.000000 SerializerAraseniiShmatovNEW-0.1.1/SerializerAraseniiShmatovNEW.egg-info/top_level.txt
-drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 22:57:50.840099 SerializerAraseniiShmatovNEW-0.1.1/SerilizerShmatovA/
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      409 2023-05-10 19:32:29.000000 SerializerAraseniiShmatovNEW-0.1.1/SerilizerShmatovA/Creator.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     3151 2023-05-10 19:28:51.000000 SerializerAraseniiShmatovNEW-0.1.1/SerilizerShmatovA/JSONSerializer.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     3268 2023-05-10 19:32:13.000000 SerializerAraseniiShmatovNEW-0.1.1/SerilizerShmatovA/XMLSerializator.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      120 2023-05-10 19:27:47.000000 SerializerAraseniiShmatovNEW-0.1.1/SerilizerShmatovA/__init__.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      554 2023-05-10 18:20:03.000000 SerializerAraseniiShmatovNEW-0.1.1/SerilizerShmatovA/constans.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)    11989 2023-06-06 22:54:57.000000 SerializerAraseniiShmatovNEW-0.1.1/SerilizerShmatovA/serializer_functions.py
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       38 2023-06-06 22:57:50.840099 SerializerAraseniiShmatovNEW-0.1.1/setup.cfg
--rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     1246 2023-06-06 22:57:38.000000 SerializerAraseniiShmatovNEW-0.1.1/setup.py
+drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:05:23.979672 SerializerAraseniiShmatovNEW-0.1.2/
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      727 2023-06-06 23:05:23.975672 SerializerAraseniiShmatovNEW-0.1.2/PKG-INFO
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       38 2023-05-10 18:19:58.000000 SerializerAraseniiShmatovNEW-0.1.2/README.md
+drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:05:23.975672 SerializerAraseniiShmatovNEW-0.1.2/SerializerAraseniiShmatovNEW.egg-info/
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      727 2023-06-06 23:05:23.000000 SerializerAraseniiShmatovNEW-0.1.2/SerializerAraseniiShmatovNEW.egg-info/PKG-INFO
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      481 2023-06-06 23:05:23.000000 SerializerAraseniiShmatovNEW-0.1.2/SerializerAraseniiShmatovNEW.egg-info/SOURCES.txt
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)        1 2023-06-06 23:05:23.000000 SerializerAraseniiShmatovNEW-0.1.2/SerializerAraseniiShmatovNEW.egg-info/dependency_links.txt
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)        6 2023-06-06 23:05:23.000000 SerializerAraseniiShmatovNEW-0.1.2/SerializerAraseniiShmatovNEW.egg-info/requires.txt
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       18 2023-06-06 23:05:23.000000 SerializerAraseniiShmatovNEW-0.1.2/SerializerAraseniiShmatovNEW.egg-info/top_level.txt
+drwxrwxr-x   0 arsenii   (1000) arsenii   (1000)        0 2023-06-06 23:05:23.975672 SerializerAraseniiShmatovNEW-0.1.2/SerilizerShmatovA/
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      409 2023-05-10 19:32:29.000000 SerializerAraseniiShmatovNEW-0.1.2/SerilizerShmatovA/Creator.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     3151 2023-05-10 19:28:51.000000 SerializerAraseniiShmatovNEW-0.1.2/SerilizerShmatovA/JSONSerializer.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     3268 2023-05-10 19:32:13.000000 SerializerAraseniiShmatovNEW-0.1.2/SerilizerShmatovA/XMLSerializator.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      120 2023-05-10 19:27:47.000000 SerializerAraseniiShmatovNEW-0.1.2/SerilizerShmatovA/__init__.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)      554 2023-05-10 18:20:03.000000 SerializerAraseniiShmatovNEW-0.1.2/SerilizerShmatovA/constans.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)    12085 2023-06-06 23:04:25.000000 SerializerAraseniiShmatovNEW-0.1.2/SerilizerShmatovA/serializer_functions.py
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)       38 2023-06-06 23:05:23.979672 SerializerAraseniiShmatovNEW-0.1.2/setup.cfg
+-rw-rw-r--   0 arsenii   (1000) arsenii   (1000)     1246 2023-06-06 23:05:04.000000 SerializerAraseniiShmatovNEW-0.1.2/setup.py
```

### Comparing `SerializerAraseniiShmatovNEW-0.1.1/PKG-INFO` & `SerializerAraseniiShmatovNEW-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SerializerAraseniiShmatovNEW
-Version: 0.1.1
+Version: 0.1.2
 Summary: Demo library
 Home-page: UNKNOWN
 Author: Shmatov Arsenii
 Author-email: shmatovarsenii09@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `SerializerAraseniiShmatovNEW-0.1.1/SerializerAraseniiShmatovNEW.egg-info/PKG-INFO` & `SerializerAraseniiShmatovNEW-0.1.2/SerializerAraseniiShmatovNEW.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SerializerAraseniiShmatovNEW
-Version: 0.1.1
+Version: 0.1.2
 Summary: Demo library
 Home-page: UNKNOWN
 Author: Shmatov Arsenii
 Author-email: shmatovarsenii09@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `SerializerAraseniiShmatovNEW-0.1.1/SerilizerShmatovA/JSONSerializer.py` & `SerializerAraseniiShmatovNEW-0.1.2/SerilizerShmatovA/JSONSerializer.py`

 * *Files identical despite different names*

### Comparing `SerializerAraseniiShmatovNEW-0.1.1/SerilizerShmatovA/XMLSerializator.py` & `SerializerAraseniiShmatovNEW-0.1.2/SerilizerShmatovA/XMLSerializator.py`

 * *Files identical despite different names*

### Comparing `SerializerAraseniiShmatovNEW-0.1.1/SerilizerShmatovA/constans.py` & `SerializerAraseniiShmatovNEW-0.1.2/SerilizerShmatovA/constans.py`

 * *Files identical despite different names*

### Comparing `SerializerAraseniiShmatovNEW-0.1.1/SerilizerShmatovA/serializer_functions.py` & `SerializerAraseniiShmatovNEW-0.1.2/SerilizerShmatovA/serializer_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,17 @@
     
     elif (obj["type"] == "staticmethod"):
         return staticmethod(deserialize(obj["value"]))
     
     elif (obj["type"] == "classmethod"):
         return classmethod(deserialize(obj["value"]))  
     
+    elif (obj["type"] == "property"):
+        return property(deserialize(obj["value"]))  
+    
     elif (obj["type"] == "object"):
         return deser_object(obj["value"]) 
     
     
 def generator_type(_type, obj):
     if (_type == "int"):
         return int(obj)
```

### Comparing `SerializerAraseniiShmatovNEW-0.1.1/setup.py` & `SerializerAraseniiShmatovNEW-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="SerializerAraseniiShmatovNEW",
-    version="0.1.1",
+    version="0.1.2",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Shmatov Arsenii",
     author_email="shmatovarsenii09@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
```

