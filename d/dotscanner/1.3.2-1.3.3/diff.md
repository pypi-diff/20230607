# Comparing `tmp/dotscanner-1.3.2.tar.gz` & `tmp/dotscanner-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dotscanner-1.3.2.tar", last modified: Mon Jun  5 04:43:53 2023, max compression
+gzip compressed data, was "dist/dotscanner-1.3.3.tar", last modified: Wed Jun  7 02:15:20 2023, max compression
```

## Comparing `dotscanner-1.3.2.tar` & `dotscanner-1.3.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.366342 dotscanner-1.3.2/
--rw-r--r--   0 holly      (501) staff       (20)     1103 2023-06-05 02:24:39.000000 dotscanner-1.3.2/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)    13417 2023-06-05 04:43:53.366196 dotscanner-1.3.2/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)    12762 2023-06-05 04:37:56.000000 dotscanner-1.3.2/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.361753 dotscanner-1.3.2/dotscanner/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.2/dotscanner/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3552 2023-06-05 04:38:00.000000 dotscanner-1.3.2/dotscanner/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)    10277 2023-06-05 02:24:39.000000 dotscanner-1.3.2/dotscanner/dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     9355 2023-06-05 02:34:51.000000 dotscanner-1.3.2/dotscanner/density.py
--rw-r--r--   0 holly      (501) staff       (20)     6128 2023-06-05 02:24:39.000000 dotscanner-1.3.2/dotscanner/files.py
--rw-r--r--   0 holly      (501) staff       (20)    10494 2023-06-05 04:38:05.000000 dotscanner-1.3.2/dotscanner/lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     6692 2023-06-05 04:38:08.000000 dotscanner-1.3.2/dotscanner/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.363905 dotscanner-1.3.2/dotscanner/ui/
--rw-r--r--   0 holly      (501) staff       (20)     5179 2023-06-05 02:24:39.000000 dotscanner-1.3.2/dotscanner/ui/DefaultUserSettingsEditor.py
--rw-r--r--   0 holly      (501) staff       (20)     1858 2023-06-05 02:24:39.000000 dotscanner-1.3.2/dotscanner/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     3343 2023-06-05 02:53:52.000000 dotscanner-1.3.2/dotscanner/ui/MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     5569 2023-06-05 04:37:59.000000 dotscanner-1.3.2/dotscanner/ui/RegionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)    16340 2023-06-05 02:53:51.000000 dotscanner-1.3.2/dotscanner/ui/ThresholdAdjuster.py
--rw-r--r--   0 holly      (501) staff       (20)    15085 2023-06-05 04:38:06.000000 dotscanner-1.3.2/dotscanner/ui/UserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.2/dotscanner/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3097 2023-06-05 02:53:49.000000 dotscanner-1.3.2/dotscanner/ui/window.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.362648 dotscanner-1.3.2/dotscanner.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)    13417 2023-06-05 04:43:53.000000 dotscanner-1.3.2/dotscanner.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)     1000 2023-06-05 04:43:53.000000 dotscanner-1.3.2/dotscanner.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-06-05 04:43:53.000000 dotscanner-1.3.2/dotscanner.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       56 2023-06-05 04:43:53.000000 dotscanner-1.3.2/dotscanner.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       17 2023-06-05 04:43:53.000000 dotscanner-1.3.2/dotscanner.egg-info/requires.txt
--rw-r--r--   0 holly      (501) staff       (20)       26 2023-06-05 04:43:53.000000 dotscanner-1.3.2/dotscanner.egg-info/top_level.txt
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.364313 dotscanner-1.3.2/settings/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.2/settings/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     6218 2023-06-05 02:24:39.000000 dotscanner-1.3.2/settings/config.py
--rw-r--r--   0 holly      (501) staff       (20)    11284 2023-06-05 02:24:39.000000 dotscanner-1.3.2/settings/configmanagement.py
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-06-05 04:43:53.366398 dotscanner-1.3.2/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1444 2023-06-05 04:43:53.000000 dotscanner-1.3.2/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.365222 dotscanner-1.3.2/tests/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)    10018 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/test_dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     5572 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/test_density.py
--rw-r--r--   0 holly      (501) staff       (20)    13472 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)    10886 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/test_lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     5884 2023-06-05 04:38:07.000000 dotscanner-1.3.2/tests/test_strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 04:43:53.365961 dotscanner-1.3.2/tests/ui/
--rw-r--r--   0 holly      (501) staff       (20)      471 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/ui/FakeMicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)      962 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/ui/FakeUserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     4000 2023-06-05 02:53:50.000000 dotscanner-1.3.2/tests/ui/test_MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     8414 2023-06-05 02:24:39.000000 dotscanner-1.3.2/tests/ui/test_ThresholdAdjuster.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.578862 dotscanner-1.3.3/
+-rw-r--r--   0 holly      (501) staff       (20)     1103 2023-06-05 02:24:39.000000 dotscanner-1.3.3/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)    13417 2023-06-07 02:15:20.578693 dotscanner-1.3.3/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)    12762 2023-06-06 20:52:08.000000 dotscanner-1.3.3/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.574162 dotscanner-1.3.3/dotscanner/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.3/dotscanner/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     2755 2023-06-07 01:30:16.000000 dotscanner-1.3.3/dotscanner/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)    10277 2023-06-06 23:47:07.000000 dotscanner-1.3.3/dotscanner/dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)    10148 2023-06-07 01:30:15.000000 dotscanner-1.3.3/dotscanner/density.py
+-rw-r--r--   0 holly      (501) staff       (20)     6212 2023-06-06 23:47:08.000000 dotscanner-1.3.3/dotscanner/files.py
+-rw-r--r--   0 holly      (501) staff       (20)    10454 2023-06-07 00:24:19.000000 dotscanner-1.3.3/dotscanner/lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     6692 2023-06-06 23:47:10.000000 dotscanner-1.3.3/dotscanner/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.576466 dotscanner-1.3.3/dotscanner/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     5179 2023-06-06 23:47:11.000000 dotscanner-1.3.3/dotscanner/ui/DefaultUserSettingsEditor.py
+-rw-r--r--   0 holly      (501) staff       (20)     1858 2023-06-06 23:47:12.000000 dotscanner-1.3.3/dotscanner/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     3510 2023-06-07 01:30:18.000000 dotscanner-1.3.3/dotscanner/ui/MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     5733 2023-06-07 01:30:17.000000 dotscanner-1.3.3/dotscanner/ui/RegionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)    16388 2023-06-07 02:08:45.000000 dotscanner-1.3.3/dotscanner/ui/ThresholdAdjuster.py
+-rw-r--r--   0 holly      (501) staff       (20)    15070 2023-06-07 01:30:16.000000 dotscanner-1.3.3/dotscanner/ui/UserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.3/dotscanner/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3097 2023-06-06 23:47:14.000000 dotscanner-1.3.3/dotscanner/ui/window.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.575011 dotscanner-1.3.3/dotscanner.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)    13417 2023-06-07 02:15:20.000000 dotscanner-1.3.3/dotscanner.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)     1000 2023-06-07 02:15:20.000000 dotscanner-1.3.3/dotscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-06-07 02:15:20.000000 dotscanner-1.3.3/dotscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       56 2023-06-07 02:15:20.000000 dotscanner-1.3.3/dotscanner.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       17 2023-06-07 02:15:20.000000 dotscanner-1.3.3/dotscanner.egg-info/requires.txt
+-rw-r--r--   0 holly      (501) staff       (20)       26 2023-06-07 02:15:20.000000 dotscanner-1.3.3/dotscanner.egg-info/top_level.txt
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.576915 dotscanner-1.3.3/settings/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.3/settings/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     6219 2023-06-06 20:41:22.000000 dotscanner-1.3.3/settings/config.py
+-rw-r--r--   0 holly      (501) staff       (20)    11284 2023-06-05 02:24:39.000000 dotscanner-1.3.3/settings/configmanagement.py
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-06-07 02:15:20.578927 dotscanner-1.3.3/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1444 2023-06-07 02:15:20.000000 dotscanner-1.3.3/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.577782 dotscanner-1.3.3/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.3/tests/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)    10018 2023-06-05 02:24:39.000000 dotscanner-1.3.3/tests/test_dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     5572 2023-06-05 02:24:39.000000 dotscanner-1.3.3/tests/test_density.py
+-rw-r--r--   0 holly      (501) staff       (20)    13472 2023-06-05 02:24:39.000000 dotscanner-1.3.3/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)    10886 2023-06-05 02:24:39.000000 dotscanner-1.3.3/tests/test_lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     5884 2023-06-05 04:38:07.000000 dotscanner-1.3.3/tests/test_strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.578450 dotscanner-1.3.3/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)      471 2023-06-07 02:08:44.000000 dotscanner-1.3.3/tests/ui/FakeMicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)      964 2023-06-07 02:08:43.000000 dotscanner-1.3.3/tests/ui/FakeUserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.3/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     4000 2023-06-07 01:30:21.000000 dotscanner-1.3.3/tests/ui/test_MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     8046 2023-06-07 02:08:46.000000 dotscanner-1.3.3/tests/ui/test_ThresholdAdjuster.py
```

### Comparing `dotscanner-1.3.2/LICENSE` & `dotscanner-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/PKG-INFO` & `dotscanner-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.3.2
+Version: 1.3.3
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -148,15 +148,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.2
+* 1.3.3
      * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
