# Comparing `tmp/fairbench-0.2.2-py3-none-any.whl.zip` & `tmp/fairbench-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,10 @@
-Zip file size: 28231 bytes, number of entries: 40
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-31 10:14 fairbench/__init__.py
--rw-rw-rw-  2.0 fat      512 b- defN 23-Jan-15 16:07 fairbench/accumulate.py
--rw-rw-rw-  2.0 fat     1790 b- defN 23-Jan-15 16:07 fairbench/algorithms.py
+Zip file size: 21811 bytes, number of entries: 33
+-rw-rw-rw-  2.0 fat      382 b- defN 23-May-31 10:14 fairbench/__init__.py
 -rw-rw-rw-  2.0 fat     1952 b- defN 23-Jun-01 09:25 fairbench/export.py
--rw-rw-rw-  2.0 fat     9339 b- defN 23-May-17 23:49 fairbench/fork.py
--rw-rw-rw-  2.0 fat     1744 b- defN 23-Jan-15 16:07 fairbench/output.py
--rw-rw-rw-  2.0 fat     2393 b- defN 23-Jan-15 16:07 fairbench/reduction.py
--rw-rw-rw-  2.0 fat     1146 b- defN 23-Jan-15 16:07 fairbench/reporting.py
 -rw-rw-rw-  2.0 fat       38 b- defN 23-May-14 10:33 fairbench/bench/__init__.py
 -rw-rw-rw-  2.0 fat      583 b- defN 23-May-14 15:09 fairbench/bench/loader.py
 -rw-rw-rw-  2.0 fat      122 b- defN 23-May-13 22:58 fairbench/forks/__init__.py
 -rw-rw-rw-  2.0 fat     2130 b- defN 23-May-25 07:44 fairbench/forks/categorical.py
 -rw-rw-rw-  2.0 fat     1070 b- defN 23-Jun-02 10:01 fairbench/forks/explanation.py
 -rw-rw-rw-  2.0 fat    23803 b- defN 23-Jun-02 09:31 fairbench/forks/fork.py
 -rw-rw-rw-  2.0 fat      154 b- defN 23-Jan-14 23:08 fairbench/metrics/__init__.py
@@ -19,24 +13,23 @@
 -rw-rw-rw-  2.0 fat     1494 b- defN 23-May-31 07:41 fairbench/metrics/disparate_mistreatment.py
 -rw-rw-rw-  2.0 fat      100 b- defN 23-May-31 10:15 fairbench/mitigation/__init__.py
 -rw-rw-rw-  2.0 fat     1790 b- defN 23-May-31 10:16 fairbench/mitigation/postprocessing.py
 -rw-rw-rw-  2.0 fat      207 b- defN 23-Jan-15 14:06 fairbench/reports/__init__.py
 -rw-rw-rw-  2.0 fat     1478 b- defN 23-Jun-02 09:19 fairbench/reports/accumulate.py
 -rw-rw-rw-  2.0 fat     1629 b- defN 23-May-18 18:48 fairbench/reports/adhoc.py
 -rw-rw-rw-  2.0 fat     2259 b- defN 23-May-28 14:54 fairbench/reports/base.py
--rw-rw-rw-  2.0 fat     4980 b- defN 23-May-17 23:49 fairbench/reports/reduction.py
 -rw-rw-rw-  2.0 fat      883 b- defN 23-May-14 15:09 fairbench/reports/surrogate.py
 -rw-rw-rw-  2.0 fat      155 b- defN 23-Feb-20 08:42 fairbench/reports/reduction/__init__.py
 -rw-rw-rw-  2.0 fat      794 b- defN 23-May-28 14:54 fairbench/reports/reduction/expanders.py
 -rw-rw-rw-  2.0 fat     1853 b- defN 23-Jun-02 08:25 fairbench/reports/reduction/reduce.py
 -rw-rw-rw-  2.0 fat     2364 b- defN 23-May-28 14:54 fairbench/reports/reduction/reducers.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-26 21:15 tests/__init__.py
 -rw-rw-rw-  2.0 fat     1394 b- defN 23-May-28 18:45 tests/test_batching.py
 -rw-rw-rw-  2.0 fat     1278 b- defN 23-Jun-01 09:09 tests/test_benchmarks.py
--rw-rw-rw-  2.0 fat     4884 b- defN 23-Jun-07 08:03 tests/test_forks.py
+-rw-rw-rw-  2.0 fat     4884 b- defN 23-Jun-07 08:14 tests/test_forks.py
 -rw-rw-rw-  2.0 fat     1572 b- defN 23-Jun-02 08:24 tests/test_reduction.py
 -rw-rw-rw-  2.0 fat     6556 b- defN 23-May-31 14:04 tests/test_reports.py
