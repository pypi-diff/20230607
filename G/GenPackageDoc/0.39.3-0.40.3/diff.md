# Comparing `tmp/GenPackageDoc-0.39.3.tar.gz` & `tmp/GenPackageDoc-0.40.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenPackageDoc-0.39.3.tar", last modified: Fri May  5 14:02:42 2023, max compression
+gzip compressed data, was "GenPackageDoc-0.40.3.tar", last modified: Wed Jun  7 13:56:22 2023, max compression
```

## Comparing `GenPackageDoc-0.39.3.tar` & `GenPackageDoc-0.40.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:02:42.482193 GenPackageDoc-0.39.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:02:42.478193 GenPackageDoc-0.39.3/GenPackageDoc/
--rw-r--r--   0 runner    (1001) docker     (123)    40053 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/CDocBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/CInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)    25033 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/CPackageDocConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/CPatterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/CSourceParser.py
--rw-r--r--   0 runner    (1001) docker     (123)   277945 2023-05-05 14:02:42.000000 GenPackageDoc-0.39.3/GenPackageDoc/GenPackageDoc.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:02:42.482193 GenPackageDoc-0.39.3/GenPackageDoc/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/styles/admonitions.sty
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/styles/common.sty
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/styles/pandoc.sty
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/styles/preamble.tex
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/styles/robotframeworkaio.sty
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:02:42.482193 GenPackageDoc-0.39.3/GenPackageDoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-05 14:02:42.000000 GenPackageDoc-0.39.3/GenPackageDoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-05 14:02:42.000000 GenPackageDoc-0.39.3/GenPackageDoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:02:42.000000 GenPackageDoc-0.39.3/GenPackageDoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 14:02:42.000000 GenPackageDoc-0.39.3/GenPackageDoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 14:02:42.000000 GenPackageDoc-0.39.3/GenPackageDoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-05 14:02:42.482193 GenPackageDoc-0.39.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:02:42.482193 GenPackageDoc-0.39.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:56:22.521165 GenPackageDoc-0.40.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:56:22.517165 GenPackageDoc-0.40.3/GenPackageDoc/
+-rw-r--r--   0 runner    (1001) docker     (123)    46459 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/GenPackageDoc/CDocBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/GenPackageDoc/CInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27558 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/GenPackageDoc/CPackageDocConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/GenPackageDoc/CPatterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/GenPackageDoc/CSourceParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   337956 2023-06-07 13:56:22.000000 GenPackageDoc-0.40.3/GenPackageDoc/GenPackageDoc.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/GenPackageDoc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:56:22.521165 GenPackageDoc-0.40.3/GenPackageDoc/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/GenPackageDoc/styles/admonitions.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/GenPackageDoc/styles/common.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/GenPackageDoc/styles/pandoc.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/GenPackageDoc/styles/preamble.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/GenPackageDoc/styles/robotframeworkaio.sty
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/GenPackageDoc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:56:22.517165 GenPackageDoc-0.40.3/GenPackageDoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-07 13:56:22.000000 GenPackageDoc-0.40.3/GenPackageDoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-07 13:56:22.000000 GenPackageDoc-0.40.3/GenPackageDoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:56:22.000000 GenPackageDoc-0.40.3/GenPackageDoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 13:56:22.000000 GenPackageDoc-0.40.3/GenPackageDoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 13:56:22.000000 GenPackageDoc-0.40.3/GenPackageDoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-07 13:56:22.521165 GenPackageDoc-0.40.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:56:22.521165 GenPackageDoc-0.40.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-06-07 13:54:09.000000 GenPackageDoc-0.40.3/setup.py
```

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/CDocBuilder.py` & `GenPackageDoc-0.40.3/GenPackageDoc/CDocBuilder.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # **************************************************************************************************************
 #
 # CDocBuilder.py
 #
 # XC-CT/ECA3-Queckenstedt
 #
-# 06.01.2023
+# 13.04.2023
 #
 # --------------------------------------------------------------------------------------------------------------
 
 """
 Python module containing all methods to generate tex sources.
 """
 
@@ -340,14 +340,156 @@
       return bSuccess, sResult
 
    # eof def __CopyPictures(self):
 
    # --------------------------------------------------------------------------------------------------------------
    #TM***
 
+   def __RenderDiagrams(self):
+      """Render all diagrams in 'DIAGRAMS' folder (with PlantUML). Diagram files are expected to have the extension '.puml'.
+      """
+
+      sMethod = "CDocBuilder.__RenderDiagrams"
+
+      bSuccess = None
+      sResult  = "UNKNOWN"
+
+      sDiagramsSourceDir = self.__dictPackageDocConfig['DIAGRAMS']
+      if sDiagramsSourceDir is None:
+         bSuccess = True
+         sResult  = f"No diagrams folder configured in DIAGRAMS section of GenPackageDoc configuration; nothing to render"
+         return bSuccess, sResult
+      else:
+         if os.path.isdir(sDiagramsSourceDir) is True:
+            # -- identify diagram files
+            listDiagramFiles = []
+            for sLocalRootPath, listFolderNames, listFileNames in os.walk(sDiagramsSourceDir):
+               for sFileName in listFileNames:
+                  if sFileName.endswith('.puml'):
+                     sDiagramFile = CString.NormalizePath(os.path.join(sLocalRootPath, sFileName))
+                     if sDiagramFile not in listDiagramFiles:
+                        listDiagramFiles.append(sDiagramFile)
+            # eof for ...
+
+            nNrOfDiagramFiles = len(listDiagramFiles)
+            if nNrOfDiagramFiles == 0:
+               bSuccess = True
+               sResult  = f"No diagram files found in '{sDiagramsSourceDir}'; nothing to render"
+               return bSuccess, sResult
+
+            # diagram files available in diagrams folder (DIAGRAMS), therefore we need JAVA and PLANT_UML
+            # -- JAVA
+            JAVA = self.__dictPackageDocConfig['JAVA']
+            if JAVA is None:
+               bSuccess = False
+               sResult  = f"Java not configured in GenPackageDoc configuration; cannot render diagrams"
+               return bSuccess, sResult
+            if os.path.isfile(JAVA) is False:
+               bSuccess = False
+               sResult  = f"Java '{JAVA}' not found; check GenPackageDoc configuration; cannot render diagrams"
+               return bSuccess, sResult
+            # -- PLANT_UML
+            PLANT_UML = self.__dictPackageDocConfig['PLANT_UML']
+            if PLANT_UML is None:
+               bSuccess = False
+               sResult  = f"PlantUML not configured in GenPackageDoc configuration; cannot render diagrams"
+               return bSuccess, sResult
+            if os.path.isfile(PLANT_UML) is False:
+               bSuccess = False
+               sResult  = f"PlantUML '{PLANT_UML}' not found; check GenPackageDoc configuration; cannot render diagrams"
+               return bSuccess, sResult
+
+            print(COLBY + "Rendering diagrams ...")
+            print()
+
+            # -- render all diagrams
+            nCntDiagramFiles = 0
+            for sDiagramFile in listDiagramFiles:
+               nCntDiagramFiles = nCntDiagramFiles + 1
+               sInfo = f"* ({nCntDiagramFiles}/{nNrOfDiagramFiles}) : '{sDiagramFile}'"
+               print(sInfo)
+               print()
+               listCmdLineParts = []
+               listCmdLineParts.append(f"\"{JAVA}\"")
+               listCmdLineParts.append(f"-jar")
+               listCmdLineParts.append(f"\"{PLANT_UML}\"")
+               listCmdLineParts.append(f"\"{sDiagramFile}\"")
+
+               sCmdLine = " ".join(listCmdLineParts)
+               # -- debug
+               print("Now executing command line:\n" + sCmdLine)
+               print()
+               del listCmdLineParts
+               listCmdLineParts = shlex.split(sCmdLine)
+
+               try:
+                  nReturn = subprocess.call(listCmdLineParts)
+                  print(f"PlantUML returned {nReturn}")
+                  print()
+               except Exception as ex:
+                  bSuccess = None
+                  sResult  = str(ex)
+                  return bSuccess, CString.FormatResult(sMethod, bSuccess, sResult)
+
+            # eof for sDiagramFile in listDiagramFiles:
+
+            bSuccess = True
+            sResult  = f"{nCntDiagramFiles} diagrams within '{sDiagramsSourceDir}' rendered"
+         else:
+            bSuccess = False
+            sResult  = f"Diagrams folder '{sDiagramsSourceDir}' does not exist"
+            return bSuccess, CString.FormatResult(sMethod, bSuccess, sResult)
+      # eof else - if sDiagramsSourceDir is None:
+
+      return bSuccess, sResult
+
+   # eof def __RenderDiagrams(self):
+
+   # --------------------------------------------------------------------------------------------------------------
+   #TM***
+
+   def __CopyDiagrams(self):
+      """Copies the diagrams folder to the output folder (required to keep relative paths valid also in created tex files)
+      """
+
+      sMethod = "CDocBuilder.__CopyDiagrams"
+
+      bSuccess = None
+      sResult  = "UNKNOWN"
+
+      sDiagramsSourceDir = self.__dictPackageDocConfig['DIAGRAMS']
+      if sDiagramsSourceDir is None:
+         bSuccess = True
+         sResult  = f"No diagrams defined, nothing to copy"
+      else:
+         if os.path.isdir(sDiagramsSourceDir) is True:
+            # copy the diagrams folder to output folder
+            sDirName = os.path.basename(sDiagramsSourceDir)
+            sDiagramsDestinationDir = f"{self.__dictPackageDocConfig['OUTPUT']}/{sDirName}"
+            try:
+               shutil.copytree(sDiagramsSourceDir, sDiagramsDestinationDir)
+            except Exception as ex:
+               bSuccess = None
+               sResult  = str(ex)
+               return bSuccess, CString.FormatResult(sMethod, bSuccess, sResult)
+            bSuccess = True
+            sResult  = f"Pictures folder '{sDiagramsSourceDir}' copied to build folder '{sDiagramsDestinationDir}'"
+         else:
+            bSuccess = False
+            sResult  = f"Pictures folder '{sDiagramsSourceDir}' does not exist"
+            return bSuccess, CString.FormatResult(sMethod, bSuccess, sResult)
+      # eof else - if sDiagramsSourceDir is None:
+
+      return bSuccess, sResult
+
+   # eof def __CopyDiagrams(self):
+
+   # --------------------------------------------------------------------------------------------------------------
+   #TM***
+
    def __GenDocPDF(self):
       """Executes the LaTeX compiler to create the PDF file out of the generated source tex files
       """
 
       sMethod = "CDocBuilder.__GenDocPDF"
 
       bSuccess = None
@@ -460,14 +602,25 @@
 
       sMethod = "CDocBuilder.Build"
 
       bSuccess, sResult = self.__CleanBuildFolder()
       if bSuccess is not True:
          return bSuccess, CString.FormatResult(sMethod, bSuccess, sResult)
 
+      bSuccess, sResult = self.__RenderDiagrams()
+      if bSuccess is not True:
+         return bSuccess, CString.FormatResult(sMethod, bSuccess, sResult)
+
+      print(COLBY + sResult)
+      print()
+
+      bSuccess, sResult = self.__CopyDiagrams()
+      if bSuccess is not True:
+         return bSuccess, CString.FormatResult(sMethod, bSuccess, sResult)
+
       bSuccess, sResult = self.__CopyPictures()
       if bSuccess is not True:
          return bSuccess, CString.FormatResult(sMethod, bSuccess, sResult)
 
       sBuildFolder = self.__dictPackageDocConfig['OUTPUT']
 
       oSourceParser = CSourceParser()
```

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/CInterface.py` & `GenPackageDoc-0.40.3/GenPackageDoc/CInterface.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/CPackageDocConfig.py` & `GenPackageDoc-0.40.3/GenPackageDoc/CPackageDocConfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # **************************************************************************************************************
 #
 # CPackageDocConfig.py
 #
 # XC-CT/ECA3-Queckenstedt
 #
