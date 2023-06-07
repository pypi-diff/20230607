# Comparing `tmp/hshield-3.0.tar.gz` & `tmp/hshield-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hshield-3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hshield-4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hshield-3.0.tar` & `hshield-4.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1077 2023-06-05 18:36:09.940967 hshield-3.0/LICENSE
--rw-r--r--   0        0        0      129 2023-06-05 18:34:15.638317 hshield-3.0/README.md
--rw-r--r--   0        0        0       51 2023-06-06 22:06:49.484074 hshield-3.0/hshield/__init__.py
--rw-r--r--   0        0        0     1350 2023-06-06 22:06:08.092869 hshield-3.0/hshield/main.py
--rw-r--r--   0        0        0      447 2023-06-05 18:27:10.081946 hshield-3.0/hshield/modules/address_shield.py
--rw-r--r--   0        0        0      495 2023-06-05 18:25:54.947755 hshield-3.0/hshield/modules/document_shield.py
--rw-r--r--   0        0        0      391 2023-06-05 18:25:25.075156 hshield-3.0/hshield/modules/name_shield.py
--rw-r--r--   0        0        0       30 2023-06-05 18:21:56.713190 hshield-3.0/hshield/text.txt
--rw-r--r--   0        0        0      645 2023-06-05 19:12:35.197513 hshield-3.0/pyproject.toml
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 hshield-3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-05 18:36:09.940967 hshield-4.0/LICENSE
+-rw-r--r--   0        0        0      129 2023-06-05 18:34:15.638317 hshield-4.0/README.md
+-rw-r--r--   0        0        0       51 2023-06-07 15:42:17.668865 hshield-4.0/hshield/__init__.py
+-rw-r--r--   0        0        0      447 2023-06-05 18:27:10.081946 hshield-4.0/hshield/address_shield.py
+-rw-r--r--   0        0        0      495 2023-06-05 18:25:54.947755 hshield-4.0/hshield/document_shield.py
+-rw-r--r--   0        0        0     1346 2023-06-07 15:31:16.871037 hshield-4.0/hshield/main.py
+-rw-r--r--   0        0        0     1241 2023-06-07 15:42:04.422316 hshield-4.0/hshield/name_shield.py
+-rw-r--r--   0        0        0        5 2023-06-07 15:14:07.215849 hshield-4.0/hshield/requirements.txt
+-rw-r--r--   0        0        0     1706 2023-06-07 15:17:23.724788 hshield-4.0/hshield/tests/doc1.txt
+-rw-r--r--   0        0        0      645 2023-06-05 19:12:35.197513 hshield-4.0/pyproject.toml
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 hshield-4.0/PKG-INFO
```

### Comparing `hshield-3.0/LICENSE` & `hshield-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hshield-3.0/hshield/main.py` & `hshield-4.0/hshield/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
-from hshield.modules.name_shield import NameShield
-from hshield.modules.address_shield import AddressShield
-from hshield.modules.document_shield import DocumentShield
+from name_shield import NameShield
+from address_shield import AddressShield
+from document_shield import DocumentShield
 
 def main():
     parser = argparse.ArgumentParser(
         prog="Shield",
         description="Data anonymizer tool",
         epilog="Build by Henrique, José and Alex"
     )
@@ -21,23 +21,25 @@
     text = ""
 
     if filename:
         with open(filename,"r") as f:
             text  = f.read() 
 
         if args.name:
-            text = NameShield(text=text).shield()
+            name = NameShield(text=text)
+            print(name.shield())
 
         if args.document:
             text = DocumentShield(text=text).shield()
 
         if args.address:
             text = AddressShield(text=text).shield()
 
         if args.output:
             with open(args.output,"w") as f:
                 f.write(text)
         else:
-            print(text)
+            #print(text)
+            pass
 
 if __name__ == "__main__":
     main()
```

### Comparing `hshield-3.0/pyproject.toml` & `hshield-4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hshield-3.0/PKG-INFO` & `hshield-4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hshield
-Version: 3.0
+Version: 4.0
 Summary: Shield: Data Anonymizer tool
 Author-email: Francisco Alexandre Neves <pg50375@alunos.uminho.pt>, Henrique Parola Costa <pg50415@alunos.uminho.pt>, José Pedro Fernandes <pg50525@alunos.uminho.pt>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Source, https://github.com/LittleLevi05/spln-2223/tree/main/TP2
 
 # Shield
```

