# Comparing `tmp/iLCDirac-34.0.0a6.tar.gz` & `tmp/iLCDirac-34.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iLCDirac-34.0.0a6.tar", last modified: Wed Jun  7 06:25:35 2023, max compression
+gzip compressed data, was "iLCDirac-34.0.0a7.tar", last modified: Wed Jun  7 13:42:11 2023, max compression
```

## Comparing `iLCDirac-34.0.0a6.tar` & `iLCDirac-34.0.0a7.tar`

### file list

```diff
@@ -1,472 +1,472 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.716258 iLCDirac-34.0.0a6/
--rw-rw-rw-   0 root         (0) root         (0)    32452 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1124 2023-06-07 06:25:35.717258 iLCDirac-34.0.0a6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)    83323 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/release.notes
--rw-rw-rw-   0 root         (0) root         (0)    27753 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/releases.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4370 2023-06-07 06:25:35.718258 iLCDirac-34.0.0a6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      276 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.597259 iLCDirac-34.0.0a6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.600259 iLCDirac-34.0.0a6/src/ILCDIRAC/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.602259 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.602259 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    10978 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.603259 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)     6343 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.604259 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)    36181 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py
--rw-rw-rw-   0 root         (0) root         (0)    44494 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py
--rw-rw-rw-   0 root         (0) root         (0)     5951 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3971 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/TODO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.605259 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/
--rw-rw-rw-   0 root         (0) root         (0)    14462 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     2255 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py
--rw-rw-rw-   0 root         (0) root         (0)    51085 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py
--rw-rw-rw-   0 root         (0) root         (0)     2037 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py
--rw-rw-rw-   0 root         (0) root         (0)     9201 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.607259 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.610259 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/
--rw-rw-rw-   0 root         (0) root         (0)     3152 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py
--rw-rw-rw-   0 root         (0) root         (0)     2867 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     2682 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)     3967 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py
--rw-rw-rw-   0 root         (0) root         (0)     4968 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Helper_Functions.py
--rw-rw-rw-   0 root         (0) root         (0)     3579 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.611259 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/
--rw-rw-rw-   0 root         (0) root         (0)     1765 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt
--rw-rw-rw-   0 root         (0) root         (0)     3928 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml
--rw-rw-rw-   0 root         (0) root         (0)     1484 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py
--rw-rw-rw-   0 root         (0) root         (0)    12301 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/dev_create_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.611259 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.620258 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     3755 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py
--rw-rw-rw-   0 root         (0) root         (0)    15006 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/Configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    18781 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/DetectOS.py
--rw-rw-rw-   0 root         (0) root         (0)     4861 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/FileUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     9749 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py
--rw-rw-rw-   0 root         (0) root         (0)     2767 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py
--rw-rw-rw-   0 root         (0) root         (0)     4110 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/GeneratorModels.py
--rw-rw-rw-   0 root         (0) root         (0)    17917 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/HTML.py
--rw-rw-rw-   0 root         (0) root         (0)     6866 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/InputDataResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     4246 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     5489 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/InstalledFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/JobPathResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     7040 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/MarlinXML.py
--rw-rw-rw-   0 root         (0) root         (0)     3285 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/OverlayFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     2856 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/PrepareLibs.py
--rw-rw-rw-   0 root         (0) root         (0)    36260 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     7483 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/ProcessList.py
--rw-rw-rw-   0 root         (0) root         (0)    11004 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/ProductionData.py
--rw-rw-rw-   0 root         (0) root         (0)     3993 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/RemoveSoft.py
--rw-rw-rw-   0 root         (0) root         (0)     2690 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/ResolveSE.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/Splitting.py
--rw-rw-rw-   0 root         (0) root         (0)    21977 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/TARsoft.py
--rw-rw-rw-   0 root         (0) root         (0)     2868 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/WasteCPU.py
--rw-rw-rw-   0 root         (0) root         (0)    41912 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/WhizardOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1100 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6604 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.628259 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/
--rw-rw-rw-   0 root         (0) root         (0)     6226 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py
--rw-rw-rw-   0 root         (0) root         (0)    31722 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    23878 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py
--rw-rw-rw-   0 root         (0) root         (0)    17273 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py
--rw-rw-rw-   0 root         (0) root         (0)    16707 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py
--rw-rw-rw-   0 root         (0) root         (0)     4872 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py
--rw-rw-rw-   0 root         (0) root         (0)    10164 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     7506 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)    18959 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)     2654 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     6803 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py
--rw-rw-rw-   0 root         (0) root         (0)    26585 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py
--rw-rw-rw-   0 root         (0) root         (0)    85249 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py
--rw-rw-rw-   0 root         (0) root         (0)    14816 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py
--rw-rw-rw-   0 root         (0) root         (0)     6220 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    11294 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py
--rw-rw-rw-   0 root         (0) root         (0)     9475 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py
--rw-rw-rw-   0 root         (0) root         (0)     2278 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py
--rw-rw-rw-   0 root         (0) root         (0)    72966 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py
--rw-rw-rw-   0 root         (0) root         (0)     3214 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py
--rw-rw-rw-   0 root         (0) root         (0)    26730 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1180 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.632259 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2720 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     3224 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     6151 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     6706 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     3200 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh
--rwxrwxrwx   0 root         (0) root         (0)     2307 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh
--rwxrwxrwx   0 root         (0) root         (0)     9197 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/dirac-architecture
--rw-rw-rw-   0 root         (0) root         (0)    15857 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py
--rw-rw-rw-   0 root         (0) root         (0)    10543 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py
--rw-rw-rw-   0 root         (0) root         (0)     9819 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py
--rw-rw-rw-   0 root         (0) root         (0)    16436 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py
--rw-rw-rw-   0 root         (0) root         (0)     3960 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py
--rw-rw-rw-   0 root         (0) root         (0)     1573 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.632259 iLCDirac-34.0.0a6/src/ILCDIRAC/DataManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.632259 iLCDirac-34.0.0a6/src/ILCDIRAC/DataManagementSystem/Agent/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.633258 iLCDirac-34.0.0a6/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/
--rw-rw-rw-   0 root         (0) root         (0)     5544 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1108 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/DataManagementSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.633258 iLCDirac-34.0.0a6/src/ILCDIRAC/FrameworkSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.633258 iLCDirac-34.0.0a6/src/ILCDIRAC/FrameworkSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/FrameworkSystem/ConfigTemplate.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/FrameworkSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.634258 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.635258 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    25777 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     9996 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     5395 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.636258 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)     1934 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.638258 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/
--rw-rw-rw-   0 root         (0) root         (0)    35437 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    14308 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py
--rw-rw-rw-   0 root         (0) root         (0)    19604 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py
--rw-rw-rw-   0 root         (0) root         (0)    13782 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py
--rw-rw-rw-   0 root         (0) root         (0)    30921 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py
--rw-rw-rw-   0 root         (0) root         (0)     7554 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2889 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.639258 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     5456 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py
--rw-rw-rw-   0 root         (0) root         (0)     6462 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py
--rw-rw-rw-   0 root         (0) root         (0)     3204 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.642258 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49360 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py
--rw-rw-rw-   0 root         (0) root         (0)    46600 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py
--rw-rw-rw-   0 root         (0) root         (0)     6228 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py
--rw-rw-rw-   0 root         (0) root         (0)     3366 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py
--rw-rw-rw-   0 root         (0) root         (0)    12482 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py
--rw-rw-rw-   0 root         (0) root         (0)     7314 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py
--rwxrwxrwx   0 root         (0) root         (0)     9954 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py
--rw-rw-rw-   0 root         (0) root         (0)     4673 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py
--rw-rw-rw-   0 root         (0) root         (0)    16641 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     3536 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py
--rw-rw-rw-   0 root         (0) root         (0)    12116 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.643258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.643258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/
--rw-rw-rw-   0 root         (0) root         (0)    13833 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/DiracILC.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.593259 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.644258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/alias.properties
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py
--rw-rw-rw-   0 root         (0) root         (0)     9474 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml
--rw-rw-rw-   0 root         (0) root         (0)    10942 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.645258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.658258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/default.mac
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/defaultClicCrossingAngle.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_10gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_10gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta10.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta20.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta30.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta40.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta50.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta60.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta70.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta80.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta90.mac
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_100gev_theta5-175.mac
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_10gev_theta5-175.mac
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.659258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/
--rw-rw-rw-   0 root         (0) root         (0)     8759 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.662258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/
--rw-rw-rw-   0 root         (0) root         (0)    27099 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.670258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/
--rw-rw-rw-   0 root         (0) root         (0)     3135 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     3757 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py
--rw-rw-rw-   0 root         (0) root         (0)     2335 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py
--rw-rw-rw-   0 root         (0) root         (0)    10462 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py
--rw-rw-rw-   0 root         (0) root         (0)    10003 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py
--rw-rw-rw-   0 root         (0) root         (0)    35946 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py
--rw-rw-rw-   0 root         (0) root         (0)    12944 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py
--rw-rw-rw-   0 root         (0) root         (0)     6521 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     3885 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py
--rw-rw-rw-   0 root         (0) root         (0)     6140 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py
--rw-rw-rw-   0 root         (0) root         (0)     9573 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py
--rw-rw-rw-   0 root         (0) root         (0)    10161 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py
--rw-rw-rw-   0 root         (0) root         (0)     8281 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py
--rw-rw-rw-   0 root         (0) root         (0)    16303 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)     3918 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py
--rw-rw-rw-   0 root         (0) root         (0)     3312 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py
--rw-rw-rw-   0 root         (0) root         (0)     2090 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py
--rw-rw-rw-   0 root         (0) root         (0)     3752 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py
--rw-rw-rw-   0 root         (0) root         (0)     4434 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6174 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py
--rw-rw-rw-   0 root         (0) root         (0)     6089 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py
--rw-rw-rw-   0 root         (0) root         (0)     5479 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6957 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py
--rw-rw-rw-   0 root         (0) root         (0)     1782 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py
--rw-rw-rw-   0 root         (0) root         (0)    17277 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py
--rw-rw-rw-   0 root         (0) root         (0)    12788 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py
--rw-rw-rw-   0 root         (0) root         (0)     4441 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py
--rw-rw-rw-   0 root         (0) root         (0)     4984 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.673258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/
--rw-rw-rw-   0 root         (0) root         (0)     2831 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py
--rw-rw-rw-   0 root         (0) root         (0)     2665 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py
--rw-rw-rw-   0 root         (0) root         (0)    19613 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py
--rw-rw-rw-   0 root         (0) root         (0)    22228 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py
--rw-rw-rw-   0 root         (0) root         (0)     2834 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py
--rw-rw-rw-   0 root         (0) root         (0)     4247 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py
--rw-rw-rw-   0 root         (0) root         (0)     9857 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py
--rw-rw-rw-   0 root         (0) root         (0)    24484 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py
--rw-rw-rw-   0 root         (0) root         (0)    26292 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py
--rw-rw-rw-   0 root         (0) root         (0)    15111 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py
--rw-rw-rw-   0 root         (0) root         (0)     3097 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     2402 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py
--rw-rw-rw-   0 root         (0) root         (0)    40172 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.674258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/
--rw-rw-rw-   0 root         (0) root         (0)    27996 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py
--rw-rw-rw-   0 root         (0) root         (0)    29727 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py
--rwxrwxrwx   0 root         (0) root         (0)    35679 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py
--rw-rw-rw-   0 root         (0) root         (0)    13124 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py
--rw-rw-rw-   0 root         (0) root         (0)    12330 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.684258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/
--rw-rw-rw-   0 root         (0) root         (0)     7876 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py
--rw-rw-rw-   0 root         (0) root         (0)     2416 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     4672 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py
--rw-rw-rw-   0 root         (0) root         (0)     2878 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py
--rw-rw-rw-   0 root         (0) root         (0)    18299 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py
--rw-rw-rw-   0 root         (0) root         (0)    15725 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py
--rw-rw-rw-   0 root         (0) root         (0)    41414 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py
--rw-rw-rw-   0 root         (0) root         (0)    15653 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py
--rw-rw-rw-   0 root         (0) root         (0)     5930 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     4218 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py
--rw-rw-rw-   0 root         (0) root         (0)    13745 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py
--rw-rw-rw-   0 root         (0) root         (0)     7579 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py
--rw-rw-rw-   0 root         (0) root         (0)    12305 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py
--rw-rw-rw-   0 root         (0) root         (0)     8309 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py
--rw-rw-rw-   0 root         (0) root         (0)     6492 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py
--rw-rw-rw-   0 root         (0) root         (0)    14537 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)     4767 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py
--rw-rw-rw-   0 root         (0) root         (0)    71676 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py
--rw-rw-rw-   0 root         (0) root         (0)     4830 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py
--rw-rw-rw-   0 root         (0) root         (0)     4533 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py
--rw-rw-rw-   0 root         (0) root         (0)     4798 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6232 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py
--rw-rw-rw-   0 root         (0) root         (0)     7551 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py
--rw-rw-rw-   0 root         (0) root         (0)     5077 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py
--rw-rw-rw-   0 root         (0) root         (0)     6829 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py
--rw-rw-rw-   0 root         (0) root         (0)     4763 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py
--rw-rw-rw-   0 root         (0) root         (0)    22726 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py
--rw-rw-rw-   0 root         (0) root         (0)    20865 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py
--rw-rw-rw-   0 root         (0) root         (0)    13044 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py
--rw-rw-rw-   0 root         (0) root         (0)     4169 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9860 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.684258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Test/
--rw-rw-rw-   0 root         (0) root         (0)    20190 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py
--rw-rw-rw-   0 root         (0) root         (0)     1132 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.685258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/Tests/
--rw-rw-rw-   0 root         (0) root         (0)     2622 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.686258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     4727 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1680 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py
--rw-rw-rw-   0 root         (0) root         (0)    15312 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.688258 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2968 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7808 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py
--rw-rw-rw-   0 root         (0) root         (0)     3538 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py
--rw-rw-rw-   0 root         (0) root         (0)     2636 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3088 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py
--rw-rw-rw-   0 root         (0) root         (0)     2396 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py
--rwxrwxrwx   0 root         (0) root         (0)     3724 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.689258 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.689258 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)     2638 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.690258 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.690258 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/DB/
--rw-rw-rw-   0 root         (0) root         (0)     6376 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.690258 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/DB/Test/
--rw-rw-rw-   0 root         (0) root         (0)     9281 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/DB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.691258 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)     2462 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.691258 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.704258 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/
--rw-rw-rw-   0 root         (0) root         (0)     4515 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py
--rw-rw-rw-   0 root         (0) root         (0)     5524 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py
--rw-rw-rw-   0 root         (0) root         (0)    23026 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     5789 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/CheckCollections.py
--rw-rw-rw-   0 root         (0) root         (0)     2452 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py
--rw-rw-rw-   0 root         (0) root         (0)     3146 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    16673 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     8022 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/DummyModule.py
--rw-rw-rw-   0 root         (0) root         (0)     6809 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py
--rw-rw-rw-   0 root         (0) root         (0)    19926 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     8787 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)     4454 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py
--rw-rw-rw-   0 root         (0) root         (0)     6156 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)     6801 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5057 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py
--rw-rw-rw-   0 root         (0) root         (0)     8078 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py
--rw-rw-rw-   0 root         (0) root         (0)    13096 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18950 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    31351 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/ModuleBase.py
--rw-rw-rw-   0 root         (0) root         (0)    26082 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5266 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/MoveInFC.py
--rw-rw-rw-   0 root         (0) root         (0)    33871 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)     7960 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py
--rw-rw-rw-   0 root         (0) root         (0)     8182 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5743 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/ReportErrors.py
--rw-rw-rw-   0 root         (0) root         (0)     5915 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5740 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4935 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    11639 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    11192 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4044 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py
--rw-rw-rw-   0 root         (0) root         (0)     9340 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/StdHepCut.py
--rw-rw-rw-   0 root         (0) root         (0)     3020 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.710258 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py
--rw-rw-rw-   0 root         (0) root         (0)    14814 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py
--rw-rw-rw-   0 root         (0) root         (0)    44092 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py
--rw-rw-rw-   0 root         (0) root         (0)    18662 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)    28578 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    20599 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py
--rw-rw-rw-   0 root         (0) root         (0)    10005 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    45397 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    43848 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py
--rw-rw-rw-   0 root         (0) root         (0)    41500 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py
--rw-rw-rw-   0 root         (0) root         (0)    10867 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)     2626 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py
--rw-rw-rw-   0 root         (0) root         (0)     8844 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    28021 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py
--rw-rw-rw-   0 root         (0) root         (0)    19461 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py
--rw-rw-rw-   0 root         (0) root         (0)    14457 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py
--rw-rw-rw-   0 root         (0) root         (0)    12973 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py
--rw-rw-rw-   0 root         (0) root         (0)    10007 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    32143 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py
--rw-rw-rw-   0 root         (0) root         (0)    14235 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py
--rw-rw-rw-   0 root         (0) root         (0)    67243 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    86847 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py
--rw-rw-rw-   0 root         (0) root         (0)     6505 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)    17704 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py
--rw-rw-rw-   0 root         (0) root         (0)    15076 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    17792 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py
--rw-rw-rw-   0 root         (0) root         (0)     9795 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    22938 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.712258 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     3265 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     4526 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2714 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Utilities/RootMixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.712258 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.713258 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    24455 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.713258 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)    15894 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.714258 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Executor/
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.715258 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Tests/
--rw-rw-rw-   0 root         (0) root         (0)    13587 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py
--rw-rw-rw-   0 root         (0) root         (0)    31624 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     3345 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2395 2023-06-07 06:25:12.000000 iLCDirac-34.0.0a6/src/ILCDIRAC/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 06:25:35.716258 iLCDirac-34.0.0a6/src/iLCDirac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-06-07 06:25:35.000000 iLCDirac-34.0.0a6/src/iLCDirac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24527 2023-06-07 06:25:35.000000 iLCDirac-34.0.0a6/src/iLCDirac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 06:25:35.000000 iLCDirac-34.0.0a6/src/iLCDirac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2121 2023-06-07 06:25:35.000000 iLCDirac-34.0.0a6/src/iLCDirac.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 06:25:34.000000 iLCDirac-34.0.0a6/src/iLCDirac.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      279 2023-06-07 06:25:35.000000 iLCDirac-34.0.0a6/src/iLCDirac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-07 06:25:35.000000 iLCDirac-34.0.0a6/src/iLCDirac.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.977064 iLCDirac-34.0.0a7/
+-rw-rw-rw-   0 root         (0) root         (0)    32452 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-07 13:42:11.977064 iLCDirac-34.0.0a7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)    83448 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/release.notes
+-rw-rw-rw-   0 root         (0) root         (0)    27753 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/releases.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4370 2023-06-07 13:42:11.979064 iLCDirac-34.0.0a7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      276 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.870065 iLCDirac-34.0.0a7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.873065 iLCDirac-34.0.0a7/src/ILCDIRAC/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.874065 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.874065 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    10978 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.875064 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.876065 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Service/
+-rw-rw-rw-   0 root         (0) root         (0)    36181 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    44494 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py
+-rw-rw-rw-   0 root         (0) root         (0)     5951 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3971 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/TODO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.877065 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/
+-rw-rw-rw-   0 root         (0) root         (0)    14462 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2255 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    51085 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9201 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.879065 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.882065 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     3152 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     3967 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py
+-rw-rw-rw-   0 root         (0) root         (0)     4968 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Helper_Functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3579 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.882065 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3928 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12301 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/dev_create_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.883065 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.890065 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     3755 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py
+-rw-rw-rw-   0 root         (0) root         (0)    15006 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/Configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    18781 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/DetectOS.py
+-rw-rw-rw-   0 root         (0) root         (0)     4861 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/FileUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9749 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2767 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py
+-rw-rw-rw-   0 root         (0) root         (0)     4110 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/GeneratorModels.py
+-rw-rw-rw-   0 root         (0) root         (0)    17917 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/HTML.py
+-rw-rw-rw-   0 root         (0) root         (0)     6866 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/InputDataResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     4246 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5489 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/InstalledFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/JobPathResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     7040 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/MarlinXML.py
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/OverlayFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2856 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/PrepareLibs.py
+-rw-rw-rw-   0 root         (0) root         (0)    36260 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     7483 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/ProcessList.py
+-rw-rw-rw-   0 root         (0) root         (0)    11004 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/ProductionData.py
+-rw-rw-rw-   0 root         (0) root         (0)     3993 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/RemoveSoft.py
+-rw-rw-rw-   0 root         (0) root         (0)     2690 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/ResolveSE.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/Splitting.py
+-rw-rw-rw-   0 root         (0) root         (0)    21977 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/TARsoft.py
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/WasteCPU.py
+-rw-rw-rw-   0 root         (0) root         (0)    41912 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/WhizardOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6604 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.897065 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py
+-rw-rw-rw-   0 root         (0) root         (0)    31722 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    23878 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py
+-rw-rw-rw-   0 root         (0) root         (0)    17273 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)    16707 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     4872 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py
+-rw-rw-rw-   0 root         (0) root         (0)    10164 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     7506 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    18959 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     6803 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py
+-rw-rw-rw-   0 root         (0) root         (0)    26585 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py
+-rw-rw-rw-   0 root         (0) root         (0)    85249 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)    14816 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py
+-rw-rw-rw-   0 root         (0) root         (0)     6220 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    11294 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py
+-rw-rw-rw-   0 root         (0) root         (0)     9475 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2278 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py
+-rw-rw-rw-   0 root         (0) root         (0)    72966 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py
+-rw-rw-rw-   0 root         (0) root         (0)    26730 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.901064 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     3224 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     6151 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     6706 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     3200 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2307 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh
+-rwxrwxrwx   0 root         (0) root         (0)     9197 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/dirac-architecture
+-rw-rw-rw-   0 root         (0) root         (0)    15857 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py
+-rw-rw-rw-   0 root         (0) root         (0)    10543 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py
+-rw-rw-rw-   0 root         (0) root         (0)     9819 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    16436 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3960 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.901064 iLCDirac-34.0.0a7/src/ILCDIRAC/DataManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.901064 iLCDirac-34.0.0a7/src/ILCDIRAC/DataManagementSystem/Agent/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.902064 iLCDirac-34.0.0a7/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/
+-rw-rw-rw-   0 root         (0) root         (0)     5544 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/DataManagementSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.902064 iLCDirac-34.0.0a7/src/ILCDIRAC/FrameworkSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.902064 iLCDirac-34.0.0a7/src/ILCDIRAC/FrameworkSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/FrameworkSystem/ConfigTemplate.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/FrameworkSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.903065 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.904065 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    25777 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     9996 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     5395 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.904065 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.906064 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)    35437 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    14308 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py
+-rw-rw-rw-   0 root         (0) root         (0)    19604 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13782 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    30921 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7554 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2889 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.907065 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     5456 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     6462 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.910065 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49360 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py
+-rw-rw-rw-   0 root         (0) root         (0)    46600 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6228 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py
+-rw-rw-rw-   0 root         (0) root         (0)     3366 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12482 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     7314 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py
+-rwxrwxrwx   0 root         (0) root         (0)     9954 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py
+-rw-rw-rw-   0 root         (0) root         (0)     4673 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    16641 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12116 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.910065 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.911064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/
+-rw-rw-rw-   0 root         (0) root         (0)    13833 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/DiracILC.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.866065 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.912064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/alias.properties
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py
+-rw-rw-rw-   0 root         (0) root         (0)     9474 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml
+-rw-rw-rw-   0 root         (0) root         (0)    10942 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.912064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.924064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/default.mac
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/defaultClicCrossingAngle.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/e-_10gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/gamma_10gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_100gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_10gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_200gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta10.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta20.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta30.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta40.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta50.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta60.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta70.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta80.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/mu-_50gev_theta90.mac
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_100gev_theta5-175.mac
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/slicMacros/pi-_10gev_theta5-175.mac
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.924064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/
+-rw-rw-rw-   0 root         (0) root         (0)     8759 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.927065 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/
+-rw-rw-rw-   0 root         (0) root         (0)    27099 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.934064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2335 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py
+-rw-rw-rw-   0 root         (0) root         (0)    10462 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py
+-rw-rw-rw-   0 root         (0) root         (0)    10032 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py
+-rw-rw-rw-   0 root         (0) root         (0)    35946 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py
+-rw-rw-rw-   0 root         (0) root         (0)    12973 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py
+-rw-rw-rw-   0 root         (0) root         (0)     6521 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     3885 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     6140 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py
+-rw-rw-rw-   0 root         (0) root         (0)     9573 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py
+-rw-rw-rw-   0 root         (0) root         (0)    10161 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8281 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py
+-rw-rw-rw-   0 root         (0) root         (0)    16303 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)     3918 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3312 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py
+-rw-rw-rw-   0 root         (0) root         (0)     2090 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py
+-rw-rw-rw-   0 root         (0) root         (0)     3752 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6174 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py
+-rw-rw-rw-   0 root         (0) root         (0)     5479 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6957 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py
+-rw-rw-rw-   0 root         (0) root         (0)    17277 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    12788 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4441 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py
+-rw-rw-rw-   0 root         (0) root         (0)     4984 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.937064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py
+-rw-rw-rw-   0 root         (0) root         (0)     2665 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    19613 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py
+-rw-rw-rw-   0 root         (0) root         (0)    22228 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py
+-rw-rw-rw-   0 root         (0) root         (0)     4247 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py
+-rw-rw-rw-   0 root         (0) root         (0)     9857 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    24484 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py
+-rw-rw-rw-   0 root         (0) root         (0)    26292 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py
+-rw-rw-rw-   0 root         (0) root         (0)    15111 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py
+-rw-rw-rw-   0 root         (0) root         (0)     3097 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2402 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)    40301 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.938064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/
+-rw-rw-rw-   0 root         (0) root         (0)    27996 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    29727 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py
+-rwxrwxrwx   0 root         (0) root         (0)    35679 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py
+-rw-rw-rw-   0 root         (0) root         (0)    13124 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py
+-rw-rw-rw-   0 root         (0) root         (0)    12330 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.946064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7876 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4672 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2878 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18299 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py
+-rw-rw-rw-   0 root         (0) root         (0)    15725 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py
+-rw-rw-rw-   0 root         (0) root         (0)    41414 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py
+-rw-rw-rw-   0 root         (0) root         (0)    15653 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     4218 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    13745 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py
+-rw-rw-rw-   0 root         (0) root         (0)     7579 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py
+-rw-rw-rw-   0 root         (0) root         (0)    12305 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py
+-rw-rw-rw-   0 root         (0) root         (0)     8309 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6492 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py
+-rw-rw-rw-   0 root         (0) root         (0)    14537 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)     4767 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)    71676 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4798 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6232 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py
+-rw-rw-rw-   0 root         (0) root         (0)     7551 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py
+-rw-rw-rw-   0 root         (0) root         (0)     5077 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6829 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)     4763 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py
+-rw-rw-rw-   0 root         (0) root         (0)    22726 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py
+-rw-rw-rw-   0 root         (0) root         (0)    20865 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13044 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4169 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9860 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.947064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Test/
+-rw-rw-rw-   0 root         (0) root         (0)    20190 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.947064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2622 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.948064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    15312 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.950064 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2968 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7808 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py
+-rw-rw-rw-   0 root         (0) root         (0)     3538 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py
+-rw-rw-rw-   0 root         (0) root         (0)     2636 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3088 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2396 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     3724 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.950064 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.951064 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)     2638 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.951064 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.952064 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/DB/
+-rw-rw-rw-   0 root         (0) root         (0)     6376 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.952064 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/DB/Test/
+-rw-rw-rw-   0 root         (0) root         (0)     9281 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/DB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.953064 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Service/
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.953064 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.965064 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/
+-rw-rw-rw-   0 root         (0) root         (0)     4515 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py
+-rw-rw-rw-   0 root         (0) root         (0)     5524 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py
+-rw-rw-rw-   0 root         (0) root         (0)    23026 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5789 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/CheckCollections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py
+-rw-rw-rw-   0 root         (0) root         (0)     3146 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    16673 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8022 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/DummyModule.py
+-rw-rw-rw-   0 root         (0) root         (0)     6809 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)    19926 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8787 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)     4454 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     6156 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     6801 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5057 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8078 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)    13096 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18950 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    31351 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/ModuleBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    26082 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5266 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/MoveInFC.py
+-rw-rw-rw-   0 root         (0) root         (0)    33871 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)     7960 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)     8182 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5743 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/ReportErrors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5915 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5740 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    11639 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    11192 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4044 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9340 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/StdHepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)     3020 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.971064 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)    14814 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)    44092 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    18662 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)    28578 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    20599 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py
+-rw-rw-rw-   0 root         (0) root         (0)    10005 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    45397 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    43848 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    41500 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py
+-rw-rw-rw-   0 root         (0) root         (0)    10867 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     2626 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8844 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    28021 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py
+-rw-rw-rw-   0 root         (0) root         (0)    19461 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py
+-rw-rw-rw-   0 root         (0) root         (0)    14457 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py
+-rw-rw-rw-   0 root         (0) root         (0)    12973 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    10007 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    32143 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py
+-rw-rw-rw-   0 root         (0) root         (0)    14235 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    67243 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    86847 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py
+-rw-rw-rw-   0 root         (0) root         (0)     6505 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    17704 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    15076 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    17792 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py
+-rw-rw-rw-   0 root         (0) root         (0)     9795 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    22938 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.972064 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     3265 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4526 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2714 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Utilities/RootMixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.973064 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.973064 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    24455 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.974064 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)    15894 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.974064 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Executor/
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.975064 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13587 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    31624 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3345 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2023-06-07 13:41:49.000000 iLCDirac-34.0.0a7/src/ILCDIRAC/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:42:11.977064 iLCDirac-34.0.0a7/src/iLCDirac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-07 13:42:11.000000 iLCDirac-34.0.0a7/src/iLCDirac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24527 2023-06-07 13:42:11.000000 iLCDirac-34.0.0a7/src/iLCDirac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 13:42:11.000000 iLCDirac-34.0.0a7/src/iLCDirac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-06-07 13:42:11.000000 iLCDirac-34.0.0a7/src/iLCDirac.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 13:42:11.000000 iLCDirac-34.0.0a7/src/iLCDirac.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-07 13:42:11.000000 iLCDirac-34.0.0a7/src/iLCDirac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-07 13:42:11.000000 iLCDirac-34.0.0a7/src/iLCDirac.egg-info/top_level.txt
```

### Comparing `iLCDirac-34.0.0a6/LICENSE` & `iLCDirac-34.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/PKG-INFO` & `iLCDirac-34.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iLCDirac
-Version: 34.0.0a6
+Version: 34.0.0a7
 Summary: iLCDirac is the iLC/CLIC/FCC extension of DIRAC
 Home-page: https://gitlab.cern.ch/clicdp/ilcdirac/ilcdirac.git
 Maintainer: Andre Sailer
 Maintainer-email: ilcdirac-support@cern.ch
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://its.cern.ch/jira/browse/ILCDIRAC
 Project-URL: Documentation, https://ilcdirac-doc.web.cern.ch/
