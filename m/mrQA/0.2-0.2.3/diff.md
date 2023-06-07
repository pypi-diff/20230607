# Comparing `tmp/mrQA-0.2.tar.gz` & `tmp/mrQA-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrQA-0.2.tar", last modified: Wed Feb  1 21:06:41 2023, max compression
+gzip compressed data, was "mrQA-0.2.3.tar", last modified: Wed Jun  7 17:12:41 2023, max compression
```

## Comparing `mrQA-0.2.tar` & `mrQA-0.2.3.tar`

### file list

```diff
@@ -1,50 +1,63 @@
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-02-01 21:06:41.693433 mrQA-0.2/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      177 2022-11-07 22:31:28.000000 mrQA-0.2/AUTHORS.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     3491 2022-11-07 22:31:28.000000 mrQA-0.2/CONTRIBUTING.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       89 2022-11-07 22:31:28.000000 mrQA-0.2/HISTORY.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      583 2022-11-07 22:31:28.000000 mrQA-0.2/LICENSE
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      335 2022-11-07 22:31:28.000000 mrQA-0.2/MANIFEST.in
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1483 2023-02-01 21:06:41.693433 mrQA-0.2/PKG-INFO
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      641 2022-12-23 17:48:53.000000 mrQA-0.2/README.rst
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-02-01 21:06:41.693433 mrQA-0.2/docs/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      389 2022-12-19 21:59:18.000000 mrQA-0.2/docs/API.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      604 2022-11-07 22:31:28.000000 mrQA-0.2/docs/Makefile
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       28 2022-11-07 22:31:28.000000 mrQA-0.2/docs/authors.rst
--rwxrwxr-x   0 sinhah    (1000) sinhah    (1000)     4987 2022-11-07 22:31:28.000000 mrQA-0.2/docs/conf.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       33 2022-11-07 22:31:28.000000 mrQA-0.2/docs/contributing.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      316 2022-12-23 17:38:52.000000 mrQA-0.2/docs/index.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1114 2022-11-07 22:31:28.000000 mrQA-0.2/docs/installation.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      765 2022-11-07 22:31:28.000000 mrQA-0.2/docs/make.bat
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       27 2022-11-07 22:31:28.000000 mrQA-0.2/docs/readme.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      403 2022-12-23 17:48:53.000000 mrQA-0.2/docs/usage.rst
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-02-01 21:06:41.697433 mrQA-0.2/mrQA/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      336 2022-11-07 22:31:28.000000 mrQA-0.2/mrQA/__compliance__.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      239 2022-11-07 22:31:28.000000 mrQA-0.2/mrQA/__init__.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      495 2023-02-01 21:06:41.697433 mrQA-0.2/mrQA/_version.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     4502 2022-12-27 20:55:08.000000 mrQA-0.2/mrQA/cli.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      641 2022-11-07 22:31:28.000000 mrQA-0.2/mrQA/common.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1094 2022-12-19 21:59:18.000000 mrQA-0.2/mrQA/config.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     4092 2022-12-29 22:28:25.000000 mrQA-0.2/mrQA/formatter.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     9849 2022-12-24 14:30:36.000000 mrQA-0.2/mrQA/parallel_utils.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     4260 2022-12-29 22:26:03.000000 mrQA-0.2/mrQA/project.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     3933 2022-12-21 22:59:58.000000 mrQA-0.2/mrQA/run_merge.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     8646 2022-12-22 22:21:39.000000 mrQA-0.2/mrQA/run_parallel.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     3936 2022-12-21 21:56:31.000000 mrQA-0.2/mrQA/run_subset.py
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-02-01 21:06:41.693433 mrQA-0.2/mrQA/tests/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       34 2022-11-07 22:31:28.000000 mrQA-0.2/mrQA/tests/__init__.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      125 2022-11-07 22:31:28.000000 mrQA-0.2/mrQA/tests/config.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    11064 2022-12-21 22:34:18.000000 mrQA-0.2/mrQA/tests/test_compliance.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     5628 2022-12-27 15:42:11.000000 mrQA-0.2/mrQA/tests/test_parallel.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     6876 2022-12-26 18:08:29.000000 mrQA-0.2/mrQA/tests/test_utils.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    15916 2022-12-29 22:45:38.000000 mrQA-0.2/mrQA/utils.py
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-02-01 21:06:41.693433 mrQA-0.2/mrQA.egg-info/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1483 2023-02-01 21:06:41.000000 mrQA-0.2/mrQA.egg-info/PKG-INFO
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      817 2023-02-01 21:06:41.000000 mrQA-0.2/mrQA.egg-info/SOURCES.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        1 2023-02-01 21:06:41.000000 mrQA-0.2/mrQA.egg-info/dependency_links.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      120 2023-02-01 21:06:41.000000 mrQA-0.2/mrQA.egg-info/entry_points.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        1 2023-02-01 21:06:41.000000 mrQA-0.2/mrQA.egg-info/not-zip-safe
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       58 2023-02-01 21:06:41.000000 mrQA-0.2/mrQA.egg-info/requires.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        5 2023-02-01 21:06:41.000000 mrQA-0.2/mrQA.egg-info/top_level.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      575 2023-02-01 21:06:41.697433 mrQA-0.2/setup.cfg
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1760 2022-12-27 15:52:44.000000 mrQA-0.2/setup.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    81180 2022-11-07 22:31:28.000000 mrQA-0.2/versioneer.py
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:12:41.617409 mrQA-0.2.3/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      170 2023-06-07 17:11:42.000000 mrQA-0.2.3/AUTHORS.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     3491 2022-11-07 22:31:28.000000 mrQA-0.2.3/CONTRIBUTING.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       89 2022-11-07 22:31:28.000000 mrQA-0.2.3/HISTORY.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      583 2022-11-07 22:31:28.000000 mrQA-0.2.3/LICENSE
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      335 2022-11-07 22:31:28.000000 mrQA-0.2.3/MANIFEST.in
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     2403 2023-06-07 17:12:41.617409 mrQA-0.2.3/PKG-INFO
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1559 2023-06-07 17:11:42.000000 mrQA-0.2.3/README.rst
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:12:41.617409 mrQA-0.2.3/docs/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      496 2023-06-07 17:11:42.000000 mrQA-0.2.3/docs/API.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      604 2022-11-07 22:31:28.000000 mrQA-0.2.3/docs/Makefile
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       28 2022-11-07 22:31:28.000000 mrQA-0.2.3/docs/authors.rst
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:12:41.613409 mrQA-0.2.3/docs/build/
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:12:41.613409 mrQA-0.2.3/docs/build/html/
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:12:41.617409 mrQA-0.2.3/docs/build/html/_images/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)   144544 2023-03-13 20:29:31.000000 mrQA-0.2.3/docs/build/html/_images/schematic_mrQA.png
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:12:41.617409 mrQA-0.2.3/docs/build/html/_static/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      286 2022-07-14 07:38:19.000000 mrQA-0.2.3/docs/build/html/_static/file.png
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       90 2022-07-14 07:38:19.000000 mrQA-0.2.3/docs/build/html/_static/minus.png
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       90 2022-07-14 07:38:19.000000 mrQA-0.2.3/docs/build/html/_static/plus.png
+-rwxrwxr-x   0 sinhah    (1000) sinhah    (1000)     4987 2023-06-07 17:11:42.000000 mrQA-0.2.3/docs/conf.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       33 2022-11-07 22:31:28.000000 mrQA-0.2.3/docs/contributing.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     8176 2023-06-07 17:11:42.000000 mrQA-0.2.3/docs/examples.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1818 2023-06-07 17:11:42.000000 mrQA-0.2.3/docs/index.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1114 2022-11-07 22:31:28.000000 mrQA-0.2.3/docs/installation.rst
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      765 2022-11-07 22:31:28.000000 mrQA-0.2.3/docs/make.bat
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)   144544 2023-06-07 17:11:42.000000 mrQA-0.2.3/docs/schematic_mrQA.png
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      831 2023-06-07 17:11:42.000000 mrQA-0.2.3/docs/usage.rst
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:12:41.621409 mrQA-0.2.3/mrQA/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      336 2022-11-07 22:31:28.000000 mrQA-0.2.3/mrQA/__compliance__.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      272 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/__init__.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      497 2023-06-07 17:12:41.621409 mrQA-0.2.3/mrQA/_version.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     5204 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/cli.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      451 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/common.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     2552 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/config.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     4150 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/formatter.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     7852 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/monitor.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     9861 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/parallel_utils.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     6481 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/project.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     3987 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/run_merge.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    13002 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/run_parallel.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     4148 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/run_subset.py
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:12:41.617409 mrQA-0.2.3/mrQA/tests/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       34 2022-11-07 22:31:28.000000 mrQA-0.2.3/mrQA/tests/__init__.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1097 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/tests/config.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      141 2023-02-22 17:41:50.000000 mrQA-0.2.3/mrQA/tests/conftest.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    11070 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/tests/test_compliance.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     7155 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/tests/test_monitor.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     5688 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/tests/test_parallel.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     8959 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/tests/unit_tests.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     4336 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/tests/utils.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    30481 2023-06-07 17:11:42.000000 mrQA-0.2.3/mrQA/utils.py
+drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:12:41.617409 mrQA-0.2.3/mrQA.egg-info/
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     2403 2023-06-07 17:12:41.000000 mrQA-0.2.3/mrQA.egg-info/PKG-INFO
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1072 2023-06-07 17:12:41.000000 mrQA-0.2.3/mrQA.egg-info/SOURCES.txt
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        1 2023-06-07 17:12:41.000000 mrQA-0.2.3/mrQA.egg-info/dependency_links.txt
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      146 2023-06-07 17:12:41.000000 mrQA-0.2.3/mrQA.egg-info/entry_points.txt
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        1 2023-06-07 17:12:41.000000 mrQA-0.2.3/mrQA.egg-info/not-zip-safe
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       51 2023-06-07 17:12:41.000000 mrQA-0.2.3/mrQA.egg-info/requires.txt
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        5 2023-06-07 17:12:41.000000 mrQA-0.2.3/mrQA.egg-info/top_level.txt
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      575 2023-06-07 17:12:41.621409 mrQA-0.2.3/setup.cfg
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1792 2023-06-07 17:11:42.000000 mrQA-0.2.3/setup.py
+-rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    81180 2023-03-16 21:25:02.000000 mrQA-0.2.3/versioneer.py
```

### Comparing `mrQA-0.2/CONTRIBUTING.rst` & `mrQA-0.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mrQA-0.2/LICENSE` & `mrQA-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mrQA-0.2/docs/Makefile` & `mrQA-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mrQA-0.2/docs/conf.py` & `mrQA-0.2.3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'mrQA'
-copyright = "2022, Harsh Sinha"
+copyright = "2023, Harsh Sinha"
 author = "Harsh Sinha"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
