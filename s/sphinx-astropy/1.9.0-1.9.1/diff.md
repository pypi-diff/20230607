# Comparing `tmp/sphinx-astropy-1.9.0.tar.gz` & `tmp/sphinx-astropy-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-astropy-1.9.0.tar", last modified: Tue Jun  6 21:56:28 2023, max compression
+gzip compressed data, was "sphinx-astropy-1.9.1.tar", last modified: Wed Jun  7 18:45:02 2023, max compression
```

## Comparing `sphinx-astropy-1.9.0.tar` & `sphinx-astropy-1.9.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.672796 sphinx-astropy-1.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.672796 sphinx-astropy-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/.github/workflows/python-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.672796 sphinx-astropy-1.9.0/sphinx_astropy/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/sphinx_astropy/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/conf/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/conf/v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/sphinx_astropy/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/ext/changelog_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/ext/edit_on_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/ext/generate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/ext/intersphinx_toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/ext/missing_static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/sphinx_astropy/local/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/local/python3_local_links.inv
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/local/python3_local_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.676796 sphinx-astropy-1.9.0/sphinx_astropy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/tests/test_conf_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/sphinx_astropy/tests/test_conf_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:56:28.672796 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 21:56:28.000000 sphinx-astropy-1.9.0/sphinx_astropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-06 21:56:14.000000 sphinx-astropy-1.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:45:02.600991 sphinx-astropy-1.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:45:02.588991 sphinx-astropy-1.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:45:02.592991 sphinx-astropy-1.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/.github/workflows/python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-07 18:45:02.600991 sphinx-astropy-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-07 18:45:02.600991 sphinx-astropy-1.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:45:02.592991 sphinx-astropy-1.9.1/sphinx_astropy/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:45:02.596991 sphinx-astropy-1.9.1/sphinx_astropy/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/conf/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/conf/v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:45:02.600991 sphinx-astropy-1.9.1/sphinx_astropy/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/ext/changelog_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/ext/edit_on_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/ext/generate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/ext/intersphinx_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/ext/missing_static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:45:02.600991 sphinx-astropy-1.9.1/sphinx_astropy/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/local/python3_local_links.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/local/python3_local_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:45:02.600991 sphinx-astropy-1.9.1/sphinx_astropy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/tests/test_conf_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/sphinx_astropy/tests/test_conf_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 18:45:02.000000 sphinx-astropy-1.9.1/sphinx_astropy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:45:02.596991 sphinx-astropy-1.9.1/sphinx_astropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-07 18:45:02.000000 sphinx-astropy-1.9.1/sphinx_astropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-07 18:45:02.000000 sphinx-astropy-1.9.1/sphinx_astropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:45:02.000000 sphinx-astropy-1.9.1/sphinx_astropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:45:02.000000 sphinx-astropy-1.9.1/sphinx_astropy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-07 18:45:02.000000 sphinx-astropy-1.9.1/sphinx_astropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 18:45:02.000000 sphinx-astropy-1.9.1/sphinx_astropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-07 18:44:45.000000 sphinx-astropy-1.9.1/tox.ini
```

### Comparing `sphinx-astropy-1.9.0/.github/workflows/publish.yml` & `sphinx-astropy-1.9.1/.github/workflows/publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - uses: actions/setup-python@v4
       with:
-        python-version: "3.11"
+        python-version: "3.8"
 
     - name: Install build dependencies
       run: python -m pip install pip build "twine>=3.3" -U
 
     - name: Build package
       run: python -m build --sdist --wheel .
```

### Comparing `sphinx-astropy-1.9.0/.github/workflows/python-tests.yml` & `sphinx-astropy-1.9.1/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/.gitignore` & `sphinx-astropy-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/CHANGES.rst` & `sphinx-astropy-1.9.1/CHANGES.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changes in sphinx-astropy
 =========================
 