```

### Comparing `iLCDirac-34.0.0a6/release.notes` & `iLCDirac-34.0.0a7/release.notes`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 NEW: Depend on DIRAC version 7.3
 NEW: Python3 only
 NEW: (!430) Addition of some functionalities to the Gaudi Application interface.
 NEW: (!430) Correct paths for storing FCC simulations outputs.
 NEW: (!430) Implementation of the Delphes Application interface.
 NEW: (!440) Documentation for FCC production code.
 FIX: (!421) client installation: corrected (a typo in) the URL of the configuration service, fixes problems during dirac-configure.
+
+*Interfaces
+
+FIX: (!447) Setting extensions of Gaudi and Delphes applications to 'root' for production output definitions.
+
 *Workflows
 
 FIX: (!444) Putting randomSeed modulo 900000000 in the Pythia cards to avoid having a random seed bigger than the Pythia limit.
 
 [v32r0p3]
 Release date: 2021-11-18
```

### Comparing `iLCDirac-34.0.0a6/releases.cfg` & `iLCDirac-34.0.0a7/releases.cfg`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/setup.cfg` & `iLCDirac-34.0.0a7/setup.cfg`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Agent/CalibrationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Client/CalibrationClient.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Client/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Service/CalibrationHandler.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Service/CalibrationRun.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Service/DetectorSettings.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Service/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/TODO` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/TODO`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationClient.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/Test_CalibrationService.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_fileutils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/Test_Util_functions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Test/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Test/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/ECal_Digi_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/EM_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_GeVToMIP.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Extract_SimCaloHitMIPMPV.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Final_Calibration.py.orig`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Digi_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Direction_Corrections_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Digi_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/HCal_Ring_Gear_Information.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Had_Extract.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/Python_Read_Scripts/Python_Read_Scripts.tgz`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/parameterListMarlinSteeringFile.txt`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/auxiliaryFiles/pfoAnalysis.xml`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/fileutils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/functions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/mergePandoraLikelihoodData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/Utilities/objectFactory.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/CalibrationSystem/dev_create_events.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/CalibrationSystem/dev_create_events.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/CheckAndGetProdProxy.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/CheckXMLValidity.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/CombinedSoftwareInstallation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/Configuration.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/Configuration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/DetectOS.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/DetectOS.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/FileUtils.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/FileUtils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/FilenameEncoder.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/FindSteeringFileDir.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/GeneratorModels.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/GeneratorModels.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/HTML.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/HTML.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/InputDataResolution.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/InputDataResolution.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/InputFilesUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/InstalledFiles.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/InstalledFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/JobPathResolution.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/JobPathResolution.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/LFNPathUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/MarlinXML.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/MarlinXML.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/OutputDataPolicy.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/OverlayFiles.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/OverlayFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/PrepareLibs.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/PrepareLibs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/PrepareOptionFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/ProcessList.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/ProcessList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/ProductionData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/ProductionData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/RemoveSoft.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/RemoveSoft.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/ResolveDependencies.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/ResolveSE.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/ResolveSE.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/Splitting.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/Splitting.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/TARsoft.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/TARsoft.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/Utilities.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/Utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/WasteCPU.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/WasteCPU.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/WhizardOptions.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/WhizardOptions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/resolvePathsAndNames.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_CheckAndGetProd.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_CombinedSoftwareInstallation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_Configuration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_DetectOS.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_FileUtils.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_FilenameEncoder.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_FindSteeringFileDir.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_InputDataResolution.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_InputFilesUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_LFNPathUtilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_OutputDataPolicy.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_OverlayFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareLibs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareMarlinXML.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_PrepareOptionsFiles.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_ProcessList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_ProductionOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_ResolvePathsandNames.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_ResolveSEs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_Splitting.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_TARsoft.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_Utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_WasteCPU.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/Utilities/tests/Test_WhizardOptions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/createJavaTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/createLCIOTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/createMarlinTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/createMokkaTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/createSlicPandoraTarBall.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/createTarBallForProgram.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/dirac-architecture` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/dirac-architecture`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/dirac_ilc_add_cvmfs_software.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/dirac_ilc_add_software.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/dirac_ilc_add_user.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/dirac_ilc_add_whizard.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/dirac_ilc_list_users.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Core/scripts/ilcdirac-install.sh`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/DataManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/DataManagementSystem/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/DataManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/FrameworkSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/FrameworkSystem/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/FrameworkSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Agent/FileStatusTransformationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Agent/TarTheLogsAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Agent/TransformationPlugin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Client/Transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_FileStatusTransformationAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_ReleaseHelper.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_TransformationPlugin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_createMovingTransformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/Test_diracClicMakeProductions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/test_diracIlcAddTasks.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Utilities/DataParameters.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Utilities/ReleaseHelper.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Utilities/Utilities.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_clic_make_productions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_fcc_make_productions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_add_tasks_to_prod.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_filestatus_transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_info.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_get_prod_log.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_make_ddsimtarball.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_moving_transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_production_summary.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_replication_transformation.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/ILCTransformationSystem/scripts/dirac_ilc_upload_gen_files.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/DiracILC.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/DiracILC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/bannedSites.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsim.xml`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/defaultPrePandoraLcsimOverlay.xml`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testSimList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SIDChain/fileLists/testStdhepList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Examples/SiDProduction/sid_dbd_sim_production_default.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Application.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckCollections.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/CheckWNs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DDSim.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/DelphesApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     self.pythia8CardContent = ''
     super(DelphesApp, self).__init__(paramdict)
     # Those 5 need to come after default constructor
     self._modulename = 'DelphesAppModule'
     self._moduledescription = 'Module to run DelphesApp'
     self.appname = 'delphesapp'
     self._ops = Operations()
