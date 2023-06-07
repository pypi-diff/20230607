# Comparing `tmp/streamlit-chitchat-0.1.2.tar.gz` & `tmp/streamlit-chitchat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chitchat-0.1.2.tar", max compression
+gzip compressed data, was "streamlit-chitchat-0.1.3.tar", max compression
```

## Comparing `streamlit-chitchat-0.1.2.tar` & `streamlit-chitchat-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      820 2023-06-07 15:44:01.184625 streamlit-chitchat-0.1.2/README.md
--rw-r--r--   0        0        0      620 2023-06-07 16:00:06.164202 streamlit-chitchat-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       58 2023-06-07 15:59:12.528983 streamlit-chitchat-0.1.2/streamlit-chitchat/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 23:53:56.560425 streamlit-chitchat-0.1.2/streamlit-chitchat/streamlit_chitchat/__init__.py
--rw-r--r--   0        0        0     5187 2023-06-06 22:15:39.989109 streamlit-chitchat-0.1.2/streamlit-chitchat/streamlit_chitchat/chitchat.py
--rw-r--r--   0        0        0        0 2023-06-06 23:57:13.754028 streamlit-chitchat-0.1.2/streamlit-chitchat/tests/__init__.py
--rw-r--r--   0        0        0     1146 2023-06-07 00:13:14.318438 streamlit-chitchat-0.1.2/streamlit-chitchat/tests/main.py
--rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 streamlit-chitchat-0.1.2/setup.py
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 streamlit-chitchat-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      820 2023-06-07 15:44:01.184625 streamlit-chitchat-0.1.3/README.md
+-rw-r--r--   0        0        0      620 2023-06-07 16:14:16.703136 streamlit-chitchat-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-06-07 16:18:25.669290 streamlit-chitchat-0.1.3/streamlit_chitchat/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:53:56.560425 streamlit-chitchat-0.1.3/streamlit_chitchat/streamlit_chitchat/__init__.py
+-rw-r--r--   0        0        0     5187 2023-06-06 22:15:39.989109 streamlit-chitchat-0.1.3/streamlit_chitchat/streamlit_chitchat/chitchat.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:57:13.754028 streamlit-chitchat-0.1.3/streamlit_chitchat/tests/__init__.py
+-rw-r--r--   0        0        0     1146 2023-06-07 00:13:14.318438 streamlit-chitchat-0.1.3/streamlit_chitchat/tests/main.py
+-rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 streamlit-chitchat-0.1.3/setup.py
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 streamlit-chitchat-0.1.3/PKG-INFO
```

### Comparing `streamlit-chitchat-0.1.2/README.md` & `streamlit-chitchat-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-chitchat-0.1.2/pyproject.toml` & `streamlit-chitchat-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "streamlit-chitchat"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["k4144 <you@example.com>"]
 readme = "README.md"
-packages = [{include = "streamlit-chitchat"}]
+packages = [{include = "streamlit_chitchat"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `streamlit-chitchat-0.1.2/streamlit-chitchat/streamlit_chitchat/chitchat.py` & `streamlit-chitchat-0.1.3/streamlit_chitchat/streamlit_chitchat/chitchat.py`

 * *Files identical despite different names*

### Comparing `streamlit-chitchat-0.1.2/streamlit-chitchat/tests/main.py` & `streamlit-chitchat-0.1.3/streamlit_chitchat/tests/main.py`

 * *Files identical despite different names*

### Comparing `streamlit-chitchat-0.1.2/setup.py` & `streamlit-chitchat-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['streamlit-chitchat',
- 'streamlit-chitchat.streamlit_chitchat',
- 'streamlit-chitchat.tests']
+['streamlit_chitchat',
+ 'streamlit_chitchat.streamlit_chitchat',
+ 'streamlit_chitchat.tests']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'streamlit-chitchat',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': '<br>\n\n  \n\n<img  src="https://user-images.githubusercontent.com/7164864/217935870-c0bc60a3-6fc0-4047-b011-7b4c59488c91.png"  alt="Streamlit logo"  style="margin-top:50px"></img>\n\n  \n\n# streamlit-chitchat\n\n  \n\n**make chat messages easier to style in streamlit**\n\n  \n\nstreamlit-chitchat lets you style messages from the user and responses from a bot differently. you can also update an existing message, so that streamed tokens render as they are received. \n\n\n  \n\n## Installation\n\n  \n\nOpen a terminal and run:\n\n  \n\n```bash\n\n$  pip  install  streamlit-chitchat\n\n```\n\n## example use\n  \n\nin your streamlit app, insert:\n\n  \n\n```bash\n\nfrom streamlit-chitchat.chitchat import message\nmessage(\'hello, how are you?\', is_user=True)\nbot=message()\nfor w in \'excellent! have any plans for tonight?\'.split(\' \'):\n\tbot.write(w+\' \')\n```\n\n\n',
     'author': 'k4144',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `streamlit-chitchat-0.1.2/PKG-INFO` & `streamlit-chitchat-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chitchat
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: k4144
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

