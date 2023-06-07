# Comparing `tmp/llm-blocks-0.2.0.tar.gz` & `tmp/llm-blocks-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-blocks-0.2.0.tar", last modified: Wed Jun  7 16:05:33 2023, max compression
+gzip compressed data, was "llm-blocks-0.2.1.tar", last modified: Wed Jun  7 16:23:52 2023, max compression
```

## Comparing `llm-blocks-0.2.0.tar` & `llm-blocks-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 16:05:33.050712 llm-blocks-0.2.0/
--rw-rw-rw-   0        0        0     2771 2023-06-07 16:05:33.049713 llm-blocks-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2327 2023-06-07 15:34:54.000000 llm-blocks-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 16:05:33.039559 llm-blocks-0.2.0/llm_blocks/
--rw-rw-rw-   0        0        0        0 2023-06-06 22:53:28.000000 llm-blocks-0.2.0/llm_blocks/__init__.py
--rw-rw-rw-   0        0        0     1620 2023-06-07 15:34:54.000000 llm-blocks-0.2.0/llm_blocks/chat_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 16:05:33.047706 llm-blocks-0.2.0/llm_blocks.egg-info/
--rw-rw-rw-   0        0        0     2771 2023-06-07 16:05:32.000000 llm-blocks-0.2.0/llm_blocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-07 16:05:32.000000 llm-blocks-0.2.0/llm_blocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 16:05:32.000000 llm-blocks-0.2.0/llm_blocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-07 16:05:32.000000 llm-blocks-0.2.0/llm_blocks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-07 16:05:32.000000 llm-blocks-0.2.0/llm_blocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 16:05:33.050712 llm-blocks-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      891 2023-06-07 16:03:22.000000 llm-blocks-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:23:52.334385 llm-blocks-0.2.1/
+-rw-rw-rw-   0        0        0     2771 2023-06-07 16:23:52.333393 llm-blocks-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2327 2023-06-07 15:34:54.000000 llm-blocks-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 16:23:52.322861 llm-blocks-0.2.1/llm_blocks/
+-rw-rw-rw-   0        0        0        0 2023-06-06 22:53:28.000000 llm-blocks-0.2.1/llm_blocks/__init__.py
+-rw-rw-rw-   0        0        0     1620 2023-06-07 15:34:54.000000 llm-blocks-0.2.1/llm_blocks/chat_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:23:52.331385 llm-blocks-0.2.1/llm_blocks.egg-info/
+-rw-rw-rw-   0        0        0     2771 2023-06-07 16:23:52.000000 llm-blocks-0.2.1/llm_blocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-07 16:23:52.000000 llm-blocks-0.2.1/llm_blocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 16:23:52.000000 llm-blocks-0.2.1/llm_blocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-07 16:23:52.000000 llm-blocks-0.2.1/llm_blocks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 16:23:52.000000 llm-blocks-0.2.1/llm_blocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 16:23:52.334385 llm-blocks-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      891 2023-06-07 16:23:11.000000 llm-blocks-0.2.1/setup.py
```

### Comparing `llm-blocks-0.2.0/PKG-INFO` & `llm-blocks-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-blocks
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple interface for creating and managing LLM chains
 Home-page: https://github.com/voynow/llm-blocks
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm-blocks-0.2.0/README.md` & `llm-blocks-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `llm-blocks-0.2.0/llm_blocks/chat_utils.py` & `llm-blocks-0.2.1/llm_blocks/chat_utils.py`

 * *Files identical despite different names*

### Comparing `llm-blocks-0.2.0/llm_blocks.egg-info/PKG-INFO` & `llm-blocks-0.2.1/llm_blocks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-blocks
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple interface for creating and managing LLM chains
 Home-page: https://github.com/voynow/llm-blocks
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm-blocks-0.2.0/setup.py` & `llm-blocks-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="llm-blocks",
-    version="0.2.0",
+    version="0.2.1",
     author="Jamie Voynow",
     author_email="voynow99@gmail.com",
     description="Simple interface for creating and managing LLM chains",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/voynow/llm-blocks",
     packages=find_packages(),
```

