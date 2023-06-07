# Comparing `tmp/dotscanner-1.3.3.tar.gz` & `tmp/dotscanner-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dotscanner-1.3.3.tar", last modified: Wed Jun  7 02:15:20 2023, max compression
+gzip compressed data, was "dist/dotscanner-1.3.4.tar", last modified: Wed Jun  7 06:19:21 2023, max compression
```

## Comparing `dotscanner-1.3.3.tar` & `dotscanner-1.3.4.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.578862 dotscanner-1.3.3/
--rw-r--r--   0 holly      (501) staff       (20)     1103 2023-06-05 02:24:39.000000 dotscanner-1.3.3/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)    13417 2023-06-07 02:15:20.578693 dotscanner-1.3.3/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)    12762 2023-06-06 20:52:08.000000 dotscanner-1.3.3/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.574162 dotscanner-1.3.3/dotscanner/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.3/dotscanner/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     2755 2023-06-07 01:30:16.000000 dotscanner-1.3.3/dotscanner/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)    10277 2023-06-06 23:47:07.000000 dotscanner-1.3.3/dotscanner/dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)    10148 2023-06-07 01:30:15.000000 dotscanner-1.3.3/dotscanner/density.py
--rw-r--r--   0 holly      (501) staff       (20)     6212 2023-06-06 23:47:08.000000 dotscanner-1.3.3/dotscanner/files.py
--rw-r--r--   0 holly      (501) staff       (20)    10454 2023-06-07 00:24:19.000000 dotscanner-1.3.3/dotscanner/lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     6692 2023-06-06 23:47:10.000000 dotscanner-1.3.3/dotscanner/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.576466 dotscanner-1.3.3/dotscanner/ui/
--rw-r--r--   0 holly      (501) staff       (20)     5179 2023-06-06 23:47:11.000000 dotscanner-1.3.3/dotscanner/ui/DefaultUserSettingsEditor.py
--rw-r--r--   0 holly      (501) staff       (20)     1858 2023-06-06 23:47:12.000000 dotscanner-1.3.3/dotscanner/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     3510 2023-06-07 01:30:18.000000 dotscanner-1.3.3/dotscanner/ui/MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     5733 2023-06-07 01:30:17.000000 dotscanner-1.3.3/dotscanner/ui/RegionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)    16388 2023-06-07 02:08:45.000000 dotscanner-1.3.3/dotscanner/ui/ThresholdAdjuster.py
--rw-r--r--   0 holly      (501) staff       (20)    15070 2023-06-07 01:30:16.000000 dotscanner-1.3.3/dotscanner/ui/UserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.3/dotscanner/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3097 2023-06-06 23:47:14.000000 dotscanner-1.3.3/dotscanner/ui/window.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.575011 dotscanner-1.3.3/dotscanner.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)    13417 2023-06-07 02:15:20.000000 dotscanner-1.3.3/dotscanner.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)     1000 2023-06-07 02:15:20.000000 dotscanner-1.3.3/dotscanner.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-06-07 02:15:20.000000 dotscanner-1.3.3/dotscanner.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       56 2023-06-07 02:15:20.000000 dotscanner-1.3.3/dotscanner.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       17 2023-06-07 02:15:20.000000 dotscanner-1.3.3/dotscanner.egg-info/requires.txt
--rw-r--r--   0 holly      (501) staff       (20)       26 2023-06-07 02:15:20.000000 dotscanner-1.3.3/dotscanner.egg-info/top_level.txt
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.576915 dotscanner-1.3.3/settings/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.3/settings/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     6219 2023-06-06 20:41:22.000000 dotscanner-1.3.3/settings/config.py
--rw-r--r--   0 holly      (501) staff       (20)    11284 2023-06-05 02:24:39.000000 dotscanner-1.3.3/settings/configmanagement.py
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-06-07 02:15:20.578927 dotscanner-1.3.3/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1444 2023-06-07 02:15:20.000000 dotscanner-1.3.3/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.577782 dotscanner-1.3.3/tests/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.3/tests/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)    10018 2023-06-05 02:24:39.000000 dotscanner-1.3.3/tests/test_dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     5572 2023-06-05 02:24:39.000000 dotscanner-1.3.3/tests/test_density.py
--rw-r--r--   0 holly      (501) staff       (20)    13472 2023-06-05 02:24:39.000000 dotscanner-1.3.3/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)    10886 2023-06-05 02:24:39.000000 dotscanner-1.3.3/tests/test_lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     5884 2023-06-05 04:38:07.000000 dotscanner-1.3.3/tests/test_strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 02:15:20.578450 dotscanner-1.3.3/tests/ui/
--rw-r--r--   0 holly      (501) staff       (20)      471 2023-06-07 02:08:44.000000 dotscanner-1.3.3/tests/ui/FakeMicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)      964 2023-06-07 02:08:43.000000 dotscanner-1.3.3/tests/ui/FakeUserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.3/tests/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     4000 2023-06-07 01:30:21.000000 dotscanner-1.3.3/tests/ui/test_MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     8046 2023-06-07 02:08:46.000000 dotscanner-1.3.3/tests/ui/test_ThresholdAdjuster.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.222840 dotscanner-1.3.4/
+-rw-r--r--   0 holly      (501) staff       (20)     1103 2023-06-05 02:24:39.000000 dotscanner-1.3.4/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)    13417 2023-06-07 06:19:21.222635 dotscanner-1.3.4/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)    12762 2023-06-07 06:18:08.000000 dotscanner-1.3.4/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.217968 dotscanner-1.3.4/dotscanner/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.4/dotscanner/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     2755 2023-06-07 06:04:06.000000 dotscanner-1.3.4/dotscanner/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)    10277 2023-06-06 23:47:07.000000 dotscanner-1.3.4/dotscanner/dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)    10147 2023-06-07 06:04:08.000000 dotscanner-1.3.4/dotscanner/density.py
+-rw-r--r--   0 holly      (501) staff       (20)     6212 2023-06-07 06:04:08.000000 dotscanner-1.3.4/dotscanner/files.py
+-rw-r--r--   0 holly      (501) staff       (20)    10595 2023-06-07 06:04:07.000000 dotscanner-1.3.4/dotscanner/lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     6692 2023-06-06 23:47:10.000000 dotscanner-1.3.4/dotscanner/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.219983 dotscanner-1.3.4/dotscanner/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     5179 2023-06-06 23:47:11.000000 dotscanner-1.3.4/dotscanner/ui/DefaultUserSettingsEditor.py
+-rw-r--r--   0 holly      (501) staff       (20)     1858 2023-06-06 23:47:12.000000 dotscanner-1.3.4/dotscanner/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     3510 2023-06-07 03:30:32.000000 dotscanner-1.3.4/dotscanner/ui/MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     5764 2023-06-07 06:04:13.000000 dotscanner-1.3.4/dotscanner/ui/RegionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)    16392 2023-06-07 06:12:10.000000 dotscanner-1.3.4/dotscanner/ui/ThresholdAdjuster.py
+-rw-r--r--   0 holly      (501) staff       (20)    15070 2023-06-07 06:04:14.000000 dotscanner-1.3.4/dotscanner/ui/UserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.4/dotscanner/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3097 2023-06-06 23:47:14.000000 dotscanner-1.3.4/dotscanner/ui/window.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.218858 dotscanner-1.3.4/dotscanner.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)    13417 2023-06-07 06:19:21.000000 dotscanner-1.3.4/dotscanner.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)     1050 2023-06-07 06:19:21.000000 dotscanner-1.3.4/dotscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-06-07 06:19:21.000000 dotscanner-1.3.4/dotscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       56 2023-06-07 06:19:21.000000 dotscanner-1.3.4/dotscanner.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       17 2023-06-07 06:19:21.000000 dotscanner-1.3.4/dotscanner.egg-info/requires.txt
+-rw-r--r--   0 holly      (501) staff       (20)       26 2023-06-07 06:19:21.000000 dotscanner-1.3.4/dotscanner.egg-info/top_level.txt
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.220538 dotscanner-1.3.4/settings/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.4/settings/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     6219 2023-06-06 20:41:22.000000 dotscanner-1.3.4/settings/config.py
+-rw-r--r--   0 holly      (501) staff       (20)    11284 2023-06-05 02:24:39.000000 dotscanner-1.3.4/settings/configmanagement.py
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-06-07 06:19:21.222900 dotscanner-1.3.4/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1444 2023-06-07 06:19:20.000000 dotscanner-1.3.4/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.221579 dotscanner-1.3.4/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.4/tests/__init__.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.221739 dotscanner-1.3.4/tests/data/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.4/tests/data/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)    10018 2023-06-05 02:24:39.000000 dotscanner-1.3.4/tests/test_dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     5619 2023-06-07 06:18:09.000000 dotscanner-1.3.4/tests/test_density.py
+-rw-r--r--   0 holly      (501) staff       (20)    13472 2023-06-07 06:04:11.000000 dotscanner-1.3.4/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)     6341 2023-06-07 06:18:10.000000 dotscanner-1.3.4/tests/test_fullAnalysis.py
+-rw-r--r--   0 holly      (501) staff       (20)    10886 2023-06-05 02:24:39.000000 dotscanner-1.3.4/tests/test_lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     5740 2023-06-07 03:30:33.000000 dotscanner-1.3.4/tests/test_strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.222383 dotscanner-1.3.4/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)      487 2023-06-07 03:30:33.000000 dotscanner-1.3.4/tests/ui/FakeMicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     1086 2023-06-07 06:04:14.000000 dotscanner-1.3.4/tests/ui/FakeUserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.4/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     4099 2023-06-07 03:02:28.000000 dotscanner-1.3.4/tests/ui/test_MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     8287 2023-06-07 06:12:11.000000 dotscanner-1.3.4/tests/ui/test_ThresholdAdjuster.py
```

### Comparing `dotscanner-1.3.3/LICENSE` & `dotscanner-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/PKG-INFO` & `dotscanner-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.3.3
+Version: 1.3.4
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
 