--rw-rw-rw-  2.0 fat      809 b- defN 23-Jun-07 08:06 fairbench-0.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 08:06 fairbench-0.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-07 08:06 fairbench-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     3335 b- defN 23-Jun-07 08:06 fairbench-0.2.2.dist-info/RECORD
-40 files, 91612 bytes uncompressed, 22909 bytes compressed:  75.0%
+-rw-rw-rw-  2.0 fat      809 b- defN 23-Jun-07 08:24 fairbench-0.2.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 08:24 fairbench-0.2.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-07 08:24 fairbench-0.2.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2783 b- defN 23-Jun-07 08:24 fairbench-0.2.3.dist-info/RECORD
+33 files, 69536 bytes uncompressed, 17333 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -1,31 +1,13 @@
 Filename: fairbench/__init__.py
 Comment: 
 
-Filename: fairbench/accumulate.py
-Comment: 
-
-Filename: fairbench/algorithms.py
-Comment: 
-
 Filename: fairbench/export.py
 Comment: 
 
-Filename: fairbench/fork.py
-Comment: 
-
-Filename: fairbench/output.py
-Comment: 
-
-Filename: fairbench/reduction.py
-Comment: 
-
-Filename: fairbench/reporting.py
-Comment: 
-
 Filename: fairbench/bench/__init__.py
 Comment: 
 
 Filename: fairbench/bench/loader.py
 Comment: 
 
 Filename: fairbench/forks/__init__.py
@@ -66,17 +48,14 @@
 
 Filename: fairbench/reports/adhoc.py
 Comment: 
 
 Filename: fairbench/reports/base.py
 Comment: 
 
-Filename: fairbench/reports/reduction.py
-Comment: 
-
 Filename: fairbench/reports/surrogate.py
 Comment: 
 
 Filename: fairbench/reports/reduction/__init__.py
 Comment: 
 
 Filename: fairbench/reports/reduction/expanders.py
@@ -102,20 +81,20 @@
 
 Filename: tests/test_reduction.py
 Comment: 
 
 Filename: tests/test_reports.py
 Comment: 
 
-Filename: fairbench-0.2.2.dist-info/METADATA
+Filename: fairbench-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: fairbench-0.2.2.dist-info/WHEEL
+Filename: fairbench-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: fairbench-0.2.2.dist-info/top_level.txt
+Filename: fairbench-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: fairbench-0.2.2.dist-info/RECORD
+Filename: fairbench-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fairbench/__init__.py

```diff
@@ -1 +1,13 @@
+from fairbench.forks import *
+from fairbench.metrics import *
+from fairbench.reports import *
+from fairbench.export import *
+from fairbench.mitigation import *
+from fairbench.bench import *
 
+from fairbench import forks
+from fairbench import metrics
+from fairbench import reports
+from fairbench import export
+from fairbench import mitigation
+from fairbench import bench
```

