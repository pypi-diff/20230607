# Comparing `tmp/xia_git-0.0.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_git-0.0.2-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 91714 bytes, number of entries: 7
--rw-r--r--  2.0 unx       76 b- defN 23-May-17 17:13 xia_git/__init__.py
--rw-r--r--  2.0 unx   219648 b- defN 23-May-17 17:18 xia_git/git.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      150 b- defN 23-May-17 17:18 xia_git-0.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      600 b- defN 23-May-17 17:18 xia_git-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-17 17:18 xia_git-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-May-17 17:18 xia_git-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      550 b- defN 23-May-17 17:18 xia_git-0.0.1.dist-info/RECORD
-7 files, 221131 bytes uncompressed, 90736 bytes compressed:  59.0%
+Zip file size: 71193 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-07 19:05 xia_git/__init__.py
+-rw-r--r--  2.0 unx   201064 b- defN 23-Jun-07 19:05 xia_git/git.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-07 19:05 xia_git-0.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      563 b- defN 23-Jun-07 19:05 xia_git-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-07 19:05 xia_git-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-07 19:05 xia_git-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      554 b- defN 23-Jun-07 19:05 xia_git-0.0.2.dist-info/RECORD
+7 files, 202524 bytes uncompressed, 70209 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_git/__init__.py
 Comment: 
 
-Filename: xia_git/git.cp39-win_amd64.pyd
+Filename: xia_git/git.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_git-0.0.1.dist-info/LICENSE.txt
+Filename: xia_git-0.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_git-0.0.1.dist-info/METADATA
+Filename: xia_git-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_git-0.0.1.dist-info/WHEEL
+Filename: xia_git-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_git-0.0.1.dist-info/top_level.txt
+Filename: xia_git-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_git-0.0.1.dist-info/RECORD
+Filename: xia_git-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_git/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_git.git import Git
 
 __all__ = [
     "Git"
 ]
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## Comparing `xia_git-0.0.1.dist-info/METADATA` & `xia_git-0.0.2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-git
-Version: 0.0.1
+Version: 0.0.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-git/0.0.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-git/0.0.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 .. image:: https://img.shields.io/pypi/v/xia-git.svg?color=blue
    :alt: PyPI-Server
    :target: https://pypi.org/project/xia-git/
@@ -25,9 +23,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