-# 17.03.2023
+# 06.06.2023
 #
 # --------------------------------------------------------------------------------------------------------------
 
 """
 Python module containing the configuration for **GenPackageDoc**. This includes the repository configurantion
 and command line values.
 """
@@ -87,65 +87,65 @@
 
       # get repository configuration
       dictRepositoryConfig = oRepositoryConfig.GetConfig()
 
       # read the documentation build configuration from separate json file
       #    - the path to the folder containing this json file is taken out of the repository configuration
       #    - the name of the json file is fix
-      sJsonFileName = "packagedoc_config.json"
-      sDocumentationProjectConfigFile = f"{dictRepositoryConfig['PACKAGEDOC']}/{sJsonFileName}"
+      sDocumentationProjectConfigFile = f"{dictRepositoryConfig['PACKAGEDOC']}/packagedoc_config.json"
 
       # The json file may contain lines that are commented out by a '#' at the beginning of the line.
       # Therefore we read in this file in text format, remove the comments and save the cleaned file within the temp folder.
       # Now it's a valid json file and we read the file from there.
 
       sTmpPath = None
       sPlatformSystem = platform.system()
       if sPlatformSystem == "Windows":
-         sTmpPath = CString.NormalizePath("%TMP%")
+         # currently nothing to do
+         pass
       elif sPlatformSystem == "Linux":
