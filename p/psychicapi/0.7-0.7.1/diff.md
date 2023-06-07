# Comparing `tmp/psychicapi-0.7.tar.gz` & `tmp/psychicapi-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychicapi-0.7.tar", last modified: Wed Jun  7 02:33:51 2023, max compression
+gzip compressed data, was "psychicapi-0.7.1.tar", last modified: Wed Jun  7 02:42:11 2023, max compression
```

## Comparing `psychicapi-0.7.tar` & `psychicapi-0.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-07 02:33:51.550005 psychicapi-0.7/
--rw-r--r--   0 jasonfan   (501) staff       (20)     1774 2023-06-07 02:33:51.549877 psychicapi-0.7/PKG-INFO
--rw-r--r--   0 jasonfan   (501) staff       (20)     1509 2023-05-29 20:05:07.000000 psychicapi-0.7/README.md
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-07 02:33:51.548938 psychicapi-0.7/psychicapi/
--rw-r--r--   0 jasonfan   (501) staff       (20)       41 2023-05-19 18:59:00.000000 psychicapi-0.7/psychicapi/__init__.py
--rw-r--r--   0 jasonfan   (501) staff       (20)     2561 2023-06-07 02:33:11.000000 psychicapi-0.7/psychicapi/psychic.py
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-07 02:33:51.549677 psychicapi-0.7/psychicapi.egg-info/
--rw-r--r--   0 jasonfan   (501) staff       (20)     1774 2023-06-07 02:33:51.000000 psychicapi-0.7/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 jasonfan   (501) staff       (20)      232 2023-06-07 02:33:51.000000 psychicapi-0.7/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)        1 2023-06-07 02:33:51.000000 psychicapi-0.7/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)        9 2023-06-07 02:33:51.000000 psychicapi-0.7/psychicapi.egg-info/requires.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)       11 2023-06-07 02:33:51.000000 psychicapi-0.7/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)       38 2023-06-07 02:33:51.550046 psychicapi-0.7/setup.cfg
--rw-r--r--   0 jasonfan   (501) staff       (20)      664 2023-06-07 02:33:11.000000 psychicapi-0.7/setup.py
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-07 02:42:11.441211 psychicapi-0.7.1/
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1776 2023-06-07 02:42:11.441073 psychicapi-0.7.1/PKG-INFO
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1509 2023-05-29 20:05:07.000000 psychicapi-0.7.1/README.md
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-07 02:42:11.439919 psychicapi-0.7.1/psychicapi/
+-rw-r--r--   0 jasonfan   (501) staff       (20)       41 2023-05-19 18:59:00.000000 psychicapi-0.7.1/psychicapi/__init__.py
+-rw-r--r--   0 jasonfan   (501) staff       (20)     2563 2023-06-07 02:41:01.000000 psychicapi-0.7.1/psychicapi/psychic.py
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-07 02:42:11.440861 psychicapi-0.7.1/psychicapi.egg-info/
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1776 2023-06-07 02:42:11.000000 psychicapi-0.7.1/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 jasonfan   (501) staff       (20)      232 2023-06-07 02:42:11.000000 psychicapi-0.7.1/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)        1 2023-06-07 02:42:11.000000 psychicapi-0.7.1/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)        9 2023-06-07 02:42:11.000000 psychicapi-0.7.1/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)       11 2023-06-07 02:42:11.000000 psychicapi-0.7.1/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)       38 2023-06-07 02:42:11.441275 psychicapi-0.7.1/setup.cfg
+-rw-r--r--   0 jasonfan   (501) staff       (20)      666 2023-06-07 02:42:07.000000 psychicapi-0.7.1/setup.py
```

### Comparing `psychicapi-0.7/PKG-INFO` & `psychicapi-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7
+Version: 0.7.1
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
```

### Comparing `psychicapi-0.7/README.md` & `psychicapi-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `psychicapi-0.7/psychicapi/psychic.py` & `psychicapi-0.7.1/psychicapi/psychic.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     confluence = "confluence"
     zendesk = "zendesk"
     gdrive = "gdrive"
     slack = "slack"
 
 class Psychic:
     def __init__(self, secret_key: str):
-        self.api_url = "http://localhost:8080/"
+        self.api_url = "https://api.psychic.dev/"
         self.secret_key = secret_key
 
     def get_documents(self, *, account_id: str, connector_id: Optional[ConnectorId] = None):
         body = {
             "account_id": account_id
         }
         if connector_id is not None:
```

### Comparing `psychicapi-0.7/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.7.1/psychicapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7
+Version: 0.7.1
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
```

### Comparing `psychicapi-0.7/setup.py` & `psychicapi-0.7.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.7',
+    version='0.7.1',
     description='Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
     author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
```