-* 1.3.3
+* 1.3.4
      * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
```

### Comparing `dotscanner-1.3.3/README.md` & `dotscanner-1.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.3
+* 1.3.4
      * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
```

### Comparing `dotscanner-1.3.3/dotscanner/__main__.py` & `dotscanner-1.3.4/dotscanner/__main__.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/dotscanner/dataprocessing.py` & `dotscanner-1.3.4/dotscanner/dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/dotscanner/density.py` & `dotscanner-1.3.4/dotscanner/density.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 	targetPath = files.getReanalysisTargetPath(directory, cfg.DENSITY_OUTPUT_FILENAME)
 	adjustmentsMade = False
 	
 	numberOfFiles = len(list(userSettings.densityData.keys()))
 	count = 0
 	for filename, data in userSettings.densityData.items():
 		microscopeImage = MicroscopeImage(directory, filename, userSettings)
-				
+			
 		if not adjustmentsMade:
 			thresholdAdjuster = ThresholdAdjuster(microscopeImage, userSettings)
 			
 			print("Re-analyzing images...")
 			ui.printProgressBar(0, numberOfFiles)
 			
 			userSettings = thresholdAdjuster.userSettings # Updating with the threshold adjustments
```

### Comparing `dotscanner-1.3.3/dotscanner/files.py` & `dotscanner-1.3.4/dotscanner/files.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/dotscanner/lifetime.py` & `dotscanner-1.3.4/dotscanner/lifetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 	firstFrameOfBackEdge = list(imageNumberToCoordMap.keys())[-1] - skipsAllowed
 	lastFrame = list(imageNumberToCoordMap.keys())[-1] + 1
 	
 	firstFrames = range(firstFrame, lastFrameOfFrontEdge)
 	lastFrames = range(firstFrameOfBackEdge, lastFrame)
 	return set(list(firstFrames) + list(lastFrames))
 
