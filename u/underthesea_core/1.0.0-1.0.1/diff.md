# Comparing `tmp/underthesea_core-1.0.0-cp39-none-win_amd64.whl.zip` & `tmp/underthesea_core-1.0.1-cp39-cp39-manylinux2010_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 502288 bytes, number of entries: 4
--rw-r--r--  4.6 unx     1707 b- defN 23-Feb-26 03:21 underthesea_core-1.0.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Feb-26 03:21 underthesea_core-1.0.0.dist-info/WHEEL
--rwxr-xr-x  4.6 unx  1384448 b- defN 23-Feb-26 03:21 underthesea_core.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      328 b- defN 23-Feb-26 03:21 underthesea_core-1.0.0.dist-info/RECORD
-4 files, 1386577 bytes uncompressed, 501650 bytes compressed:  63.8%
+Zip file size: 657813 bytes, number of entries: 4
+-rw-r--r--  4.6 unx     1680 b- defN 23-Jun-07 08:10 underthesea_core-1.0.1.dist-info/METADATA
+-rw-r--r--  4.6 unx      105 b- defN 23-Jun-07 08:10 underthesea_core-1.0.1.dist-info/WHEEL
+-rwxr-xr-x  4.6 unx  1817024 b- defN 23-Jun-07 08:10 underthesea_core.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      341 b- defN 23-Jun-07 08:10 underthesea_core-1.0.1.dist-info/RECORD
+4 files, 1819150 bytes uncompressed, 657151 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: underthesea_core-1.0.0.dist-info/METADATA
+Filename: underthesea_core-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: underthesea_core-1.0.0.dist-info/WHEEL
+Filename: underthesea_core-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: underthesea_core.cp39-win_amd64.pyd
+Filename: underthesea_core.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: underthesea_core-1.0.0.dist-info/RECORD
+Filename: underthesea_core-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment: zip-rs
```

## Comparing `underthesea_core-1.0.0.dist-info/METADATA` & `underthesea_core-1.0.1.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: underthesea_core
-Version: 1.0.0
+Version: 1.0.1
 Summary: Underthesea Core
 Home-Page: https://github.com/undertheseanlp/underthesea/tree/main/extensions/underthesea_core
 Author: Vu Anh <anhv.ict91@gmail.com>
 Author-Email: Vu Anh <anhv.ict91@gmail.com>
 License: GPL-3.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-# Underthesea Core
-
-Underthesea Core is a powerful extension of the popular natural language processing library Underthesea, which includes a range of efficient data preprocessing tools and machine learning models for training. Built with Rust for optimal performance, Underthesea Core offers fast processing speeds and is easy to implement, with Python bindings for seamless integration into existing projects. This extension is an essential tool for developers looking to build high-performance NLP systems that deliver accurate and reliable results.
-
-## Usage
-
-CRFFeaturizer
-
-```python
->>> from underthesea_core import CRFFeaturizer
->>> features = ["T[-1]", "T[0]", "T[1]"]
->>> dictionary = set(["sinh viên"])
->>> featurizer = CRFFeaturizer(features, dictionary)
->>> sentences = [[["sinh", "X"], ["viên", "X"], ["đi", "X"], ["học", "X"]]]
->>> featurizer.process(sentences)
-[[['T[-1]=BOS', 'T[0]=sinh', 'T[1]=viên'],
-  ['T[-1]=sinh', 'T[0]=viên', 'T[1]=đi'],
-  ['T[-1]=viên', 'T[0]=đi', 'T[1]=học'],
-  ['T[-1]=đi', 'T[0]=học', 'T[1]=EOS']]]
-```
-
-## Release Workflow
-
-1. Change version in `Cargo.toml` and `pyproject.toml`
-2. Push to branch `core` with commit `Publish Underthesea Core`
-  * This will trigger `release-pypi-core` action
-3. Check latest version in [pypi](https://pypi.org/project/underthesea_core/)
+# Underthesea Core
+
+Underthesea Core is a powerful extension of the popular natural language processing library Underthesea, which includes a range of efficient data preprocessing tools and machine learning models for training. Built with Rust for optimal performance, Underthesea Core offers fast processing speeds and is easy to implement, with Python bindings for seamless integration into existing projects. This extension is an essential tool for developers looking to build high-performance NLP systems that deliver accurate and reliable results.
+
+## Usage
+
+CRFFeaturizer
+
+```python
+>>> from underthesea_core import CRFFeaturizer
+>>> features = ["T[-1]", "T[0]", "T[1]"]
+>>> dictionary = set(["sinh viên"])
+>>> featurizer = CRFFeaturizer(features, dictionary)
+>>> sentences = [[["sinh", "X"], ["viên", "X"], ["đi", "X"], ["học", "X"]]]
+>>> featurizer.process(sentences)
+[[['T[-1]=BOS', 'T[0]=sinh', 'T[1]=viên'],
+  ['T[-1]=sinh', 'T[0]=viên', 'T[1]=đi'],
+  ['T[-1]=viên', 'T[0]=đi', 'T[1]=học'],
+  ['T[-1]=đi', 'T[0]=học', 'T[1]=EOS']]]
+```
+
+## Release Workflow
+
+1. Change version in `Cargo.toml` and `pyproject.toml`
+2. Push to branch `core` with commit `Publish Underthesea Core`
+  * This will trigger `release-pypi-core` action
+3. Check latest version in [pypi](https://pypi.org/project/underthesea_core/)
```

