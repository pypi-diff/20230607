# Comparing `tmp/xgo-pythonlib-0.0.6.tar.gz` & `tmp/xgo-pythonlib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.0.6.tar", last modified: Wed Jun  7 00:15:52 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.0.7.tar", last modified: Wed Jun  7 00:18:19 2023, max compression
```

## Comparing `xgo-pythonlib-0.0.6.tar` & `xgo-pythonlib-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 00:15:52.239144 xgo-pythonlib-0.0.6/
--rw-rw-rw-   0        0        0     1208 2023-06-07 00:15:52.238147 xgo-pythonlib-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-06-06 23:47:08.000000 xgo-pythonlib-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 00:15:52.239144 xgo-pythonlib-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     3738 2023-06-07 00:15:46.000000 xgo-pythonlib-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 00:15:52.221444 xgo-pythonlib-0.0.6/xgo/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.6/xgo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 00:15:52.226695 xgo-pythonlib-0.0.6/xgo/screen/
--rw-rw-rw-   0        0        0     5327 2023-06-07 00:15:14.000000 xgo-pythonlib-0.0.6/xgo/screen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.6/xgo/screen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.6/xgo/screen/lcdconfig.py
--rw-rw-rw-   0        0        0    33476 2023-06-07 00:11:44.000000 xgo-pythonlib-0.0.6/xgo/xgoedu.py
--rw-rw-rw-   0        0        0    24818 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.6/xgo/xgolib.py
-drwxrwxrwx   0        0        0        0 2023-06-07 00:15:52.235653 xgo-pythonlib-0.0.6/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     1208 2023-06-07 00:15:52.000000 xgo-pythonlib-0.0.6/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-06-07 00:15:52.000000 xgo-pythonlib-0.0.6/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 00:15:52.000000 xgo-pythonlib-0.0.6/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-07 00:15:52.000000 xgo-pythonlib-0.0.6/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 00:18:19.767229 xgo-pythonlib-0.0.7/
+-rw-rw-rw-   0        0        0     1208 2023-06-07 00:18:19.767229 xgo-pythonlib-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2023-06-06 23:47:08.000000 xgo-pythonlib-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 00:18:19.768221 xgo-pythonlib-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     3738 2023-06-07 00:18:13.000000 xgo-pythonlib-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 00:18:19.754220 xgo-pythonlib-0.0.7/xgo/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.7/xgo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 00:18:19.758220 xgo-pythonlib-0.0.7/xgo/screen/
+-rw-rw-rw-   0        0        0     5340 2023-06-07 00:17:28.000000 xgo-pythonlib-0.0.7/xgo/screen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.7/xgo/screen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.7/xgo/screen/lcdconfig.py
+-rw-rw-rw-   0        0        0    33489 2023-06-07 00:18:01.000000 xgo-pythonlib-0.0.7/xgo/xgoedu.py
+-rw-rw-rw-   0        0        0    24818 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.7/xgo/xgolib.py
+drwxrwxrwx   0        0        0        0 2023-06-07 00:18:19.764224 xgo-pythonlib-0.0.7/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     1208 2023-06-07 00:18:19.000000 xgo-pythonlib-0.0.7/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-06-07 00:18:19.000000 xgo-pythonlib-0.0.7/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 00:18:19.000000 xgo-pythonlib-0.0.7/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-07 00:18:19.000000 xgo-pythonlib-0.0.7/xgo_pythonlib.egg-info/top_level.txt
```

### Comparing `xgo-pythonlib-0.0.6/PKG-INFO` & `xgo-pythonlib-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: jd3096
 Author-email: 1091329318@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `xgo-pythonlib-0.0.6/README.md` & `xgo-pythonlib-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.0.6/setup.py` & `xgo-pythonlib-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = '1091329318@qq.com'
 AUTHOR = 'jd3096'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.0.6/xgo/screen/LCD_2inch.py` & `xgo-pythonlib-0.0.7/xgo/screen/LCD_2inch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import time
-import xgo.screen.lcdconfig
+import xgo.screen.lcdconfig as lcdconfig
 
 class LCD_2inch(lcdconfig.RaspberryPi):
 
     width = 240
     height = 320 
     def command(self, cmd):
         self.digital_write(self.DC_PIN, self.GPIO.LOW)
```

### Comparing `xgo-pythonlib-0.0.6/xgo/screen/lcdconfig.py` & `xgo-pythonlib-0.0.7/xgo/screen/lcdconfig.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.0.6/xgo/xgoedu.py` & `xgo-pythonlib-0.0.7/xgo/xgoedu.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 xgo图形化python库  edu库
 '''
 import cv2
 import numpy as np
 import math
 import os,sys,time
 import spidev as SPI
-import xgo.screen.LCD_2inch
+import xgo.screen.LCD_2inch as LCD_2inch
 import RPi.GPIO as GPIO
 from PIL import Image,ImageDraw,ImageFont
 import json
 from xgolib import XGO
 # from keras.preprocessing import image
```

### Comparing `xgo-pythonlib-0.0.6/xgo/xgolib.py` & `xgo-pythonlib-0.0.7/xgo/xgolib.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.0.6/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.0.7/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: jd3096
 Author-email: 1091329318@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