```

### Comparing `dotscanner-1.3.2/README.md` & `dotscanner-1.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.2
+* 1.3.3
      * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
```

### Comparing `dotscanner-1.3.2/dotscanner/__main__.py` & `dotscanner-1.3.3/dotscanner/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,81 +9,61 @@
 from dotscanner.strings import ProgramType
 from dotscanner.ui.MicroscopeImage import MicroscopeImage
 from dotscanner.ui.RegionSelector import RegionSelector
 from dotscanner.ui.ThresholdAdjuster import ThresholdAdjuster
 from dotscanner.ui.UserSettings import UserSettings
 import settings.config as cfg
 
-def main():	
+def main():
 	while True:
 		userSettings = UserSettings()
 		directory, filenames = files.getDirectoryAndFilenames(userSettings)
 		if userSettings.program == ProgramType.DENSITY:
 			getDensityData(directory, filenames, userSettings)
 		elif userSettings.program == ProgramType.LIFETIME:
 			getLifetimeData(directory, filenames, userSettings)
 		else:
 			raise Exception(strings.programNameException)
 	
 def getDensityData(directory, filenames, userSettings):
 	if userSettings.reanalysis:
-		reanalyzeDensityData(directory, userSettings)
+		density.reanalyzeDensityData(directory, userSettings)
 		return
 	
 	density.checkUnitsConsistent(directory)
 	alreadyMeasured = density.getAlreadyMeasured(directory)
-	targetPath = files.getReanalysisTargetPath(directory, cfg.DENSITY_OUTPUT_FILENAME)
+	targetPath = files.getAnalysisTargetPath(directory, cfg.DENSITY_OUTPUT_FILENAME)
 	for filename in filenames:
 		if filename in alreadyMeasured:
 			print(strings.alreadyMeasuredNotification(filename))
 			continue
 		
 		print(f"\n----------\nDisplaying {filename}\n----------")
 		microscopeImage = MicroscopeImage(directory, filename, userSettings)
 		
 		thresholdAdjuster = ThresholdAdjuster(microscopeImage, userSettings)
+		userSettings = thresholdAdjuster.userSettings # Updating with the threshold adjustments
 		if microscopeImage.skipped:
-			
-			density.skipFile(directory, filename, targetPath, thresholdAdjuster.userSettings, 
-				microscopeImage)
+			density.skipFile(directory, filename, targetPath, userSettings, microscopeImage)
 			continue
 		
-		RegionSelector(microscopeImage, thresholdAdjuster.userSettings)
+		RegionSelector(microscopeImage, userSettings)
 		if microscopeImage.skipped:
-			density.skipFile(directory, filename, targetPath, thresholdAdjuster.userSettings, 
-				microscopeImage)
+			density.skipFile(directory, filename, targetPath, userSettings, microscopeImage)
 			continue
 		
 		density.measureDensity(directory, filename, targetPath, microscopeImage, userSettings)
 
 def getLifetimeData(directory, filenames, userSettings):
 	lifetime.checkEnoughFramesForLifetimes(filenames, userSettings)
 	
 	middleIndex = len(filenames) // 2
 	middleMicroscopeImage = MicroscopeImage(directory, filenames[middleIndex], userSettings)
 	
 	thresholdAdjuster = ThresholdAdjuster(middleMicroscopeImage, userSettings, skipButton=False)
