# Comparing `tmp/xgo-pythonlib-0.0.9.tar.gz` & `tmp/xgo-pythonlib-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.0.9.tar", last modified: Wed Jun  7 11:41:18 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.1.0.tar", last modified: Wed Jun  7 11:45:01 2023, max compression
```

## Comparing `xgo-pythonlib-0.0.9.tar` & `xgo-pythonlib-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 11:41:18.593512 xgo-pythonlib-0.0.9/
--rw-rw-rw-   0        0        0     1567 2023-06-07 11:41:18.592509 xgo-pythonlib-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      940 2023-06-07 00:33:33.000000 xgo-pythonlib-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 11:41:18.593512 xgo-pythonlib-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     3684 2023-06-07 11:41:03.000000 xgo-pythonlib-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:41:18.584194 xgo-pythonlib-0.0.9/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     1567 2023-06-07 11:41:18.000000 xgo-pythonlib-0.0.9/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-06-07 11:41:18.000000 xgo-pythonlib-0.0.9/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 11:41:18.000000 xgo-pythonlib-0.0.9/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 11:41:18.000000 xgo-pythonlib-0.0.9/xgo_pythonlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 11:41:18.587208 xgo-pythonlib-0.0.9/xgoedu/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.9/xgoedu/__init__.py
--rw-rw-rw-   0        0        0    33490 2023-06-07 00:20:27.000000 xgo-pythonlib-0.0.9/xgoedu/xgoedu.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:41:18.590510 xgo-pythonlib-0.0.9/xgolib/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.0.9/xgolib/__init__.py
--rw-rw-rw-   0        0        0    24818 2023-06-06 01:30:25.000000 xgo-pythonlib-0.0.9/xgolib/xgolib.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:45:01.965333 xgo-pythonlib-0.1.0/
+-rw-rw-rw-   0        0        0     1563 2023-06-07 11:45:01.964332 xgo-pythonlib-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2023-06-07 11:42:17.000000 xgo-pythonlib-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 11:45:01.965333 xgo-pythonlib-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3684 2023-06-07 11:44:56.000000 xgo-pythonlib-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:45:01.949466 xgo-pythonlib-0.1.0/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     1563 2023-06-07 11:45:01.000000 xgo-pythonlib-0.1.0/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-07 11:45:01.000000 xgo-pythonlib-0.1.0/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 11:45:01.000000 xgo-pythonlib-0.1.0/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-07 11:45:01.000000 xgo-pythonlib-0.1.0/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 11:45:01.953470 xgo-pythonlib-0.1.0/xgoedu/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.0/xgoedu/__init__.py
+-rw-rw-rw-   0        0        0    33489 2023-06-07 11:44:09.000000 xgo-pythonlib-0.1.0/xgoedu/xgoedu.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:45:01.957326 xgo-pythonlib-0.1.0/xgolib/
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.0/xgolib/__init__.py
+-rw-rw-rw-   0        0        0    24818 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.0/xgolib/xgolib.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:45:01.962332 xgo-pythonlib-0.1.0/xgoscreen/
+-rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.0/xgoscreen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.0/xgoscreen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.0/xgoscreen/lcdconfig.py
```

### Comparing `xgo-pythonlib-0.0.9/PKG-INFO` & `xgo-pythonlib-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.0.9
+Version: 0.1.0
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -41,15 +41,15 @@
 ```
 
 ## Examples
 
 Perform gesture recognition on the current camera and press the "c" key to exit.
 
 ```python
-from xgo.xgoedu import XGOEDU 
+from xgoedu import XGOEDU 
 edu = XGOEDU()
 
 while True:
     result=edu.gestureRecognition()  
     print(result)
     if edu.xgoButton("c"):  
         break
```

### Comparing `xgo-pythonlib-0.0.9/README.md` & `xgo-pythonlib-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ```
 
 ## Examples
 
 Perform gesture recognition on the current camera and press the "c" key to exit.
 
 ```python
-from xgo.xgoedu import XGOEDU 
+from xgoedu import XGOEDU 
 edu = XGOEDU()
 
 while True:
     result=edu.gestureRecognition()  
     print(result)
     if edu.xgoButton("c"):  
         break
```

### Comparing `xgo-pythonlib-0.0.9/setup.py` & `xgo-pythonlib-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = 'hello@xgorobot.com'
 AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.0.9/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.1.0/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.0.9
+Version: 0.1.0
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -41,15 +41,15 @@
 ```
 
 ## Examples
 
 Perform gesture recognition on the current camera and press the "c" key to exit.
 
 ```python
-from xgo.xgoedu import XGOEDU 
+from xgoedu import XGOEDU 
 edu = XGOEDU()
 
 while True:
     result=edu.gestureRecognition()  
     print(result)
     if edu.xgoButton("c"):  
         break
```

### Comparing `xgo-pythonlib-0.0.9/xgoedu/xgoedu.py` & `xgo-pythonlib-0.1.0/xgoedu/xgoedu.py`

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
-import xgo.screen.LCD_2inch as LCD_2inch
+import xgoscreen.LCD_2inch as LCD_2inch
 import RPi.GPIO as GPIO
 from PIL import Image,ImageDraw,ImageFont
 import json
 #from xgolib import XGO
 # from keras.preprocessing import image
```

### Comparing `xgo-pythonlib-0.0.9/xgolib/xgolib.py` & `xgo-pythonlib-0.1.0/xgolib/xgolib.py`

 * *Files identical despite different names*

