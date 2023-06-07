# Comparing `tmp/SouPyX-1.0.4.tar.gz` & `tmp/SouPyX-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SouPyX-1.0.4.tar", last modified: Thu Mar  9 14:27:57 2023, max compression
+gzip compressed data, was "SouPyX-1.0.5.tar", last modified: Wed Jun  7 14:03:50 2023, max compression
```

## Comparing `SouPyX-1.0.4.tar` & `SouPyX-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 14:27:57.150796 SouPyX-1.0.4/
--rw-rw-rw-   0        0        0     1086 2023-03-05 15:20:06.000000 SouPyX-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1055 2023-03-09 14:27:57.150796 SouPyX-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6805 2023-03-08 13:36:20.000000 SouPyX-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-09 14:27:57.147843 SouPyX-1.0.4/SouPyX/
--rw-rw-rw-   0        0        0     1407 2023-03-05 15:46:00.000000 SouPyX-1.0.4/SouPyX/__init__.py
--rw-rw-rw-   0        0        0    14653 2023-03-09 14:16:28.000000 SouPyX-1.0.4/SouPyX/core.py
--rw-rw-rw-   0        0        0    12418 2023-03-05 15:40:41.000000 SouPyX-1.0.4/SouPyX/display.py
--rw-rw-rw-   0        0        0    12632 2023-03-05 15:40:41.000000 SouPyX-1.0.4/SouPyX/effects.py
--rw-rw-rw-   0        0        0    10163 2023-03-05 15:40:41.000000 SouPyX-1.0.4/SouPyX/models.py
--rw-rw-rw-   0        0        0    14796 2023-03-08 13:36:42.000000 SouPyX-1.0.4/SouPyX/spatial.py
--rw-rw-rw-   0        0        0    23919 2023-03-05 15:40:41.000000 SouPyX-1.0.4/SouPyX/synths.py
--rw-rw-rw-   0        0        0     1342 2023-03-09 14:10:00.000000 SouPyX-1.0.4/SouPyX/version.py
-drwxrwxrwx   0        0        0        0 2023-03-09 14:27:57.150796 SouPyX-1.0.4/SouPyX.egg-info/
--rw-rw-rw-   0        0        0     1055 2023-03-09 14:27:57.000000 SouPyX-1.0.4/SouPyX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-03-09 14:27:57.000000 SouPyX-1.0.4/SouPyX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 14:27:57.000000 SouPyX-1.0.4/SouPyX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-09 14:27:57.000000 SouPyX-1.0.4/SouPyX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-09 14:27:57.000000 SouPyX-1.0.4/SouPyX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-09 14:27:57.150796 SouPyX-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2724 2023-03-09 14:09:47.000000 SouPyX-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:03:50.438282 SouPyX-1.0.5/
+-rw-rw-rw-   0        0        0     1086 2023-06-07 13:43:53.000000 SouPyX-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1055 2023-06-07 14:03:50.437278 SouPyX-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6805 2023-06-07 13:43:53.000000 SouPyX-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 14:03:50.430479 SouPyX-1.0.5/SouPyX/
+-rw-rw-rw-   0        0        0     1407 2023-06-07 13:43:53.000000 SouPyX-1.0.5/SouPyX/__init__.py
+-rw-rw-rw-   0        0        0    14653 2023-06-07 13:43:53.000000 SouPyX-1.0.5/SouPyX/core.py
+-rw-rw-rw-   0        0        0    12418 2023-06-07 13:43:53.000000 SouPyX-1.0.5/SouPyX/display.py
+-rw-rw-rw-   0        0        0    12632 2023-06-07 13:43:53.000000 SouPyX-1.0.5/SouPyX/effects.py
+-rw-rw-rw-   0        0        0    10163 2023-06-07 13:43:53.000000 SouPyX-1.0.5/SouPyX/models.py
+-rw-rw-rw-   0        0        0    14796 2023-06-07 13:43:53.000000 SouPyX-1.0.5/SouPyX/spatial.py
+-rw-rw-rw-   0        0        0    23919 2023-06-07 13:43:53.000000 SouPyX-1.0.5/SouPyX/synths.py
+-rw-rw-rw-   0        0        0     1342 2023-06-07 13:59:14.000000 SouPyX-1.0.5/SouPyX/version.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:03:50.435252 SouPyX-1.0.5/SouPyX.egg-info/
+-rw-rw-rw-   0        0        0     1055 2023-06-07 14:03:50.000000 SouPyX-1.0.5/SouPyX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-06-07 14:03:50.000000 SouPyX-1.0.5/SouPyX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:03:50.000000 SouPyX-1.0.5/SouPyX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-07 14:03:50.000000 SouPyX-1.0.5/SouPyX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-07 14:03:50.000000 SouPyX-1.0.5/SouPyX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 14:03:50.438282 SouPyX-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2729 2023-06-07 13:44:29.000000 SouPyX-1.0.5/setup.py
```

### Comparing `SouPyX-1.0.4/LICENSE` & `SouPyX-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SouPyX-1.0.4/PKG-INFO` & `SouPyX-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SouPyX
-Version: 1.0.4
+Version: 1.0.5
 Summary: Sound Python Library
 Home-page: https://github.com/Yuan-ManX/SouPy
 Author: Yuan Man
 Author-email: ym1076302261@gmail.com
 License: MIT
 Keywords: audio music speech dsp soundsynthesis audioeffect spatialaudio signalprocessing machinelearning deeplearning
 Platform: UNKNOWN
