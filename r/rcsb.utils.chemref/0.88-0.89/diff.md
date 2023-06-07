# Comparing `tmp/rcsb.utils.chemref-0.88.tar.gz` & `tmp/rcsb.utils.chemref-0.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.chemref-0.88.tar", last modified: Mon May 22 13:46:14 2023, max compression
+gzip compressed data, was "rcsb.utils.chemref-0.89.tar", last modified: Wed Jun  7 16:07:53 2023, max compression
```

## Comparing `rcsb.utils.chemref-0.88.tar` & `rcsb.utils.chemref-0.89.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:46:14.064298 rcsb.utils.chemref-0.88/
--rw-r--r--   0 vsts      (1001) docker     (122)     5567 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1730 2023-05-22 13:46:14.064298 rcsb.utils.chemref-0.88/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1034 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:46:14.060297 rcsb.utils.chemref-0.88/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:46:14.060297 rcsb.utils.chemref-0.88/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:46:14.064298 rcsb.utils.chemref-0.88/rcsb/utils/chemref/
--rw-r--r--   0 vsts      (1001) docker     (122)    10179 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/AtcProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6625 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/BirdProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3616 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/CARDProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4726 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/CODProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12549 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/ChEMBLProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7749 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/ChemCompModelProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9068 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/ChemCompProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16161 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/DrugBankProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9477 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/DrugBankReader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3674 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/DrugCentralProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3858 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/PharosProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2509 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/PharosReadSqlDump.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7494 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/PsiModProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4060 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/PubChemProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    54562 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/PubChemUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6478 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/RcsbLigandScoreProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6669 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/ResidProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1586 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/ResidReader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-22 13:36:40.000000 rcsb.utils.chemref-0.88/rcsb/utils/chemref/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:46:14.060297 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1730 2023-05-22 13:46:14.000000 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1077 2023-05-22 13:46:14.000000 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 13:46:14.000000 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 13:37:28.000000 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      197 2023-05-22 13:46:14.000000 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-22 13:46:14.000000 rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-05-22 13:36:41.000000 rcsb.utils.chemref-0.88/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-22 13:46:14.064298 rcsb.utils.chemref-0.88/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2227 2023-05-22 13:36:41.000000 rcsb.utils.chemref-0.88/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 16:07:53.688623 rcsb.utils.chemref-0.89/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5628 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1730 2023-06-07 16:07:53.688623 rcsb.utils.chemref-0.89/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1034 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 16:07:53.684623 rcsb.utils.chemref-0.89/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 16:07:53.684623 rcsb.utils.chemref-0.89/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 16:07:53.688623 rcsb.utils.chemref-0.89/rcsb/utils/chemref/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10179 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/AtcProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6625 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/BirdProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3616 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/CARDProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4726 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/CODProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12549 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/ChEMBLProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7749 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/ChemCompModelProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9678 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/ChemCompProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16161 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/DrugBankProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9477 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/DrugBankReader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3674 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/DrugCentralProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3858 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/PharosProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2509 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/PharosReadSqlDump.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7494 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/PsiModProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4060 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/PubChemProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    54562 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/PubChemUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6478 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/RcsbLigandScoreProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6669 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/ResidProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1586 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/ResidReader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/rcsb/utils/chemref/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 16:07:53.684623 rcsb.utils.chemref-0.89/rcsb.utils.chemref.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1730 2023-06-07 16:07:53.000000 rcsb.utils.chemref-0.89/rcsb.utils.chemref.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1077 2023-06-07 16:07:53.000000 rcsb.utils.chemref-0.89/rcsb.utils.chemref.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-07 16:07:53.000000 rcsb.utils.chemref-0.89/rcsb.utils.chemref.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-07 15:59:01.000000 rcsb.utils.chemref-0.89/rcsb.utils.chemref.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      197 2023-06-07 16:07:53.000000 rcsb.utils.chemref-0.89/rcsb.utils.chemref.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-06-07 16:07:53.000000 rcsb.utils.chemref-0.89/rcsb.utils.chemref.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-06-07 16:07:53.688623 rcsb.utils.chemref-0.89/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2227 2023-06-07 15:58:15.000000 rcsb.utils.chemref-0.89/setup.py
```

### Comparing `rcsb.utils.chemref-0.88/HISTORY.txt` & `rcsb.utils.chemref-0.89/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -74,7 +74,8 @@
  28-Mar-2022  - V0.82 Fix pylint issue with "Iterated dict modified inside for loop body" in testChemCompProvider
  25-Jul-2022  - V0.83 Revert last change to AtcProvider - source NCBO ATC files were updated again to restore previous format
  27-Jul-2022  - V0.84 Adapt to multiple possible naming schemes for ATC class IDs
   9-Jan-2023  - V0.85 Configuration changes to support tox 4
  22-Mar-2023  - V0.86 Update references to py-rcsb_exdb_assets master branch
  19-Apr-2023  - V0.87 Update file path in ATCProvider
  19-May-2023  - V0.88 Update DNS to PDB archive