-         sTmpPath = "/tmp"
+         # currently nothing to do
+         pass
       else:
          bSuccess = None
          sResult  = f"Platform system '{sPlatformSystem}' is not supported"
          raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
 
-      sJsonFileCleaned = f"{sTmpPath}/{sJsonFileName}"
-
       oJsonFileSource = CFile(sDocumentationProjectConfigFile)
       listLines, bSuccess, sResult = oJsonFileSource.ReadLines(bSkipBlankLines=True, sComment='#')
       del oJsonFileSource
       if bSuccess is not True:
          raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
-      oJsonFileCleaned = CFile(sJsonFileCleaned)
-      bSuccess, sResult = oJsonFileCleaned.Write(listLines)
-      del oJsonFileCleaned
-      if bSuccess is not True:
-         raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
 
-      dictJsonValues = {}
+      dictJsonValues = None
       try:
-         hDocumentationProjectConfigFile = open(sJsonFileCleaned)
-         dictJsonValues = json.load(hDocumentationProjectConfigFile)
-         hDocumentationProjectConfigFile.close()
+         dictJsonValues = json.loads("\n".join(listLines))
       except Exception as reason:
          bSuccess = None
-         sResult  = str(reason) + f" - while reading from '{sDocumentationProjectConfigFile}'"
+         sResult  = str(reason) + f" - while parsing JSON content of '{sDocumentationProjectConfigFile}'"
+         raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
+
+      if dictJsonValues is None:
+         bSuccess = None
+         sResult  = "dictJsonValues is None"
          raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
 
       # check for unexpected keys
       tupleKeysAllowedInPackageDocConfig = ("CONTROL",
                                             "TOC",
                                             "PARAMS",
                                             "DOCUMENT",
                                             "PICTURES",
+                                            "DIAGRAMS",
                                             "OUTPUT",
                                             "PDFDEST",
                                             "CONFIGDEST",
-                                            "TEX")
+                                            "TEX",
+                                            "JAVA",
+                                            "PLANT_UML")
 
       for sKey in dictJsonValues.keys():
          if sKey not in tupleKeysAllowedInPackageDocConfig:
             bSuccess = None
             sResult  = f"Found not expected key '{sKey}' within '{sDocumentationProjectConfigFile}'"
             raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
 