-	RegionSelector(middleMicroscopeImage, thresholdAdjuster.userSettings, skipButton=False)
+	userSettings = thresholdAdjuster.userSettings # Updating with the threshold adjustments
+	RegionSelector(middleMicroscopeImage, userSettings, skipButton=False)
 	
-	lifetime.measureLifetime(directory, filenames, middleMicroscopeImage, 
-		thresholdAdjuster.userSettings)
-
-def reanalyzeDensityData(directory, userSettings):
-	targetPath = files.getReanalysisTargetPath(directory, cfg.DENSITY_OUTPUT_FILENAME)
-	adjustmentsMade = False
-	for filename, data in userSettings.densityData.items():
-		microscopeImage = MicroscopeImage(directory, filename, userSettings)
-		
-		if not adjustmentsMade:
-			thresholdAdjuster = ThresholdAdjuster(microscopeImage, userSettings)
-			newUserSettings = thresholdAdjuster.userSettings
-			adjustments = density.getReanalysisAdjustments(data, newUserSettings, microscopeImage)
-			density.setReanalysisDataValues(adjustments, userSettings, microscopeImage, data)
-			adjustmentsMade = not microscopeImage.skipped
-		
-		else:
-			density.setReanalysisDataValues(adjustments, userSettings, microscopeImage, data)
-		
-		density.measureDensity(directory, filename, targetPath, microscopeImage, userSettings)
+	lifetime.measureLifetime(directory, filenames, middleMicroscopeImage, userSettings)
 
 if __name__ == '__main__':
 	main()
```

### Comparing `dotscanner-1.3.2/dotscanner/dataprocessing.py` & `dotscanner-1.3.3/dotscanner/dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/dotscanner/density.py` & `dotscanner-1.3.3/dotscanner/density.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import dotscanner.dataprocessing as dp
 import dotscanner.files as files
 import dotscanner.strings as strings
 from dotscanner.ui.DialogWindow import DialogWindow
+from dotscanner.ui.MicroscopeImage import MicroscopeImage
+from dotscanner.ui.ThresholdAdjuster import ThresholdAdjuster
+import dotscanner.ui.window as ui
 import settings.config as cfg
 import settings.configmanagement as cm
 import matplotlib.pyplot as pl
 import numpy as np
 import os
 
 if cfg.SCALE is None:
@@ -97,14 +100,42 @@
 	dotTotal, surveyedArea, density, error, dotsInPoly, blobsInPoly = getDensityErrorAndCoords(
 		microscopeImage, blobSize)
 	
 	microscopeImage.dotCoords, microscopeImage.blobCoords = dotsInPoly, blobsInPoly
 	saveDensityDataFiles(directory, filename, targetPath, dotTotal, surveyedArea, density, error, 
 		microscopeImage, userSettings)
 
+def reanalyzeDensityData(directory, userSettings):
+	targetPath = files.getReanalysisTargetPath(directory, cfg.DENSITY_OUTPUT_FILENAME)
+	adjustmentsMade = False
+	
+	numberOfFiles = len(list(userSettings.densityData.keys()))
+	count = 0
+	for filename, data in userSettings.densityData.items():
+		microscopeImage = MicroscopeImage(directory, filename, userSettings)
+				
+		if not adjustmentsMade:
+			thresholdAdjuster = ThresholdAdjuster(microscopeImage, userSettings)
+			
+			print("Re-analyzing images...")
+			ui.printProgressBar(0, numberOfFiles)
+			
+			userSettings = thresholdAdjuster.userSettings # Updating with the threshold adjustments
+			adjustments = getReanalysisAdjustments(data, userSettings, microscopeImage)
+			setReanalysisDataValues(adjustments, userSettings, microscopeImage, data)
+			adjustmentsMade = not microscopeImage.skipped
+		
+		else:
+			setReanalysisDataValues(adjustments, userSettings, microscopeImage, data)
+		
+		measureDensity(directory, filename, targetPath, microscopeImage, userSettings)
+		
+		ui.printProgressBar(count + 1, numberOfFiles)
+		count += 1
+
 def getReanalysisAdjustments(densityData, newUserSettings, microscopeImage):
 	adjustments = [None for _ in range(8)]
 	if densityData[0] != microscopeImage.lowerDotThreshScale:
 		adjustments[0] = microscopeImage.lowerDotThreshScale
 	if densityData[1] != microscopeImage.upperDotThreshScale:
 		adjustments[1] = microscopeImage.upperDotThreshScale
 	if densityData[2] != microscopeImage.lowerBlobThreshScale:
@@ -113,28 +144,26 @@
 		adjustments[3] = newUserSettings.blobSize
 	if densityData[4] != newUserSettings.dotSize:
 		adjustments[4] = newUserSettings.dotSize
 	if densityData[5] != newUserSettings.lowerContrast:
 		adjustments[5] = newUserSettings.lowerContrast
 	if densityData[6] != newUserSettings.upperContrast:
 		adjustments[6] = newUserSettings.upperContrast
-	if densityData[7] != newUserSettings.polygon:
-		adjustments[7] = newUserSettings.polygon
+	if densityData[7] != microscopeImage.polygon:
+		adjustments[7] = microscopeImage.polygon
 	return adjustments
 
 def setReanalysisDataValues(adjustments, userSettings, microscopeImage, data):
 	# Set the data to what is read from the file
-	userSettings.lowerDotThresh = data[0]
-	userSettings.upperDotThresh = data[1]
-	userSettings.lowerBlobThresh = data[2]
-	userSettings.thresholds = (data[0], data[1], data[2])
-	userSettings.blobSize = data[3]
-	userSettings.dotSize = data[4]
-	microscopeImage.blobSize = userSettings.blobSize
-	microscopeImage.dotSize = userSettings.dotSize
+	microscopeImage.lowerDotThreshScale = data[0]
+	microscopeImage.upperDotThreshScale = data[1]
+	microscopeImage.lowerBlobThreshScale = data[2]
+	microscopeImage.thresholds = (data[0], data[1], data[2])
+	microscopeImage.blobSize = data[3]
+	microscopeImage.dotSize = data[4]
 	userSettings.lowerContrast = data[5]
 	userSettings.upperContrast = data[6]
 	microscopeImage.polygon = data[7]
 	
 	# Adjust the data that was adjusted to be different from the previous analysis
 	threshAdjusted = False
 	for index, adjustment in enumerate(adjustments):
