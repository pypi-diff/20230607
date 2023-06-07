# Comparing `tmp/chatdocs-0.2.1.tar.gz` & `tmp/chatdocs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatdocs-0.2.1.tar", last modified: Sun Jun  4 21:21:05 2023, max compression
+gzip compressed data, was "chatdocs-0.2.2.tar", last modified: Wed Jun  7 20:40:58 2023, max compression
```

## Comparing `chatdocs-0.2.1.tar` & `chatdocs-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 21:21:05.441810 chatdocs-0.2.1/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7448 2023-06-04 21:21:05.441810 chatdocs-0.2.1/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4917 2023-06-04 21:11:41.000000 chatdocs-0.2.1/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 21:21:05.431810 chatdocs-0.2.1/chatdocs/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.2.1/chatdocs/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.2.1/chatdocs/__main__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5657 2023-06-04 03:56:33.000000 chatdocs-0.2.1/chatdocs/add.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      554 2023-06-04 12:15:53.000000 chatdocs-0.2.1/chatdocs/chains.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1307 2023-06-04 17:42:56.000000 chatdocs-0.2.1/chatdocs/chat.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      665 2023-06-04 04:02:06.000000 chatdocs-0.2.1/chatdocs/config.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 21:21:05.431810 chatdocs-0.2.1/chatdocs/data/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      456 2023-06-04 15:38:55.000000 chatdocs-0.2.1/chatdocs/data/chatdocs.yml
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4272 2023-06-04 20:29:35.000000 chatdocs-0.2.1/chatdocs/data/index.html
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      232 2023-06-04 02:56:51.000000 chatdocs-0.2.1/chatdocs/download.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      491 2023-06-04 01:27:28.000000 chatdocs-0.2.1/chatdocs/embeddings.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1108 2023-06-04 17:37:23.000000 chatdocs-0.2.1/chatdocs/llms.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1259 2023-06-04 11:04:07.000000 chatdocs-0.2.1/chatdocs/main.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1693 2023-06-04 19:41:17.000000 chatdocs-0.2.1/chatdocs/ui.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      368 2023-06-04 01:08:37.000000 chatdocs-0.2.1/chatdocs/utils.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      914 2023-06-04 03:51:59.000000 chatdocs-0.2.1/chatdocs/vectorstores.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 21:21:05.431810 chatdocs-0.2.1/chatdocs.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7448 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      544 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/entry_points.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      413 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-04 21:21:05.000000 chatdocs-0.2.1/chatdocs.egg-info/top_level.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-04 21:21:05.441810 chatdocs-0.2.1/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2179 2023-06-04 21:20:27.000000 chatdocs-0.2.1/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-07 20:40:58.232766 chatdocs-0.2.2/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9830 2023-06-07 20:40:58.232766 chatdocs-0.2.2/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6774 2023-06-07 20:34:43.000000 chatdocs-0.2.2/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-07 20:40:58.222766 chatdocs-0.2.2/chatdocs/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.2.2/chatdocs/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.2.2/chatdocs/__main__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5657 2023-06-04 03:56:33.000000 chatdocs-0.2.2/chatdocs/add.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      554 2023-06-04 12:15:53.000000 chatdocs-0.2.2/chatdocs/chains.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1376 2023-06-07 13:32:32.000000 chatdocs-0.2.2/chatdocs/chat.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      665 2023-06-04 04:02:06.000000 chatdocs-0.2.2/chatdocs/config.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-07 20:40:58.232766 chatdocs-0.2.2/chatdocs/data/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      639 2023-06-07 13:37:27.000000 chatdocs-0.2.2/chatdocs/data/chatdocs.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4272 2023-06-04 20:29:35.000000 chatdocs-0.2.2/chatdocs/data/index.html
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      232 2023-06-07 19:32:55.000000 chatdocs-0.2.2/chatdocs/download.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      491 2023-06-04 01:27:28.000000 chatdocs-0.2.2/chatdocs/embeddings.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2668 2023-06-07 19:29:24.000000 chatdocs-0.2.2/chatdocs/llms.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1259 2023-06-04 11:04:07.000000 chatdocs-0.2.2/chatdocs/main.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1693 2023-06-04 19:41:17.000000 chatdocs-0.2.2/chatdocs/ui.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      219 2023-06-07 13:30:29.000000 chatdocs-0.2.2/chatdocs/utils.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      914 2023-06-04 03:51:59.000000 chatdocs-0.2.2/chatdocs/vectorstores.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-07 20:40:58.222766 chatdocs-0.2.2/chatdocs.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9830 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      544 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/entry_points.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      445 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-07 20:40:58.000000 chatdocs-0.2.2/chatdocs.egg-info/top_level.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-07 20:40:58.232766 chatdocs-0.2.2/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2247 2023-06-07 20:38:45.000000 chatdocs-0.2.2/setup.py
```

### Comparing `chatdocs-0.2.1/chatdocs/add.py` & `chatdocs-0.2.2/chatdocs/add.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.1/chatdocs/chains.py` & `chatdocs-0.2.2/chatdocs/chains.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.1/chatdocs/chat.py` & `chatdocs-0.2.2/chatdocs/chat.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from typing import Any, Dict, Optional
 
 from rich import print
 from rich.markup import escape
 from rich.panel import Panel
 
 from .chains import get_retrieval_qa
-from .utils import print_answer
+
+
+def print_answer(text: str) -> None:
+    print(f"[bright_cyan]{escape(text)}", end="", flush=True)
 
 
 def chat(config: Dict[str, Any], query: Optional[str] = None) -> None:
     qa = get_retrieval_qa(config, callback=print_answer)
 
     interactive = not query
     print()
```

### Comparing `chatdocs-0.2.1/chatdocs/config.py` & `chatdocs-0.2.2/chatdocs/config.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.1/chatdocs/data/index.html` & `chatdocs-0.2.2/chatdocs/data/index.html`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.1/chatdocs/main.py` & `chatdocs-0.2.2/chatdocs/main.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.1/chatdocs/ui.py` & `chatdocs-0.2.2/chatdocs/ui.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.1/chatdocs/vectorstores.py` & `chatdocs-0.2.2/chatdocs/vectorstores.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.1/chatdocs.egg-info/SOURCES.txt` & `chatdocs-0.2.2/chatdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.1/setup.py` & `chatdocs-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md") as f:
     long_description = f.read()
 
 name = "chatdocs"
 
 setup(
     name=name,
-    version="0.2.1",
+    version="0.2.2",
     description="Chat with your documents offline using AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ravindra Marella",
     author_email="mv.ravindra007@gmail.com",
     url="https://github.com/marella/{}".format(name),
     license="MIT",
@@ -40,14 +40,17 @@
         "pypandoc>=1.11,<2.0.0",
         "pdfminer.six==20221105",
         "unstructured>=0.6.0,<0.7.0",
         # Temporary fix for `rich`, `numpy` version conflicts.
         "argilla==1.8.0",
     ],
     extras_require={
+        "gptq": [
+            "auto-gptq>=0.2.1,<0.3.0",
+        ],
         "tests": [
             "pytest",
         ],
     },
     zip_safe=False,
     classifiers=[
         "Development Status :: 1 - Planning",
```