@@ -164,15 +164,15 @@
       #    distingushing between required and optional parameters and checking the
       #    availability of mandatory values
       # TODO: Moo much for a constructor? Move to separate method? Better ways to
       #       validate the content in json file?
 
       # required
       if 'CONTROL' in dictJsonValues:
-         self.__dictPackageDocConfig['CONTROL']  = dictJsonValues['CONTROL']
+         self.__dictPackageDocConfig['CONTROL'] = dictJsonValues['CONTROL']
       else:
          bSuccess = None
          sResult  = f"Missing key 'CONTROL' within '{sDocumentationProjectConfigFile}'"
          raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
       # ==============================================================================================================
       # 21.11.2022 Feature 'INCLUDEPRIVATE' switched off. TODO: needs several bugfixes
       self.__dictPackageDocConfig['CONTROL']['INCLUDEPRIVATE'] = False
@@ -214,14 +214,20 @@
 
       # optional
       if 'PICTURES' in dictJsonValues:
          self.__dictPackageDocConfig['PICTURES'] = dictJsonValues['PICTURES']
       else:
          self.__dictPackageDocConfig['PICTURES'] = None
 
+      # optional
+      if 'DIAGRAMS' in dictJsonValues:
+         self.__dictPackageDocConfig['DIAGRAMS'] = dictJsonValues['DIAGRAMS']
+      else:
+         self.__dictPackageDocConfig['DIAGRAMS'] = None
+
       # required
       if 'OUTPUT' in dictJsonValues:
          self.__dictPackageDocConfig['OUTPUT'] = dictJsonValues['OUTPUT']
       else:
          bSuccess = None
          sResult  = f"Missing key 'OUTPUT' within '{sDocumentationProjectConfigFile}'"
          raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
@@ -242,14 +248,26 @@
       if 'TEX' in dictJsonValues:
          self.__dictPackageDocConfig['TEX'] = dictJsonValues['TEX']
       else:
          bSuccess = None
          sResult  = f"Missing key 'TEX' within '{sDocumentationProjectConfigFile}'"
          raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
 
+      # optional (but PLANT_UML requires JAVA; in case of PLANT_UML is requested, JAVA needs to be defined)
+      if 'JAVA' in dictJsonValues:
+         self.__dictPackageDocConfig['JAVA'] = dictJsonValues['JAVA']
+      else:
+         self.__dictPackageDocConfig['JAVA'] = None
+
+      # optional
+      if 'PLANT_UML' in dictJsonValues:
+         self.__dictPackageDocConfig['PLANT_UML'] = dictJsonValues['PLANT_UML']
+      else:
+         self.__dictPackageDocConfig['PLANT_UML'] = None
+
       # Now we have all configuration values available in self.__dictPackageDocConfig. Next steps are:
       # - resolve placeholders (possible placeholders are the keys from repository configuration)
       # - normalize paths
 
       # - check document parts in TOC section
       listDocumentPartsDefined = self.__dictPackageDocConfig['TOC'].keys()
       listDocumentPartsUsed = self.__dictPackageDocConfig['TOC']['DOCUMENTPARTS']
@@ -292,28 +310,28 @@
 
       # - normalize paths in 'DOCUMENTPARTS' section
       listDocumentParts = self.__dictPackageDocConfig['TOC']['DOCUMENTPARTS']
       for sDocumentPart in listDocumentParts:
          self.__dictPackageDocConfig['TOC'][sDocumentPart] = CString.NormalizePath(sPath=self.__dictPackageDocConfig['TOC'][sDocumentPart], sReferencePathAbs=sReferencePathAbs)
 
       # -- set further config keys (to enable the resolve of placeholders and the normalizing of paths running in a loop)
-      tupleFurtherConfigKeys = ('PICTURES', 'OUTPUT', 'PDFDEST', 'CONFIGDEST') # values contain paths and can contain placeholders; some of them are optional
+      tupleFurtherConfigKeys = ('PICTURES', 'DIAGRAMS', 'OUTPUT', 'PDFDEST', 'CONFIGDEST') # values contain paths and can contain placeholders; some of them are optional
       # -- resolve placeholder and normalize paths
       for sConfigKey in tupleFurtherConfigKeys:
          sPackageDocValue = self.__dictPackageDocConfig[sConfigKey]
          if sPackageDocValue is not None:
             # resolve placeholder in further config keys (possible placeholder are the keys from repository configuration)
             for repo_key, repo_value in dictRepositoryConfig.items():
                if type(repo_value) == str:
                   sPackageDocValue = sPackageDocValue.replace(f"###{repo_key}###", repo_value)
 
             # normalize path and write value back to dict
             self.__dictPackageDocConfig[sConfigKey] = CString.NormalizePath(sPath=sPackageDocValue, sReferencePathAbs=sReferencePathAbs)
 
