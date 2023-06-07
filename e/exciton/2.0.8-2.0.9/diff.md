# Comparing `tmp/exciton-2.0.8-py3-none-any.whl.zip` & `tmp/exciton-2.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 62424 bytes, number of entries: 66
+Zip file size: 62423 bytes, number of entries: 66
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:14 exciton/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:14 exciton/ml/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-26 00:50 exciton/ml/classification/__init__.py
 -rw-rw-r--  2.0 unx     1461 b- defN 23-Mar-26 01:24 exciton/ml/classification/utils.py
 -rw-rw-r--  2.0 unx       98 b- defN 23-Mar-26 03:49 exciton/ml/classification/bert/__init__.py
 -rw-rw-r--  2.0 unx     5860 b- defN 23-Mar-29 15:08 exciton/ml/classification/bert/model.py
 -rw-rw-r--  2.0 unx     1966 b- defN 23-Mar-29 14:55 exciton/ml/classification/bert/trainer.py
@@ -56,13 +56,13 @@
 -rw-rw-r--  2.0 unx     2565 b- defN 23-May-08 00:57 exciton/nlp/text_matching/exciton_matching.py
 -rw-rw-r--  2.0 unx       87 b- defN 23-Jun-02 01:26 exciton/nlp/topic_relevance/__init__.py
 -rw-rw-r--  2.0 unx     1441 b- defN 23-Jun-02 09:29 exciton/nlp/topic_relevance/exciton_relevance.py
 -rw-rw-r--  2.0 unx       50 b- defN 23-Mar-12 04:02 exciton/nlp/translation/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 23:23 exciton/nlp/translation/m2m100/__init__.py
 -rw-rw-r--  2.0 unx     4718 b- defN 23-May-08 13:23 exciton/nlp/translation/m2m100/service.py
 -rw-rw-r--  2.0 unx     2172 b- defN 23-Mar-12 03:47 exciton/nlp/translation/m2m100/utils.py
--rw-r--r--  2.0 unx    11417 b- defN 23-Jun-07 01:50 exciton-2.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1594 b- defN 23-Jun-07 01:50 exciton-2.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 01:50 exciton-2.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Jun-07 01:50 exciton-2.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6198 b- defN 23-Jun-07 01:50 exciton-2.0.8.dist-info/RECORD
-66 files, 164836 bytes uncompressed, 52306 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx    11417 b- defN 23-Jun-07 01:54 exciton-2.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1606 b- defN 23-Jun-07 01:54 exciton-2.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 01:54 exciton-2.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jun-07 01:54 exciton-2.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6198 b- defN 23-Jun-07 01:54 exciton-2.0.9.dist-info/RECORD
+66 files, 164848 bytes uncompressed, 52305 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -177,23 +177,23 @@
 
 Filename: exciton/nlp/translation/m2m100/service.py
 Comment: 
 
 Filename: exciton/nlp/translation/m2m100/utils.py
 Comment: 
 
-Filename: exciton-2.0.8.dist-info/LICENSE
+Filename: exciton-2.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: exciton-2.0.8.dist-info/METADATA
+Filename: exciton-2.0.9.dist-info/METADATA
 Comment: 
 
-Filename: exciton-2.0.8.dist-info/WHEEL
+Filename: exciton-2.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: exciton-2.0.8.dist-info/top_level.txt
+Filename: exciton-2.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: exciton-2.0.8.dist-info/RECORD
+Filename: exciton-2.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `exciton-2.0.8.dist-info/LICENSE` & `exciton-2.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `exciton-2.0.8.dist-info/METADATA` & `exciton-2.0.9.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exciton
-Version: 2.0.8
+Version: 2.0.9
 Summary: Natural Language Processing by the Exciton Research
 Home-page: https://excitonx.com
 Author: The Exciton Research Team
 Author-email: excitonx@gmail.com
 License: UNKNOWN
 Keywords: NLP Deep Learning
 Platform: UNKNOWN
@@ -25,15 +25,15 @@
 Requires-Dist: spacy (==3.5.2)
 Requires-Dist: torch (==2.0.0)
 Requires-Dist: tqdm (==4.65.0)
 Requires-Dist: transformers (==4.28.1)
 
 # Exciton NLP - A tool for natural language processing
 
-Exciton NLP is designed and maintained by ExcitonX for different NLP tasks, including multilingual classification, NER, translation, etc.
+Exciton NLP is designed and maintained by the Exciton Research for different NLP tasks, including multilingual classification, NER, translation, etc.
 
 ## Installation
 Use ``pip`` to install exciton. Run:
 
 ```
 pip install -U exciton
 ```
```

## Comparing `exciton-2.0.8.dist-info/RECORD` & `exciton-2.0.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -55,12 +55,12 @@
 exciton/nlp/text_matching/exciton_matching.py,sha256=a99bzY5117DLAGb_AgV_4ai6buVYrMmyvengo18CeIU,2565
 exciton/nlp/topic_relevance/__init__.py,sha256=lKpWm-3G17hrZR86ckItV9w6gYxd1yULD_NE18-OFBY,87
 exciton/nlp/topic_relevance/exciton_relevance.py,sha256=bo3tZkum03mGiV8ZhbPQUcX0hseAum9hE4J8hFAWwYU,1441
 exciton/nlp/translation/__init__.py,sha256=gE0YV-s4pB7VQWdsg04hALOBBpuWaQ3AUqpY9rvgI_8,50
 exciton/nlp/translation/m2m100/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 exciton/nlp/translation/m2m100/service.py,sha256=FIXc5sUtZzywzis_CZ2doF6sqrPcKcyMO8EhLgFTwjY,4718
 exciton/nlp/translation/m2m100/utils.py,sha256=GE8qg2deaHBMVMIHS32Hb5TCxO453kuncQrdJsnRIoU,2172
-exciton-2.0.8.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
-exciton-2.0.8.dist-info/METADATA,sha256=VkgthdUqeRAy9eXkoPe9_lQMFmTQZ8YAoR6VD5W1AP4,1594
-exciton-2.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-exciton-2.0.8.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
-exciton-2.0.8.dist-info/RECORD,,
+exciton-2.0.9.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
+exciton-2.0.9.dist-info/METADATA,sha256=HnMvf3loWmFnSM_Lp5jfpmveqa9NbcCRm6su15E_OuU,1606
+exciton-2.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+exciton-2.0.9.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
+exciton-2.0.9.dist-info/RECORD,,
```

