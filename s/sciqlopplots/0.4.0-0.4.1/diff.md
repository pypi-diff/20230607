# Comparing `tmp/sciqlopplots-0.4.0-cp39-cp39-win_amd64.whl.zip` & `tmp/sciqlopplots-0.4.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2683588 bytes, number of entries: 7
-?rw-rw-r--  2.0 fat     3120 b- stor 23-Jun-04 17:40 sciqlopplots-0.4.0.dist-info/METADATA
-?rw-rw-r--  2.0 fat       83 b- stor 23-Jun-04 17:40 sciqlopplots-0.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1585 b- stor 23-Jun-04 17:28 sciqlopplots-0.4.0.dist-info/COPYING
--rw-rw-rw-  2.0 fat  2674688 b- stor 23-Jun-04 17:40 SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2232 b- stor 23-Jun-04 17:40 SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.lib
--rw-rw-rw-  2.0 fat      171 b- stor 23-Jun-04 17:28 SciQLopPlots/__init__.py
-?rw-rw-r--  2.0 fat      615 b- stor 23-Jun-04 17:40 sciqlopplots-0.4.0.dist-info/RECORD
-7 files, 2682494 bytes uncompressed, 2682494 bytes compressed:  0.0%
+Zip file size: 2684100 bytes, number of entries: 7
+?rw-rw-r--  2.0 fat     3120 b- stor 23-Jun-07 16:58 sciqlopplots-0.4.1.dist-info/METADATA
+?rw-rw-r--  2.0 fat       83 b- stor 23-Jun-07 16:58 sciqlopplots-0.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1585 b- stor 23-Jun-07 16:50 sciqlopplots-0.4.1.dist-info/COPYING
+-rw-rw-rw-  2.0 fat  2675200 b- stor 23-Jun-07 16:58 SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2232 b- stor 23-Jun-07 16:58 SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.lib
+-rw-rw-rw-  2.0 fat      171 b- stor 23-Jun-07 16:50 SciQLopPlots/__init__.py
+?rw-rw-r--  2.0 fat      615 b- stor 23-Jun-07 16:58 sciqlopplots-0.4.1.dist-info/RECORD
+7 files, 2683006 bytes uncompressed, 2683006 bytes compressed:  0.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: sciqlopplots-0.4.0.dist-info/METADATA
+Filename: sciqlopplots-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: sciqlopplots-0.4.0.dist-info/WHEEL
+Filename: sciqlopplots-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: sciqlopplots-0.4.0.dist-info/COPYING
+Filename: sciqlopplots-0.4.1.dist-info/COPYING
 Comment: 
 
 Filename: SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.pyd
 Comment: 
 
 Filename: SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.lib
 Comment: 
 
 Filename: SciQLopPlots/__init__.py
 Comment: 
 
-Filename: sciqlopplots-0.4.0.dist-info/RECORD
+Filename: sciqlopplots-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SciQLopPlots/__init__.py

```diff
@@ -1,5 +1,5 @@
 from PySide6 import QtCore, QtGui, QtWidgets
 from .SciQLopPlotsBindings import *
 from .SciQLopPlotsBindings import _QCustomPlot as QCustomPlot
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
```

## Comparing `sciqlopplots-0.4.0.dist-info/METADATA` & `sciqlopplots-0.4.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciqlopplots
-Version: 0.4.0
+Version: 0.4.1
 Summary: SciQLop plot API based on QCustomPlot
 Home-page: https://github.com/SciQLop/SciQLopPlots
 Author-Email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 License: GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
             An easy to use ISTP loader package.
```

## Comparing `sciqlopplots-0.4.0.dist-info/COPYING` & `sciqlopplots-0.4.1.dist-info/COPYING`

 * *Files identical despite different names*