## Comparing `fairbench-0.2.2.dist-info/METADATA` & `fairbench-0.2.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbench
-Version: 0.2.2
+Version: 0.2.3
 Summary: Fairness model assessment framework
 Home-page: https://github.com/mever-team/FairBench
 Author: Emmanouil (Manios) Krasanakis
 Author-email: maniospas@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `fairbench-0.2.2.dist-info/RECORD` & `fairbench-0.2.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,9 @@
-fairbench/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-fairbench/accumulate.py,sha256=vyDGY-RTP-aX3ygiHc56WPefRFWQOCjg7KJ4kC3kwFg,512
-fairbench/algorithms.py,sha256=CF2WcAWQKKfNRJ4yvNqIjuNdLaCBrSIpI_XNhmfiUkY,1790
+fairbench/__init__.py,sha256=g4MfDvLSXjrRh6EjPFGI7SwfQeL2BeBfl-YreWxGEQU,382
 fairbench/export.py,sha256=_u97-Yi8VArkwof63mcVXgnUD-i9AY1vjxtCnQ_jKcs,1952
-fairbench/fork.py,sha256=VAgJ6MeD5a6mK_BMrIJdXPxLpp7wz0wjTSy59IJOSJU,9339
-fairbench/output.py,sha256=wvusKkx72F9i0EZoWpM8vR3NYTkpJTc8rtj5oLTKkRA,1744
-fairbench/reduction.py,sha256=PkHMY4B8SuwwV7-dq_dQXW2bhx2tr8jQ7iAXy9kilVE,2393
-fairbench/reporting.py,sha256=jcZtJXjTQAstzTPMjcnQei053k_LUkVrA1oLVsfOIog,1146
 fairbench/bench/__init__.py,sha256=piA_S0SAZ96_-MxdcGO_V7pCKngOFBeAv8KGj9rkGRA,38
 fairbench/bench/loader.py,sha256=BXmttN9Ee-TA6FAb1gXMhlJutDN2B6XIea6TU0Cre14,583
 fairbench/forks/__init__.py,sha256=eBRDSxc31Pc1yKCc1VjFBvPMsBVaOzVOfXHpkYQodG0,122
 fairbench/forks/categorical.py,sha256=nfsA1ZjrrywMzOhEoPUF6_9oazIJWcZEI4gvil-1VIs,2130
 fairbench/forks/explanation.py,sha256=F-QBVQvnN1O25gMDugV--UiykAp4LtAcPGh512pBtis,1070
 fairbench/forks/fork.py,sha256=dvhM3s8UepBEvC6Jt2e7iiWJHcLeh0XTKwBJIlcDo84,23803
 fairbench/metrics/__init__.py,sha256=i2kNaDKTfTSEh1aGZ83ByaVXwv0gYE-guFNjj9XlF6I,154
@@ -18,23 +12,22 @@
 fairbench/metrics/disparate_mistreatment.py,sha256=ORoUcMU_Dh18Ytz4dgQn8wPyaNJ_w98m_oegxI90vc4,1494
 fairbench/mitigation/__init__.py,sha256=f-owl1xAKGweXEuVbFJGYSel3-7kccvTo6SEziKmXRk,100
 fairbench/mitigation/postprocessing.py,sha256=CF2WcAWQKKfNRJ4yvNqIjuNdLaCBrSIpI_XNhmfiUkY,1790
 fairbench/reports/__init__.py,sha256=YQm7A6K3PUB4uNOw3iDu2RUaoWa07Rsn3GJr4wZkn2M,207
 fairbench/reports/accumulate.py,sha256=JMpjsfs4dc4jfMn3I0a9W-kcHzJk1hmX26qUC5BySyU,1478
 fairbench/reports/adhoc.py,sha256=7FhOawdzoK3MtY6o8wLaxKDrJ1QZmG5XTTSxra4-D-w,1629
 fairbench/reports/base.py,sha256=_5wXT5qfDYCWMTw-e9D-HQLyFAh0IWb2ywMLzdRwdTU,2259
-fairbench/reports/reduction.py,sha256=zSo8Whi-tW8trPmN946e2gyLp6xR7b8WMZzYyPmWgIc,4980
 fairbench/reports/surrogate.py,sha256=LnV6kkNPMGL2SYEBSSIFWjkXQ8N5m2k4y5as2zUyDt8,883
 fairbench/reports/reduction/__init__.py,sha256=a3c0w4bKV3f6NXnGMPPGFRxdfg_YIrcccy_mEBSr8zk,155
 fairbench/reports/reduction/expanders.py,sha256=eiytghNbie7zqZht6PtbdpXSbBn68Fb_x7JL1VYiGmY,794
 fairbench/reports/reduction/reduce.py,sha256=yrdQY7Bdr1LaFh8FwiPjZMrY13z1kqaKWbebeNXfbK8,1853
 fairbench/reports/reduction/reducers.py,sha256=zZKHhJDIdBdiMbRotxdRUGS-sKcLFqGgDZ8MebzNMrE,2364
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_batching.py,sha256=bXewsKXAlDTeyZZ8OlG74-qYQ_hhiwcYJigxy0M_YKY,1394
 tests/test_benchmarks.py,sha256=RZwehxePgR6fwFCh9HWbK3rXsXQNLHomrn7M6BboiMw,1278
 tests/test_forks.py,sha256=39cnpaRVvz7xfUz2YijRIZMg9_v0FrjFM1-a0hDNGM8,4884
 tests/test_reduction.py,sha256=MK72DJomkokS-pxTgmZVXwqDd5t-9OOCVJK2zDKTObA,1572
 tests/test_reports.py,sha256=2nNSZjkrTdZl8P5bvEz8dDdRd_W7CmSvn51GDdHFPvo,6556
-fairbench-0.2.2.dist-info/METADATA,sha256=1twKoVa7RLp7Uihkuk3hbFhGTOoiFJO11P-lJ4iHn_A,809
-fairbench-0.2.2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-fairbench-0.2.2.dist-info/top_level.txt,sha256=lrkG910bN_2UdVUqCXaR6aeRjjXfOQX2-wSeVjhhFnM,16
-fairbench-0.2.2.dist-info/RECORD,,
+fairbench-0.2.3.dist-info/METADATA,sha256=qGsfwRFicKL_dI7bhwMMjDC-1VzUibdwaGHXCKpus9Q,809
+fairbench-0.2.3.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+fairbench-0.2.3.dist-info/top_level.txt,sha256=lrkG910bN_2UdVUqCXaR6aeRjjXfOQX2-wSeVjhhFnM,16
+fairbench-0.2.3.dist-info/RECORD,,
```