-def measureLifetime(directory, filenames, middleMicroscopeImage, userSettings):
+def measureLifetime(directory, filenames, middleMicroscopeImage, userSettings, testing=False):
 	if len(middleMicroscopeImage.polygon) < 3:
 		return
 	
 	blobSize = userSettings.blobSize
 	dotSize = userSettings.dotSize
 	skipsAllowed = userSettings.skipsAllowed
 	removeEdgeFrames = userSettings.removeEdgeFrames
@@ -88,30 +88,33 @@
 	xMin, xMax, yMin, yMax = dp.getPolygonLimits(middleMicroscopeImage.polygon)
 	
 	imageNumberToCoordMap = {}
 	imageNumberToBlobCoordMap = {}
 	imageNumberToFilenameMap = {}
 	
 	numberOfFiles = len(filenames)
-	print("Getting coordinates of all dots...")
-	ui.printProgressBar(0, numberOfFiles)
+	if not testing:
+		print("Getting coordinates of all dots...")
+		ui.printProgressBar(0, numberOfFiles)
+	
 	for index, filename in enumerate(filenames):
 		microscopeImage = MicroscopeImage(directory, filename, userSettings)
 		
 		dotCoords, blobCoords = dp.getCoordMapsWithinPolygon(microscopeImage.data, 
 			microscopeImage.sums, lowerDotThresh, upperDotThresh, lowerBlobThresh, dotSize, 
 			middleImagePolygonCoordMap, xMin, xMax, yMin, yMax)
 		dp.cleanDotCoords(microscopeImage.data, dotCoords, blobCoords, blobSize, dotSize)
 		
 		imageNumberToCoordMap[index] = dotCoords
 		imageNumberToFilenameMap[index] = filename
 		if cfg.PLOT_BLOBS:
 			imageNumberToBlobCoordMap[index] = blobCoords
 		