@@ -63,15 +63,15 @@
 release = mrQA.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `mrQA-0.2/docs/installation.rst` & `mrQA-0.2.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mrQA-0.2/docs/make.bat` & `mrQA-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mrQA-0.2/mrQA/formatter.py` & `mrQA-0.2.3/mrQA/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,16 @@
         template_env = jinja2.Environment(loader=fs_loader, extensions=extn)
 
         template_file = "templates/layout.html"
         template = template_env.get_template(template_file)
 
         output_text = template.render(
             dataset=self.params['ds'],
-            subject_list=self.params['subject_list'],
+            sub_lists_by_modality=self.params['sub_lists_by_modality'],
+            # time=self.params['time'],
             imp0rt=importlib.import_module
         )
         # self.output = weasyprint.HTML(string=output_text)
         f = open(self.filepath, 'w')
         f.write(output_text)
```

### Comparing `mrQA-0.2/mrQA/parallel_utils.py` & `mrQA-0.2.3/mrQA/parallel_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,68 +6,69 @@
 
 from MRdataset.log import logger
 from MRdataset.utils import valid_dirs
 
 from mrQA.utils import is_integer_number, execute_local, list2txt
 
 
-def _check_args(data_source_folders: Union[str, Path, Iterable] = None,
-                style: str = 'dicom',
+def _check_args(data_source: Union[str, Path, Iterable] = None,
+                ds_format: str = 'dicom',
                 output_dir: Union[str, Path] = None,
                 debug: bool = False,
                 subjects_per_job: int = None,
                 hpc: bool = False,
                 conda_dist: str = None,
                 conda_env: str = None):
     # It is not possible to submit jobs while debugging, why would you submit
     # a job, if code is still being debugged
     if debug and hpc:
         raise AttributeError('Dont debug on hpc!')
-    if style != 'dicom':
-        raise NotImplementedError(f'Expects dicom, Got {style}')
+    if ds_format != 'dicom':
+        raise NotImplementedError(f'Expects dicom, Got {ds_format}')
     if not is_integer_number(subjects_per_job):
         raise RuntimeError('Expects an integer value for subjects per job.'
                            f'Got {subjects_per_job}')
     if subjects_per_job < 1:
         raise RuntimeError('subjects_per_job cannot be less than 1')
 
-    # Check if data_root is a valid directory, or list of valid directories
-    data_source_folders = valid_dirs(data_source_folders)
+    # Check if data_source is a valid directory, or list of valid directories
+    data_source = valid_dirs(data_source)
 
     # RULE : If output_dir not provided, output wil be saved in 'mrqa_files'
-    # created in the parent folder of data_root
+    # created in the parent folder of data_source
     if not output_dir:
-        if isinstance(data_source_folders, Iterable):
-            # If data_root is a bunch of directories, the above RULE cannot
+        if isinstance(data_source, Iterable):
+            # If data_source is a bunch of directories, the above RULE cannot
             # be followed, just pass a directory to save the file.
-            raise RuntimeError("Need an output directory to store files")
+            raise RuntimeError('Need an output directory to store files')
 
         # Didn't find a good alternative to os.access
         # in pathlib, please raise a issue if you know one, happy to incorporate
-        output_dir = data_source_folders.parent / (
-            data_source_folders.name + '_mrqa_files')
+        output_dir = data_source.parent / (
+            data_source.name + '_mrqa_files')
 
-        # Check if permission to create a folder in data_root.parent
-        if os.access(data_source_folders.parent, os.W_OK):
+        # Check if permission to create a folder in data_source.parent
+        if os.access(data_source.parent, os.W_OK):
             logger.warning('Expected a directory to save job scripts. Using '
-                           'parent folder of --data_root instead.')
+                           'parent folder of --data_source instead.')
         else:
             raise PermissionError(f'You do not have write permission to'
                                   f'create a folder in '
-                                  f'{data_source_folders.parent}'
+                                  f'{data_source.parent}'
                                   f'Please provide output_dir')
