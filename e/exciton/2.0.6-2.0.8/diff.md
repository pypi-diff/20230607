# Comparing `tmp/exciton-2.0.6-py3-none-any.whl.zip` & `tmp/exciton-2.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,19 @@
-Zip file size: 57758 bytes, number of entries: 60
+Zip file size: 62424 bytes, number of entries: 66
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:14 exciton/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 03:14 exciton/ml/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-26 00:50 exciton/ml/classification/__init__.py
 -rw-rw-r--  2.0 unx     1461 b- defN 23-Mar-26 01:24 exciton/ml/classification/utils.py
 -rw-rw-r--  2.0 unx       98 b- defN 23-Mar-26 03:49 exciton/ml/classification/bert/__init__.py
 -rw-rw-r--  2.0 unx     5860 b- defN 23-Mar-29 15:08 exciton/ml/classification/bert/model.py
 -rw-rw-r--  2.0 unx     1966 b- defN 23-Mar-29 14:55 exciton/ml/classification/bert/trainer.py
+-rw-rw-r--  2.0 unx       98 b- defN 23-Mar-26 03:49 exciton/ml/classification/xlm_roberta/__init__.py
+-rw-rw-r--  2.0 unx     4845 b- defN 23-Jun-02 09:27 exciton/ml/classification/xlm_roberta/model.py
+-rw-rw-r--  2.0 unx     2075 b- defN 23-Jun-02 02:38 exciton/ml/classification/xlm_roberta/trainer.py
+-rw-rw-r--  2.0 unx     1775 b- defN 23-Jun-02 02:13 exciton/ml/classification/xlm_roberta/utils.py
 -rw-rw-r--  2.0 unx       98 b- defN 23-Mar-26 03:44 exciton/ml/classification/xlmroberta/__init__.py
 -rw-rw-r--  2.0 unx     4679 b- defN 23-Mar-26 03:45 exciton/ml/classification/xlmroberta/model.py
 -rw-rw-r--  2.0 unx     1959 b- defN 23-Mar-26 03:38 exciton/ml/classification/xlmroberta/trainer.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-09 19:06 exciton/ml/engine/__init__.py
 -rw-rw-r--  2.0 unx     8476 b- defN 23-May-28 12:41 exciton/ml/engine/end2end.py
 -rw-rw-r--  2.0 unx      916 b- defN 23-Mar-17 00:44 exciton/ml/engine/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-09 19:06 exciton/ml/tagging/__init__.py
@@ -46,17 +50,19 @@
 -rw-rw-r--  2.0 unx     3192 b- defN 23-Mar-23 02:02 exciton/nlp/named_entity_recogonition/utils.py
 -rw-rw-r--  2.0 unx     3876 b- defN 23-Mar-23 02:49 exciton/nlp/named_entity_recogonition/xlmroberta.py
 -rw-rw-r--  2.0 unx       59 b- defN 23-May-05 01:21 exciton/nlp/sentence_tokenizer/__init__.py
 -rw-rw-r--  2.0 unx     4983 b- defN 23-May-09 15:57 exciton/nlp/sentence_tokenizer/exciton_sbd.py
 -rw-rw-r--  2.0 unx     3977 b- defN 23-May-02 03:18 exciton/nlp/sentence_tokenizer/service.py
 -rw-rw-r--  2.0 unx       84 b- defN 23-May-01 15:45 exciton/nlp/text_matching/__init__.py
 -rw-rw-r--  2.0 unx     2565 b- defN 23-May-08 00:57 exciton/nlp/text_matching/exciton_matching.py
+-rw-rw-r--  2.0 unx       87 b- defN 23-Jun-02 01:26 exciton/nlp/topic_relevance/__init__.py
+-rw-rw-r--  2.0 unx     1441 b- defN 23-Jun-02 09:29 exciton/nlp/topic_relevance/exciton_relevance.py
 -rw-rw-r--  2.0 unx       50 b- defN 23-Mar-12 04:02 exciton/nlp/translation/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-11 23:23 exciton/nlp/translation/m2m100/__init__.py
 -rw-rw-r--  2.0 unx     4718 b- defN 23-May-08 13:23 exciton/nlp/translation/m2m100/service.py
 -rw-rw-r--  2.0 unx     2172 b- defN 23-Mar-12 03:47 exciton/nlp/translation/m2m100/utils.py