-		ui.printProgressBar(index + 1, numberOfFiles)
+		if not testing:
+			ui.printProgressBar(index + 1, numberOfFiles)
 	
 	lifetimes, resultCoords, startImages, displacements = [], [], [], []
 	edgeFrameNumbers = getEdgeFrameNumbers(imageNumberToCoordMap, skipsAllowed)
 	coordsToPlot = {} # Maps image numbers to coordinate maps for plotting
 	
 	for imageNumber, coordMap in imageNumberToCoordMap.items():
 		if removeEdgeFrames and imageNumber in edgeFrameNumbers:
@@ -121,37 +124,39 @@
 			for x in xSet:
 				updateLifetimeResults(imageNumber, y, x, lifetimes, resultCoords, startImages, 
 					displacements, imageNumberToCoordMap, edgeFrameNumbers, dotSize, skipsAllowed, 
 					removeEdgeFrames, userSettings.saveFigures, coordsToPlot)
 	
 	saveLifetimeDataFiles(directory, lifetimes, resultCoords, startImages, displacements,
 		imageNumberToCoordMap, imageNumberToBlobCoordMap, imageNumberToFilenameMap, 
-		middleMicroscopeImage, userSettings, coordsToPlot, middleMicroscopeImage.polygon)
+		middleMicroscopeImage, userSettings, coordsToPlot, middleMicroscopeImage.polygon, 
+		testing=testing)
 
 def saveLifetimeDataFiles(directory, lifetimes, resultCoords, startImages, displacements, 
 	imageNumberToCoordMap, imageNumberToBlobCoordMap, imageNumberToFilenameMap, microscopeImage, 
-	userSettings, coordsToPlot, polygon):
+	userSettings, coordsToPlot, polygon, testing=False):
 	if userSettings.reanalysis:
 		targetPath = files.getReanalysisTargetPath(directory, cfg.LIFETIME_OUTPUT_FILENAME)
 	else:
-		targetPath = directory + cfg.LIFETIME_OUTPUT_FILENAME
+		targetPath = files.getAnalysisTargetPath(directory, cfg.LIFETIME_OUTPUT_FILENAME)
 		if os.path.exists(targetPath):
 			os.remove(targetPath)
 	
 	with open(targetPath, "a") as file:
 		file.write(strings.lifetimeOutputFileHeader(microscopeImage, userSettings))
 		for lifetime, resultCoord, startImage, displacement in zip(lifetimes, resultCoords, 
 			startImages, displacements):
 			y, x = resultCoord
 			filename = imageNumberToFilenameMap[startImage]
 			output = f"{x} {y} {lifetime} {filename} {displacement}\n"
 			file.write(output)
 	
 	outputFilename = targetPath.split("/")[-1]