-      # -- prepare path to LaTeX interpreter
+      # -- prepare path to LaTeX interpreter (mandatory)
       sLaTeXInterpreter = None
       sKey = sPlatformSystem.upper()
       if sKey in self.__dictPackageDocConfig['TEX']:
          sLaTeXInterpreter = CString.NormalizePath(sPath=self.__dictPackageDocConfig['TEX'][sKey], sReferencePathAbs=sReferencePathAbs)
       else:
          bSuccess = None
          sResult  = f"LaTeX interpreter not defined for current operating system '{sPlatformSystem}' in section 'TEX' of '{sDocumentationProjectConfigFile}'"
@@ -326,14 +344,44 @@
       sStylesFolder = f"{sThisFilePath}/styles"
       if os.path.isdir(sStylesFolder) is False:
          bSuccess = None
          sResult  = f"Missing LaTeX stylesheet folder '{sStylesFolder}'"
          raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
       self.__dictPackageDocConfig['LATEXSTYLESFOLDER'] = sStylesFolder
 
+      # -- Prepare path to Java (optional)
+      #    Usage of Java depends on availability of diagram files (DIAGRAMS) and PLANT_UML (like configured in packagedoc_config.json;
+      #    computation in CDocBuilder)
+      if self.__dictPackageDocConfig['JAVA'] is not None:
+         JAVA = None
+         sKey = sPlatformSystem.upper()
+         if sKey in self.__dictPackageDocConfig['JAVA']:
+            JAVA = CString.NormalizePath(sPath=self.__dictPackageDocConfig['JAVA'][sKey], sReferencePathAbs=sReferencePathAbs)
+         else:
+            bSuccess = None
+            sResult  = f"Java not defined for current operating system '{sPlatformSystem}' in section 'JAVA' of '{sDocumentationProjectConfigFile}'"
+            raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
+         self.__dictPackageDocConfig['JAVA'] = JAVA
+      # eof if self.__dictPackageDocConfig['JAVA'] is not None:
+
+      # -- Prepare path to PlantUML (optional)
+      #    Usage of PlantUML depends on availability of diagram files (DIAGRAMS) and PLANT_UML (like configured in packagedoc_config.json;
+      #    computation in CDocBuilder; PlantUML also requires JAVA)
+      if self.__dictPackageDocConfig['PLANT_UML'] is not None:
+         PLANT_UML = None
+         sKey = sPlatformSystem.upper()
+         if sKey in self.__dictPackageDocConfig['PLANT_UML']:
+            PLANT_UML = CString.NormalizePath(sPath=self.__dictPackageDocConfig['PLANT_UML'][sKey], sReferencePathAbs=sReferencePathAbs)
+         else:
+            bSuccess = None
+            sResult  = f"PlantUML not defined for current operating system '{sPlatformSystem}' in section 'PLANT_UML' of '{sDocumentationProjectConfigFile}'"
+            raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
+         self.__dictPackageDocConfig['PLANT_UML'] = PLANT_UML
+      # eof if self.__dictPackageDocConfig['PLANT_UML'] is not None:
+
       # ---- prepare dictionary with all parameter that shall have runtime character (flat list instead of nested dict like in packagedoc configuration)
 
       dictRuntimeVariables = None
 
       # -- 1. from repository configuration
       dictRuntimeVariables = oRepositoryConfig.GetConfig()