-
+    else:
+        output_dir = Path(output_dir)
     # Information about conda env is required for creating slurm scripts
     # The snippet below sets some defaults, may not be true for everyone.
     # The user can use the arguments to specify
     if not conda_env:
         conda_env = 'mrqa' if hpc else 'mrcheck'
     if not conda_dist:
         conda_dist = 'miniconda3' if hpc else 'anaconda3'
-    return data_source_folders, output_dir, conda_env, conda_dist
+    return data_source, output_dir, conda_env, conda_dist
 
 
 def _make_file_folders(output_dir):
     output_dir.mkdir(parents=True, exist_ok=True)
     # Create a folder id_lists for saving list of subject ids for each job
     # in a separate txt file.
     # Create a folder bash_scripts for saving bash_script for each job
@@ -112,27 +113,28 @@
     if isinstance(output_mrds_path, str):
         output_mrds_path = Path(output_mrds_path)
 
     if not output_mrds_path.exists():
         if hpc:
             # If running on a hpc, use the sbatch command
             # to submit the script
-            out = subprocess.Popen(['sbatch', script_path])
+            # TODO: Add try/except block here
+            subprocess.run(['sbatch', script_path], check=True, shell=True)
             # print(out.stdout)
             # some way to check was submitted/accepted
 
         else:
             # If running locally, and the user does not want to
             # submit the job, run the script using the bash command
             execute_local(script_path)
             # check successful completion, or log error
 
     else:
