# Comparing `tmp/appsignal_beta-0.1.0-py3-none-musllinux_1_1_x86_64.whl.zip` & `tmp/appsignal_beta-0.1.1-py3-none-musllinux_1_1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,16 @@
-Zip file size: 2283196 bytes, number of entries: 18
--rw-r--r--  2.0 unx      936 b- defN 20-Feb-02 00:00 conftest.py
+Zip file size: 2401788 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 appsignal/__about__.py
 -rw-r--r--  2.0 unx       65 b- defN 20-Feb-02 00:00 appsignal/__init__.py
 -rw-r--r--  2.0 unx      895 b- defN 20-Feb-02 00:00 appsignal/agent.py
 -rwxr-xr-x  2.0 unx  5618008 b- defN 20-Feb-02 00:00 appsignal/appsignal-agent
 -rw-r--r--  2.0 unx     9737 b- defN 20-Feb-02 00:00 appsignal/cli.py
 -rw-r--r--  2.0 unx     2078 b- defN 20-Feb-02 00:00 appsignal/client.py
 -rw-r--r--  2.0 unx    11278 b- defN 20-Feb-02 00:00 appsignal/config.py
 -rw-r--r--  2.0 unx     3952 b- defN 20-Feb-02 00:00 appsignal/opentelemetry.py
--rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 tests/__init__.py
--rw-r--r--  2.0 unx     4412 b- defN 20-Feb-02 00:00 tests/test_cli.py
--rw-r--r--  2.0 unx     4984 b- defN 20-Feb-02 00:00 tests/test_client.py
--rw-r--r--  2.0 unx     9297 b- defN 20-Feb-02 00:00 tests/test_config.py
--rw-r--r--  2.0 unx     1480 b- defN 20-Feb-02 00:00 tests/test_opentelemetry.py
-?rw-r--r--  2.0 unx     2227 b- defN 20-Feb-02 00:00 appsignal_beta-0.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 appsignal_beta-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx       48 b- defN 20-Feb-02 00:00 appsignal_beta-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1401 b- defN 20-Feb-02 00:00 appsignal_beta-0.1.0.dist-info/RECORD
-18 files, 5670925 bytes uncompressed, 2280932 bytes compressed:  59.8%
+-rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 appsignal/py.typed
+-rw-r--r--  2.0 unx   216583 b- defN 20-Feb-02 00:00 appsignal/resources/cacert.pem
+?rw-r--r--  2.0 unx     2227 b- defN 20-Feb-02 00:00 appsignal_beta-0.1.1.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 appsignal_beta-0.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx       48 b- defN 20-Feb-02 00:00 appsignal_beta-0.1.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1112 b- defN 20-Feb-02 00:00 appsignal_beta-0.1.1.dist-info/RECORD
+14 files, 5866110 bytes uncompressed, 2399956 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -1,10 +1,7 @@
-Filename: conftest.py
-Comment: 
-
 Filename: appsignal/__about__.py
 Comment: 
 
 Filename: appsignal/__init__.py
 Comment: 
 
 Filename: appsignal/agent.py
@@ -21,35 +18,26 @@
 
 Filename: appsignal/config.py
 Comment: 
 
 Filename: appsignal/opentelemetry.py
 Comment: 
 
-Filename: tests/__init__.py
-Comment: 
-
-Filename: tests/test_cli.py
-Comment: 
-
-Filename: tests/test_client.py
-Comment: 
-
-Filename: tests/test_config.py
+Filename: appsignal/py.typed
 Comment: 
 
-Filename: tests/test_opentelemetry.py
+Filename: appsignal/resources/cacert.pem
 Comment: 
 
-Filename: appsignal_beta-0.1.0.dist-info/METADATA
+Filename: appsignal_beta-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: appsignal_beta-0.1.0.dist-info/WHEEL
+Filename: appsignal_beta-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: appsignal_beta-0.1.0.dist-info/entry_points.txt
+Filename: appsignal_beta-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: appsignal_beta-0.1.0.dist-info/RECORD
+Filename: appsignal_beta-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appsignal/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## Comparing `appsignal_beta-0.1.0.dist-info/METADATA` & `appsignal_beta-0.1.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appsignal-beta
-Version: 0.1.0
+Version: 0.1.1
 Summary: The AppSignal integration for the Python programming language
 Project-URL: Documentation, https://docs.appsignal.com/python
 Project-URL: Issues, https://github.com/appsignal/appsignal-python/issues
 Project-URL: Source, https://github.com/appsignal/appsignal-python
 Author-email: Tom de Bruijn <tom@tomdebruijn.com>, Noemi Lapresta <noemi@appsignal.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