-	print(f"{outputFilename} saved.")
+	if not testing:
+		print(f"{outputFilename} saved.")
 	
 	saveHistogram(directory, outputFilename, lifetimes)
 	
 	if userSettings.saveFigures:
 		saveLifetimeFigures(directory, outputFilename, coordsToPlot, imageNumberToBlobCoordMap, 
 							imageNumberToFilenameMap, userSettings, polygon, lifetimes)
```

### Comparing `dotscanner-1.3.3/dotscanner/strings.py` & `dotscanner-1.3.4/dotscanner/strings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/dotscanner/ui/DefaultUserSettingsEditor.py` & `dotscanner-1.3.4/dotscanner/ui/DefaultUserSettingsEditor.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/dotscanner/ui/DialogWindow.py` & `dotscanner-1.3.4/dotscanner/ui/DialogWindow.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/dotscanner/ui/MicroscopeImage.py` & `dotscanner-1.3.4/dotscanner/ui/MicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/dotscanner/ui/RegionSelector.py` & `dotscanner-1.3.4/dotscanner/ui/RegionSelector.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 	def finish(self):
 		if not self.image.polygon:
 			if len(self.xList) > 2: # If a valid enclosed polygon was drawn
 				self.xList.append(self.xList[0]) # Enclose the polygon to the beginning vertex
 				self.yList.append(self.yList[0])
 				for y, x in zip(self.yList, self.xList):
 					self.image.polygon.append([int(round(y, 0)), int(round(x, 0))])
+				print(self.image.polygon)
 			
 			else: # An invalid polygon was drawn
 				print(strings.invalidPolygonWarning)
 		
 		self.line.figure.canvas.mpl_disconnect(self.connectId)
 		self.window.destroy()
 		self.window.after(100, self.window.quit)
```

### Comparing `dotscanner-1.3.3/dotscanner/ui/ThresholdAdjuster.py` & `dotscanner-1.3.4/dotscanner/ui/ThresholdAdjuster.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 class ThresholdAdjuster:
 	def __init__(self, microscopeImage, userSettings, skipButton=True, drawUi=True):
 		self.index = 0
 		self.skipButtonExists = skipButton
 		
 		self.image = microscopeImage
 		self.userSettings = userSettings
