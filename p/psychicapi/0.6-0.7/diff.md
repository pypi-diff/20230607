# Comparing `tmp/psychicapi-0.6.tar.gz` & `tmp/psychicapi-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychicapi-0.6.tar", last modified: Wed May 31 22:25:16 2023, max compression
+gzip compressed data, was "psychicapi-0.7.tar", last modified: Wed Jun  7 02:33:51 2023, max compression
```

## Comparing `psychicapi-0.6.tar` & `psychicapi-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-05-31 22:25:16.542425 psychicapi-0.6/
--rw-r--r--   0 jasonfan   (501) staff       (20)     1774 2023-05-31 22:25:16.542214 psychicapi-0.6/PKG-INFO
--rw-r--r--   0 jasonfan   (501) staff       (20)     1509 2023-05-29 20:05:07.000000 psychicapi-0.6/README.md
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-05-31 22:25:16.540854 psychicapi-0.6/psychicapi/
--rw-r--r--   0 jasonfan   (501) staff       (20)       41 2023-05-19 18:59:00.000000 psychicapi-0.6/psychicapi/__init__.py
--rw-r--r--   0 jasonfan   (501) staff       (20)     2504 2023-05-31 15:17:19.000000 psychicapi-0.6/psychicapi/psychic.py
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-05-31 22:25:16.541931 psychicapi-0.6/psychicapi.egg-info/
--rw-r--r--   0 jasonfan   (501) staff       (20)     1774 2023-05-31 22:25:16.000000 psychicapi-0.6/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 jasonfan   (501) staff       (20)      232 2023-05-31 22:25:16.000000 psychicapi-0.6/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)        1 2023-05-31 22:25:16.000000 psychicapi-0.6/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)        9 2023-05-31 22:25:16.000000 psychicapi-0.6/psychicapi.egg-info/requires.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)       11 2023-05-31 22:25:16.000000 psychicapi-0.6/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)       38 2023-05-31 22:25:16.542479 psychicapi-0.6/setup.cfg
--rw-r--r--   0 jasonfan   (501) staff       (20)      664 2023-05-31 22:24:28.000000 psychicapi-0.6/setup.py
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-07 02:33:51.550005 psychicapi-0.7/
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1774 2023-06-07 02:33:51.549877 psychicapi-0.7/PKG-INFO
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1509 2023-05-29 20:05:07.000000 psychicapi-0.7/README.md
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-07 02:33:51.548938 psychicapi-0.7/psychicapi/
+-rw-r--r--   0 jasonfan   (501) staff       (20)       41 2023-05-19 18:59:00.000000 psychicapi-0.7/psychicapi/__init__.py
+-rw-r--r--   0 jasonfan   (501) staff       (20)     2561 2023-06-07 02:33:11.000000 psychicapi-0.7/psychicapi/psychic.py
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-07 02:33:51.549677 psychicapi-0.7/psychicapi.egg-info/
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1774 2023-06-07 02:33:51.000000 psychicapi-0.7/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 jasonfan   (501) staff       (20)      232 2023-06-07 02:33:51.000000 psychicapi-0.7/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)        1 2023-06-07 02:33:51.000000 psychicapi-0.7/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)        9 2023-06-07 02:33:51.000000 psychicapi-0.7/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)       11 2023-06-07 02:33:51.000000 psychicapi-0.7/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)       38 2023-06-07 02:33:51.550046 psychicapi-0.7/setup.cfg
+-rw-r--r--   0 jasonfan   (501) staff       (20)      664 2023-06-07 02:33:11.000000 psychicapi-0.7/setup.py
```

### Comparing `psychicapi-0.6/PKG-INFO` & `psychicapi-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.6
+Version: 0.7
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
```

### Comparing `psychicapi-0.6/README.md` & `psychicapi-0.7/README.md`

 * *Files identical despite different names*

### Comparing `psychicapi-0.6/psychicapi/psychic.py` & `psychicapi-0.7/psychicapi/psychic.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,36 +7,38 @@
     confluence = "confluence"
     zendesk = "zendesk"
     gdrive = "gdrive"
     slack = "slack"
 
 class Psychic:
     def __init__(self, secret_key: str):
-        self.api_url = "https://sidekick-ezml2kwdva-uc.a.run.app/"
+        self.api_url = "http://localhost:8080/"
         self.secret_key = secret_key
 
-    def get_documents(self, connector_id: ConnectorId, account_id: str):
+    def get_documents(self, *, account_id: str, connector_id: Optional[ConnectorId] = None):
+        body = {
+            "account_id": account_id
+        }
+        if connector_id is not None:
+            body["connector_id"] = connector_id.value
         response = requests.post(
             self.api_url + "get-documents",
-            json={
-                "connector_id": connector_id.value,
-                "account_id": account_id,
-            },
+            json=body,
             headers={
                 'Authorization': 'Bearer ' + self.secret_key,
                 'Accept': 'application/json'
             }
         )
         if response.status_code == 200:
             documents = response.json()["documents"]
             return documents
         else:
             return None
         
-    def get_connections(self, connector_id: Optional[ConnectorId] = None, account_id: Optional[str] = None):
+    def get_connections(self, *, connector_id: Optional[ConnectorId] = None, account_id: Optional[str] = None):
         filter = {}
 
         if connector_id is not None:
             filter["connector_id"] = connector_id.value
         if account_id is not None:
             filter["account_id"] = account_id
 
@@ -52,15 +54,15 @@
         )
         if response.status_code == 200:
             documents = response.json()["connections"]
             return documents
         else:
             return None
         
-    def get_conversations(self, connector_id: ConnectorId, account_id: str, oldest_timestamp: Optional[int] = None):
+    def get_conversations(self, *, account_id: str, connector_id: ConnectorId, oldest_timestamp: Optional[int] = None):
         body = {
             "connector_id": connector_id.value,
             "account_id": account_id,
         }
         if oldest_timestamp is not None:
             body["oldest_timestamp"] = oldest_timestamp
```

### Comparing `psychicapi-0.6/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.7/psychicapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.6
+Version: 0.7
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
```

### Comparing `psychicapi-0.6/setup.py` & `psychicapi-0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.6',
+    version='0.7',
     description='Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
     author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
```

