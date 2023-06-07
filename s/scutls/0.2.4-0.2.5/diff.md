# Comparing `tmp/scutls-0.2.4.tar.gz` & `tmp/scutls-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scutls-0.2.4.tar", max compression
+gzip compressed data, was "scutls-0.2.5.tar", max compression
```

## Comparing `scutls-0.2.4.tar` & `scutls-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      583 2023-06-07 03:41:55.781899 scutls-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-07 03:42:17.555914 scutls-0.2.4/scutls/__init__.py
--rw-r--r--   0        0        0     6256 2023-05-10 15:48:41.694697 scutls-0.2.4/scutls/arguments.py
--rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.2.4/scutls/assets/genome_ensembl_107_54_54_54.json
--rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.2.4/scutls/assets/genome_ensembl_release_all.txt
--rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.2.4/scutls/assets/genome_ensembl_release_use.txt
--rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.2.4/scutls/assets/genome_ucsc.json
--rw-r--r--   0        0        0     5001 2023-06-07 00:17:17.566877 scutls-0.2.4/scutls/barcode.py
--rw-r--r--   0        0        0     1074 2023-05-10 15:45:19.722039 scutls-0.2.4/scutls/cli.py
--rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.2.4/scutls/download.py
--rw-r--r--   0        0        0     3845 2023-06-02 19:44:04.605614 scutls-0.2.4/scutls/fastq.py
--rw-r--r--   0        0        0     9201 2023-06-07 03:41:47.913117 scutls-0.2.4/scutls/util.py
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.2.4/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-06-07 03:49:29.237022 scutls-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-07 03:49:41.441593 scutls-0.2.5/scutls/__init__.py
+-rw-r--r--   0        0        0     6256 2023-05-10 15:48:41.694697 scutls-0.2.5/scutls/arguments.py
+-rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.2.5/scutls/assets/genome_ensembl_107_54_54_54.json
+-rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.2.5/scutls/assets/genome_ensembl_release_all.txt
+-rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.2.5/scutls/assets/genome_ensembl_release_use.txt
+-rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.2.5/scutls/assets/genome_ucsc.json
+-rw-r--r--   0        0        0     5001 2023-06-07 00:17:17.566877 scutls-0.2.5/scutls/barcode.py
+-rw-r--r--   0        0        0     1074 2023-05-10 15:45:19.722039 scutls-0.2.5/scutls/cli.py
+-rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.2.5/scutls/download.py
+-rw-r--r--   0        0        0     3845 2023-06-02 19:44:04.605614 scutls-0.2.5/scutls/fastq.py
+-rw-r--r--   0        0        0     9253 2023-06-07 03:48:53.820816 scutls-0.2.5/scutls/util.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.2.5/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.2.5/PKG-INFO
```

### Comparing `scutls-0.2.4/pyproject.toml` & `scutls-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scutls"
-version = "0.2.4"
+version = "0.2.5"
 description = "Single-cell data processing utility tools"
 authors = ["Kai Hu <kai.hu@umassmed.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-resources = "^5.8.0"
 wget = "^3.2"
```

### Comparing `scutls-0.2.4/scutls/arguments.py` & `scutls-0.2.5/scutls/arguments.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.4/scutls/assets/genome_ensembl_107_54_54_54.json` & `scutls-0.2.5/scutls/assets/genome_ensembl_107_54_54_54.json`

 * *Files identical despite different names*

### Comparing `scutls-0.2.4/scutls/assets/genome_ensembl_release_all.txt` & `scutls-0.2.5/scutls/assets/genome_ensembl_release_all.txt`

 * *Files identical despite different names*

### Comparing `scutls-0.2.4/scutls/assets/genome_ucsc.json` & `scutls-0.2.5/scutls/assets/genome_ucsc.json`

 * *Files identical despite different names*

### Comparing `scutls-0.2.4/scutls/barcode.py` & `scutls-0.2.5/scutls/barcode.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.4/scutls/cli.py` & `scutls-0.2.5/scutls/cli.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.4/scutls/download.py` & `scutls-0.2.5/scutls/download.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.4/scutls/fastq.py` & `scutls-0.2.5/scutls/fastq.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.4/scutls/util.py` & `scutls-0.2.5/scutls/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,16 @@
         barcodes = pattern.split(",")
         if rc_barcode:
             barcodes = barcodes[::-1]
             
         for barcode in barcodes:
             if rc_barcode:
                 pattern = str(Seq(barcode).reverse_complement())
+            else:
+                pattern = barcode
             barcode_pattern += "(" + pattern + "){e<=" + str(error) + "}(.*?)"
     return(barcode_pattern)
 
 # obtain fastq coordinates for specified barcode
 def fastq_locate_barcode(interval, fastq, barcode_pattern, pos = 0):
     """
     pos: which match to return: use 0 for the first match, use -1 for the last match.
```

### Comparing `scutls-0.2.4/setup.py` & `scutls-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wget>=3.2,<4.0']
 
 entry_points = \
 {'console_scripts': ['scutls = scutls.arguments:main']}
 
 setup_kwargs = {
     'name': 'scutls',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'Single-cell data processing utility tools',
     'long_description': 'None',
     'author': 'Kai Hu',
     'author_email': 'kai.hu@umassmed.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scutls-0.2.4/PKG-INFO` & `scutls-0.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scutls
-Version: 0.2.4
+Version: 0.2.5
 Summary: Single-cell data processing utility tools
 Author: Kai Hu
 Author-email: kai.hu@umassmed.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