+		
 		self.dotSize = userSettings.dotSize
 		self.blobSize = userSettings.blobSize
 		self.defaultThresholds = userSettings.thresholds
 		
 		self.xBounds = [
 			(0,                           len(self.image.data[0]) - 1),
 			(0,                           len(self.image.data[0]) / 2),
```

### Comparing `dotscanner-1.3.3/dotscanner/ui/UserSettings.py` & `dotscanner-1.3.4/dotscanner/ui/UserSettings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/dotscanner/ui/window.py` & `dotscanner-1.3.4/dotscanner/ui/window.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/dotscanner.egg-info/PKG-INFO` & `dotscanner-1.3.4/dotscanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.3.3
+Version: 1.3.4
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
 
-* 1.3.3
+* 1.3.4
      * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
```

### Comparing `dotscanner-1.3.3/dotscanner.egg-info/SOURCES.txt` & `dotscanner-1.3.4/dotscanner.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 settings/__init__.py
 settings/config.py
 settings/configmanagement.py
 tests/__init__.py
 tests/test_dataprocessing.py
 tests/test_density.py
 tests/test_files.py
+tests/test_fullAnalysis.py
 tests/test_lifetime.py
 tests/test_strings.py
+tests/data/__init__.py
 tests/ui/FakeMicroscopeImage.py
 tests/ui/FakeUserSettings.py
 tests/ui/__init__.py
 tests/ui/test_MicroscopeImage.py
 tests/ui/test_ThresholdAdjuster.py
```

### Comparing `dotscanner-1.3.3/settings/config.py` & `dotscanner-1.3.4/settings/config.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/settings/configmanagement.py` & `dotscanner-1.3.4/settings/configmanagement.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/setup.py` & `dotscanner-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='dotscanner',
-    version='1.3.3', # Required 
+    version='1.3.4', # Required 
     description='A program designed for analysis of microscope imaging data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/dotscanner',
     author='Holly Allen and Brian Davis',
     author_email='holly.allen@colorado.edu',
     classifiers=[
```

### Comparing `dotscanner-1.3.3/tests/test_dataprocessing.py` & `dotscanner-1.3.4/tests/test_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/tests/test_density.py` & `dotscanner-1.3.4/tests/test_density.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 			[6, 3],
 			[1, 3],
 			[1, 1]
 		]
 
 		return dp.getCoordsInPolygon(data, points, polygonVertices)
 	
-	@mock.patch("settings.config.DENSITY_OUTPUT_FILENAME", "fakeData.txt")
+	@mock.patch("settings.config.DENSITY_OUTPUT_FILENAME", "data/fakeData.txt")
 	def test_getAlreadyMeasured(self):
 		dir_path = os.path.dirname(os.path.realpath(__file__))
 		directory = dir_path if dir_path.endswith("/") else dir_path + "/"
 		alreadyMeasured = density.getAlreadyMeasured(directory)
 		
 		self.assertEqual(len(alreadyMeasured), 3)
 		self.assertIn("108.TIF", alreadyMeasured)
@@ -94,14 +94,15 @@
 			blobSize, 
 			dotSize, 
 			lowerContrast, 
 			upperContrast, 
 			polygon
 		]
 		microscopeImage = FakeMicroscopeImage(
+			polygon=polygon,
 			lowerDotThreshScale=1.5, 
 			upperDotThreshScale=5.0, 
 			lowerBlobThreshScale=2.0
 		)
 		newUserSettings = FakeUserSettings(
 			dotSize=2, 
 			blobSize=5, 
@@ -125,26 +126,27 @@
 			lowerBlobThresh, 
 			blobSize, 
 			dotSize, 
 			lowerContrast, 
 			upperContrast, 
 			polygon
 		]
-		microscopeImage = FakeMicroscopeImage(
-			lowerDotThreshScale=1.7, 
-			upperDotThreshScale=4.8, 
-			lowerBlobThreshScale=2.0
-		)
 		newUserSettings = FakeUserSettings(
 			dotSize=2, 
 			blobSize=6, 
 			lowerContrast=0.0, 
 			upperContrast=5.5, 
 			polygon=polygon
 		)
+		microscopeImage = FakeMicroscopeImage(
+			polygon=polygon,
+			lowerDotThreshScale=1.7, 
+			upperDotThreshScale=4.8, 
+			lowerBlobThreshScale=2.0
+		)
 		adjustments = density.getReanalysisAdjustments(data, newUserSettings, microscopeImage)
 		
 		self.assertEqual(adjustments[0], 1.7)
 		self.assertEqual(adjustments[1], 4.8)
 		self.assertEqual(adjustments[2], None)
 		self.assertEqual(adjustments[3], 6)
 		self.assertEqual(adjustments[4], None)
```

### Comparing `dotscanner-1.3.3/tests/test_files.py` & `dotscanner-1.3.4/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/tests/test_lifetime.py` & `dotscanner-1.3.4/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.3/tests/test_strings.py` & `dotscanner-1.3.4/tests/test_strings.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,18 @@
         
         self.assertEqual(
             output, 
             f"\nFile test.png already measured in density.txt file. Skipping."
         )
     
     def test_densityOutput(self):
-        polygon = [[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]]
-        thresholds=(1.5, 5.0, 2.0)
-        fakeMicroscopeImage = FakeMicroscopeImage(polygon, thresholds)
         fakeUserSettings = FakeUserSettings(dotSize=2, blobSize=5)
