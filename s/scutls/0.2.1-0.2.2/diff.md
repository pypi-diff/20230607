# Comparing `tmp/scutls-0.2.1.tar.gz` & `tmp/scutls-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scutls-0.2.1.tar", max compression
+gzip compressed data, was "scutls-0.2.2.tar", max compression
```

## Comparing `scutls-0.2.1.tar` & `scutls-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      583 2023-06-05 20:05:32.972181 scutls-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-05 20:05:52.115138 scutls-0.2.1/scutls/__init__.py
--rw-r--r--   0        0        0     6256 2023-05-10 15:48:41.694697 scutls-0.2.1/scutls/arguments.py
--rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.2.1/scutls/assets/genome_ensembl_107_54_54_54.json
--rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.2.1/scutls/assets/genome_ensembl_release_all.txt
--rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.2.1/scutls/assets/genome_ensembl_release_use.txt
--rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.2.1/scutls/assets/genome_ucsc.json
--rw-r--r--   0        0        0     4938 2023-06-02 19:36:09.942327 scutls-0.2.1/scutls/barcode.py
--rw-r--r--   0        0        0     1074 2023-05-10 15:45:19.722039 scutls-0.2.1/scutls/cli.py
--rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.2.1/scutls/download.py
--rw-r--r--   0        0        0     3845 2023-06-02 19:44:04.605614 scutls-0.2.1/scutls/fastq.py
--rw-r--r--   0        0        0     9201 2023-06-05 20:04:42.981372 scutls-0.2.1/scutls/util.py
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.2.1/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-06-07 00:09:01.859249 scutls-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-07 00:09:15.673421 scutls-0.2.2/scutls/__init__.py
+-rw-r--r--   0        0        0     6256 2023-05-10 15:48:41.694697 scutls-0.2.2/scutls/arguments.py
+-rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.2.2/scutls/assets/genome_ensembl_107_54_54_54.json
+-rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.2.2/scutls/assets/genome_ensembl_release_all.txt
+-rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.2.2/scutls/assets/genome_ensembl_release_use.txt
+-rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.2.2/scutls/assets/genome_ucsc.json
+-rw-r--r--   0        0        0     4999 2023-06-07 00:05:05.280933 scutls-0.2.2/scutls/barcode.py
+-rw-r--r--   0        0        0     1074 2023-05-10 15:45:19.722039 scutls-0.2.2/scutls/cli.py
+-rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.2.2/scutls/download.py
+-rw-r--r--   0        0        0     3845 2023-06-02 19:44:04.605614 scutls-0.2.2/scutls/fastq.py
+-rw-r--r--   0        0        0     9201 2023-06-05 20:04:42.981372 scutls-0.2.2/scutls/util.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.2.2/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.2.2/PKG-INFO
```

### Comparing `scutls-0.2.1/pyproject.toml` & `scutls-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scutls"
-version = "0.2.1"
+version = "0.2.2"
 description = "Single-cell data processing utility tools"
 authors = ["Kai Hu <kai.hu@umassmed.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-resources = "^5.8.0"
 wget = "^3.2"
```

### Comparing `scutls-0.2.1/scutls/arguments.py` & `scutls-0.2.2/scutls/arguments.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.1/scutls/assets/genome_ensembl_107_54_54_54.json` & `scutls-0.2.2/scutls/assets/genome_ensembl_107_54_54_54.json`

 * *Files identical despite different names*

### Comparing `scutls-0.2.1/scutls/assets/genome_ensembl_release_all.txt` & `scutls-0.2.2/scutls/assets/genome_ensembl_release_all.txt`

 * *Files identical despite different names*

### Comparing `scutls-0.2.1/scutls/assets/genome_ucsc.json` & `scutls-0.2.2/scutls/assets/genome_ucsc.json`

 * *Files identical despite different names*

### Comparing `scutls-0.2.1/scutls/barcode.py` & `scutls-0.2.2/scutls/barcode.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     # use True since args can be either None or False
     # arguments.py defines requirments of each argument
 
     # check if input fastq contains specified barcode:
     if contain:
         # prepare search pattern
         barcode_pattern = get_search_pattern(pattern = contain, error = error, rc_barcode = rc_barcode)
+        
+        print("barcode_pattern: ", barcode_pattern)
 
         # multiprocessing
         if not output == None:
             print("Saving to " + output + " ...")
         else:
             print("Processing ...")
         intervals = fastq_chunk_interval(input, nproc = nproc)
```

### Comparing `scutls-0.2.1/scutls/cli.py` & `scutls-0.2.2/scutls/cli.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.1/scutls/download.py` & `scutls-0.2.2/scutls/download.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.1/scutls/fastq.py` & `scutls-0.2.2/scutls/fastq.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.1/scutls/util.py` & `scutls-0.2.2/scutls/util.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.1/setup.py` & `scutls-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wget>=3.2,<4.0']
 
 entry_points = \
 {'console_scripts': ['scutls = scutls.arguments:main']}
 
 setup_kwargs = {
     'name': 'scutls',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Single-cell data processing utility tools',
     'long_description': 'None',
     'author': 'Kai Hu',
     'author_email': 'kai.hu@umassmed.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scutls-0.2.1/PKG-INFO` & `scutls-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scutls
-Version: 0.2.1
+Version: 0.2.2
 Summary: Single-cell data processing utility tools
 Author: Kai Hu
 Author-email: kai.hu@umassmed.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