--rw-r--r--  2.0 unx    11417 b- defN 23-May-28 12:42 exciton-2.0.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1598 b- defN 23-May-28 12:42 exciton-2.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-28 12:42 exciton-2.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-May-28 12:42 exciton-2.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5584 b- defN 23-May-28 12:42 exciton-2.0.6.dist-info/RECORD
-60 files, 153905 bytes uncompressed, 48648 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx    11417 b- defN 23-Jun-07 01:50 exciton-2.0.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1594 b- defN 23-Jun-07 01:50 exciton-2.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 01:50 exciton-2.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jun-07 01:50 exciton-2.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6198 b- defN 23-Jun-07 01:50 exciton-2.0.8.dist-info/RECORD
+66 files, 164836 bytes uncompressed, 52306 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -15,14 +15,26 @@
 
 Filename: exciton/ml/classification/bert/model.py
 Comment: 
 
 Filename: exciton/ml/classification/bert/trainer.py
 Comment: 
 
+Filename: exciton/ml/classification/xlm_roberta/__init__.py
+Comment: 
+
+Filename: exciton/ml/classification/xlm_roberta/model.py
+Comment: 
+
+Filename: exciton/ml/classification/xlm_roberta/trainer.py
+Comment: 
+
+Filename: exciton/ml/classification/xlm_roberta/utils.py
+Comment: 
+
 Filename: exciton/ml/classification/xlmroberta/__init__.py
 Comment: 
 
 Filename: exciton/ml/classification/xlmroberta/model.py
 Comment: 
 
 Filename: exciton/ml/classification/xlmroberta/trainer.py
@@ -147,35 +159,41 @@
 
 Filename: exciton/nlp/text_matching/__init__.py
 Comment: 
 
 Filename: exciton/nlp/text_matching/exciton_matching.py
 Comment: 
 
+Filename: exciton/nlp/topic_relevance/__init__.py
+Comment: 
+
+Filename: exciton/nlp/topic_relevance/exciton_relevance.py
+Comment: 
+
 Filename: exciton/nlp/translation/__init__.py
 Comment: 
 
 Filename: exciton/nlp/translation/m2m100/__init__.py
 Comment: 
 
 Filename: exciton/nlp/translation/m2m100/service.py
 Comment: 
 
 Filename: exciton/nlp/translation/m2m100/utils.py
 Comment: 
 
-Filename: exciton-2.0.6.dist-info/LICENSE
+Filename: exciton-2.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: exciton-2.0.6.dist-info/METADATA
+Filename: exciton-2.0.8.dist-info/METADATA
 Comment: 
 
-Filename: exciton-2.0.6.dist-info/WHEEL
+Filename: exciton-2.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: exciton-2.0.6.dist-info/top_level.txt
+Filename: exciton-2.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: exciton-2.0.6.dist-info/RECORD
+Filename: exciton-2.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `exciton-2.0.6.dist-info/LICENSE` & `exciton-2.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `exciton-2.0.6.dist-info/METADATA` & `exciton-2.0.8.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: exciton
-Version: 2.0.6
-Summary: Domain-specific Natural Language Processing with exciton
-Home-page: https://exciton.com
-Author: The ExcitonX Team
+Version: 2.0.8
+Summary: Natural Language Processing by the Exciton Research
+Home-page: https://excitonx.com
+Author: The Exciton Research Team
 Author-email: excitonx@gmail.com
 License: UNKNOWN
-Keywords: exciton NLP Deep Learning
+Keywords: NLP Deep Learning
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
```

## Comparing `exciton-2.0.6.dist-info/RECORD` & `exciton-2.0.8.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 exciton/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 exciton/ml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 exciton/ml/classification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 exciton/ml/classification/utils.py,sha256=NNT86drSZehboUDkPmbQYIkUk89DCGYVk61uz9HUBk8,1461
 exciton/ml/classification/bert/__init__.py,sha256=IkYH6Xlck8ob9ZrVpg2jbpJgvdwjYEjy2OriQuGZ-kI,98
 exciton/ml/classification/bert/model.py,sha256=a_G8QztS037P-pzUpNnNkyhSfqOrKaQF24F1ZI63mEQ,5860
 exciton/ml/classification/bert/trainer.py,sha256=o3reQ1DecPbuVkLT0Ld6XyULD4I4XD9xdzMMoUc_Q10,1966