```

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/CPatterns.py` & `GenPackageDoc-0.40.3/GenPackageDoc/CPatterns.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/CSourceParser.py` & `GenPackageDoc-0.40.3/GenPackageDoc/CSourceParser.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/GenPackageDoc.pdf` & `GenPackageDoc-0.40.3/GenPackageDoc/GenPackageDoc.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 22% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 GenPackageDoc
-v. 0.39.3
+v. 0.40.3
 Holger Queckenstedt
-05.05.2023
+06.06.2023
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -80,148 +80,173 @@
 
 2.7.2
 
 Syntax extensions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 9
 
+Diagrams . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+
+10
+
+2.8.1
+
+Example 1: Sequence diagram
+
+. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+
+10
+
+2.8.2
+
+Example 2: JSON diagram . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+
+11
+
+2.8.3
+
+Picture import . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+
+11
+
+2.8
+
 3 CDocBuilder.py
 3.1
 
-10
+12
 
 Class: CDocBuilder . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-10
+12
 
 3.1.1
 
-10
+12
 
 Method: Build . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 4 CInterface.py
 4.1
 
-11
+13
 
 Class: CInterface . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-11
+13
 
 4.1.1
 
-11
+13
 
 Method: GetLaTeXStyles . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 5 CPackageDocConfig.py
 
-12
+14
 
 5.1
 
 Function: printerror . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-12
+14
 
 5.2
 
 Class: CPackageDocConfig . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-12
+14
 
 5.2.1
 
 Method: PrintConfig . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-12
+14
 
 5.2.2
 
 Method: PrintConfigKeys . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-12
+14
 
 5.2.3
 
 Method: Get . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-12
+14
 
 5.2.4
 
 Method: GetConfig
 
-12
+14
 
 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 6 CPatterns.py
 6.1
 
-13
+15
 
 Class: CPatterns . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-13
+15
 
 6.1.1
 
 Method: GetHeader . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-13
+15
 
 6.1.2
 
 Method: GetChapter . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-14
+16
+
+A
+
+CONTENTS
+
+CONTENTS
 
 6.1.3
 
 Method: GetFooter . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-14
+16
 
 6.1.4
 
 Method: GetAutodefinedHeader . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-14
+16
 
 7 CSourceParser.py
-
-15
-
-A
-
-CONTENTS
-
 7.1
 
-CONTENTS
+17
 
 Class: CSourceParser . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-15
+17
 
 7.1.1
 
-15
+17
 
 Method: ParseSourceFile . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 8 Appendix
 
-16
+18
 
 9 History
 
-17
+19
 
 B
 
 CHAPTER 1. INTRODUCTION
 
 Chapter 1
 
@@ -599,14 +624,101 @@
 line!
 Internally this double slash is mapped to the LaTeX command \newpage.
 These syntax extensions can currently be used in separate RST files only and are not available within docstrings of
 Python modules.
 
 9
 
+CHAPTER 2. DESCRIPTION
+
+2.8
+
+2.8. DIAGRAMS
+
+Diagrams
+
+A diagram in this context is a picture that is rendered out of source code. GenPackageDoc supports PlantUML
+that supports a wide range of diagrams.
+To use the PlantUML functionality with GenPackageDoc, some preconditions have to be fulfilled:
+1. PlantUML is installed (either as stand-alone installation or as VSCodium extension)
+2. GenPackageDoc is configured (packagedoc config.json):
+a. In section "DIAGRAMS" a path to a diagrams folder is defined (containing the diagrams source code).
+b. In section "JAVA" path and name of the java interpreter is defined (because PlantUML is a java application).
+c. In section "PLANT UML" path and name of the PlantUML application is defined.
+All PlantUML source code files within the "DIAGRAMS" folder need to have the extension puml.
+
+2.8.1
+
+Example 1: Sequence diagram
+
+The following code of a puml file produces a sequence diagram:
+@startuml
+GenPackageDoc -> ConstructionWorkerBob: Hello Bob!
+ConstructionWorkerBob --> GenPackageDoc: Hi GenPackageDoc, how are you?
+GenPackageDoc -> ConstructionWorkerBob: Fine, thanks.
+ConstructionWorkerBob --> GenPackageDoc: Have a nice day.
+@enduml
+Result:
+
+10
+
+CHAPTER 2. DESCRIPTION
+
+2.8.2
+
+2.8. DIAGRAMS
+
+Example 2: JSON diagram
+
+The following code of a puml file produces a sequence diagram:
+@startjson
+{
+"WelcomeString"
+
+: "Hello World",
+
+"Maximum_version" : "1.0.0",
+"Minimum_version" : "0.6.0",
+"Project"
+"TargetName"
+
+: "Example Project",
+: "Example Target",
+
+"params" : {
+"global" : {
+"str_val"
+: "string value",
+"int_val"
+: 123,
+"float_val" : 4.56,
+"bool_val" : true,
+"null_val" : null,
+"dict_val" : {"keyA" : "keyA_val", "keyB" : "keyB_val"},
+"list_val" : ["A", 1, true]}
+}
+}
+@endjson
+Result:
+
+2.8.3
+
+Picture import
+
+In case of PlantUML is configured in the GenPackageDoc configuration and in case of puml files are available
+within the diagrams folder, GenPackageDoc automatically calls PlantUML to render the diagrams. They can be
+imported in the following way:
+1. Import in RST code:
+.. image:: ./diagrams/SequenceDiagram.png
+2. Import in LaTeX code:
+\includegraphics[scale=0.7]{./diagrams/SequenceDiagram.png}
+The user needs to adapt the scaling to make the rendered diagrams fit to a page of a PDF document in best way.
+But this scaling only works in LaTeX code, but not in RST code.
+11
+
 CHAPTER 3. CDOCBUILDER.PY
 
 Chapter 3
 
 CDocBuilder.py
 Python module containing all methods to generate tex sources.
 
@@ -633,15 +745,15 @@
 / Type: bool /
 Indicates if the computation of the method sMethod was successful or not.
  sResult
 
 / Type: str /
 The result of the computation of the method sMethod.
 
-10
+12
 
 CHAPTER 4. CINTERFACE.PY
 
 Chapter 4
 
 CInterface.py
 Python module containing an interface for GenPackageDoc. This interface can be used to get access to the LaTeX
@@ -671,15 +783,15 @@
 / Type: bool /
 Indicates if the computation of the method sMethod was successful or not.
  sResult
 
 / Type: str /
 The result of the computation of the method sMethod.
 
-11
+13
 
 CHAPTER 5. CPACKAGEDOCCONFIG.PY
 
 Chapter 5
 
 CPackageDocConfig.py
 Python module containing the configuration for GenPackageDoc. This includes the repository configurantion and
@@ -716,15 +828,15 @@
 
 5.2.4
 
 Method: GetConfig
 
 Returns the complete configuration dictionary.
 
-12
+14
 
 CHAPTER 6. CPATTERNS.PY
 
 Chapter 6
 
 CPatterns.py
 Python module containing source patterns used to generate the tex file output.
@@ -763,15 +875,15 @@
 The date of the output document (date of the described package)
 Returns:
  sHeader
 
 / Type: str /
 LaTeX code containing the header of main tex file.
 
-13
+15
 
 CHAPTER 6. CPATTERNS.PY
 
 6.1.2
 
 6.1. CLASS: CPATTERNS
 
@@ -822,15 +934,15 @@
 (no arguments)
 Returns:
  sAutodefinedHeader
 
 / Type: str /
 LaTeX code containing the header of the autodefined LaTeX sty file.
 
-14
+16
 
 CHAPTER 7. CSOURCEPARSER.PY
 
 Chapter 7
 
 CSourceParser.py
 Python module containing all methods to parse the documentation content of Python source files.
@@ -873,15 +985,15 @@
 / Type: bool /
 Indicates if the computation of the method sMethod was successful or not.
  sResult
 
 / Type: str /
 The result of the computation of the method sMethod.
 
-15
+17
 
 CHAPTER 8. APPENDIX
 
 Chapter 8
 
 Appendix
 About this package:
@@ -892,19 +1004,19 @@
 
 Name
 
 GenPackageDoc
 
 Version
 
-0.39.3
+0.40.3
 
 Date
 
-05.05.2023
+06.06.2023
 
 Description
 
 Documentation builder for Python packages
 
 Package URL
 
@@ -942,15 +1054,15 @@
 
 Intended Audience :: Developers
 
 Topic
 
 Topic :: Software Development
 
-16
+18
 
 CHAPTER 9. HISTORY
 
 Chapter 9
 
 History
 History of GenPackageDoc (hosted in repository python-genpackagedoc).
@@ -1028,15 +1140,15 @@
 - Admonitions added, based on LaTeX environment tcolorbox
 - Layout adaptions in titlepage
 - Page numbering fix in TOC
 0.13.0
 
 24.05.2022
 
-17
+19
 
 CHAPTER 9. HISTORY
 
 LaTeX style definitions moved to separate folder
 0.14.0
 
 27.05.2022
@@ -1134,15 +1246,15 @@
 12.09.2022
 
 Fix of import path of a module in PDF file
 0.32.0
 
 16.09.2022
 
-18
+20
 
 CHAPTER 9. HISTORY
 
 - Added labels at chapter level
 - partial rework of label mechanisms
 0.33.0
 
@@ -1184,16 +1296,21 @@
 Removed harming ligatures that were added by Pandoc automatically to LaTeX
 code in case of multiple minus characters in names
 0.39.0
 
 06.01.2023
 
 Added masking of underlines in case of the content of \repo or \pkg contain
-underlines (masking required by LaTeX).
+underlines (masking required by LaTeX)
+0.40.0
+
+09.05.2023
+
+Added PlantUML support to render diagrams out of source code in text format
 
 GenPackageDoc.pdf
-Created at 05.05.2023 - 14:02:38
-by GenPackageDoc v. 0.39.3
+Created at 07.06.2023 - 13:56:19
+by GenPackageDoc v. 0.40.3
 
-19
+21
```

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/__init__.py` & `GenPackageDoc-0.40.3/GenPackageDoc/__init__.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/styles/admonitions.sty` & `GenPackageDoc-0.40.3/GenPackageDoc/styles/admonitions.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/styles/common.sty` & `GenPackageDoc-0.40.3/GenPackageDoc/styles/common.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/styles/pandoc.sty` & `GenPackageDoc-0.40.3/GenPackageDoc/styles/pandoc.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/styles/preamble.tex` & `GenPackageDoc-0.40.3/GenPackageDoc/styles/preamble.tex`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/styles/robotframeworkaio.sty` & `GenPackageDoc-0.40.3/GenPackageDoc/styles/robotframeworkaio.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc/version.py` & `GenPackageDoc-0.40.3/GenPackageDoc/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of GenPackageDoc
 #
-VERSION      = "0.39.3"
-VERSION_DATE = "05.05.2023"
+VERSION      = "0.40.3"
+VERSION_DATE = "06.06.2023"
```

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc.egg-info/PKG-INFO` & `GenPackageDoc-0.40.3/GenPackageDoc.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenPackageDoc
-Version: 0.39.3
+Version: 0.40.3
 Summary: Documentation builder for Python packages
 Home-page: https://github.com/test-fullautomation/python-genpackagedoc
 Author: Holger Queckenstedt
 Author-email: Holger.Queckenstedt@de.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -49,28 +49,69 @@
     pip install GenPackageDoc
     ```
 
     [GenPackageDoc in PyPi](https://pypi.org/project/GenPackageDoc/)
 
 2.  Installation via GitHub (recommended for developers)
 
-    Clone the **python-genpackagedoc** repository to your machine.
+    -   Clone the **python-genpackagedoc** repository to your machine
 
-    ``` {.}
-    git clone https://github.com/test-fullautomation/python-genpackagedoc.git
-    ```
+        ``` {.}
+        git clone https://github.com/test-fullautomation/python-genpackagedoc.git
+        ```
 
-    [GenPackageDoc in
-    GitHub](https://github.com/test-fullautomation/python-genpackagedoc)
+        [GenPackageDoc in
+        GitHub](https://github.com/test-fullautomation/python-genpackagedoc)
 
-    Use the following command to install **GenPackageDoc**:
+    -   Install dependencies
 
-    ``` {.}
-    setup.py install
-    ```
+        **GenPackageDoc** requires some additional Python libraries.
+        Before you install the cloned repository sources you have to
+        install the dependencies manually. The names of all related
+        packages you can find in the file `requirements.txt` in the
+        repository root folder. Use pip to install them:
+
+        ``` {.}
+        pip install -r requirements.txt
+        ```
+
+        Additionally install **LaTeX** (recommended: TeX Live). This is
+        required.
+
+        Additionally install **PlantUML**. This is an option.
+
+    -   Configure dependencies
+
+        **GenPackageDoc** uses **LaTeX** to generate the documentation
+        in PDF format. **GenPackageDoc** also supports **PlantUML**.
+        **PlantUML** requires **Java**.
+
+        **GenPackageDoc** needs to know where to find those
+        applications. This is defined in the **GenPackageDoc**
+        configuration file
+
+        ``` {.}
+        packagedoc\packagedoc_config.json
+        ```
+
+        Before you start the installation you have to introduce the
+        following environment variables, that are used in
+        `packagedoc_config.json`:
+
+        -   `GENDOC_LATEXPATH` : path to `pdflatex` executable
+        -   `GENDOC_PLANTUML_PATH` : path to `plantuml` executable
+            (optional)
+        -   `JAVA_HOME` : path to `java` executable (optional, only in
+            case of **PlantUML** is used)
+
+    -   Use the following command to install **GenPackageDoc**:
+
+        ``` {.}
+        setup.py install
+        ```
 
 How to use
 ----------
 
 **GenPackageDoc** provides a toolchain to generate documentation out of
 Python sources that are stored within a repository. **GenPackageDoc** is
 also designed to be able to consider setup informations of a repository.
```

