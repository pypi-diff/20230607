# Comparing `tmp/pypi-packaging-tutorial-0.1.1.tar.gz` & `tmp/pypi-packaging-tutorial-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi-packaging-tutorial-0.1.1.tar", max compression
+gzip compressed data, was "pypi-packaging-tutorial-0.1.2.tar", max compression
```

## Comparing `pypi-packaging-tutorial-0.1.1.tar` & `pypi-packaging-tutorial-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1069 2023-06-07 10:45:19.492445 pypi-packaging-tutorial-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      261 2023-06-07 10:44:41.254558 pypi-packaging-tutorial-0.1.1/README.txt
--rw-r--r--   0        0        0        0 2023-06-07 10:04:15.445423 pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/divide/__init__.py
--rw-r--r--   0        0        0      164 2023-06-07 10:20:49.930464 pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/divide/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      287 2023-06-07 10:20:49.930464 pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/divide/__pycache__/divide_by_three.cpython-310.pyc
--rw-r--r--   0        0        0       41 2023-06-07 10:00:23.063639 pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/divide/divide_by_three.py
--rw-r--r--   0        0        0        0 2023-06-07 09:57:40.882397 pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/multiply/__init__.py
--rw-r--r--   0        0        0      166 2023-06-07 10:07:01.182699 pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/multiply/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      293 2023-06-07 10:07:01.182699 pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/multiply/__pycache__/multiply_by_three.cpython-310.pyc
--rw-r--r--   0        0        0       43 2023-06-07 10:00:36.095739 pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/multiply/multiply_by_three.py
--rw-r--r--   0        0        0     1677 2023-06-07 10:49:18.898287 pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/pypi_pyckyging_tutorial.egg-info/PKG-INFO
--rw-r--r--   0        0        0      425 2023-06-07 10:49:18.902287 pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/pypi_pyckyging_tutorial.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-06-07 10:49:18.898287 pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/pypi_pyckyging_tutorial.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       16 2023-06-07 10:49:18.898287 pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/pypi_pyckyging_tutorial.egg-info/top_level.txt
--rw-r--r--   0        0        0      739 2023-06-07 14:54:50.678063 pypi-packaging-tutorial-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 pypi-packaging-tutorial-0.1.1/setup.py
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 pypi-packaging-tutorial-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-07 10:45:19.492445 pypi-packaging-tutorial-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      261 2023-06-07 10:44:41.254558 pypi-packaging-tutorial-0.1.2/README.txt
+-rw-r--r--   0        0        0      148 2023-06-07 14:57:46.554211 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:04:15.445423 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/divide/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-07 10:20:49.930464 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/divide/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      287 2023-06-07 10:20:49.930464 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/divide/__pycache__/divide_by_three.cpython-310.pyc
+-rw-r--r--   0        0        0       41 2023-06-07 10:00:23.063639 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/divide/divide_by_three.py
+-rw-r--r--   0        0        0        0 2023-06-07 09:57:40.882397 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/multiply/__init__.py
+-rw-r--r--   0        0        0      166 2023-06-07 10:07:01.182699 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/multiply/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      293 2023-06-07 10:07:01.182699 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/multiply/__pycache__/multiply_by_three.cpython-310.pyc
+-rw-r--r--   0        0        0       43 2023-06-07 10:00:36.095739 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/multiply/multiply_by_three.py
+-rw-r--r--   0        0        0     1677 2023-06-07 10:49:18.898287 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/pypi_pyckyging_tutorial.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      425 2023-06-07 10:49:18.902287 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/pypi_pyckyging_tutorial.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-06-07 10:49:18.898287 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/pypi_pyckyging_tutorial.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       16 2023-06-07 10:49:18.898287 pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/pypi_pyckyging_tutorial.egg-info/top_level.txt
+-rw-r--r--   0        0        0      739 2023-06-07 14:59:45.266767 pypi-packaging-tutorial-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 pypi-packaging-tutorial-0.1.2/setup.py
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 pypi-packaging-tutorial-0.1.2/PKG-INFO
```

### Comparing `pypi-packaging-tutorial-0.1.1/LICENSE.txt` & `pypi-packaging-tutorial-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypi-packaging-tutorial-0.1.1/pypi_packaging_tutorial/pypi_pyckyging_tutorial.egg-info/PKG-INFO` & `pypi-packaging-tutorial-0.1.2/pypi_packaging_tutorial/pypi_pyckyging_tutorial.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pypi-packaging-tutorial-0.1.1/pyproject.toml` & `pypi-packaging-tutorial-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #[build-system]
 #requires = ['setuptools>=42']
 #build-backend = 'setuptools.build_meta'
 
 [tool.poetry]
 name = "pypi-packaging-tutorial"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.txt"
 packages = [{include = "pypi_packaging_tutorial"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pypi-packaging-tutorial-0.1.1/setup.py` & `pypi-packaging-tutorial-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  'pypi_packaging_tutorial.multiply']
 
 package_data = \
 {'': ['*'], 'pypi_packaging_tutorial': ['pypi_pyckyging_tutorial.egg-info/*']}
 
 setup_kwargs = {
     'name': 'pypi-packaging-tutorial',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': '`pypi_pyckaging_tutorial` provides a simple example to create your first Python package and upload it to pypi.\n\n\nexample usage:\nfrom multiply.by_three import multiply_by_three\nfrom divide.by_three import divide_by_three\n\nmultiply_by_three(9)\ndivide_by_three(21)',
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pypi-packaging-tutorial-0.1.1/PKG-INFO` & `pypi-packaging-tutorial-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-packaging-tutorial
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/plain
```