+  5-Jun-2023  - V0.89 Include bond count in ChemCompProvider
```

### Comparing `rcsb.utils.chemref-0.88/LICENSE` & `rcsb.utils.chemref-0.89/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/PKG-INFO` & `rcsb.utils.chemref-0.89/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.chemref
-Version: 0.88
+Version: 0.89
 Summary: RCSB Python Chemical Reference Data Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_chemref
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.chemref-0.88/README.md` & `rcsb.utils.chemref-0.89/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/AtcProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/AtcProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/BirdProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/BirdProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/CARDProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/CARDProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/CODProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/CODProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/ChEMBLProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/ChEMBLProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/ChemCompModelProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/ChemCompModelProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/ChemCompProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/ChemCompProvider.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ##
 # File:    ChemCompProvider.py
 # Author:  J. Westbrook
 # Date:    22-Nov-2019
 #
 # Updates:
-#
+#   7-Jun-2023 aae  Include bond count in chem comp data and fix typo
 ##
 """
 Utilities to provide essential data items for chemical component definitions.
 """
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
@@ -33,15 +33,15 @@
         super(ChemCompProvider, self).__init__(cachePath, [dirName])
         #
         urlTarget = kwargs.get("ccUrlTarget", "http://files.wwpdb.org/pub/pdb/data/monomers/components.cif.gz")
         # self.__birdUrlTarget = kwargs.get("birdUrlTarget", "ftp://ftp.wwpdb.org/pub/pdb/data/bird/prd/prdcc-all.cif.gz")
         #
         dirPath = os.path.join(cachePath, dirName)
         useCache = kwargs.get("useCache", True)
-        ccdFileName = kwargs.get("ccdFileName", "ccd_abbridged_definitions.json")
+        ccdFileName = kwargs.get("ccdFileName", "ccd_abridged_definitions.json")
         #
         self.__mU = MarshalUtil(workPath=dirPath)
         #
         relDataUrlTarget = kwargs.get("relDataUrlTarget", "https://github.com/rcsb/py-rcsb_exdb_assets/raw/master/fall_back/chem-comp-release-data-summary.json")
         self.__ccdRelD = self.__reloadRelData(relDataUrlTarget, dirPath, useCache=useCache)
         #
         self.__ccdD = self.__reload(urlTarget, dirPath, ccdFileName, useCache=useCache)
@@ -95,29 +95,36 @@
     def getAtomCountChiral(self, ccId):
         try:
             return self.__ccdD[ccId]["atom_count_chiral"]
         except Exception:
             pass
         return 0
 
+    def getBondCount(self, ccId):
+        try:
+            return self.__ccdD[ccId]["bond_count"]
+        except Exception:
+            pass
+        return 0
+
     def getFormulaWeight(self, ccId):
         try:
             return float(self.__ccdD[ccId]["formula_weight"])
         except Exception:
             pass
         return None
 
     def getComponentIds(self):
         try:
             return list(self.__ccdD.keys())
         except Exception:
             pass
         return []
 
