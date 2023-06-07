# Comparing `tmp/xgo-pythonlib-0.0.8.tar.gz` & `tmp/xgo-pythonlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.0.8.tar", last modified: Wed Jun  7 00:20:46 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.0.9.tar", last modified: Wed Jun  7 11:41:18 2023, max compression
```

## Comparing `xgo-pythonlib-0.0.8.tar` & `xgo-pythonlib-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 00:20:46.245589 xgo-pythonlib-0.0.8/
--rw-rw-rw-   0        0        0     1208 2023-06-07 00:20:46.245589 xgo-pythonlib-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-06-06 23:47:08.000000 xgo-pythonlib-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 00:20:46.245589 xgo-pythonlib-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3738 2023-06-07 00:20:42.000000 xgo-pythonlib-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 00:20:46.231270 xgo-pythonlib-0.0.8/xgo/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.8/xgo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 00:20:46.235692 xgo-pythonlib-0.0.8/xgo/screen/
--rw-rw-rw-   0        0        0     5340 2023-06-07 00:17:28.000000 xgo-pythonlib-0.0.8/xgo/screen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.8/xgo/screen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.8/xgo/screen/lcdconfig.py
--rw-rw-rw-   0        0        0    33490 2023-06-07 00:20:27.000000 xgo-pythonlib-0.0.8/xgo/xgoedu.py
--rw-rw-rw-   0        0        0    24818 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.8/xgo/xgolib.py
-drwxrwxrwx   0        0        0        0 2023-06-07 00:20:46.243589 xgo-pythonlib-0.0.8/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     1208 2023-06-07 00:20:46.000000 xgo-pythonlib-0.0.8/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-06-07 00:20:46.000000 xgo-pythonlib-0.0.8/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 00:20:46.000000 xgo-pythonlib-0.0.8/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-07 00:20:46.000000 xgo-pythonlib-0.0.8/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 11:41:18.593512 xgo-pythonlib-0.0.9/
+-rw-rw-rw-   0        0        0     1567 2023-06-07 11:41:18.592509 xgo-pythonlib-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2023-06-07 00:33:33.000000 xgo-pythonlib-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 11:41:18.593512 xgo-pythonlib-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3684 2023-06-07 11:41:03.000000 xgo-pythonlib-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:41:18.584194 xgo-pythonlib-0.0.9/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     1567 2023-06-07 11:41:18.000000 xgo-pythonlib-0.0.9/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-07 11:41:18.000000 xgo-pythonlib-0.0.9/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 11:41:18.000000 xgo-pythonlib-0.0.9/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 11:41:18.000000 xgo-pythonlib-0.0.9/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 11:41:18.587208 xgo-pythonlib-0.0.9/xgoedu/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.9/xgoedu/__init__.py
+-rw-rw-rw-   0        0        0    33490 2023-06-07 00:20:27.000000 xgo-pythonlib-0.0.9/xgoedu/xgoedu.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:41:18.590510 xgo-pythonlib-0.0.9/xgolib/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.9/xgolib/__init__.py
+-rw-rw-rw-   0        0        0    24818 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.9/xgolib/xgolib.py
```

### Comparing `xgo-pythonlib-0.0.8/setup.py` & `xgo-pythonlib-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import sys
 from shutil import rmtree
 from setuptools import find_packages, setup, Command
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
-EMAIL = '1091329318@qq.com'
-AUTHOR = 'jd3096'
+EMAIL = 'hello@xgorobot.com'
+AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
@@ -92,17 +92,14 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(),
-    package_data={
-        'xgo':['Font/msyh.ttc']
-    },
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
```

### Comparing `xgo-pythonlib-0.0.8/xgo/xgoedu.py` & `xgo-pythonlib-0.0.9/xgoedu/xgoedu.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.0.8/xgo/xgolib.py` & `xgo-pythonlib-0.0.9/xgolib/xgolib.py`

 * *Files identical despite different names*