+exciton/ml/classification/xlm_roberta/__init__.py,sha256=IkYH6Xlck8ob9ZrVpg2jbpJgvdwjYEjy2OriQuGZ-kI,98
+exciton/ml/classification/xlm_roberta/model.py,sha256=0wACKbH9ZtdV4DZ1Di9cCSQRhNENcp7A9kMEuDAbO-M,4845
+exciton/ml/classification/xlm_roberta/trainer.py,sha256=P0sHlxwboTcYUJXeGV_3AR2o5wtZFyFCDtJPaVjV3F0,2075
+exciton/ml/classification/xlm_roberta/utils.py,sha256=7lAzlUpmnR-mLKJyXP18VTzHLkXCKXzBm7ZIDt_0FLo,1775
 exciton/ml/classification/xlmroberta/__init__.py,sha256=IkYH6Xlck8ob9ZrVpg2jbpJgvdwjYEjy2OriQuGZ-kI,98
 exciton/ml/classification/xlmroberta/model.py,sha256=UHibJ5_wK4QhAJlvSElbd2HtT841yXRl9Lv5wCtDWto,4679
 exciton/ml/classification/xlmroberta/trainer.py,sha256=_jvLsjMRvA7Y6F54d9dFrmyr9zUtNdTdov1-Cc-esz8,1959
 exciton/ml/engine/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 exciton/ml/engine/end2end.py,sha256=mo7XqwdetDk5hsaF1prJzSf6cb89Eph_Ivgt7j1pBXw,8476
 exciton/ml/engine/utils.py,sha256=3ESCGANQSePXMl7BEglPSXS_DIAyhOTciR6R5C-8ok0,916
 exciton/ml/tagging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -45,16 +49,18 @@
 exciton/nlp/named_entity_recogonition/utils.py,sha256=0GaerSJudvinee0rxL6zRtrSOhvGSUzbNoNci7KTzl4,3192
 exciton/nlp/named_entity_recogonition/xlmroberta.py,sha256=av4mSyZ5DNaN0KmmpEw4WkzGsrgupR8X0FiU1cdA4dw,3876
 exciton/nlp/sentence_tokenizer/__init__.py,sha256=1hIgq6ayPk2yVdhBgLHe5vXxU2fcDrenz51iKXhx28s,59
 exciton/nlp/sentence_tokenizer/exciton_sbd.py,sha256=ZZ20UBYzIRKwPe7DD56BWqwbm5-SED0eyEJJVNXetMo,4983
 exciton/nlp/sentence_tokenizer/service.py,sha256=3Ssq2UNmhDCezhBJq4V8csacA_0XenYmgPLZfmBtBYc,3977
 exciton/nlp/text_matching/__init__.py,sha256=tgQvyWZupI0QAHlnLAJldpOPBCF01OFq2poLH49tAVg,84
 exciton/nlp/text_matching/exciton_matching.py,sha256=a99bzY5117DLAGb_AgV_4ai6buVYrMmyvengo18CeIU,2565
+exciton/nlp/topic_relevance/__init__.py,sha256=lKpWm-3G17hrZR86ckItV9w6gYxd1yULD_NE18-OFBY,87
+exciton/nlp/topic_relevance/exciton_relevance.py,sha256=bo3tZkum03mGiV8ZhbPQUcX0hseAum9hE4J8hFAWwYU,1441
 exciton/nlp/translation/__init__.py,sha256=gE0YV-s4pB7VQWdsg04hALOBBpuWaQ3AUqpY9rvgI_8,50
 exciton/nlp/translation/m2m100/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 exciton/nlp/translation/m2m100/service.py,sha256=FIXc5sUtZzywzis_CZ2doF6sqrPcKcyMO8EhLgFTwjY,4718
 exciton/nlp/translation/m2m100/utils.py,sha256=GE8qg2deaHBMVMIHS32Hb5TCxO453kuncQrdJsnRIoU,2172
-exciton-2.0.6.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
-exciton-2.0.6.dist-info/METADATA,sha256=v_gbyjxBqqDRm--RVq0fS72Rr2Foo9Xg6GPmU2aiQ1o,1598
-exciton-2.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-exciton-2.0.6.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
-exciton-2.0.6.dist-info/RECORD,,
+exciton-2.0.8.dist-info/LICENSE,sha256=eaaQRm1hnsFuOwXep1_FkcP0t2c5T_wkOJknzzhxf2U,11417
+exciton-2.0.8.dist-info/METADATA,sha256=VkgthdUqeRAy9eXkoPe9_lQMFmTQZ8YAoR6VD5W1AP4,1594
+exciton-2.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+exciton-2.0.8.dist-info/top_level.txt,sha256=4a5H-nIPFHu7soZB2r0pfjYuciFSwQFnkl5PhaaT4pY,8
+exciton-2.0.8.dist-info/RECORD,,
```