```

### Comparing `SouPyX-1.0.4/README.md` & `SouPyX-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `SouPyX-1.0.4/SouPyX/__init__.py` & `SouPyX-1.0.5/SouPyX/__init__.py`

 * *Files identical despite different names*

### Comparing `SouPyX-1.0.4/SouPyX/core.py` & `SouPyX-1.0.5/SouPyX/core.py`

 * *Files identical despite different names*

### Comparing `SouPyX-1.0.4/SouPyX/display.py` & `SouPyX-1.0.5/SouPyX/display.py`

 * *Files identical despite different names*

### Comparing `SouPyX-1.0.4/SouPyX/effects.py` & `SouPyX-1.0.5/SouPyX/effects.py`

 * *Files identical despite different names*

### Comparing `SouPyX-1.0.4/SouPyX/models.py` & `SouPyX-1.0.5/SouPyX/models.py`

 * *Files identical despite different names*

### Comparing `SouPyX-1.0.4/SouPyX/spatial.py` & `SouPyX-1.0.5/SouPyX/spatial.py`

 * *Files identical despite different names*

### Comparing `SouPyX-1.0.4/SouPyX/synths.py` & `SouPyX-1.0.5/SouPyX/synths.py`

 * *Files identical despite different names*

### Comparing `SouPyX-1.0.4/SouPyX/version.py` & `SouPyX-1.0.5/SouPyX/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
 
 r"""Separate file for storing the current version of SouPy.
 Stored in a separate file so that setup.py can reference the version without
 pulling in all the dependencies in __init__.py.
 """
 
-__version__ = '1.0.4'
+__version__ = '1.0.5'
```

### Comparing `SouPyX-1.0.4/SouPyX.egg-info/PKG-INFO` & `SouPyX-1.0.5/SouPyX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SouPyX
-Version: 1.0.4
+Version: 1.0.5
 Summary: Sound Python Library
 Home-page: https://github.com/Yuan-ManX/SouPy
 Author: Yuan Man
 Author-email: ym1076302261@gmail.com
 License: MIT
 Keywords: audio music speech dsp soundsynthesis audioeffect spatialaudio signalprocessing machinelearning deeplearning
 Platform: UNKNOWN
```

### Comparing `SouPyX-1.0.4/setup.py` & `SouPyX-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     url='https://github.com/Yuan-ManX/SouPy',
     license='MIT',
     packages=setuptools.find_packages(),
     long_description=__doc__,
     install_requires=[
         'numpy',
         'scipy',
-        'sklearn',
+        'scikit-learn',
         'torch',
         'matplotlib',
         'mido',
         'h5py'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