-        logger.warning(f"{output_mrds_path} already exists, skipping. "
-                       f" Use 'sbatch {script_path} to overwrite")
+        logger.warning('%s already exists, skipping.  Use sbatch %s to'
+                       ' overwrite', output_mrds_path, script_path)
 
 
 def _create_slurm_script(output_script_path: Union[str, Path],
                          ids_filepath: Union[str, Path],
                          env: str = 'mrqa',
                          conda_dist: str = 'anaconda3',
                          num_subj_per_job: int = 50,
@@ -156,18 +158,14 @@
         Number of subjects to process in each slurm job
     verbose : bool
         If True, prints the output of the script
     include_phantom : bool
         If True, includes phantom, localizer and calibration studies
     output_mrds_path : str
         Path to the partial mrds pickle file
-
-    Returns
-    -------
-    None
     """
 
     # Memory and CPU time :  typical usage observed locally
 
     # For subjects_per_job = 50             100
     # Max RSS Size (Memory) ~150 MB,        ~160 MB
     # Sys Time (CPU Time) : 10 minutes      20 minutes
@@ -185,16 +183,16 @@
     if verbose:
         python_cmd += ' --verbose'
     if include_phantom:
         python_cmd += ' --include_phantom'
     python_cmd += ' --is_partial'
 
     # Create the slurm script file
-    with open(output_script_path, 'w') as fp:
-        fp.writelines("\n".join([
+    with open(output_script_path, 'w', encoding='utf-8') as fp:
+        fp.writelines('\n'.join([
             '#!/bin/bash',
             '#SBATCH -A med220005p',
             '#SBATCH -N 1',
             '#SBATCH -p RM-shared',
             f'#SBATCH --mem-per-cpu={mem_reqd}M #memory per cpu-core',
             f'#SBATCH --time={time_limit}:00:00',
             '#SBATCH --ntasks-per-node=1',
@@ -213,49 +211,49 @@
         )
 
 
 def _get_num_workers(subjects_per_job, subject_list):
     if subjects_per_job > len(subject_list):
         # If subjects_per_job is greater than the number of subjects,
         # process all subjects in a single job. Stop execution.
-        raise RuntimeError("Trying to create more jobs than total number of "
-                           "subjects in the directory. Why?")
+        raise RuntimeError('Trying to create more jobs than total number of '
+                           'subjects in the directory. Why?')
 
     # Get the number of jobs
     workers = len(subject_list) // subjects_per_job
     if workers == 1:
         # If there is only one job, process all subjects in a single job
-        raise RuntimeError("Decrease number of subjects per job. Expected"
-                           "workers > 1 for parallel processing. Got 1")
+        raise RuntimeError('Decrease number of subjects per job. Expected'
+                           'workers > 1 for parallel processing. Got 1')
 
     return workers
 
 
-def _get_subject_ids(data_source_folders: Union[str, Path],
+def _get_subject_ids(data_source: Union[str, Path],
                      all_ids_path: Union[str, Path]) -> list:
     """
     Get the list of subject ids from the data source folder
 
     Parameters
     ----------
-    data_source_folders : Union[str, Path]
+    data_source : Union[str, Path]
         Path to the root directory of the data
     all_ids_path : Union[str, Path]
         Path to the output directory
 
     Returns
     -------
     subject_list : list
         List of subject ids
     """
     subject_list = []
     # Get the list of subject ids
-    for root, dirs, files in os.walk(data_source_folders):
+    for root, _, _ in os.walk(data_source):
         if 'sub-' in Path(root).name:
             # Get the subject id
-            num_files_in_root =  len(list(Path(root).rglob('*/*')))
+            num_files_in_root = len(list(Path(root).rglob('*/*')))
             if num_files_in_root > 0:
                 subject_list.append(root)
     # Store the list of unique subject ids to a text file given by
     # output_path
     list2txt(all_ids_path, list(set(subject_list)))
     return subject_list
```

### Comparing `mrQA-0.2/mrQA/project.py` & `mrQA-0.2.3/mrQA/project.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,182 @@
 from pathlib import Path
 from typing import Union
 
+from MRdataset import save_mr_dataset
 from MRdataset.base import BaseDataset
+from MRdataset.log import logger
+from MRdataset.config import DatasetEmptyException
 
 from mrQA.config import STRATEGIES_ALLOWED
 from mrQA.formatter import HtmlFormatter
-from mrQA.utils import timestamp, majority_attribute_values, _get_runs_by_echo, \
-    _check_against_reference, _cli_report, _validate_reference, subject_list2txt
+from mrQA.utils import majority_attribute_values, _get_runs_by_echo, \
+    _check_against_reference, _cli_report, _validate_reference, \
+    export_subject_lists, record_out_paths
 
 
 def check_compliance(dataset: BaseDataset,
                      strategy: str = 'majority',
                      decimals: int = 3,
-                     output_dir: Union[Path, str] = None):
+                     output_dir: Union[Path, str] = None,
+                     verbose: bool = False,
+                     tolerance: float = 0.1,) -> Path:
     """
     Main function for checking compliance. Infers the reference protocol
     according to the user chosen strategy, and then generates a compliance
     report
 
     Parameters
     ----------
     dataset : BaseDataset
         BaseDataset instance for the dataset to be checked for compliance
-
     strategy : str
         Strategy employed to specify or automatically infer the
         reference protocol. Allowed options are 'majority'
-
     output_dir: Union[Path, str]
         Path to save the report
+    decimals : int
+        Number of decimal places to round to (default:3).
+    verbose : bool
+        print more if true
+    tolerance : float
+        Tolerance for checking against reference protocol. Default is 0.1
 
     Returns
     -------
-    None
+    report_path : Path
+        Path to the generated report
 
     Raises
     ------
     ValueError
         If the input dataset is empty or otherwise invalid
-
+    NotImplementedError
+        If the input strategy is not supported
+    NotADirectoryError
+        If the output directory doesn't exist
     """
+    if verbose:
+        logger.setLevel('INFO')
+    else:
+        logger.setLevel('WARNING')
 
     if not dataset.modalities:
-        raise ValueError("Dataset is empty.")
+        raise DatasetEmptyException
 
     if strategy == 'majority':
-        dataset = compare_with_majority(dataset, decimals)
+        dataset = compare_with_majority(dataset, decimals, tolerance=tolerance)
     else:
         raise NotImplementedError(
-            'Only the following strategies are allowed : \n\t'
-            '{}'.format(STRATEGIES_ALLOWED))
+            f'Only the following strategies are allowed : \n\t'
+            f'{STRATEGIES_ALLOWED}')
 
-    report_path = generate_report(dataset, output_dir)
+    output_dir = Path(output_dir).resolve()
+    output_dir.mkdir(exist_ok=True, parents=True)
+    if not output_dir.is_dir():
+        raise NotADirectoryError('Provide a valid output directory')
+
+    report_path, mrds_path, sub_lists_dir_path = record_out_paths(output_dir,
+                                                                  dataset.name)
+    save_mr_dataset(mrds_path, dataset)
+    generate_report(dataset,
+                    report_path,
+                    sub_lists_dir_path,
+                    output_dir)
+
+    # Print a small message on the console, about non-compliance of dataset
+    print(_cli_report(dataset, str(report_path)))
     return report_path
 
 
-def compare_with_majority(dataset: "BaseDataset",
-                          decimals: int = 3) -> BaseDataset:
+def compare_with_majority(dataset: BaseDataset,
+                          decimals: int = 3,
+                          tolerance: float = 0.1) -> BaseDataset:
     """
     Method for post-acquisition compliance. Infers the reference protocol/values
     by looking for the most frequent values, and then identifying deviations
 
     Parameters
     ----------
     dataset : BaseDataset
         BaseDataset instance for the dataset which is to be checked
         for compliance
+    decimals : int
+        Number of decimal places to round to (default:3).
+    tolerance : float
+        Tolerance for checking against reference protocol. Default is 0.1
 
     Returns
     -------
     dataset : BaseDataset
         Adds the non-compliance information to the same BaseDataset instance and
         returns it.
     """
     # TODO: Check for subset, if incomplete dataset throw error and stop
 
     for modality in dataset.modalities:
+        # Reset compliance calculation before re-computing it.
+        modality.reset_compliance()
+
         # Infer reference protocol for each echo_time
+        # TODO: segregation via echo_time should be deprecated as multiple TE is
+        #   part of the same run
         run_by_echo = _get_runs_by_echo(modality, decimals)
 
         # For each echo time, find the most common values
-        for echo_time in run_by_echo.keys():
-            reference = majority_attribute_values(run_by_echo[echo_time])
+        for echo_time, run_list in run_by_echo.items():
+            reference = majority_attribute_values(run_list, echo_time)
             if _validate_reference(reference):
                 modality.set_reference(reference, echo_time)
 
-        modality.compliant = _check_against_reference(modality, decimals)
+        modality = _check_against_reference(modality, decimals,
+                                            tolerance=tolerance)
         if modality.compliant:
             dataset.add_compliant_modality_name(modality.name)
-
+        else:
+            dataset.add_non_compliant_modality_name(modality.name)
     # As we are updating the same dataset by adding non-compliant subject names,
     # and non-compliant modality names, we can return the same dataset
     return dataset
 
 
-def generate_report(dataset: BaseDataset, output_dir: Union[Path, str]):
+def generate_report(dataset: BaseDataset,
+                    report_path: str or Path,
+                    sub_lists_dir_path: str,
+                    output_dir: Union[Path, str]) -> Path:
     """
     Generates an HTML report aggregating and summarizing the non-compliance
     discovered in the dataset.
 
     Parameters
     ----------
     dataset : BaseDataset
         BaseDataset instance for the dataset which is to be checked
+    report_path : str
+        Name of the file to be generated, without extension. Ensures that
+        naming is consistent across the report, dataset and record files
+    sub_lists_dir_path : str
+        Path to the directory in which the subject lists should be stored
     output_dir : Union[Path, str]
         Directory in which the generated report should be stored.
+
+    Returns
+    -------
+    output_path : Path
+        Path to the generated report
+
     """
     output_dir = Path(output_dir).resolve()
     output_dir.mkdir(parents=True, exist_ok=True)
 
-    if not Path(output_dir).is_dir():
-        raise OSError('Expected valid output_directory, '
-                      'Got {0}'.format(output_dir))
-    filename = '{}_{}.html'.format(dataset.name, timestamp())
+    # time_dict = get_timestamps()
+    sub_lists_by_modality = export_subject_lists(output_dir,
+                                                 dataset,
+                                                 sub_lists_dir_path)
+    # export_record(output_dir, filename, time_dict)
     # Generate the HTML report and save it to the output_path
-    output_path = output_dir / filename
-    subject_list_dir = output_dir / 'subject_lists'
-    subjectlist_files = subject_list2txt(dataset, subject_list_dir)
     args = {
         'ds': dataset,
-        'subject_list': subjectlist_files
+        'sub_lists_by_modality': sub_lists_by_modality,
+        # 'time': time_dict
     }
-    HtmlFormatter(filepath=output_path, params=args)
-    # Print a small message on the console, about non-compliance of dataset
-    print(_cli_report(dataset, str(output_path)))
-    return output_path
-
-
-
+    HtmlFormatter(filepath=report_path, params=args)
+    return Path(report_path)
```

### Comparing `mrQA-0.2/mrQA/run_merge.py` & `mrQA-0.2.3/mrQA/run_merge.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+""" Script to merge partial mrds files into a single mrds file after
+parallel processing"""
 from pathlib import Path
 from typing import List, Union
 
 from MRdataset import load_mr_dataset
 from MRdataset import save_mr_dataset
 from MRdataset.base import BaseDataset
-from MRdataset.config import MRDS_EXT
 
 from mrQA.utils import txt2list
 
 
 def _check_partial_datasets(mrds_list_filepath: str) -> List[Path]:
     """
     Given a list of paths, check if all of them are valid and all of them
```

### Comparing `mrQA-0.2/mrQA/run_parallel.py` & `mrQA-0.2.3/mrQA/run_parallel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,201 @@
+""" This module contains functions to run the compliance checks in parallel"""
+import argparse
+import sys
 import time
 from pathlib import Path
-from typing import Iterable, Union, List
+from typing import Iterable, Union
 
+from MRdataset import load_mr_dataset
 from MRdataset.config import MRDS_EXT
-from MRdataset.utils import valid_paths
+from MRdataset.log import logger
+from MRdataset.utils import valid_paths, is_writable
 
+from mrQA.config import PATH_CONFIG
 from mrQA.parallel_utils import _check_args, _make_file_folders, \
     _run_single_batch, _create_slurm_script, _get_num_workers, _get_subject_ids
 from mrQA.run_merge import check_and_merge
 from mrQA.utils import list2txt, split_list, \
     txt2list
+from mrQA import check_compliance
 
 
-def process_parallel(data_root,
-                     output_dir,
-                     output_path,
-                     name=None):
+def get_parser():
+    parser = argparse.ArgumentParser(
+        description='Parallelize the mrQA compliance checks',
+        add_help=False
+    )
+
+    required = parser.add_argument_group('required arguments')
+    optional = parser.add_argument_group('optional arguments')
+
+    # Add help
+    optional.add_argument('-h', '--help', action='help',
+                          help='show this help message and exit')
+    required.add_argument('-d', '--data-source', type=str, required=True,
+                          help='directory containing downloaded dataset with '
+                               'dicom files, supports nested hierarchies')
+    optional.add_argument('-o', '--output-dir', type=str,
+                          help='specify the directory where the report'
+                               ' would be saved. By default, the --data_source '
+                               'directory will be used to save reports')
+    optional.add_argument('-p', '--out-mrds-path', type=str,
+                          help='specify the path to the output mrds file. ')
+    optional.add_argument('-n', '--name', type=str,
+                          help='provide a identifier/name for the dataset')
+    optional.add_argument('-s', '--subjects-per-job', type=int, default=5,
+                          help='number of subjects to process per job')
+    optional.add_argument('-e', '--conda-env', type=str, default='mrcheck',
+                          help='name of conda environment to use')
+    optional.add_argument('-c', '--conda-dist', type=str, default='anaconda3',
+                          help='name of conda distribution to use')
+    optional.add_argument('-H', '--hpc', action='store_true',
+                          help='flag to run on HPC')
+    optional.add_argument('-v', '--verbose', action='store_true',
+                          help='allow verbose output on console')
+    if len(sys.argv) < 2:
+        logger.critical('Too few arguments!')
+        parser.print_help()
+        parser.exit(1)
+
+    return parser
+
+
+def main():
+    args = parse_args()
+    process_parallel(data_source=args.data_source,
+                     output_dir=args.output_dir,
+                     out_mrds_path=args.out_mrds_path,
+                     name=args.name,
+                     subjects_per_job=args.subjects_per_job,
+                     conda_env=args.conda_env,
+                     conda_dist=args.conda_dist,
+                     hpc=args.hpc)
+    dataset = load_mr_dataset(args.out_mrds_path)
+    check_compliance(dataset=dataset,
+                     output_dir=args.output_dir)
+
+
+def parse_args():
+    parser = get_parser()
+    args = parser.parse_args()
+
+    if args.verbose:
+        logger.setLevel('INFO')
+    else:
+        logger.setLevel('WARNING')
+
+    if args.output_dir is None:
+        logger.info('Use --output-dir to specify dir for final directory. '
+                    'Using default')
+        args.output_dir = PATH_CONFIG['output_dir'] / args.name.lower()
+    else:
+        if not Path(args.output_dir).is_dir():
+            try:
+                Path(args.output_dir).mkdir(parents=True, exist_ok=True)
+            except OSError as exc:
+                raise exc
+
+    if not is_writable(args.output_dir):
+        raise OSError(f'Output Folder {args.output_dir} is not writable')
+    return args
+
+
+def process_parallel(data_source: Union[str, Path],
+                     output_dir: Union[str, Path],
+                     out_mrds_path: Union[str, Path],
+                     name: str = None,
+                     subjects_per_job: int = 5,
+                     conda_env: str = 'mrcheck',
+                     conda_dist: str = 'anaconda3',
+                     hpc: bool = False):
+    """
+    Given a folder(or List[folder]) it will divide the work into smaller
+    jobs. Each job will contain a fixed number of subjects. These jobs can be
+    executed in parallel to save time.
+
+    Parameters
+    ----------
+    data_source: str or Path
+        Path to the folder containing the subject folders
+    output_dir: str or Path
+        Path to the folder where the output will be saved
+    out_mrds_path: str or Path
+        Path to the final output mrds file
+    name: str
+        Name of the final output file
+    subjects_per_job: int
+        Number of subjects to be processed in each job
+    conda_env: str
+        Name of the conda environment to be used
+    conda_dist: str
+        Name of the conda distribution to be used
+    hpc: bool
+        Whether to use HPC or not
+    """
     # One function to process them all!
     # note that it will generate scripts only
     script_list_filepath, mrds_list_filepath = create_script(
-                                                data_source_folders=data_root,
-                                                subjects_per_job=5,
-                                                conda_env='mrcheck',
-                                                conda_dist='anaconda3',
-                                                output_dir=output_dir,
-                                                hpc=False,
-                                                )
+        data_source=data_source,
+        subjects_per_job=subjects_per_job,
+        conda_env=conda_env,
+        conda_dist=conda_dist,
+        output_dir=output_dir,
+        hpc=hpc,
+    )
     # Generate slurm scripts and submit jobs, for local parallel processing
     submit_job(scripts_list_filepath=script_list_filepath,
                mrds_list_filepath=mrds_list_filepath,
-               hpc=False)
+               hpc=hpc)
 
     # wait until processing completes
