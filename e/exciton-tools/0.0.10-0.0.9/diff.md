# Comparing `tmp/exciton_tools-0.0.10-py3-none-any.whl.zip` & `tmp/exciton_tools-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 9466 bytes, number of entries: 16
+Zip file size: 9598 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-04 01:58 exciton_tools/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-06 20:06 exciton_tools/elasticsearch/__init__.py
 -rw-rw-r--  2.0 unx     1512 b- defN 23-Jun-07 01:30 exciton_tools/elasticsearch/document.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-06 20:07 exciton_tools/rabbitmq/__init__.py
 -rw-rw-r--  2.0 unx     1318 b- defN 23-Jun-07 01:30 exciton_tools/rabbitmq/document.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-04 01:58 extools/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-06 20:06 extools/elasticsearch/__init__.py
 -rw-rw-r--  2.0 unx     1512 b- defN 23-Jun-07 01:30 extools/elasticsearch/document.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-04 01:58 extools/ml/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-06 20:07 extools/rabbitmq/__init__.py
 -rw-rw-r--  2.0 unx     1318 b- defN 23-Jun-07 01:30 extools/rabbitmq/document.py
--rw-r--r--  2.0 unx    11417 b- defN 23-Jun-07 01:44 exciton_tools-0.0.10.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1331 b- defN 23-Jun-07 01:44 exciton_tools-0.0.10.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 01:44 exciton_tools-0.0.10.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Jun-07 01:44 exciton_tools-0.0.10.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1362 b- defN 23-Jun-07 01:44 exciton_tools-0.0.10.dist-info/RECORD
-16 files, 19876 bytes uncompressed, 7172 bytes compressed:  63.9%
+-rw-r--r--  2.0 unx    11417 b- defN 23-Jun-07 01:37 exciton_tools-0.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1568 b- defN 23-Jun-07 01:37 exciton_tools-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 01:37 exciton_tools-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jun-07 01:37 exciton_tools-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1357 b- defN 23-Jun-07 01:37 exciton_tools-0.0.9.dist-info/RECORD
+16 files, 20108 bytes uncompressed, 7314 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: extools/rabbitmq/__init__.py
 Comment: 
 
 Filename: extools/rabbitmq/document.py
 Comment: 
 
-Filename: exciton_tools-0.0.10.dist-info/LICENSE
+Filename: exciton_tools-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: exciton_tools-0.0.10.dist-info/METADATA
+Filename: exciton_tools-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: exciton_tools-0.0.10.dist-info/WHEEL
+Filename: exciton_tools-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: exciton_tools-0.0.10.dist-info/top_level.txt
+Filename: exciton_tools-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: exciton_tools-0.0.10.dist-info/RECORD
+Filename: exciton_tools-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `exciton_tools-0.0.10.dist-info/LICENSE` & `exciton_tools-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `exciton_tools-0.0.10.dist-info/METADATA` & `exciton_tools-0.0.9.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exciton-tools
-Version: 0.0.10
+Version: 0.0.9
 Summary: Exciton Infrastructure Tools
 Home-page: https://excitonx.com
 Author: The Exciton Research
 Author-email: excitonx@gmail.com
 License: UNKNOWN
 Keywords: exciton tools
 Platform: UNKNOWN
@@ -31,20 +31,25 @@
 
 Exciton NLP is designed and maintained by ExcitonX for different NLP tasks, including multilingual classification, NER, translation, etc.
 
 ## Installation
 Use ``pip`` to install exciton. Run:
 
 ```
-pip install -U exciton_tools
+pip install -U exciton
 ```
 
 ## Usage
 
 ```
 
-from exciton_tools.elasticsearch import get_all_documents
-
+from exciton.nlp.translation import M2M100
 
+model = M2M100(model="m2m100_1.2b", device="cuda")
+source = [
+    {"id": 1, "source": "I love you!", "source_lang": "en", "target_lang": "zh"},
+    {"id": 2, "source": "我爱你！", "source_lang": "zh", "target_lang": "en"}
+]
+results = model.predict(source)
 
 ```
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `exciton_tools-0.0.10.dist-info/RECORD` & `exciton_tools-0.0.9.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 exciton_tools/rabbitmq/document.py,sha256=psO1hJIL8ZO0n30bchPnMAaw3IC_8r8MXKjGJ-XGd6Q,1318
 extools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 extools/elasticsearch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 extools/elasticsearch/document.py,sha256=hkdEERVWmVHUUA-vKMxLKic86Lehrto4Lv2qbF9Cb-o,1512
 extools/ml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 extools/rabbitmq/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 extools/rabbitmq/document.py,sha256=psO1hJIL8ZO0n30bchPnMAaw3IC_8r8MXKjGJ-XGd6Q,1318
-exciton_tools-0.0.10.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
-exciton_tools-0.0.10.dist-info/METADATA,sha256=H7XxxJTKIBIUqvXfMxxDN_zphUulnTj-xS5MOazuGTo,1331
-exciton_tools-0.0.10.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-exciton_tools-0.0.10.dist-info/top_level.txt,sha256=nztTLDVnIrMd3Pv2FFtih6C_oClvYZoNorctjafXEUI,14
-exciton_tools-0.0.10.dist-info/RECORD,,
+exciton_tools-0.0.9.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
+exciton_tools-0.0.9.dist-info/METADATA,sha256=s2_SvIJ13-5leCUmZu6ZOhDR8YJih6i2AB9c0CWYobg,1568
+exciton_tools-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+exciton_tools-0.0.9.dist-info/top_level.txt,sha256=nztTLDVnIrMd3Pv2FFtih6C_oClvYZoNorctjafXEUI,14
+exciton_tools-0.0.9.dist-info/RECORD,,
```