@@ -146,72 +175,59 @@
 				microscopeImage.upperDotThreshScale = adjustment
 				threshAdjusted = True
 			elif index == 2:
 				microscopeImage.lowerBlobThreshScale = adjustment
 				threshAdjusted = True
 			elif index == 3:
 				userSettings.blobSize = adjustment
-				microscopeImage.blobSize = adjustment
 			elif index == 4:
 				userSettings.dotSize = adjustment
-				microscopeImage.dotSize = adjustment
 			elif index == 5:
 				userSettings.lowerContrast = adjustment
 			elif index == 6:
 				userSettings.upperContrast = adjustment
 			elif index == 7:
 				microscopeImage.polygon = adjustment
 	if threshAdjusted:
 		microscopeImage.thresholds = (microscopeImage.lowerDotThreshScale, 
 			microscopeImage.upperDotThreshScale, microscopeImage.lowerBlobThreshScale)
 
 def saveDensityDataFiles(directory, filename, targetPath, dotTotal, surveyedArea, density, error, 
 	microscopeImage, userSettings, skipped=False):
-	saveFigures = userSettings.saveFigures
-	blobSize = userSettings.blobSize
-	dotSize = userSettings.dotSize
-	lowerContrast = userSettings.lowerContrast
-	upperContrast = userSettings.upperContrast
-	dotCoords = microscopeImage.dotCoords
-	blobCoords = microscopeImage.blobCoords
-	
 	if not os.path.exists(targetPath):
 		with open(targetPath, "a") as file:
 			file.write(strings.densityOutputFileHeader)
 			
 	if skipped:
 		output = f"{filename} skipped - - - - - - - - - - - -\n"
 		
 	else:
 		density = np.round(density, 7)
 		error = np.round(error, 7)
 		output = strings.densityOutput(filename, dotTotal, surveyedArea, density, error, 
 			microscopeImage, userSettings)
 	
-	if (not skipped and saveFigures) or userSettings.reanalysis:
+	if (not skipped and userSettings.saveFigures) or userSettings.reanalysis:
 		outputFilename = targetPath.split("/")[-1]
 		saveDensityFigure(directory, filename, outputFilename, microscopeImage, userSettings)
 	
 	with open(targetPath, "a") as file:
 		file.write(output)
 
 def saveDensityFigure(directory, filename, outputFilename, microscopeImage, userSettings):
-	dotSize = userSettings.dotSize
-	program = userSettings.program
-	
 	data = microscopeImage.data
 	polygon = microscopeImage.polygon
 	dotCoords = microscopeImage.dotCoords
 	blobCoords = microscopeImage.blobCoords
 	
 	for fileExtension in cfg.FIGURE_FILETYPES:
 		figure, axes = pl.subplots()
 		axes.imshow(data, origin="lower", cmap="gray", vmin=userSettings.lowerContrast, 
 			vmax=userSettings.upperContrast * np.std(data), zorder=0)