-    mrds_files = valid_paths(txt2list(mrds_list_filepath))
+    mrds_files = txt2list(mrds_list_filepath)
     for file in mrds_files:
-        while not file.exists():
+        while not Path(file).exists():
             time.sleep(100)
 
     check_and_merge(
         mrds_list_filepath=mrds_list_filepath,
-        output_path=output_path,
+        output_path=out_mrds_path,
         name=name
     )
 
 
 def submit_job(scripts_list_filepath: Union[str, Path],
                mrds_list_filepath: Union[str, Path],
-               debug: bool = False,
                hpc: bool = False) -> None:
     """
     Given a folder(or List[folder]) it will divide the work into smaller
     jobs. Each job will contain a fixed number of subjects. These jobs can be
     executed in parallel to save time.
 
     Parameters
     ----------
     scripts_list_filepath: str
         Path to the file containing list of bash scripts to be executed
     mrds_list_filepath: str
         Path to the file containing list of partial mrds files to be created
-    debug: bool
-        If True, the dataset will be created locally. This is useful for testing
     hpc: bool
         If True, the scripts will be generated for HPC, not for local execution
     Returns
     -------
     None
     """
 
-    processes = []
     bash_scripts = valid_paths(txt2list(scripts_list_filepath))
     mrds_files = txt2list(mrds_list_filepath)
     for script_path, output_mrds_path in zip(bash_scripts, mrds_files):
         # Run the script file
         _run_single_batch(script_path=script_path,
-                                   hpc=hpc,
-                                   output_mrds_path=output_mrds_path)
+                          hpc=hpc,
+                          output_mrds_path=output_mrds_path)
 
 
-def create_script(data_source_folders: Union[str, Path, Iterable] = None,
-                  style: str = 'dicom',
+def create_script(data_source: Union[str, Path, Iterable] = None,
+                  ds_format: str = 'dicom',
                   include_phantom: bool = False,
                   verbose: bool = False,
                   output_dir: Union[str, Path] = None,
                   debug: bool = False,
                   subjects_per_job: int = None,
                   hpc: bool = False,
                   conda_dist: str = None,
@@ -91,17 +203,17 @@
     """
     Given a folder(or List[folder]) it will divide the work into smaller
     jobs. Each job will contain a fixed number of subjects. These jobs can be
     executed in parallel to save time.
 
     Parameters
     ----------
-    data_source_folders: str or List[str]
+    data_source: str or List[str]
         /path/to/my/dataset containing files
-    style: str
+    ds_format: str
         Specify dataset type. Use one of [dicom]
     include_phantom: bool
         Include phantom scans in the dataset
     verbose: bool
         Print progress
     output_dir: str
         Path to save the output dataset
@@ -113,15 +225,15 @@
         If True, the scripts will be generated for HPC, not for local execution
     conda_dist: str
         Name of conda distribution
     conda_env: str
         Name of conda environment
     """
 
-    data_src, output_dir, env, dist = _check_args(data_source_folders, style,
+    data_src, output_dir, env, dist = _check_args(data_source, ds_format,
                                                   output_dir, debug,
                                                   subjects_per_job, hpc,
                                                   conda_dist, conda_env)
     folder_paths, files_per_batch, all_ids_path = _make_file_folders(output_dir)
     ids_path_list = split_ids_list(
         data_src,
         all_ids_path=all_ids_path,
@@ -156,35 +268,39 @@
                              num_subj_per_job=subjects_per_job,
                              verbose=verbose,
                              include_phantom=include_phantom,
                              output_mrds_path=partial_mrds_filepath)
 
     # Finally, save the all the paths to create mrds pickle files and all the
     # paths to generated scripts in a text file for reference.
-    list2txt(path=files_per_batch['mrds'], list_=mrds_path_list)
-    list2txt(path=files_per_batch['scripts'], list_=scripts_path_list)
+    list2txt(fpath=files_per_batch['mrds'], list_=mrds_path_list)
+    list2txt(fpath=files_per_batch['scripts'], list_=scripts_path_list)
     return files_per_batch['scripts'], files_per_batch['mrds']
 
 
-def split_ids_list(data_source_folders: Union[str, Path],
+def split_ids_list(data_source: Union[str, Path],
                    all_ids_path: Union[str, Path],
-                   per_batch_ids,
+                   per_batch_ids: Union[str, Path],
                    output_dir: Union[str, Path],
                    subjects_per_job: int = 50):
     """
     Splits a given set of subjects into multiple jobs and creates separate
     text files containing the list of subjects. Each text file
     contains the list of subjects to be processed in a single job.
 
     Parameters
     ----------
-    data_source_folders : Union[str, Path]
+    data_source : Union[str, Path]
         Path to the root directory of the data
     all_ids_path : Union[str, Path]
         Path to the output directory
+    per_batch_ids : Union[str, Path]
+        filepath to a file which has paths to all txt files for all jobs.
+        Each of these txt files contains a list of subject ids for
+        corresponding job.
     output_dir : Union[str, Path]
         Name of the output directory
     subjects_per_job : int
         Number of subjects to process in each job
 
     Returns
     -------
@@ -193,25 +309,23 @@
     """
 
     all_ids_path = Path(all_ids_path)
     # List of paths to the txt files,
     # each containing the list of subjects per job
     batch_ids_path_list = []
 
-    subject_list = _get_subject_ids(data_source_folders, all_ids_path)
+    subject_list = _get_subject_ids(data_source, all_ids_path)
     # Get the list of subjects for each job
     workers = _get_num_workers(subjects_per_job, subject_list)
     subject_subsets = split_list(subject_list, num_chunks=workers)
 
     # Create a text file for each job
     for i, subset in enumerate(subject_subsets):
         # Create a text file containing the list of subjects for each job
         batch_filepath = output_dir / f'batch{i:04}.txt'
         # Store to the path given to the text file
         list2txt(batch_filepath, subset)
         # Add the path to the text file ( containing the
         # list of subjects for each job) to a list, return the list
         batch_ids_path_list.append(batch_filepath)
-    list2txt(path=per_batch_ids, list_=batch_ids_path_list)
+    list2txt(fpath=per_batch_ids, list_=batch_ids_path_list)
     return batch_ids_path_list
-
-
```

### Comparing `mrQA-0.2/mrQA/run_subset.py` & `mrQA-0.2.3/mrQA/run_subset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+""" Console script for running subset of dataset, a part of parallel
+processing"""
 import argparse
 import sys
 from pathlib import Path
 
 from MRdataset import import_dataset, save_mr_dataset
 from MRdataset.base import BaseDataset
 from MRdataset.log import logger
 
-from mrQA.common import set_logging
 from mrQA.utils import txt2list
 
 
 def main():
     """Console script for mrQA."""
     parser = argparse.ArgumentParser(
         description='Protocol Compliance of MRI scans',
@@ -49,60 +50,66 @@
         logger.setLevel('INFO')
     else:
         logger.setLevel('WARNING')
 
     if not output_path.exists():
         partial_dataset = read_subset(output_path=args.output_path,
                                       batch_ids_file=args.batch_ids_file,
-                                      style='dicom',
+                                      ds_format='dicom',
                                       verbose=args.verbose,
                                       include_phantom=args.include_phantom,
                                       is_complete=not args.is_partial)
 
         partial_dataset.is_complete = False
         save_mr_dataset(args.output_path, partial_dataset)
 
 
 def read_subset(batch_ids_file: str,
-                style: str,
+                ds_format: str,
                 verbose: bool,
                 include_phantom: bool,
-                **_kwargs) -> BaseDataset:
+                **kwargs) -> BaseDataset:
     """
     Given a list of folder paths, reads all dicom files in those folders
     and returns a MRdataset object. In context, when this function was created,
     each folder corresponds to a different subject.
 
     Parameters
     ----------
     batch_ids_file : str
         path to a text file containing a list of paths (to several folders)
-    style : str
+    ds_format : str
         what kind of MRdataset to create, dicom, bids etc.
     verbose : bool
         print more while doing the job
     include_phantom : bool
         whether to include phantom files in processing
+    **kwargs: dict
+        additional arguments to pass to import_dataset
 
     Returns
     -------
-    MRdataset.base.Project
+    BaseDataset
 
+    Raises
+    ------
+    NotImplementedError
+        if ds_format is not dicom
     """
     # Supports only dicom for now
-    if style != 'dicom':
-        raise NotImplementedError(f"Expected style as dicom, Got {style}")
+    if ds_format != 'dicom':
+        raise NotImplementedError(f'Expected ds_format as dicom, Got {ds_format}')
 
     subset = txt2list(batch_ids_file)
     identifier = Path(batch_ids_file).stem
-    partial_dataset = import_dataset(data_source_folders=subset,
-                                     style=style,
+    partial_dataset = import_dataset(data_source=subset,
+                                     ds_format=ds_format,
                                      name=identifier,
                                      verbose=verbose,
                                      include_phantom=include_phantom,
-                                     **_kwargs)
+                                     **kwargs)
     # partial_dataset.walk(), import_dataset already does this
     return partial_dataset
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     sys.exit(main())  # pragma: no cover
```

### Comparing `mrQA-0.2/mrQA/tests/test_compliance.py` & `mrQA-0.2.3/mrQA/tests/test_compliance.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,16 +176,16 @@
     assume(magnetic_field_strength != const_bids['b0'])
     assume(flip_angle != const_bids['fa'])
 
     fake_dir, dataset_info = make_bids_test_dataset(num_noncompliant_subjects,
                                                     repetition_time,
                                                     magnetic_field_strength,
                                                     flip_angle)
-    mrd = import_dataset(fake_dir, include_phantom=True, style='bids')
-    checked_dataset = check_compliance(dataset=mrd, output_dir=mrd.data_root)
+    mrd = import_dataset(fake_dir, include_phantom=True, ds_format='bids')
+    checked_dataset = check_compliance(dataset=mrd, output_dir=mrd.data_source)
 
     # Check on disk, basically the truth
     layout = BIDSLayout(fake_dir)
     sub_names_by_modality = defaultdict(set)
     subjects = layout.get_subjects()
 
     for modality in MRdataset.config.datatypes:
```

### Comparing `mrQA-0.2/mrQA/tests/test_parallel.py` & `mrQA-0.2.3/mrQA/tests/test_parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 def test_equivalence_seq_vs_parallel(data_source):
     output_dir = Path(data_source).parent / 'test_mrqa_files'
     output_path = {
         'sequential': output_dir / ('sequential' + MRDS_EXT),
         'parallel': output_dir / ('parallel' + MRDS_EXT)
     }
     if not output_path['sequential'].exists():
-        sequential_ds = import_dataset(data_source_folders=data_source,
-                                       style='dicom',
+        sequential_ds = import_dataset(data_source=data_source,
+                                       ds_format='dicom',
                                        name='sequential')
         save_mr_dataset(output_path['sequential'], sequential_ds)
     else:
         sequential_ds = load_mr_dataset(output_path['sequential'])
 
     process_parallel(data_source,
                      output_dir,
                      output_path['parallel'],
                      'parallel')
 
     # Generate a report for the merged dataset
-    parallel_ds = load_mr_dataset(output_path['parallel'], style='dicom')
+    parallel_ds = load_mr_dataset(output_path['parallel'], ds_format='dicom')
 
     report_path = {
         'sequential': check_compliance(dataset=sequential_ds,
                                        output_dir=output_dir),
         'parallel': check_compliance(dataset=parallel_ds,
                                      output_dir=output_dir)
     }
@@ -51,16 +51,16 @@
 
 def test_merging(data_source):
     # Sequential complete processing of the dataset
     output_dir = Path(data_source).parent / 'test_merge_mrqa_files'
     output_path_seq = output_dir / ('sequential' + MRDS_EXT)
 
     if not output_path_seq.exists():
-        sequential_ds = import_dataset(data_source_folders=data_source,
-                                       style='dicom',
+        sequential_ds = import_dataset(data_source=data_source,
+                                       ds_format='dicom',
                                        name='sequential')
         save_mr_dataset(output_path_seq, sequential_ds)
     else:
         sequential_ds = load_mr_dataset(output_path_seq)
 
     # Start processing in batches
     folder_paths, files_per_batch, all_ids_path = _make_file_folders(output_dir)
@@ -79,16 +79,16 @@
                    for i in range(len(ids_path_list))}
     ds_list = []
     for i, filepath in enumerate(ids_path_list):
         # Read the list of subject ids to be processed
         subject_folders_list = txt2list(filepath)
         if not output_path[i].exists():
             # Process the batch of subjects
-            ds = import_dataset(data_source_folders=subject_folders_list,
-                                style='dicom',
+            ds = import_dataset(data_source=subject_folders_list,
+                                ds_format='dicom',
                                 name=f'seq{i}')
             save_mr_dataset(output_path[i], ds)
         else:
             ds = load_mr_dataset(output_path[i])
         ds_list.append(ds)
 
     # Merge batches
@@ -131,15 +131,16 @@
                     assert run1.params == run2.params
     return True
 
 
 def is_same(file1, file2):
     file1, file2 = valid_paths([file1, file2])
     with open(file1) as f1, open(file2) as f2:
-        for line1, line2 in zip(f1, f2):
+        # Check after timestamps. Don't check 1st 3 lines
+        for line1, line2 in list(zip(f1, f2))[3:]:
             if line1 != line2:
                 return False
     return True
 
 
 if __name__ == '__main__':
     # test_equivalence_seq_vs_parallel(
```

### Comparing `mrQA-0.2/setup.cfg` & `mrQA-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `mrQA-0.2/versioneer.py` & `mrQA-0.2.3/versioneer.py`

 * *Files identical despite different names*