## Comparing `appsignal_beta-0.1.0.dist-info/RECORD` & `appsignal_beta-0.1.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-conftest.py,sha256=ybYJJV-q9Z9q0bGohoI7ROzs1z4140tulkXPIGX_pa0,936
-appsignal/__about__.py,sha256=kUR5RAFc7HCeiqdlX36dZOHkUI5wI6V_43RpEcD8b-0,22
+appsignal/__about__.py,sha256=rnObPjuBcEStqSO0S6gsdS_ot8ITOQjVj_-P1LUUYpg,22
 appsignal/__init__.py,sha256=5bIxR4Wf_qtVhVNnOT_YcmCFfWGaqBbrwEIpft24_AQ,65
 appsignal/agent.py,sha256=vIcfULHlTTC8gmkiMkw-pMQ-FktzNvjkZyDmdpSr8uk,895
 appsignal/appsignal-agent,sha256=-AYAKW3NLUHtRKSpfJBIwsbF0M7YUEJ0djLwDrHEghA,5618008
 appsignal/cli.py,sha256=hNifMfRKL3bsXdaZhv1kyDum2q3muE38AeZW97jQKmU,9737
 appsignal/client.py,sha256=fUNGUNuR9k45Bhk_aBQwwv_4UszWAOSx9nuuykabsdY,2078
 appsignal/config.py,sha256=j2w00PR6IgNtSYPWH2R2FoRejXps1uVWUarPqwHd8k8,11278
 appsignal/opentelemetry.py,sha256=7MHOKFNUtHB7h0IyqlkOscOCav4PtBy69HmOuttfPEk,3952
-tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/test_cli.py,sha256=8zr71cRIrptBWHngMG1g4e9kiJPyEM_mqXo272Od87U,4412
-tests/test_client.py,sha256=gPbw1e7RWNT4IZ4lFPXjL2rBW40Pvh-qFcrTkdg0G3U,4984
-tests/test_config.py,sha256=x4hUS97lJCg7pjj2vBnAyDm6eTu6RC7_zKzbMPgGdkw,9297
-tests/test_opentelemetry.py,sha256=1uFFP_MtA2Cw158310gWMQBya6UqCWVteAZwwfnej4s,1480
-appsignal_beta-0.1.0.dist-info/METADATA,sha256=9W3NW9UD5UX9lN78FKCG4rAzC772khw5dAd4Uhizg9A,2227
-appsignal_beta-0.1.0.dist-info/WHEEL,sha256=CJKJqmzePayXhNdhrIv5xtj-ZT64FnguRJBuxRBJ4NY,105
-appsignal_beta-0.1.0.dist-info/entry_points.txt,sha256=N6u0UxXH9eJuPjKTLIZ8Z-vtwytqijXaGXWMygYVXCQ,48
-appsignal_beta-0.1.0.dist-info/RECORD,,
+appsignal/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+appsignal/resources/cacert.pem,sha256=-x7NZB0KAsAbyQNtUTy2WLvaYqdeJGvtvAF2RWCmOfA,216583
+appsignal_beta-0.1.1.dist-info/METADATA,sha256=9h_a_pLvWc4sQWm83v-CQSRBF1mWW9U-m3iedDOx4cY,2227
+appsignal_beta-0.1.1.dist-info/WHEEL,sha256=CJKJqmzePayXhNdhrIv5xtj-ZT64FnguRJBuxRBJ4NY,105
+appsignal_beta-0.1.1.dist-info/entry_points.txt,sha256=N6u0UxXH9eJuPjKTLIZ8Z-vtwytqijXaGXWMygYVXCQ,48
+appsignal_beta-0.1.1.dist-info/RECORD,,
```

