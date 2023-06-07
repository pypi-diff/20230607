# Comparing `tmp/paper-qa-2.1.0.tar.gz` & `tmp/paper-qa-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-2.1.0.tar", last modified: Sun Jun  4 01:29:31 2023, max compression
+gzip compressed data, was "paper-qa-2.1.1.tar", last modified: Wed Jun  7 03:17:44 2023, max compression
```

## Comparing `paper-qa-2.1.0.tar` & `paper-qa-2.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:29:31.464349 paper-qa-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 01:28:55.000000 paper-qa-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-04 01:29:31.464349 paper-qa-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-06-04 01:28:55.000000 paper-qa-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:29:31.460349 paper-qa-2.1.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-04 01:29:31.000000 paper-qa-2.1.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-04 01:29:31.000000 paper-qa-2.1.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 01:29:31.000000 paper-qa-2.1.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-04 01:29:31.000000 paper-qa-2.1.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-04 01:29:31.000000 paper-qa-2.1.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:29:31.460349 paper-qa-2.1.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:29:31.464349 paper-qa-2.1.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    22971 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 01:29:31.464349 paper-qa-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-04 01:28:55.000000 paper-qa-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:29:31.464349 paper-qa-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-06-04 01:28:55.000000 paper-qa-2.1.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:17:44.571631 paper-qa-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 03:16:57.000000 paper-qa-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-07 03:17:44.571631 paper-qa-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-06-07 03:16:57.000000 paper-qa-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:17:44.567631 paper-qa-2.1.1/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-07 03:17:44.000000 paper-qa-2.1.1/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-07 03:17:44.000000 paper-qa-2.1.1/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:17:44.000000 paper-qa-2.1.1/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-07 03:17:44.000000 paper-qa-2.1.1/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 03:17:44.000000 paper-qa-2.1.1/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:17:44.571631 paper-qa-2.1.1/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:17:44.571631 paper-qa-2.1.1/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22969 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 03:16:57.000000 paper-qa-2.1.1/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 03:17:44.571631 paper-qa-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-07 03:16:57.000000 paper-qa-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:17:44.571631 paper-qa-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-06-07 03:16:57.000000 paper-qa-2.1.1/tests/test_paperqa.py
```

### Comparing `paper-qa-2.1.0/LICENSE` & `paper-qa-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-2.1.0/PKG-INFO` & `paper-qa-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 2.1.0
+Version: 2.1.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-2.1.0/README.md` & `paper-qa-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-2.1.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-2.1.1/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 2.1.0
+Version: 2.1.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-2.1.0/paperqa/agent.py` & `paper-qa-2.1.1/paperqa/agent.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.1.0/paperqa/contrib/zotero.py` & `paper-qa-2.1.1/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.1.0/paperqa/docs.py` & `paper-qa-2.1.1/paperqa/docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             key = new_key
         if text_embeddings is None:
             text_embeddings = self.embeddings.embed_documents(texts)
         if self._faiss_index is not None:
             self._faiss_index.add_embeddings(
                 list(zip(texts, text_embeddings)), metadatas=metadatas
             )
-        elif self._doc_index is not None:
+        if self._doc_index is not None:
             self._doc_index.add_texts([citation], metadatas=[{"key": key}])
         self.docs.append(
             dict(
                 texts=texts,
                 metadata=metadatas,
                 key=key,
                 hash=hash,
```

### Comparing `paper-qa-2.1.0/paperqa/qaprompts.py` & `paper-qa-2.1.1/paperqa/qaprompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.1.0/paperqa/readers.py` & `paper-qa-2.1.1/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.1.0/paperqa/types.py` & `paper-qa-2.1.1/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.1.0/paperqa/utils.py` & `paper-qa-2.1.1/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.1.0/setup.py` & `paper-qa-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.1.0/tests/test_paperqa.py` & `paper-qa-2.1.1/tests/test_paperqa.py`

 * *Files identical despite different names*