+        fakeMicroscopeImage = FakeMicroscopeImage(
+            polygon=[[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]], lowerDotThreshScale=1.5, 
+            upperDotThreshScale=5.0, lowerBlobThreshScale=2.0)
         output = strings.densityOutput(
             filename="test.png", 
             dotTotal=6,
             surveyedArea=600,
             density=0.01,
             error=0.0001,
             microscopeImage=fakeMicroscopeImage,
@@ -56,23 +56,20 @@
         self.assertEqual(
             strings.outputFileTopHeader(strings.ProgramType.LIFETIME),
             f"# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for lifetime measurement\n#"
         )
     
     def test_lifetimeOutputFileHeader(self):
-        polygon = [[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]]
-        thresholds = (1.5, 5.0, 2.0)
-        fakeMicroscopeImage = FakeMicroscopeImage(polygon, thresholds)
+        fakeMicroscopeImage = FakeMicroscopeImage(
+            polygon=[[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]], lowerDotThreshScale=1.5, 
+            upperDotThreshScale=5.0, lowerBlobThreshScale=2.0)
         fakeUserSettings = FakeUserSettings(
-                                dotSize=2, 
-                                blobSize=5, 
-                                skipsAllowed=1, 
-                                thresholds=(1.5, 5.0, 2.0), 
-                                removeEdgeFrames=True)
+            dotSize=2, blobSize=5, skipsAllowed=1, lowerDotThresh=1.5, upperDotThresh=5.0, 
+            lowerBlobThresh=2.0, removeEdgeFrames=True)
         
         output = strings.lifetimeOutputFileHeader(fakeMicroscopeImage, fakeUserSettings)
         
         self.assertEqual(
             output,
 "# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for lifetime measurement\n\
@@ -93,24 +90,20 @@
 # Remove edge frames: True | Save figures: False | Skips allowed: 1\n\
 #\n\
 # The data columns are organized as follows:\n\
 # x | y | lifetime | starting image | displacement squared (sq px)\n#\n"
         )
     
     def test_lifetimeOutputFileHeaderWithStartImage(self):
-        polygon = [[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]]
-        thresholds = (1.5, 5.0, 2.0)
-        fakeMicroscopeImage = FakeMicroscopeImage(polygon, thresholds)
+        fakeMicroscopeImage = FakeMicroscopeImage(
+            polygon=[[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]], lowerDotThreshScale=1.5, 
+            upperDotThreshScale=5.0, lowerBlobThreshScale=2.0)
         fakeUserSettings = FakeUserSettings(
-                                dotSize=2, 
-                                blobSize=5, 
-                                startImage="path/to/image.png",
-                                skipsAllowed=1, 
-                                thresholds=(1.5, 5.0, 2.0), 
-                                removeEdgeFrames=True)
+            dotSize=2, blobSize=5, startImage="path/to/image.png", skipsAllowed=1, 
+            lowerDotThresh=1.5, upperDotThresh=5.0, lowerBlobThresh=2.0, removeEdgeFrames=True)
         
         output = strings.lifetimeOutputFileHeader(fakeMicroscopeImage, fakeUserSettings)
         
         self.assertEqual(
             output,
 "# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for lifetime measurement\n\
```

### Comparing `dotscanner-1.3.3/tests/ui/FakeUserSettings.py` & `dotscanner-1.3.4/tests/ui/FakeUserSettings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 class FakeUserSettings:
     def __init__(self, filepath="test/directory/", dotSize=2, blobSize=5, saveFigures=False, 
-        startImage="", skipsAllowed=0, removeEdgeFrames=True, thresholds=(1.5, 5.0, 2.0), 
-        lowerContrast=0.0, upperContrast=5.0, lowerDotThresh=1.5, upperDotThresh=5.0, 
-        lowerBlobThresh=2.0, program="density", polygon=None):
+        startImage="", skipsAllowed=0, removeEdgeFrames=True, lowerContrast=0.0, upperContrast=5.0,
+        lowerDotThresh=1.5, upperDotThresh=5.0, lowerBlobThresh=2.0, program="density", 
+        polygon=None, densityData={}, reanalysis=False):
         self.filepath = filepath
         self.dotSize = dotSize
         self.blobSize = blobSize
         self.saveFigures = saveFigures
         self.startImage = startImage
         self.skipsAllowed = skipsAllowed
         self.removeEdgeFrames = removeEdgeFrames
