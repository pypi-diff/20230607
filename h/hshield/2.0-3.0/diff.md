# Comparing `tmp/hshield-2.0.tar.gz` & `tmp/hshield-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hshield-2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hshield-3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hshield-2.0.tar` & `hshield-3.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-06-05 18:36:09.940967 hshield-2.0/LICENSE
--rw-r--r--   0        0        0      129 2023-06-05 18:34:15.638317 hshield-2.0/README.md
--rw-r--r--   0        0        0       51 2023-06-06 21:56:34.392058 hshield-2.0/hshield/__init__.py
--rw-r--r--   0        0        0     1326 2023-06-05 19:02:57.441919 hshield-2.0/hshield/main.py
--rw-r--r--   0        0        0        0 2023-06-06 21:51:46.160060 hshield-2.0/hshield/modules/__init__.py
--rw-r--r--   0        0        0      447 2023-06-05 18:27:10.081946 hshield-2.0/hshield/modules/address_shield.py
--rw-r--r--   0        0        0      495 2023-06-05 18:25:54.947755 hshield-2.0/hshield/modules/document_shield.py
--rw-r--r--   0        0        0      391 2023-06-05 18:25:25.075156 hshield-2.0/hshield/modules/name_shield.py
--rw-r--r--   0        0        0       30 2023-06-05 18:21:56.713190 hshield-2.0/hshield/text.txt
--rw-r--r--   0        0        0      645 2023-06-05 19:12:35.197513 hshield-2.0/pyproject.toml
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 hshield-2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-05 18:36:09.940967 hshield-3.0/LICENSE
+-rw-r--r--   0        0        0      129 2023-06-05 18:34:15.638317 hshield-3.0/README.md
+-rw-r--r--   0        0        0       51 2023-06-06 22:06:49.484074 hshield-3.0/hshield/__init__.py
+-rw-r--r--   0        0        0     1350 2023-06-06 22:06:08.092869 hshield-3.0/hshield/main.py
+-rw-r--r--   0        0        0      447 2023-06-05 18:27:10.081946 hshield-3.0/hshield/modules/address_shield.py
+-rw-r--r--   0        0        0      495 2023-06-05 18:25:54.947755 hshield-3.0/hshield/modules/document_shield.py
+-rw-r--r--   0        0        0      391 2023-06-05 18:25:25.075156 hshield-3.0/hshield/modules/name_shield.py
+-rw-r--r--   0        0        0       30 2023-06-05 18:21:56.713190 hshield-3.0/hshield/text.txt
+-rw-r--r--   0        0        0      645 2023-06-05 19:12:35.197513 hshield-3.0/pyproject.toml
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 hshield-3.0/PKG-INFO
```

### Comparing `hshield-2.0/LICENSE` & `hshield-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hshield-2.0/hshield/main.py` & `hshield-3.0/hshield/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
-from modules.name_shield import NameShield
-from modules.address_shield import AddressShield
-from modules.document_shield import DocumentShield
+from hshield.modules.name_shield import NameShield
+from hshield.modules.address_shield import AddressShield
+from hshield.modules.document_shield import DocumentShield
 
 def main():
     parser = argparse.ArgumentParser(
         prog="Shield",
         description="Data anonymizer tool",
         epilog="Build by Henrique, José and Alex"
     )
```

### Comparing `hshield-2.0/pyproject.toml` & `hshield-3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hshield-2.0/PKG-INFO` & `hshield-3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hshield
-Version: 2.0
+Version: 3.0
 Summary: Shield: Data Anonymizer tool
 Author-email: Francisco Alexandre Neves <pg50375@alunos.uminho.pt>, Henrique Parola Costa <pg50415@alunos.uminho.pt>, José Pedro Fernandes <pg50525@alunos.uminho.pt>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Source, https://github.com/LittleLevi05/spln-2223/tree/main/TP2
 
 # Shield
```

