# Comparing `tmp/lucidtech-synthetic-0.4.6.tar.gz` & `tmp/lucidtech-synthetic-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucidtech-synthetic-0.4.6.tar", last modified: Mon May 22 13:47:28 2023, max compression
+gzip compressed data, was "lucidtech-synthetic-0.5.0.tar", last modified: Wed Jun  7 11:42:23 2023, max compression
```

## Comparing `lucidtech-synthetic-0.4.6.tar` & `lucidtech-synthetic-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:28.281624 lucidtech-synthetic-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-22 13:47:28.281624 lucidtech-synthetic-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:28.277624 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-22 13:47:28.000000 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 13:47:28.000000 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:47:28.000000 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 13:47:28.000000 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-22 13:47:28.000000 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 13:47:28.000000 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-22 13:47:28.281624 lucidtech-synthetic-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:28.277624 lucidtech-synthetic-0.4.6/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:28.281624 lucidtech-synthetic-0.4.6/synthetic/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/core/ground_truth.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/core/synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/iterdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:28.281624 lucidtech-synthetic-0.4.6/synthetic/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/pdf/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/pdf/synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/pdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:42:23.501045 lucidtech-synthetic-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-07 11:42:23.501045 lucidtech-synthetic-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:42:23.501045 lucidtech-synthetic-0.5.0/lucidtech_synthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-07 11:42:23.000000 lucidtech-synthetic-0.5.0/lucidtech_synthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-07 11:42:23.000000 lucidtech-synthetic-0.5.0/lucidtech_synthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:42:23.000000 lucidtech-synthetic-0.5.0/lucidtech_synthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-07 11:42:23.000000 lucidtech-synthetic-0.5.0/lucidtech_synthetic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-07 11:42:23.000000 lucidtech-synthetic-0.5.0/lucidtech_synthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 11:42:23.000000 lucidtech-synthetic-0.5.0/lucidtech_synthetic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 11:42:23.501045 lucidtech-synthetic-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:42:23.501045 lucidtech-synthetic-0.5.0/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/synthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/synthetic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/synthetic/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:42:23.501045 lucidtech-synthetic-0.5.0/synthetic/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/synthetic/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/synthetic/core/ground_truth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/synthetic/core/synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/synthetic/iterdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:42:23.501045 lucidtech-synthetic-0.5.0/synthetic/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/synthetic/pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/synthetic/pdf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/synthetic/pdf/synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-07 11:42:07.000000 lucidtech-synthetic-0.5.0/synthetic/pdf/utils.py
```

### Comparing `lucidtech-synthetic-0.4.6/LICENSE.md` & `lucidtech-synthetic-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.6/PKG-INFO` & `lucidtech-synthetic-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidtech-synthetic
-Version: 0.4.6
+Version: 0.5.0
 Summary: PDF anonymizer/synthesizer for Cradl
 Home-page: https://github.com/LucidtechAI/synthetic
 Author: Lucidtech
 Author-email: hello@lucidtech.ai
 Maintainer: August Kvernmo
 Maintainer-email: august@lucidtech.ai
 License: Apache 2.0
```

### Comparing `lucidtech-synthetic-0.4.6/README.md` & `lucidtech-synthetic-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/PKG-INFO` & `lucidtech-synthetic-0.5.0/lucidtech_synthetic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidtech-synthetic
-Version: 0.4.6
+Version: 0.5.0
 Summary: PDF anonymizer/synthesizer for Cradl
 Home-page: https://github.com/LucidtechAI/synthetic
 Author: Lucidtech
 Author-email: hello@lucidtech.ai
 Maintainer: August Kvernmo
 Maintainer-email: august@lucidtech.ai
 License: Apache 2.0
```

### Comparing `lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/SOURCES.txt` & `lucidtech-synthetic-0.5.0/lucidtech_synthetic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.6/setup.py` & `lucidtech-synthetic-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.6/synthetic/__main__.py` & `lucidtech-synthetic-0.5.0/synthetic/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,22 @@
         type=int,
         help=(
             'Maximum number of pages to accept in PDF. Any PDF containing more pages than --max-pages will not be '
             'synthesized. Use this option if synthesizing is slow for some PDFs.'
         )
     )
     pdf_parser.add_argument('--synthesizer-class', type=load_class, default=BasicPdfSynthesizer)
+    pdf_parser.add_argument(
+        '--timeout-in-seconds',
+        type=int,
+        help='Time to wait for a single pdf to be parsed',
+        default=5,
+    )
     cmd = partial(parse_documents, accepted_document_types=[Pdf], parse_fn=parse_pdf)
-    pdf_parser.set_defaults(optionals=['max_fonts', 'max_pages'])
+    pdf_parser.set_defaults(optionals=['max_fonts', 'max_pages', 'timeout_in_seconds'])
     pdf_parser.set_defaults(cmd=cmd)
 
 
 def int_range(value):
     from_size, to_size = value.split('-')
     from_size = int(from_size)
     to_size = int(to_size)
```

### Comparing `lucidtech-synthetic-0.4.6/synthetic/core/ground_truth.py` & `lucidtech-synthetic-0.5.0/synthetic/core/ground_truth.py`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.6/synthetic/iterdata.py` & `lucidtech-synthetic-0.5.0/synthetic/iterdata.py`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.6/synthetic/pdf/parser.py` & `lucidtech-synthetic-0.5.0/synthetic/pdf/parser.py`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.6/synthetic/pdf/synthesizer.py` & `lucidtech-synthetic-0.5.0/synthetic/pdf/synthesizer.py`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.6/synthetic/pdf/utils.py` & `lucidtech-synthetic-0.5.0/synthetic/pdf/utils.py`

 * *Files identical despite different names*