-        self.thresholds = thresholds
         self.lowerContrast = lowerContrast
         self.upperContrast = upperContrast
         self.lowerDotThresh = lowerDotThresh
         self.upperDotThresh = upperDotThresh
         self.lowerBlobThresh = lowerBlobThresh
+        self.thresholds = (lowerDotThresh, upperDotThresh, lowerBlobThresh)
         self.program = program
         self.polygon = polygon
+        self.densityData = densityData
+        self.reanalysis = reanalysis
```

### Comparing `dotscanner-1.3.3/tests/ui/test_MicroscopeImage.py` & `dotscanner-1.3.4/tests/ui/test_MicroscopeImage.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,19 @@
 			[0, 5, 8, 0, 0, 1, 0, 0, 0],
 			[0, 0, 0, 0, 0, 0, 0, 0, 0],
 			[0, 10, 0, 0, 0, 0, 0, 0, 0],
 			[0, 0, 0, 7, 0, 0, 0, 0, 1],
 			[0, 0, 0, 0, 0, 0, 0, 0, 0]
 		])
 		userSettings = FakeUserSettings(
-							dotSize=2,
-							blobSize=5,
-							saveFigures=False,
-							startImage="fakeImage01.png",
-							skipsAllowed=3,
-							removeEdgeFrames=True,
-							thresholds=(1.5, 5.0, 2.0))
+			filepath="test/directory/", dotSize=2, blobSize=5, saveFigures=False, 
+			startImage="fakeImage01.png", skipsAllowed=3, removeEdgeFrames=True, lowerContrast=0.0, 
+			upperContrast=5.0, lowerDotThresh=1.5, upperDotThresh=5.0, lowerBlobThresh=2.0, 
+			program="density", polygon=None)
+		
 		return MicroscopeImage("test/directory/", "filename.png", userSettings), userSettings
 	
 	def test_properLoading_whenClassInitializes(self):
 		microscopeImage, userSettings = self.getMicroscopeImageAndUserSettings()
 		
 		self.assertEqual(userSettings.dotSize, 2)
 		self.assertEqual(userSettings.blobSize, 5)
```

### Comparing `dotscanner-1.3.3/tests/ui/test_ThresholdAdjuster.py` & `dotscanner-1.3.4/tests/ui/test_ThresholdAdjuster.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,19 @@
  			[ 0,  0,  0,  0,  0,  0,  2,  0, -1,  0,  0,  0,  0],
  			[ 0,  0,  0,  0,  0,  0,  0, -1, -1,  0,  0,  0,  0],
  			[ 0,  7,  0,  0,  0,  0,  0,  0,  0,  0,  0,  1,  0],
  			[ 0,  5,  9,  0,  0,  0,  0,  1,  0,  0,  0,  8,  0],
  			[-1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  1,  0],
  		])
 		mock_getData.return_value = testData
-		fakeUserSettings = FakeUserSettings(dotSize=2, blobSize=3, thresholds=(1.2, 1.8, 1.3))
+		fakeUserSettings = FakeUserSettings(
+			filepath="test/directory/", dotSize=2, blobSize=3, saveFigures=False, 
+			startImage="", skipsAllowed=0, removeEdgeFrames=True, lowerContrast=0.0, 
+			upperContrast=5.0, lowerDotThresh=1.2, upperDotThresh=1.8, lowerBlobThresh=1.3, 
+			program="density", polygon=None, densityData={})
 		microscopeImage = MicroscopeImage("test/directory/", "filename.png", fakeUserSettings)
 		return microscopeImage, fakeUserSettings
 	
 	def test_upperDotThresholdScaleDown(self):
 		'''getFullDataSquareSum generates the following from the given test data:
  		[[ 6  6  2  0  1 -1 -2 -4 -2 -1  0  0  0]
 		 [ 6  6  2  0  1 -1 -2 -6 -4 -1  2  2  0]
```