-    def getAbbridged(self):
+    def getAbridged(self):
         return self.__ccdD
 
     def getReleaseDate(self, ccId):
         try:
             return self.__ccdRelD[ccId.upper()][1]
         except Exception:
             pass
@@ -162,15 +169,15 @@
         elif not useCache:
             ok = True
             if not (useCache and fU.exists(filePath)):
                 logger.info("Fetching url %s for resource file %s", urlTarget, filePath)
                 ok = fU.get(urlTarget, filePath)
             if ok:
                 cL = self.__mU.doImport(filePath, fmt="mmcif")
-                mD = self.__buildAbbridged(cL)
+                mD = self.__buildAbridged(cL)
                 ok = self.__mU.doExport(ccdFilePath, mD, fmt="json", indent=3)
         #
         return mD
 
     def __reloadRelData(self, urlTarget, dirPath, useCache=True):
         """Reload chemical component release data details.
 
@@ -205,16 +212,16 @@
                 logger.info("Fetching url %s for resource file %s", urlTarget, filePath)
                 ok = fU.get(urlTarget, filePath)
             if ok:
                 cD = self.__mU.doImport(filePath, fmt="json")
         #
         return cD["release_data"] if "release_data" in cD else {}
 
-    def __buildAbbridged(self, cL):
-        """Return a dictionary of abbridged CCD info."""
+    def __buildAbridged(self, cL):
+        """Return a dictionary of abridged CCD info."""
         atNameList = [
             "id",
             "name",
             "type",
             "pdbx_type",
             "formula",
             "mon_nstd_parent_comp_id",
@@ -254,18 +261,29 @@
                 for ii in range(numAtoms):
                     el = cObj.getValue("type_symbol", ii)
                     if el != "H":
                         numAtomsHeavy += 1
                     chFlag = cObj.getValue("pdbx_stereo_config", ii)
                     if chFlag != "N":
                         numAtomsChiral += 1
-            except Exception:
+            except AttributeError:
                 logger.warning("Missing chem_comp_atom category for %s", ccId)
                 numAtoms = 0
                 numAtomsHeavy = 0
                 numAtomsChiral = 0
             #
             retD[ccId]["atom_count"] = numAtoms
             retD[ccId]["atom_count_chiral"] = numAtomsChiral
             retD[ccId]["atom_count_heavy"] = numAtomsHeavy
             #
+            # Get the number of bonds
+            try:
+                cObj = dataContainer.getObj("chem_comp_bond")
+                numBonds = cObj.getRowCount()
+            except AttributeError:
+                logger.warning("Missing chem_comp_bond category for %s", ccId)
+                numBonds = 0
+            #
+            retD[ccId]["bond_count"] = numBonds
+
+            #
         return retD
```

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/DrugBankProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/DrugBankProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/DrugBankReader.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/DrugBankReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/DrugCentralProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/DrugCentralProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/PharosProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/PharosProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/PharosReadSqlDump.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/PharosReadSqlDump.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/PsiModProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/PsiModProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/PubChemProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/PubChemProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/PubChemUtils.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/PubChemUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/RcsbLigandScoreProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/RcsbLigandScoreProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/ResidProvider.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/ResidProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb/utils/chemref/ResidReader.py` & `rcsb.utils.chemref-0.89/rcsb/utils/chemref/ResidReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/PKG-INFO` & `rcsb.utils.chemref-0.89/rcsb.utils.chemref.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.chemref
-Version: 0.88
+Version: 0.89
 Summary: RCSB Python Chemical Reference Data Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_chemref
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.chemref-0.88/rcsb.utils.chemref.egg-info/SOURCES.txt` & `rcsb.utils.chemref-0.89/rcsb.utils.chemref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.88/setup.py` & `rcsb.utils.chemref-0.89/setup.py`

 * *Files identical despite different names*

