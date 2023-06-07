# Comparing `tmp/enalog-0.1.1.tar.gz` & `tmp/enalog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enalog-0.1.1.tar", max compression
+gzip compressed data, was "enalog-0.2.0.tar", max compression
```

## Comparing `enalog-0.1.1.tar` & `enalog-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      365 2023-03-05 10:16:40.183050 enalog-0.1.1/README.md
--rw-r--r--   0        0        0     1355 2023-03-05 10:16:40.183050 enalog-0.1.1/enalog/__init__.py
--rw-r--r--   0        0        0      444 2023-03-05 10:16:40.183050 enalog-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 enalog-0.1.1/setup.py
--rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 enalog-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      390 2023-06-07 08:42:38.480467 enalog-0.2.0/README.md
+-rw-r--r--   0        0        0     3768 2023-06-07 08:42:38.480467 enalog-0.2.0/enalog/__init__.py
+-rw-r--r--   0        0        0      444 2023-06-07 08:42:38.480467 enalog-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 enalog-0.2.0/setup.py
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 enalog-0.2.0/PKG-INFO
```

### Comparing `enalog-0.1.1/setup.py` & `enalog-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'enalog',
-    'version': '0.1.1',
+    'version': '0.2.0',
     'description': 'Python package for sending events to EnaLog',
-    'long_description': "# enalog-py\n\nPython library for sending events to EnaLog\n\n### Usage\n\n```python\nfrom enalog import push\n\npush_event(api_token='dummy_api_token', event={\n    'project': 'enalog'\n    'name': 'user-subscribed',\n    'description': 'User has subscribed to EnaLog',\n    'push': False,\n    'icon': '💰',\n    'tags': ['app': 'EnaLog'],\n    'meta': {'user_id': 123}\n})\n```\n",
+    'long_description': "# enalog-py\n\nEnaLog Python SDK\n\n### Usage\n\n```python\nfrom enalog import push\n\npush_event(api_token='dummy_api_token', event={\n    'project': 'enalog'\n    'name': 'user-subscribed',\n    'description': 'User has subscribed to EnaLog',\n    'push': False,\n    'icon': '💰',\n    'tags': ['app': 'EnaLog'],\n    'meta': {'user_id': 123},\n    'channels': {'slack': '<slack-channel-name>'}\n})\n```\n",
     'author': 'Sam Newby',
     'author_email': 'sam.newby19@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `enalog-0.1.1/PKG-INFO` & `enalog-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: enalog
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python package for sending events to EnaLog
 Author: Sam Newby
 Author-email: sam.newby19@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # enalog-py
 
-Python library for sending events to EnaLog
+EnaLog Python SDK
 
 ### Usage
 
 ```python
 from enalog import push
 
 push_event(api_token='dummy_api_token', event={
     'project': 'enalog'
     'name': 'user-subscribed',
     'description': 'User has subscribed to EnaLog',
     'push': False,
     'icon': '💰',
     'tags': ['app': 'EnaLog'],
-    'meta': {'user_id': 123}
+    'meta': {'user_id': 123},
+    'channels': {'slack': '<slack-channel-name>'}
 })
 ```
```

