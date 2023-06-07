# Comparing `tmp/streamlit-chitchat-0.1.3.tar.gz` & `tmp/streamlit-chitchat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chitchat-0.1.3.tar", max compression
+gzip compressed data, was "streamlit-chitchat-0.1.4.tar", max compression
```

## Comparing `streamlit-chitchat-0.1.3.tar` & `streamlit-chitchat-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      820 2023-06-07 15:44:01.184625 streamlit-chitchat-0.1.3/README.md
--rw-r--r--   0        0        0      620 2023-06-07 16:14:16.703136 streamlit-chitchat-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       58 2023-06-07 16:18:25.669290 streamlit-chitchat-0.1.3/streamlit_chitchat/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 23:53:56.560425 streamlit-chitchat-0.1.3/streamlit_chitchat/streamlit_chitchat/__init__.py
--rw-r--r--   0        0        0     5187 2023-06-06 22:15:39.989109 streamlit-chitchat-0.1.3/streamlit_chitchat/streamlit_chitchat/chitchat.py
--rw-r--r--   0        0        0        0 2023-06-06 23:57:13.754028 streamlit-chitchat-0.1.3/streamlit_chitchat/tests/__init__.py
--rw-r--r--   0        0        0     1146 2023-06-07 00:13:14.318438 streamlit-chitchat-0.1.3/streamlit_chitchat/tests/main.py
--rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 streamlit-chitchat-0.1.3/setup.py
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 streamlit-chitchat-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      820 2023-06-07 15:44:01.184625 streamlit-chitchat-0.1.4/README.md
+-rw-r--r--   0        0        0      620 2023-06-07 16:29:53.419050 streamlit-chitchat-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-07 16:29:09.035394 streamlit-chitchat-0.1.4/streamlit_chitchat/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:53:56.560425 streamlit-chitchat-0.1.4/streamlit_chitchat/streamlit_chitchat/__init__.py
+-rw-r--r--   0        0        0     5187 2023-06-06 22:15:39.989109 streamlit-chitchat-0.1.4/streamlit_chitchat/streamlit_chitchat/chitchat.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:57:13.754028 streamlit-chitchat-0.1.4/streamlit_chitchat/tests/__init__.py
+-rw-r--r--   0        0        0     1146 2023-06-07 00:13:14.318438 streamlit-chitchat-0.1.4/streamlit_chitchat/tests/main.py
+-rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 streamlit-chitchat-0.1.4/setup.py
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 streamlit-chitchat-0.1.4/PKG-INFO
```

### Comparing `streamlit-chitchat-0.1.3/README.md` & `streamlit-chitchat-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-chitchat-0.1.3/pyproject.toml` & `streamlit-chitchat-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit-chitchat"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["k4144 <you@example.com>"]
 readme = "README.md"
 packages = [{include = "streamlit_chitchat"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `streamlit-chitchat-0.1.3/streamlit_chitchat/streamlit_chitchat/chitchat.py` & `streamlit-chitchat-0.1.4/streamlit_chitchat/streamlit_chitchat/chitchat.py`

 * *Files identical despite different names*

### Comparing `streamlit-chitchat-0.1.3/streamlit_chitchat/tests/main.py` & `streamlit-chitchat-0.1.4/streamlit_chitchat/tests/main.py`

 * *Files identical despite different names*

### Comparing `streamlit-chitchat-0.1.3/setup.py` & `streamlit-chitchat-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  'streamlit_chitchat.tests']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'streamlit-chitchat',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': '<br>\n\n  \n\n<img  src="https://user-images.githubusercontent.com/7164864/217935870-c0bc60a3-6fc0-4047-b011-7b4c59488c91.png"  alt="Streamlit logo"  style="margin-top:50px"></img>\n\n  \n\n# streamlit-chitchat\n\n  \n\n**make chat messages easier to style in streamlit**\n\n  \n\nstreamlit-chitchat lets you style messages from the user and responses from a bot differently. you can also update an existing message, so that streamed tokens render as they are received. \n\n\n  \n\n## Installation\n\n  \n\nOpen a terminal and run:\n\n  \n\n```bash\n\n$  pip  install  streamlit-chitchat\n\n```\n\n## example use\n  \n\nin your streamlit app, insert:\n\n  \n\n```bash\n\nfrom streamlit-chitchat.chitchat import message\nmessage(\'hello, how are you?\', is_user=True)\nbot=message()\nfor w in \'excellent! have any plans for tonight?\'.split(\' \'):\n\tbot.write(w+\' \')\n```\n\n\n',
     'author': 'k4144',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `streamlit-chitchat-0.1.3/PKG-INFO` & `streamlit-chitchat-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chitchat
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: k4144
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

