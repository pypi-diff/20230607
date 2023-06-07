# Comparing `tmp/xgo-pythonlib-0.0.5.tar.gz` & `tmp/xgo-pythonlib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.0.5.tar", last modified: Wed Jun  7 00:12:12 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.0.6.tar", last modified: Wed Jun  7 00:15:52 2023, max compression
```

## Comparing `xgo-pythonlib-0.0.5.tar` & `xgo-pythonlib-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 00:12:12.358534 xgo-pythonlib-0.0.5/
--rw-rw-rw-   0        0        0     1208 2023-06-07 00:12:12.357538 xgo-pythonlib-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-06-06 23:47:08.000000 xgo-pythonlib-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 00:12:12.358534 xgo-pythonlib-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     3738 2023-06-07 00:12:06.000000 xgo-pythonlib-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 00:12:12.345126 xgo-pythonlib-0.0.5/xgo/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.5/xgo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 00:12:12.349524 xgo-pythonlib-0.0.5/xgo/screen/
--rw-rw-rw-   0        0        0     5316 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.5/xgo/screen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.5/xgo/screen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.5/xgo/screen/lcdconfig.py
--rw-rw-rw-   0        0        0    33476 2023-06-07 00:11:44.000000 xgo-pythonlib-0.0.5/xgo/xgoedu.py
--rw-rw-rw-   0        0        0    24818 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.5/xgo/xgolib.py
-drwxrwxrwx   0        0        0        0 2023-06-07 00:12:12.355535 xgo-pythonlib-0.0.5/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     1208 2023-06-07 00:12:12.000000 xgo-pythonlib-0.0.5/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-06-07 00:12:12.000000 xgo-pythonlib-0.0.5/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 00:12:12.000000 xgo-pythonlib-0.0.5/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-07 00:12:12.000000 xgo-pythonlib-0.0.5/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 00:15:52.239144 xgo-pythonlib-0.0.6/
+-rw-rw-rw-   0        0        0     1208 2023-06-07 00:15:52.238147 xgo-pythonlib-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2023-06-06 23:47:08.000000 xgo-pythonlib-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 00:15:52.239144 xgo-pythonlib-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     3738 2023-06-07 00:15:46.000000 xgo-pythonlib-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 00:15:52.221444 xgo-pythonlib-0.0.6/xgo/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.6/xgo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 00:15:52.226695 xgo-pythonlib-0.0.6/xgo/screen/
+-rw-rw-rw-   0        0        0     5327 2023-06-07 00:15:14.000000 xgo-pythonlib-0.0.6/xgo/screen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.6/xgo/screen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.6/xgo/screen/lcdconfig.py
+-rw-rw-rw-   0        0        0    33476 2023-06-07 00:11:44.000000 xgo-pythonlib-0.0.6/xgo/xgoedu.py
+-rw-rw-rw-   0        0        0    24818 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.6/xgo/xgolib.py
+drwxrwxrwx   0        0        0        0 2023-06-07 00:15:52.235653 xgo-pythonlib-0.0.6/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     1208 2023-06-07 00:15:52.000000 xgo-pythonlib-0.0.6/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-06-07 00:15:52.000000 xgo-pythonlib-0.0.6/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 00:15:52.000000 xgo-pythonlib-0.0.6/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-07 00:15:52.000000 xgo-pythonlib-0.0.6/xgo_pythonlib.egg-info/top_level.txt
```

### Comparing `xgo-pythonlib-0.0.5/PKG-INFO` & `xgo-pythonlib-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.0.5
+Version: 0.0.6
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: jd3096
 Author-email: 1091329318@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `xgo-pythonlib-0.0.5/README.md` & `xgo-pythonlib-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.0.5/setup.py` & `xgo-pythonlib-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = '1091329318@qq.com'
 AUTHOR = 'jd3096'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.0.5/xgo/screen/LCD_2inch.py` & `xgo-pythonlib-0.0.6/xgo/screen/LCD_2inch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import time
-import lcdconfig
+import xgo.screen.lcdconfig
 
 class LCD_2inch(lcdconfig.RaspberryPi):
 
     width = 240
     height = 320 
     def command(self, cmd):
         self.digital_write(self.DC_PIN, self.GPIO.LOW)
```

### Comparing `xgo-pythonlib-0.0.5/xgo/screen/lcdconfig.py` & `xgo-pythonlib-0.0.6/xgo/screen/lcdconfig.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.0.5/xgo/xgoedu.py` & `xgo-pythonlib-0.0.6/xgo/xgoedu.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.0.5/xgo/xgolib.py` & `xgo-pythonlib-0.0.6/xgo/xgolib.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.0.5/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.0.6/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.0.5
+Version: 0.0.6
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: jd3096
 Author-email: 1091329318@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