+    self._extension = 'root'
 
   def setRandomSeed(self, randomSeed):
     """Define random seed to use. Default is the jobID.
 
     :param int randomSeed: Seed to use during simulation.
     """
     self._checkArgs({'randomSeed': int})
```

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Fcc.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GaudiApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     self.keepRecFile = None
     super(GaudiApp, self).__init__(paramdict)
     # Those 5 need to come after default constructor
     self._modulename = 'GaudiAppModule'
     self._moduledescription = 'Module to run GaudiApp'
     self.appname = 'gaudiapp'
     self._ops = Operations()
+    self._extension = 'root'
 
   @property
   def detectortype(self):
     """DetectorType needed for transformations.
 
     Backward compatibility needed for Mokka?
     """
```

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GenericApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/GetSRMFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/KKMC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/LCSIM.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Marlin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Mokka.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/PostGenSelection.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Pythia.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootMacro.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/RootScript.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOConcatenate.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLCIOSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLIC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/SLICPandora.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/StdhepCutJava.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Tomato.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/Whizard2.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/_Root.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Applications/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ConditionalOverlay.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/FullILDChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainDBD.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ILDProductionChainOpt2017.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MarlinExample.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/MokkaMarlinOverlayMarlin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ParametricJobExample.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/ReplicationAkiya.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Examples/SIDProductionChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobDBD.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/ILDProductionJobOpt2017.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Job.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/LCApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/LCUtilityApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/ProductionJob.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,14 +514,19 @@
       LOG.error("Not transformation defined earlier")
       return S_ERROR("No transformation defined")
     if prodinfo:
       self.prodparameters = prodinfo
 
     info = []
     info.append('%s Production %s has following parameters:\n' % (self.prodparameters['JobType'], currtrans))