+1.9.1 (2023-06-07)
+------------------
+
+- Renamed ``[v2]`` optional dependencies key to ``[confv2]``
+  to avoid triggering build error in Python 3.10 or earlier. [#63]
+
 1.9 (2023-06-06)
 ----------------
 
 - To switch to ``pydata-sphinx-theme``, use ``sphinx_astropy.conf.v2``
   and install the ``[v2]`` optional dependencies. [#59]
 
 - Update minimum required version of Sphinx to 3.0.0. [#57]
```

### Comparing `sphinx-astropy-1.9.0/LICENSE.rst` & `sphinx-astropy-1.9.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/PKG-INFO` & `sphinx-astropy-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sphinx-astropy
-Version: 1.9.0
+Version: 1.9.1
 Summary: Sphinx extensions and configuration specific to the Astropy project
 Home-page: https://github.com/astropy/sphinx-astropy
 Author: The Astropy Developers
 Author-email: astropy.team@gmail.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: v2
+Provides-Extra: confv2
 Provides-Extra: all
 Provides-Extra: tests
 License-File: LICENSE.rst
 
 About
 =====
 
@@ -66,21 +66,21 @@
 * `numpydoc <https://numpydoc.readthedocs.io>`_ - an extension to parse docstrings in NumpyDoc format
 
 * `pillow <https://pillow.readthedocs.io/en/latest/>`_ - a package to deal with
   images, used by some examples in the astropy core documentation.
 
 * `pytest-doctestplus <https://github.com/astropy/pytest-doctestplus/>`_ - providing the 'doctestplus' extension to skip code snippets in narrative documentation.
 
-pydata-sphinx-theme (v2)
-^^^^^^^^^^^^^^^^^^^^^^^^
+pydata-sphinx-theme (confv2)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 To use the new `pydata-sphinx-theme` with `sphinx_astropy.conf.v2`, you have to install
-the optional `[v2]` dependencies::
+the optional `[confv2]` dependencies::
 
-    pip install sphinx-astropy[v2]
+    pip install sphinx-astropy[confv2]
 
 That would pull in the following as well:
 
 * `pydata-sphinx-theme <https://github.com/pydata/pydata-sphinx-theme/>`_ - a clean, three-column,
   Bootstrap-based Sphinx theme by and for the `PyData community <https://pydata.org/>`_.
 
 * `sphinx-copybutton <https://github.com/executablebooks/sphinx-copybutton>`_ - a small Sphinx
```

### Comparing `sphinx-astropy-1.9.0/README.rst` & `sphinx-astropy-1.9.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -46,21 +46,21 @@
 * `numpydoc <https://numpydoc.readthedocs.io>`_ - an extension to parse docstrings in NumpyDoc format
 
 * `pillow <https://pillow.readthedocs.io/en/latest/>`_ - a package to deal with
   images, used by some examples in the astropy core documentation.
 
 * `pytest-doctestplus <https://github.com/astropy/pytest-doctestplus/>`_ - providing the 'doctestplus' extension to skip code snippets in narrative documentation.
 
-pydata-sphinx-theme (v2)
-^^^^^^^^^^^^^^^^^^^^^^^^
+pydata-sphinx-theme (confv2)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 To use the new `pydata-sphinx-theme` with `sphinx_astropy.conf.v2`, you have to install
-the optional `[v2]` dependencies::
+the optional `[confv2]` dependencies::
 
-    pip install sphinx-astropy[v2]
+    pip install sphinx-astropy[confv2]
 
 That would pull in the following as well:
 
 * `pydata-sphinx-theme <https://github.com/pydata/pydata-sphinx-theme/>`_ - a clean, three-column,
   Bootstrap-based Sphinx theme by and for the `PyData community <https://pydata.org/>`_.
 
 * `sphinx-copybutton <https://github.com/executablebooks/sphinx-copybutton>`_ - a small Sphinx
```

### Comparing `sphinx-astropy-1.9.0/setup.cfg` & `sphinx-astropy-1.9.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	sphinx-automodapi
 	sphinx-gallery
 	sphinxcontrib-jquery
 	pillow
 	pytest-doctestplus>=0.11
 
 [options.extras_require]
-v2 = 
+confv2 = 
 	pydata-sphinx-theme
 	sphinx-copybutton
 all = astropy
 tests = pytest
 
 [options.package_data]
 sphinx_astropy = local/*
```

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy/conf/__init__.py` & `sphinx-astropy-1.9.1/sphinx_astropy/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy/conf/v1.py` & `sphinx-astropy-1.9.1/sphinx_astropy/conf/v1.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy/conf/v2.py` & `sphinx-astropy-1.9.1/sphinx_astropy/conf/v2.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy/ext/changelog_links.py` & `sphinx-astropy-1.9.1/sphinx_astropy/ext/changelog_links.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy/ext/edit_on_github.py` & `sphinx-astropy-1.9.1/sphinx_astropy/ext/edit_on_github.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy/ext/generate_config.py` & `sphinx-astropy-1.9.1/sphinx_astropy/ext/generate_config.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy/ext/intersphinx_toggle.py` & `sphinx-astropy-1.9.1/sphinx_astropy/ext/intersphinx_toggle.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy/ext/missing_static.py` & `sphinx-astropy-1.9.1/sphinx_astropy/ext/missing_static.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy/local/python3_local_links.inv` & `sphinx-astropy-1.9.1/sphinx_astropy/local/python3_local_links.inv`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy/local/python3_local_links.txt` & `sphinx-astropy-1.9.1/sphinx_astropy/local/python3_local_links.txt`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy/tests/test_conf_v1.py` & `sphinx-astropy-1.9.1/sphinx_astropy/tests/test_conf_v1.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy/tests/test_conf_v2.py` & `sphinx-astropy-1.9.1/sphinx_astropy/tests/test_conf_v2.py`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy.egg-info/PKG-INFO` & `sphinx-astropy-1.9.1/sphinx_astropy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sphinx-astropy
-Version: 1.9.0
+Version: 1.9.1
 Summary: Sphinx extensions and configuration specific to the Astropy project
 Home-page: https://github.com/astropy/sphinx-astropy
 Author: The Astropy Developers
 Author-email: astropy.team@gmail.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: v2
+Provides-Extra: confv2
 Provides-Extra: all
 Provides-Extra: tests
 License-File: LICENSE.rst
 
 About
 =====
 
@@ -66,21 +66,21 @@
 * `numpydoc <https://numpydoc.readthedocs.io>`_ - an extension to parse docstrings in NumpyDoc format
 
 * `pillow <https://pillow.readthedocs.io/en/latest/>`_ - a package to deal with
   images, used by some examples in the astropy core documentation.
 
 * `pytest-doctestplus <https://github.com/astropy/pytest-doctestplus/>`_ - providing the 'doctestplus' extension to skip code snippets in narrative documentation.
 
-pydata-sphinx-theme (v2)
-^^^^^^^^^^^^^^^^^^^^^^^^
+pydata-sphinx-theme (confv2)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 To use the new `pydata-sphinx-theme` with `sphinx_astropy.conf.v2`, you have to install
-the optional `[v2]` dependencies::
+the optional `[confv2]` dependencies::
 
-    pip install sphinx-astropy[v2]
+    pip install sphinx-astropy[confv2]
 
 That would pull in the following as well:
 
 * `pydata-sphinx-theme <https://github.com/pydata/pydata-sphinx-theme/>`_ - a clean, three-column,
   Bootstrap-based Sphinx theme by and for the `PyData community <https://pydata.org/>`_.
 
 * `sphinx-copybutton <https://github.com/executablebooks/sphinx-copybutton>`_ - a small Sphinx
```

### Comparing `sphinx-astropy-1.9.0/sphinx_astropy.egg-info/SOURCES.txt` & `sphinx-astropy-1.9.1/sphinx_astropy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx-astropy-1.9.0/tox.ini` & `sphinx-astropy-1.9.1/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 isolated_build = true
 
 [testenv]
 changedir = .tmp/{envname}
 description = run tests
 extras =
     tests
-    v2deps: v2
+    v2deps: confv2
 deps =
     sphinx30: sphinx==3.0.*
     sphinx30: docutils==0.17.*
     sphinx30: Jinja2==3.0.3
     sphinx35: sphinx==3.5.*
     sphinx35: Jinja2==3.0.3
     sphinx40: sphinx==4.0.*
```