### Comparing `GenPackageDoc-0.39.3/GenPackageDoc.egg-info/SOURCES.txt` & `GenPackageDoc-0.40.3/GenPackageDoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.3/LICENSE` & `GenPackageDoc-0.40.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.3/PKG-INFO` & `GenPackageDoc-0.40.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenPackageDoc
-Version: 0.39.3
+Version: 0.40.3
 Summary: Documentation builder for Python packages
 Home-page: https://github.com/test-fullautomation/python-genpackagedoc
 Author: Holger Queckenstedt
 Author-email: Holger.Queckenstedt@de.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -49,28 +49,69 @@
     pip install GenPackageDoc
     ```
 
     [GenPackageDoc in PyPi](https://pypi.org/project/GenPackageDoc/)
 
 2.  Installation via GitHub (recommended for developers)
 
-    Clone the **python-genpackagedoc** repository to your machine.
+    -   Clone the **python-genpackagedoc** repository to your machine
 
-    ``` {.}
-    git clone https://github.com/test-fullautomation/python-genpackagedoc.git
-    ```
+        ``` {.}
+        git clone https://github.com/test-fullautomation/python-genpackagedoc.git
+        ```
 
-    [GenPackageDoc in
-    GitHub](https://github.com/test-fullautomation/python-genpackagedoc)
+        [GenPackageDoc in
+        GitHub](https://github.com/test-fullautomation/python-genpackagedoc)
 
-    Use the following command to install **GenPackageDoc**:
+    -   Install dependencies
 
-    ``` {.}
-    setup.py install
-    ```
+        **GenPackageDoc** requires some additional Python libraries.
+        Before you install the cloned repository sources you have to
+        install the dependencies manually. The names of all related
+        packages you can find in the file `requirements.txt` in the
+        repository root folder. Use pip to install them:
+
+        ``` {.}
+        pip install -r requirements.txt
+        ```
+
+        Additionally install **LaTeX** (recommended: TeX Live). This is
+        required.
+
+        Additionally install **PlantUML**. This is an option.
+
+    -   Configure dependencies
+
+        **GenPackageDoc** uses **LaTeX** to generate the documentation
+        in PDF format. **GenPackageDoc** also supports **PlantUML**.
+        **PlantUML** requires **Java**.
+
+        **GenPackageDoc** needs to know where to find those
+        applications. This is defined in the **GenPackageDoc**
+        configuration file
+
+        ``` {.}
+        packagedoc\packagedoc_config.json
+        ```
+
+        Before you start the installation you have to introduce the
+        following environment variables, that are used in
+        `packagedoc_config.json`:
+
+        -   `GENDOC_LATEXPATH` : path to `pdflatex` executable
+        -   `GENDOC_PLANTUML_PATH` : path to `plantuml` executable
+            (optional)
+        -   `JAVA_HOME` : path to `java` executable (optional, only in
+            case of **PlantUML** is used)
+
+    -   Use the following command to install **GenPackageDoc**:
+
+        ``` {.}
+        setup.py install
+        ```
 
 How to use
 ----------
 
 **GenPackageDoc** provides a toolchain to generate documentation out of
 Python sources that are stored within a repository. **GenPackageDoc** is
 also designed to be able to consider setup informations of a repository.
```

### Comparing `GenPackageDoc-0.39.3/setup.py` & `GenPackageDoc-0.40.3/setup.py`

 * *Files identical despite different names*

