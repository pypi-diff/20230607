# Comparing `tmp/fairbench-0.2.4-py3-none-any.whl.zip` & `tmp/fairbench-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 21892 bytes, number of entries: 33
+Zip file size: 21873 bytes, number of entries: 33
 -rw-rw-rw-  2.0 fat      382 b- defN 23-May-31 10:14 fairbench/__init__.py
 -rw-rw-rw-  2.0 fat     1952 b- defN 23-Jun-01 09:25 fairbench/export.py
 -rw-rw-rw-  2.0 fat       38 b- defN 23-May-14 10:33 fairbench/bench/__init__.py
 -rw-rw-rw-  2.0 fat      583 b- defN 23-May-14 15:09 fairbench/bench/loader.py
 -rw-rw-rw-  2.0 fat      122 b- defN 23-May-13 22:58 fairbench/forks/__init__.py
 -rw-rw-rw-  2.0 fat     2130 b- defN 23-May-25 07:44 fairbench/forks/categorical.py
 -rw-rw-rw-  2.0 fat     1161 b- defN 23-Jun-07 09:00 fairbench/forks/explanation.py
@@ -24,12 +24,12 @@
 -rw-rw-rw-  2.0 fat     2364 b- defN 23-May-28 14:54 fairbench/reports/reduction/reducers.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-26 21:15 tests/__init__.py
 -rw-rw-rw-  2.0 fat     1394 b- defN 23-May-28 18:45 tests/test_batching.py
 -rw-rw-rw-  2.0 fat     1278 b- defN 23-Jun-01 09:09 tests/test_benchmarks.py
 -rw-rw-rw-  2.0 fat     4884 b- defN 23-Jun-07 08:14 tests/test_forks.py
 -rw-rw-rw-  2.0 fat     1572 b- defN 23-Jun-02 08:24 tests/test_reduction.py
 -rw-rw-rw-  2.0 fat     6556 b- defN 23-May-31 14:04 tests/test_reports.py
--rw-rw-rw-  2.0 fat      848 b- defN 23-Jun-07 09:36 fairbench-0.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 09:36 fairbench-0.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-07 09:36 fairbench-0.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2783 b- defN 23-Jun-07 09:36 fairbench-0.2.4.dist-info/RECORD
-33 files, 69815 bytes uncompressed, 17414 bytes compressed:  75.1%
+-rw-rw-rw-  2.0 fat      809 b- defN 23-Jun-07 09:48 fairbench-0.2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 09:48 fairbench-0.2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-07 09:48 fairbench-0.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2783 b- defN 23-Jun-07 09:48 fairbench-0.2.5.dist-info/RECORD
+33 files, 69776 bytes uncompressed, 17395 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -81,20 +81,20 @@
 
 Filename: tests/test_reduction.py
 Comment: 
 
 Filename: tests/test_reports.py
 Comment: 
 
-Filename: fairbench-0.2.4.dist-info/METADATA
+Filename: fairbench-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: fairbench-0.2.4.dist-info/WHEEL
+Filename: fairbench-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: fairbench-0.2.4.dist-info/top_level.txt
+Filename: fairbench-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: fairbench-0.2.4.dist-info/RECORD
+Filename: fairbench-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fairbench-0.2.4.dist-info/METADATA` & `fairbench-0.2.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: fairbench
-Version: 0.2.4
+Version: 0.2.5
 Summary: Fairness model assessment framework
 Home-page: https://github.com/mever-team/FairBench
 Author: Emmanouil (Manios) Krasanakis
 Author-email: maniospas@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: python-version (>3.6.0)
 Requires-Dist: numpy
 Requires-Dist: eagerpy
 Requires-Dist: distributed
 Requires-Dist: makefun
 Requires-Dist: matplotlib
 Requires-Dist: wget
 Requires-Dist: scikit-learn
```

## Comparing `fairbench-0.2.4.dist-info/RECORD` & `fairbench-0.2.5.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -23,11 +23,11 @@
 fairbench/reports/reduction/reducers.py,sha256=zZKHhJDIdBdiMbRotxdRUGS-sKcLFqGgDZ8MebzNMrE,2364
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_batching.py,sha256=bXewsKXAlDTeyZZ8OlG74-qYQ_hhiwcYJigxy0M_YKY,1394
 tests/test_benchmarks.py,sha256=RZwehxePgR6fwFCh9HWbK3rXsXQNLHomrn7M6BboiMw,1278
 tests/test_forks.py,sha256=39cnpaRVvz7xfUz2YijRIZMg9_v0FrjFM1-a0hDNGM8,4884
 tests/test_reduction.py,sha256=MK72DJomkokS-pxTgmZVXwqDd5t-9OOCVJK2zDKTObA,1572
 tests/test_reports.py,sha256=2nNSZjkrTdZl8P5bvEz8dDdRd_W7CmSvn51GDdHFPvo,6556
-fairbench-0.2.4.dist-info/METADATA,sha256=4hAg7nUT4RDC_L8Z71cB6_-0ivMk469eh6jzz597Kbs,848
-fairbench-0.2.4.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-fairbench-0.2.4.dist-info/top_level.txt,sha256=lrkG910bN_2UdVUqCXaR6aeRjjXfOQX2-wSeVjhhFnM,16
-fairbench-0.2.4.dist-info/RECORD,,
+fairbench-0.2.5.dist-info/METADATA,sha256=gIR50QUPwu5pyari7QSGHSXsGwV7QJtWMYRUXvFuOB0,809
+fairbench-0.2.5.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+fairbench-0.2.5.dist-info/top_level.txt,sha256=lrkG910bN_2UdVUqCXaR6aeRjjXfOQX2-wSeVjhhFnM,16
+fairbench-0.2.5.dist-info/RECORD,,
```