-		dotScatter = axes.scatter([None], [None], s=5 * dotSize, facecolors="none", 
+		dotScatter = axes.scatter([None], [None], s=5 * userSettings.dotSize, facecolors="none", 
 			edgecolors=cfg.DOT_COLOR, linewidths=cfg.DOT_THICKNESS/2, zorder=4)
 		dotScatter.set_offsets(dotCoords)
 		
 		if cfg.PLOT_BLOBS and blobCoords:
 			blobSize = userSettings.blobSize
 			blobScatter = axes.scatter([None], [None], s=0.1 * blobSize, facecolors="none", 
 				edgecolors=cfg.BLOB_COLOR, linewidths=cfg.BLOB_THICKNESS/2, zorder=3)
@@ -220,15 +236,15 @@
 		if cfg.PLOT_POLYGON:
 			polygonY, polygonX = dp.getYAndXFromCoordList(polygon)
 			underLine, = axes.plot(polygonX, polygonY, linestyle="-", color="k", linewidth=0.75, 
 				zorder=1)
 			line, = axes.plot(polygonX, polygonY, linestyle="-", color=cfg.POLYGON_COLOR, 
 				linewidth=cfg.POLYGON_THICKNESS, zorder=2)
 		
-		targetPath = files.getTargetPath(directory, outputFilename, fileExtension)
+		targetPath = files.getFigureTargetPath(directory, outputFilename, fileExtension)
 		
 		truncatedFilename = ".".join(filename.split(".")[:-1])
 		
 		if fileExtension == "pdf":
 			figure.savefig(f"{targetPath}{truncatedFilename}.{fileExtension}", 
 				bbox_inches="tight", pad_inches=0)
 		else:
```

### Comparing `dotscanner-1.3.2/dotscanner/files.py` & `dotscanner-1.3.3/dotscanner/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,35 +135,16 @@
 	startImageNumber = getTrailingNumber(startImage)
 	filenamesFromStartingImage = []
 	for filename in filenames:
 		if getTrailingNumber(filename) >= startImageNumber:
 			filenamesFromStartingImage.append(filename)
 	return filenamesFromStartingImage
 
-def getTargetPath(directory, outputFilename, fileExtension):
-	figureDirectoryName = cfg.FIGURE_DIRECTORY_NAME
-	if not figureDirectoryName.endswith("/"):
-		figureDirectoryName += "/"
-	
-	figurePathWithoutExtension = f"{directory}{figureDirectoryName}"
-	
-	if not os.path.exists(figurePathWithoutExtension):
-		os.mkdir(figurePathWithoutExtension)
-	
-	figurePath = f"{directory}{figureDirectoryName}{fileExtension}/"
-	
-	if not os.path.exists(figurePath):
-		os.mkdir(figurePath)
-	
-	outputFilenameWithoutExtension = outputFilename.split(".")[0]
-	targetPath = figurePath + f"{outputFilenameWithoutExtension}/"
-	if not os.path.exists(targetPath):
-		os.mkdir(targetPath)
-	
-	return targetPath
+def getAnalysisTargetPath(directory, filename):
+	return directory + filename
 
 def getReanalysisTargetPath(directory, filename):
 	targetPath = directory + filename
 	while os.path.exists(targetPath):
 		targetPath = incrementTargetPathName(targetPath)
 	return targetPath
 
@@ -191,15 +172,37 @@
 			continue
 		
 		if not periodReached:
 			continue
 		
 		return char.isdigit()
 
-def getTargetPathForLifetimeHistogram(directory):
+def getFigureTargetPath(directory, outputFilename, fileExtension):
+	figureDirectoryName = cfg.FIGURE_DIRECTORY_NAME
+	if not figureDirectoryName.endswith("/"):
+		figureDirectoryName += "/"
+	
+	figurePathWithoutExtension = f"{directory}{figureDirectoryName}"
+	
+	if not os.path.exists(figurePathWithoutExtension):
+		os.mkdir(figurePathWithoutExtension)
+	
+	figurePath = f"{directory}{figureDirectoryName}{fileExtension}/"
+	
+	if not os.path.exists(figurePath):
+		os.mkdir(figurePath)
+	
+	outputFilenameWithoutExtension = outputFilename.split(".")[0]
+	targetPath = figurePath + f"{outputFilenameWithoutExtension}/"
+	if not os.path.exists(targetPath):
+		os.mkdir(targetPath)
+	
+	return targetPath
+
+def getLifetimeHistogramTargetPath(directory):
 	figureDirectoryName = cfg.FIGURE_DIRECTORY_NAME
 	if not figureDirectoryName.endswith("/"):
 		figureDirectoryName += "/"
 	
 	figurePath = f"{directory}{figureDirectoryName}/"
 	
 	if not os.path.exists(figurePath):
```

### Comparing `dotscanner-1.3.2/dotscanner/lifetime.py` & `dotscanner-1.3.3/dotscanner/lifetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 	saveLifetimeDataFiles(directory, lifetimes, resultCoords, startImages, displacements,
 		imageNumberToCoordMap, imageNumberToBlobCoordMap, imageNumberToFilenameMap, 
 		middleMicroscopeImage, userSettings, coordsToPlot, middleMicroscopeImage.polygon)
 
 def saveLifetimeDataFiles(directory, lifetimes, resultCoords, startImages, displacements, 
 	imageNumberToCoordMap, imageNumberToBlobCoordMap, imageNumberToFilenameMap, microscopeImage, 
 	userSettings, coordsToPlot, polygon):
-	if userSettings.polygon: # A polygon from a previous analysis was used
+	if userSettings.reanalysis:
 		targetPath = files.getReanalysisTargetPath(directory, cfg.LIFETIME_OUTPUT_FILENAME)
 	else:
 		targetPath = directory + cfg.LIFETIME_OUTPUT_FILENAME
 		if os.path.exists(targetPath):
 			os.remove(targetPath)
 	
 	with open(targetPath, "a") as file:
@@ -186,15 +186,15 @@
 			if cfg.PLOT_POLYGON:
 				polygonY, polygonX = dp.getYAndXFromCoordList(polygon)
 				underLine, = axes.plot(polygonX, polygonY, linestyle="-", color="k", linewidth=0.75, 
 					zorder=1)
 				line, = axes.plot(polygonX, polygonY, linestyle="-", color=cfg.POLYGON_COLOR, 
 					linewidth=cfg.POLYGON_THICKNESS, zorder=2)
 			
-			targetPath = files.getTargetPath(directory, outputFilename, fileExtension)
+			targetPath = files.getFigureTargetPath(directory, outputFilename, fileExtension)
 			truncatedFilename = ".".join(filename.split(".")[:-1])
 			
 			if fileExtension == "pdf":
 				figure.savefig(f"{targetPath}{truncatedFilename}.{fileExtension}", 
 					bbox_inches="tight", pad_inches=0)
 			else:
 				figure.savefig(f"{targetPath}{truncatedFilename}.{fileExtension}", 
@@ -225,15 +225,15 @@
 	else:
 		maxCounts = max(histData[0])
 		for i in range(plotBins - 1):
 			if histData[0][i] == maxCounts:
 				axes.text(i+1, histData[0][i] + yOffset, int(histData[0][i]), fontsize=6, color="C1", horizontalalignment="center")
 				break
 
-	targetPath = files.getTargetPathForLifetimeHistogram(directory)
+	targetPath = files.getLifetimeHistogramTargetPath(directory)
 	outputFilenameWithoutExtension = outputFilename.split(".")[0]
 	figure.savefig(f"{targetPath}{outputFilenameWithoutExtension}_hist.pdf")
 
 	figure.clf()
 	pl.close(figure)
 
 def updateLifetimeResults(imageNumber, y, x, lifetimes, resultCoords, startImages, displacements,
```

### Comparing `dotscanner-1.3.2/dotscanner/strings.py` & `dotscanner-1.3.3/dotscanner/strings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/dotscanner/ui/DefaultUserSettingsEditor.py` & `dotscanner-1.3.3/dotscanner/ui/DefaultUserSettingsEditor.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/dotscanner/ui/DialogWindow.py` & `dotscanner-1.3.3/dotscanner/ui/DialogWindow.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/dotscanner/ui/MicroscopeImage.py` & `dotscanner-1.3.3/dotscanner/ui/MicroscopeImage.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import dotscanner.strings as strings
 import dotscanner.ui.window as ui
 import settings.config as cfg
 
 class MicroscopeImage:
 	def __init__(self, directory, filename, userSettings):
 		self.memoizedCoords = {}
-		self.polygon = [] # Vertices of the region selected for analysis (mutated by other classes)
-		self.skipped = False # Whether the image should be skipped (mutated by other classes)
+		self.polygon = self.getPolygon(filename, userSettings)
+		self.skipped = False # Whether analysis should be skipped for this image
 		
 		self.userSettings = userSettings
 		self.thresholds = userSettings.thresholds
 		self.lowerDotThreshScale = self.thresholds[0]
 		self.upperDotThreshScale = self.thresholds[1]
 		self.lowerBlobThreshScale = self.thresholds[2]
 		
@@ -44,14 +44,22 @@
 			dotCoords, blobCoords = dp.getCoords(self.data, self.sums, self.thresholds, 
 				self.userSettings.dotSize)
 			dp.cleanDotCoords(self.data, dotCoords, blobCoords, self.userSettings.blobSize, 
 				self.userSettings.dotSize)
 			self.memoizedCoords[combination] = (dotCoords, blobCoords)
 		return dotCoords, blobCoords
 	
+	def getPolygon(self, filename, userSettings):
+		if userSettings.polygon:
+			return userSettings.polygon
+		elif userSettings.densityData:
+			return userSettings.densityData[filename][7]
+		else:
+			return []
+	
 	def increaseLowerDotThreshScale(self):
 		value = self.lowerDotThreshScale + cfg.THRESHOLD_DELTA
 		value = round(value, 1)
 		if value > self.upperDotThreshScale:
 			print(strings.upperDotThreshScaleWarning)
 			return
 		self.lowerDotThreshScale = value
```

### Comparing `dotscanner-1.3.2/dotscanner/ui/RegionSelector.py` & `dotscanner-1.3.3/dotscanner/ui/RegionSelector.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,18 @@
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 import tkinter as tk
 
 class RegionSelector:
 	def __init__(self, microscopeImage, userSettings, skipButton=True):
 		ui.setupWindow()
 		
+		self.xList, self.yList = [], []
+		self.drawingBlocked = False
 		if userSettings.reanalysis:
-			if userSettings.polygon is None:
-				raise Exception(strings.invalidPolygonWarning)
-			self.xList, self.yList = userSettings.polygon
-			self.drawingBlocked = True
-		
-		else:
-			self.xList, self.yList = [], []
-			self.drawingBlocked = False
+			self.setPolygonData(microscopeImage)
 		
 		self.image = microscopeImage
 		self.window = ui.createPlotWindow(strings.regionSelectorWindowTitle)
 		
 		self.figure, self.axes, _, self.dotScatter, self.blobScatter = ui.createPlots(
 			self.image.data, userSettings)
 		
@@ -101,22 +96,23 @@
 			self.underLine.set_data([self.xList + [self.xList[0]], self.yList + [self.yList[0]]])
 			self.dottedLine.set_data([[self.xList[0], self.xList[-1]], [self.yList[0], 
 				self.yList[-1]]])
 		self.underLine.figure.canvas.draw_idle()
 		self.line.figure.canvas.draw_idle()
 	
 	def finish(self):
-		if len(self.xList) > 2: # If a valid enclosed polygon was drawn
-			self.xList.append(self.xList[0]) # Enclose the polygon to the beginning vertex
-			self.yList.append(self.yList[0])
-			for y, x in zip(self.yList, self.xList):
-				self.image.polygon.append([int(round(y, 0)), int(round(x, 0))])
-		
-		else: # An invalid polygon was drawn
-			print(strings.invalidPolygonWarning)
+		if not self.image.polygon:
+			if len(self.xList) > 2: # If a valid enclosed polygon was drawn
+				self.xList.append(self.xList[0]) # Enclose the polygon to the beginning vertex
+				self.yList.append(self.yList[0])
+				for y, x in zip(self.yList, self.xList):
+					self.image.polygon.append([int(round(y, 0)), int(round(x, 0))])
+			
+			else: # An invalid polygon was drawn
+				print(strings.invalidPolygonWarning)
 		
 		self.line.figure.canvas.mpl_disconnect(self.connectId)
 		self.window.destroy()
 		self.window.after(100, self.window.quit)
 	
 	def finishWithReturnKey(self, event):
 		self.finish()
@@ -140,14 +136,23 @@
 	
 	def restartclickMarker(self):
 		self.clickMarkerBackdrop.set_offsets([None, None])
 		self.clickMarker.set_offsets([None, None])
 		self.clickMarkerBackdrop.figure.canvas.draw_idle()
 		self.clickMarker.figure.canvas.draw_idle()
 	
+	def setPolygonData(self, microscopeImage):
+		if not microscopeImage.polygon:
+			raise Exception(strings.invalidPolygonWarning)
+		for pair in microscopeImage.polygon:
+			y, x = pair
+			self.xList.append(x)
+			self.yList.append(y)
+		self.drawingBlocked = True
+	
 	def skip(self):
 		self.image.skipped = True
 		self.window.destroy()
 		self.window.quit()
 	
 	def skipWithEscapeKey(self, event):
 		self.skip()
```

### Comparing `dotscanner-1.3.2/dotscanner/ui/ThresholdAdjuster.py` & `dotscanner-1.3.3/dotscanner/ui/ThresholdAdjuster.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,23 +155,23 @@
 		self.editButton.pack(in_=self.thresholdEditItem, side=tk.TOP)
 		self.resetButton.pack(in_=self.thresholdEditItem, side=tk.TOP)
 		
 		self.editSpacer = tk.Label(self.window, text="---------", fg="lightgray")
 		
 		self.entryThresholdLabel1 = tk.Label(self.window, text="Dot lower:")
 		self.entryThreshold1 = tk.Entry(self.window, width=5)
-		self.entryThreshold1.insert(0, userSettings.lowerDotThresh)
+		self.entryThreshold1.insert(0, userSettings.lowerDotThresh) # Default value
 		
 		self.entryThresholdLabel2 = tk.Label(self.window, text="Dot upper:")
 		self.entryThreshold2 = tk.Entry(self.window, width=5)
-		self.entryThreshold2.insert(0, userSettings.upperDotThresh)
+		self.entryThreshold2.insert(0, userSettings.upperDotThresh) # Default value
 		
 		self.entryThresholdLabel3 = tk.Label(self.window, text="Blob lower:")
 		self.entryThreshold3 = tk.Entry(self.window, width=5)
-		self.entryThreshold3.insert(0, userSettings.lowerBlobThresh)
+		self.entryThreshold3.insert(0, userSettings.lowerBlobThresh) # Default value
 		
 		self.entryDotSizeLabel = tk.Label(self.window, text="Dot size:")
 		self.entryDotSize = tk.Entry(self.window, width=5)
 		self.entryDotSize.insert(0, userSettings.dotSize)
 		
 		self.entryBlobSizeLabel = tk.Label(self.window, text="Blob size:")
 		self.entryBlobSize = tk.Entry(self.window, width=5)
```

### Comparing `dotscanner-1.3.2/dotscanner/ui/UserSettings.py` & `dotscanner-1.3.3/dotscanner/ui/UserSettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,17 +313,19 @@
 					continue
 				
 				if lineArray[1] == "Generated":
 					programString = lineArray[5]
 					if programString == "density":
 						self.program = ProgramType.DENSITY
 						self.parseDensityFile(chosenFile)
+						return
 					else:
 						self.program = ProgramType.LIFETIME
 						self.parseLifetimeFile(chosenFile)
+						return
 		
 		print(strings.invalidAnalysisFileWarning(chosenFile))
 	
 	def parseDensityFile(self, chosenFile):
 		self.filepath = os.path.dirname(chosenFile)
 		with open(chosenFile, "r") as file:
 			for line in file:
@@ -343,44 +345,44 @@
 				lowerContrast = round(float(splitLine[10]), 1)
 				upperContrast = round(float(splitLine[11]), 1)
 				polygonString = line.split("(")[1:]
 				polygonPairsStringArray = [item.split(")")[0] for item in polygonString]
 				polygon = []
 				for pair in polygonPairsStringArray:
 					x, y = pair.split(",")
-					polygon.append([int(y), int(x)]) # More convenient shape for densities
+					polygon.append([int(y), int(x)])
 				polygon.append([polygon[0][0], polygon[0][1]])
 				
 				self.densityData[filename] = [lowerDotThreshScale, upperDotThreshScale, 
 				lowerBlobThreshScale, blobSize, dotSize, lowerContrast, upperContrast, polygon]
 		
 		self.reanalysis = True			
 		self.window.destroy()
 		self.window.quit()
 	
 	def parseLifetimeFile(self, chosenFile):
 		self.filepath = os.path.dirname(chosenFile)
-		self.polygon = [[], []]
 		with open(chosenFile, "r") as file:
 			for line in file:
 				if not line.startswith("#"): # Only read the header
 					break
 				
 				lineArray = line.split()
 				if len(lineArray) < 3:
 					continue
 				
 				if lineArray[1] == "Polygon":
+					self.polygon = []
 					polygonData = line.split(":")[1].split(")")
 					for item in polygonData:
 						polygonDataArray = item.split("(")
 						if len(polygonDataArray) > 1:
 							x, y = polygonDataArray[1].split(",")
-							self.polygon[0].append(int(x)) # More convenient shape for lifetimes
-							self.polygon[1].append(int(y))
+							self.polygon.append([int(y), int(x)])
+					self.polygon.append([self.polygon[0][0], self.polygon[0][1]])
 				
 				elif lineArray[1] == "Threshold":
 					parsedThresholds = [float(value) for value in line.split(":")[1].split(",")]
 					self.lowerDotThresh = round(parsedThresholds[0], 1)
 					self.upperDotThresh = round(parsedThresholds[1], 1)
 					self.lowerBlobThresh = round(parsedThresholds[2], 1)
 					self.thresholds = (self.lowerDotThresh, self.upperDotThresh, self.lowerBlobThresh)
```

### Comparing `dotscanner-1.3.2/dotscanner/ui/window.py` & `dotscanner-1.3.3/dotscanner/ui/window.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/dotscanner.egg-info/PKG-INFO` & `dotscanner-1.3.3/dotscanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.3.2
+Version: 1.3.3
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -148,15 +148,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.2
+* 1.3.3
      * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
```

### Comparing `dotscanner-1.3.2/dotscanner.egg-info/SOURCES.txt` & `dotscanner-1.3.3/dotscanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/settings/config.py` & `dotscanner-1.3.3/settings/config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -124,8 +124,8 @@
 FIGURE_DIRECTORY_NAME = "figures/"
 # The directory name where figures are to be saved (only if SAVE_FIGURES = True). The default is "figures/", but this can be changed if the user typically keeps a similarly named folder in their file structure for something else.
 
 FIGURE_FILETYPES = ["pdf"]
 # The filetypes for the output figures. Multiple types can also be selected, e.g., ["png", "pdf", "tif"]. Only use the supported filetypes ("eps", "tif", "ps", "tiff", "rgba", "svg", "png", "jpg", "raw", "pdf", "svgz", "pgf", and "jpeg").
 
 FIGURE_RESOLUTION = 300
-# Resolution (DPI) of the output figures. This is for images only; PDF outputs are unaffected by this value.
+# Resolution (DPI) of the output figures. This is for images only; PDF outputs are unaffected by this value.
```

### Comparing `dotscanner-1.3.2/settings/configmanagement.py` & `dotscanner-1.3.3/settings/configmanagement.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/setup.py` & `dotscanner-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='dotscanner',
-    version='1.3.2', # Required 
+    version='1.3.3', # Required 
     description='A program designed for analysis of microscope imaging data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/dotscanner',
     author='Holly Allen and Brian Davis',
     author_email='holly.allen@colorado.edu',
     classifiers=[
```

### Comparing `dotscanner-1.3.2/tests/test_dataprocessing.py` & `dotscanner-1.3.3/tests/test_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/tests/test_density.py` & `dotscanner-1.3.3/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/tests/test_files.py` & `dotscanner-1.3.3/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/tests/test_lifetime.py` & `dotscanner-1.3.3/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/tests/test_strings.py` & `dotscanner-1.3.3/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/tests/ui/FakeUserSettings.py` & `dotscanner-1.3.3/tests/ui/FakeUserSettings.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
         self.thresholds = thresholds
         self.lowerContrast = lowerContrast
         self.upperContrast = upperContrast
         self.lowerDotThresh = lowerDotThresh
         self.upperDotThresh = upperDotThresh
         self.lowerBlobThresh = lowerBlobThresh
         self.program = program
-        self.polygon = polygon
+        self.polygon = polygon
```

### Comparing `dotscanner-1.3.2/tests/ui/test_MicroscopeImage.py` & `dotscanner-1.3.3/tests/ui/test_MicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.2/tests/ui/test_ThresholdAdjuster.py` & `dotscanner-1.3.3/tests/ui/test_ThresholdAdjuster.py`

 * *Files 19% similar despite different names*

```diff
@@ -61,31 +61,26 @@
 		thresholdAdjuster.canvas.draw = MagicMock(return_value=None)
 		
 		# Expected offsets = [[6, 5], [11, 9]]
 		dotOffsets = thresholdAdjuster.dotScatter.get_offsets()
 		
 		self.assertEqual(microscopeImage.thresholds, (1.2, 1.8, 1.3))
 		self.assertEqual(len(dotOffsets), 2)
-		for offset in dotOffsets:
-			x, y = offset
-			if x == 6:
-				self.assertEqual(y, 5)
-			else:
-				self.assertEqual(y, 9)
+		self.assertIn([6, 5], dotOffsets)
+		self.assertIn([11, 9], dotOffsets)
+		self.assertEqual(len(dotOffsets), 2)
 		
 		thresholdAdjuster.upperDotThresholdScaleDown()
 		
 		# Expected offsets = [[6, 4]]
 		dotOffsets2 = thresholdAdjuster.dotScatter.get_offsets()
 		
 		self.assertEqual(microscopeImage.thresholds, (1.2, 1.7, 1.3))
 		self.assertEqual(len(dotOffsets2), 1)
-		x, y = dotOffsets2[0]
-		self.assertEqual(x, 6)
-		self.assertEqual(y, 4)
+		self.assertIn([6, 4], dotOffsets2)
 	
 	def test_upperDotThresholdScaleUp(self):
 		# This is the inverse of the previous test, scaling down first, and then back up
 		
 		microscopeImage, fakeUserSettings = self.getMicroscopeImageAndUserSettings()
 		thresholdAdjuster = ThresholdAdjuster(microscopeImage, fakeUserSettings, drawUi=False)
 		thresholdAdjuster.setThresholdEntries = MagicMock(return_value=None)
@@ -94,31 +89,25 @@
 		thresholdAdjuster.upperDotThresholdScaleDown()
 		
 		# Expected offsets = [[6, 4]]
 		dotOffsets = thresholdAdjuster.dotScatter.get_offsets()
 		
 		self.assertEqual(microscopeImage.thresholds, (1.2, 1.7, 1.3))
 		self.assertEqual(len(dotOffsets), 1)
-		x, y = dotOffsets[0]
-		self.assertEqual(x, 6)
-		self.assertEqual(y, 4)
+		self.assertIn([6, 4], dotOffsets)
 		
 		thresholdAdjuster.upperDotThresholdScaleUp()
 		
 		# Expected offsets = [[6, 5], [11, 9]]
 		dotOffsets2 = thresholdAdjuster.dotScatter.get_offsets()
 		
 		self.assertEqual(microscopeImage.thresholds, (1.2, 1.8, 1.3))
 		self.assertEqual(len(dotOffsets2), 2)
-		for offset in dotOffsets2:
-			x, y = offset
-			if x == 6:
-				self.assertEqual(y, 5)
-			else:
-				self.assertEqual(y, 9)
+		self.assertIn([6, 5], dotOffsets2)
+		self.assertIn([11, 9], dotOffsets2)
 	
 	def test_lowerDotThresholdScaleDown(self):
 		'''getFullDataSquareSum generates the following from the given test data:
  		[[ 6  6  2  0  1 -1 -2 -4 -2 -1  0  0  0]
 		 [ 6  6  2  0  1 -1 -2 -6 -4 -1  2  2  0]
 		 [ 4  4  2  0  1  1  0 -4 -4 -1  2  2  0]
 		 [-1 -1  0  0  0  1  1 -1 -2  0  2  2  0]
@@ -145,36 +134,27 @@
 		thresholdAdjuster.canvas.draw = MagicMock(return_value=None)
 		
 		# Expected offsets = [[6, 5], [11, 9]]
 		dotOffsets = thresholdAdjuster.dotScatter.get_offsets()
 		
 		self.assertEqual(microscopeImage.thresholds, (1.2, 1.8, 1.3))
 		self.assertEqual(len(dotOffsets), 2)
-		for offset in dotOffsets:
-			x, y = offset
-			if x == 6:
-				self.assertEqual(y, 5)
-			else:
-				self.assertEqual(y, 9)
+		self.assertIn([6, 5], dotOffsets)
+		self.assertIn([11, 9], dotOffsets)
 		
 		thresholdAdjuster.lowerDotThresholdScaleDown()
 		
 		# Expected offsets = [[0, 0], [6, 5], [11, 9]]
 		dotOffsets2 = thresholdAdjuster.dotScatter.get_offsets()
 		
 		self.assertEqual(microscopeImage.thresholds, (1.1, 1.8, 1.3))
 		self.assertEqual(len(dotOffsets2), 3)
-		for offset in dotOffsets2:
-			x, y = offset
-			if x == 0:
-				self.assertEqual(y, 0)
-			elif x == 6:
-				self.assertEqual(y, 5)
-			else:
-				self.assertEqual(y, 9)
+		self.assertIn([0, 0], dotOffsets2)
+		self.assertIn([6, 5], dotOffsets2)
+		self.assertIn([11, 9], dotOffsets2)
 	
 	def test_lowerDotThresholdScaleUp(self):
 		# This is the inverse of the previous test, scaling down first, and then back up
 		
 		microscopeImage, fakeUserSettings = self.getMicroscopeImageAndUserSettings()
 		thresholdAdjuster = ThresholdAdjuster(microscopeImage, fakeUserSettings, drawUi=False)
 		thresholdAdjuster.setThresholdEntries = MagicMock(return_value=None)
@@ -183,32 +163,23 @@
 		thresholdAdjuster.lowerDotThresholdScaleDown()
 		
 		# Expected offsets = [[0, 0], [6, 5], [11, 9]]
 		dotOffsets = thresholdAdjuster.dotScatter.get_offsets()
 		
 		self.assertEqual(microscopeImage.thresholds, (1.1, 1.8, 1.3))
 		self.assertEqual(len(dotOffsets), 3)
-		for offset in dotOffsets:
-			x, y = offset
-			if x == 0:
-				self.assertEqual(y, 0)
-			elif x == 6:
-				self.assertEqual(y, 5)
-			else:
-				self.assertEqual(y, 9)
+		self.assertIn([0, 0], dotOffsets)
+		self.assertIn([6, 5], dotOffsets)
+		self.assertIn([11, 9], dotOffsets)
 		
 		thresholdAdjuster.lowerDotThresholdScaleUp()
 		
 		# Expected offsets = [[6, 5], [11, 9]]
 		dotOffsets2 = thresholdAdjuster.dotScatter.get_offsets()
 		
 		self.assertEqual(microscopeImage.thresholds, (1.2, 1.8, 1.3))
 		self.assertEqual(len(dotOffsets2), 2)
-		for offset in dotOffsets2:
-			x, y = offset
-			if x == 6:
-				self.assertEqual(y, 5)
-			else:
-				self.assertEqual(y, 9)
+		self.assertIn([6, 5], dotOffsets2)
+		self.assertIn([11, 9], dotOffsets2)
 
 if __name__ == '__main__':
 	unittest.main()
```