+
+    for key, value in self.prodparameters.items():
+      if "datatype" in str(value):
+        info.append('- Output %s' % key)
+
     if "Process" in self.prodparameters:
       info.append('- Process %s' % self.prodparameters['Process'])
     if "Energy" in self.prodparameters:
       info.append('- Energy %s GeV' % self.prodparameters["Energy"])
 
     if not self.slicesize:
       self.prodparameters['nbevts'] = self.jobFileGroupSize * self.nbevts
```

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/CLICProductionChain_hzqq_420.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/ProductionChainTest.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Productions/SIDProductionChain.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/SIDProductionJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Application.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckCollections.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_CheckWNs.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DDSim.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_DelphesApp.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Fcc.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GaudiApp.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GenericApplication.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_GetSRMFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Job.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_KKMC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_LCSIM.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Marlin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Mokka.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_PostGenSelection.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_ProductionJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Pythia.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOConcatenate.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLCIOSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLIC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_SLICPandora.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_StdhepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Tomato.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_UserJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test_Whizard2.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/Test__Root.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/Tests/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/UserJob.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/NewInterface/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/Test/Test_DiracILC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/API/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/API/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/Tests/Test_JobHelpers.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/Utilities/DDInterfaceMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/Utilities/JobHelpers.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/Utilities/SplitMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/Utilities/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/TestAndProbeSites.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_find_in_FC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/dirac_ilc_show_software.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/dirac_repo_create_lfn_list.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/dirac_repo_retrieve_jobs_output_data.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Interfaces/scripts/ilcdirac_version.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Agent/ResetCounters.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Agent/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Client/OverlaySystemClient.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Client/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/DB/OverlayDB.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/DB/Test/Test_OverlayDB.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/DB/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Service/OverlayHandler.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/Service/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/OverlaySystem/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/OverlaySystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/AnalyseWN.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/ApplicationScript.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Calibration.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/CheckCollections.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/CheckCollections.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/ComputeOutputDataList.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/DBDGenRegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/DDSimAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/DelphesAppModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/DummyModule.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/DummyModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/FailoverRequest.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/FccAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/GaudiAppModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/GetSRMFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/ILDRegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/KKMCAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/LCIOConcatenate.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/LCIOSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/LCSIMAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/MarlinAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/ModuleBase.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/ModuleBase.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/MokkaAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/MoveInFC.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/MoveInFC.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/OverlayInput.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/PostGenSelection.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/PythiaAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/RegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/RemoveInputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/ReportErrors.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/ReportErrors.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/RootExecutableAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/RootMacroAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/SIDRegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/SLICAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/SLICPandoraAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/StdHepConverter.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/StdHepCut.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/StdHepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/StdHepCutJava.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/MakeRequest.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_Calibration.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_DDSimWorkflow.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_DelphesAppModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_FccAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_GaudiAppModule.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_KKMCAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_MarlinAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_ModuleBase.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_OverlayInput.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_RegisterOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_ReportErrors.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_RootExecutableAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_SLICPandoraAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_SlicPandora.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepCut.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_StdHepSplit.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadLogFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_UploadOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_UserJobFinalization.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_Whizard2Workflow.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_WhizardAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Test/Test_WorkflowModuleRequests.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/TomatoAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/UploadLogFile.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/UploadOutputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/UserJobFinalization.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/Whizard2Analysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/WhizardAnalysis.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Modules/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Modules/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Utilities/CompactMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Utilities/DD4hepMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Utilities/RootMixin.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Utilities/RootMixin.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/Utilities/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/Workflow/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/Workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Agent/JobResetAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Client/DownloadInputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Executor/SoftwareVersions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Executor/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_Client_DownloadInputData.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_JobResetAgent.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/Tests/Test_SoftwareVersions.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/WorkloadManagementSystem/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/WorkloadManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/ILCDIRAC/__init__.py` & `iLCDirac-34.0.0a7/src/ILCDIRAC/__init__.py`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/iLCDirac.egg-info/PKG-INFO` & `iLCDirac-34.0.0a7/src/iLCDirac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iLCDirac
-Version: 34.0.0a6
+Version: 34.0.0a7
 Summary: iLCDirac is the iLC/CLIC/FCC extension of DIRAC
 Home-page: https://gitlab.cern.ch/clicdp/ilcdirac/ilcdirac.git
 Maintainer: Andre Sailer
 Maintainer-email: ilcdirac-support@cern.ch
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://its.cern.ch/jira/browse/ILCDIRAC
 Project-URL: Documentation, https://ilcdirac-doc.web.cern.ch/
```

### Comparing `iLCDirac-34.0.0a6/src/iLCDirac.egg-info/SOURCES.txt` & `iLCDirac-34.0.0a7/src/iLCDirac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iLCDirac-34.0.0a6/src/iLCDirac.egg-info/entry_points.txt` & `iLCDirac-34.0.0a7/src/iLCDirac.egg-info/entry_points.txt`

 * *Files identical despite different names*

