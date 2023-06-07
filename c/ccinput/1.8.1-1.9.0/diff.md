# Comparing `tmp/ccinput-1.8.1.tar.gz` & `tmp/ccinput-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccinput-1.8.1.tar", last modified: Wed May 24 15:34:38 2023, max compression
+gzip compressed data, was "ccinput-1.9.0.tar", last modified: Wed Jun  7 00:55:14 2023, max compression
```

## Comparing `ccinput-1.8.1.tar` & `ccinput-1.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:34:38.119289 ccinput-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-24 15:33:49.000000 ccinput-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 15:33:49.000000 ccinput-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-24 15:34:38.119289 ccinput-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-24 15:33:49.000000 ccinput-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:34:38.119289 ccinput-1.8.1/ccinput/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-24 15:34:38.119289 ccinput-1.8.1/ccinput/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)    76266 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/documentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:34:38.115289 ccinput-1.8.1/ccinput/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/drivers/pysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:34:38.115289 ccinput-1.8.1/ccinput/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/nwchem.py
--rw-r--r--   0 runner    (1001) docker     (123)    15963 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/psi4.py
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/qchem.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/xtb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/presets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:34:38.119289 ccinput-1.8.1/ccinput/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   111131 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    59121 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_orca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_psi4.py
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_pysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    47385 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_qchem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    22171 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_xtb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/testing_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/verify_sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:34:38.115289 ccinput-1.8.1/ccinput.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-24 15:33:49.000000 ccinput-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-24 15:34:38.119289 ccinput-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-24 15:33:49.000000 ccinput-1.8.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-24 15:33:49.000000 ccinput-1.8.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:55:14.417142 ccinput-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-07 00:54:18.000000 ccinput-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-07 00:54:18.000000 ccinput-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-07 00:55:14.417142 ccinput-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-07 00:54:18.000000 ccinput-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:55:14.421142 ccinput-1.9.0/ccinput/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-07 00:55:14.421142 ccinput-1.9.0/ccinput/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90291 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:55:14.417142 ccinput-1.9.0/ccinput/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/drivers/pysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:55:14.417142 ccinput-1.9.0/ccinput/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/nwchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15963 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/xtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/presets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:55:14.417142 ccinput-1.9.0/ccinput/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111131 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59121 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_pysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47385 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_qchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22171 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_xtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/testing_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/verify_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:55:14.413142 ccinput-1.9.0/ccinput.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 00:54:18.000000 ccinput-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-07 00:55:14.421142 ccinput-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-07 00:54:18.000000 ccinput-1.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-07 00:54:18.000000 ccinput-1.9.0/versioneer.py
```

### Comparing `ccinput-1.8.1/LICENSE` & `ccinput-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/PKG-INFO` & `ccinput-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccinput
-Version: 1.8.1
+Version: 1.9.0
 Summary: Computational Chemistry Input Generator
 Home-page: http://github.com/cyllab/ccinput
 Author: Raphaël Robidas
 Author-email: Raphael.Robidas@USherbrooke.ca
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ccinput-1.8.1/README.md` & `ccinput-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/calculation.py` & `ccinput-1.9.0/ccinput/calculation.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/constants.py` & `ccinput-1.9.0/ccinput/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     CalcType.TS: [
         "TS Optimisation",
         "ts",
         "tsoptimisation",
         "tsoptimization",
         "optts",
         "tsopt",
+        "saddle",
     ],
     CalcType.NMR: [
         "NMR Calculation",
         "nmr",
         "nmrprediction",
         "nmrcalculation",
         "nmrcalc",
@@ -139,15 +140,15 @@
 
 THEORY_LEVELS = {
     "hf": ["hartreefock"],
     # Some old exotic semi-empirical methods in ORCA are missing
     "semiempirical": ["am1", "pm3", "pm6", "pm7", "mndo"],
     "xtb": ["gfn2xtb", "xtb2", "xtb1", "gfn1xtb", "gfn0xtb", "gfnff", "gfn2xtbgfnff"],
     "special": ["hf3c", "pbeh3c", "r2scan3c", "b973c"],
-    "mp2": ["mp2", "rimp2"],
+    "mp2": ["mp2", "rimp2", "direct_mp2"],
     "cc": [
         "ccsd",
         "ccsdt",
         "qcisd",
         "qcisdt",
         "lpnoccsd",
         "lpnoccsdt",
@@ -164,14 +165,15 @@
 # Synonyms for each software package
 SYN_SOFTWARE = {
     "gaussian": ["g16", "gaussian16"],
     "orca": ["orca5"],
     "qchem": [],
     "xtb": [],
     "psi4": ["psi4"],
+    "nwchem": [],
 }
 
 # Synonym for each solvent.
 # The keys are "canonical" and used in other dictionaries to refer to each solvent.
 SYN_SOLVENTS = {
     "acetone": ["acetone"],
     "acetonitrile": ["acetonitrile", "acn", "ch3cn", "mecn"],
@@ -370,15 +372,15 @@
     "vwn3": [],
     "bnull": [],
     "bvwn": [],
     "bp": [],
     "blyp": [],
     "gp": [],
     "glyp": [],
-    "pbe": [],
+    "pbe": ["pbe96"],
     "revpbe": [],
     "rpbe": [],
     "pwp": [],
     "olyp": [],
     "opbe": [],
     "xlyp": [],
     "m05": [],
@@ -429,15 +431,15 @@
     "wb97": [],
     "wb97x": [],
     "wb97xd": [],
     "wb97xd3": [],
     "wb97xv": [],
     "wb97xd3bj": [],
     "b98": [],
-    "tpssh": [],
+    "tpssh": ["xctpssh"],
     "tpss0": [],
     "b2plyp": [],
     "mpw2plyp": [],
     "b2gpplyp": [],
     "b2kplyp": [],
     "b2tplyp": [],
     "pwpb95": [],
@@ -495,50 +497,122 @@
     "dlpnoccsd": [],
     "dlpnoccsdt": [],
     "dlpnoqcisd": [],
     "dlpnoqcisdt": [],
 }
 
 
-# Gaussian allows the combination of exchange and correlation functionals
+# Gaussian and nwchem allow the combination of exchange and correlation functionals
 # without using any special keyword.
 
 EXCHANGE_FUNCTIONALS = {
-    "s": "S",
-    "xa": "XA",
-    "b": "B",
-    "pw91": "PW91",
-    "mpw": "mPW",
-    "g96": "G96",
-    "pbe": "PBE",
-    "o": "O",
-    "tpss": "TPSS",
-    "revtpss": "RevTPSS",
-    "brx": "BRx",
-    "pkzb": "PKZB",
-    "wpbeh": "wPBEh",
-    "pbeh": "PBEh",
+    "gaussian": {
+        "s": "S",
+        "xa": "XA",
+        "b": "B",
+        "pw91": "PW91",
+        "mpw": "mPW",
+        "g96": "G96",
+        "pbe": "PBE",
+        "o": "O",
+        "tpss": "TPSS",
+        "revtpss": "RevTPSS",
+        "brx": "BRx",
+        "pkzb": "PKZB",
+        "wpbeh": "wPBEh",
+        "pbeh": "PBEh",
+    },
+    "nwchem": {
+        "slater": "slater",
+        "becke88": "becke88",
+        "gill96": "gill96",
+        "mpw91": "mpw91",
+        "optx": "optx",
+        "revpbe": "revpbe",
+        "rpbe": "rpbe",
+        "xbecke86b": "xbecke86b",
+        "xft97": "xft97",
+        "xm05": "xm05",
+        "xm052x": "xm05-2x",
+        "xm06": "xm06",
+        "xm062x": "xm06-2x",
+        "xm06hf": "xm06-hf",
+        "xm06L": "xm06-L",
+        "xm08hx": "xm08-hx",
+        "xm08so": "xm08-so",
+        "xm11": "xm11",
+        "xm11l": "xm11-l",
+        "xmvs15": "xmvs15",
+        "xpbe96": "xpbe96",
+        "xperdew86": "xperdew86",
+        "xperdew91": "xperdew91",
+        "xpkzb99": "xpkzb99",
+        "xpw6b95": "xpw6b95",
+        "xpwb6k": "xpwb6k",
+        "xsogga": "xsogga",
+        "xsogga11": "xsogga11",
+        "xsogga11x": "xsogga11-x",
+        "xtpss03": "xtpss03",
+        "xvs98": "xvs98",
+    },
 }
 
 CORRELATION_FUNCTIONALS = {
-    "vwn": "VWN",
-    "vwn5": "VWN5",
-    "lyp": "LYP",
-    "pl": "PL",
-    "p86": "P86",
-    "pw91": "PW91",
-    "b95": "B95",
-    "pbe": "PBE",
-    "tpss": "TPSS",
-    "revtpss": "RevTPSS",
-    "kcis": "KCIS",
-    "brc": "BRC",
-    "pkzb": "PKZB",
-    "vp86": "VP86",
-    "v5lyp": "V5LYP",
+    "gaussian": {
+        "vwn": "VWN",
+        "vwn5": "VWN5",
+        "lyp": "LYP",
+        "pl": "PL",
+        "p86": "P86",
+        "pw91": "PW91",
+        "b95": "B95",
+        "pbe": "PBE",
+        "tpss": "TPSS",
+        "revtpss": "RevTPSS",
+        "kcis": "KCIS",
+        "brc": "BRC",
+        "pkzb": "PKZB",
+        "vp86": "VP86",
+        "v5lyp": "V5LYP",
+    },
+    "nwchem": {
+        "bc95": "bc95",
+        "cft97": "cft97",
+        "cm05": "cm05",
+        "cm052x": "cm05-2x",
+        "cm06": "cm06",
+        "cm062x": "cm06-2x",
+        "cm06hf": "cm06-hf",
+        "cm06L": "cm06-L",
+        "cm08hx": "cm08-hx",
+        "cm08so": "cm08-so",
+        "cm11": "cm11",
+        "cm11l": "cm11-l",
+        "cpbe96": "cpbe96",
+        "cpkzb99": "cpkzb99",
+        "cpw6b95": "cpw6b95",
+        "cpwb6k": "cpwb6k",
+        "csogga": "csogga",
+        "csogga11": "csogga11",
+        "csogga11x": "csogga11-x",
+        "ctpss03": "ctpss03",
+        "cvs98": "cvs98",
+        "lyp": "lyp",
+        "op": "op",
+        "perdew81": "perdew81",
+        "perdew86": "perdew86",
+        "perdew91": "perdew91",
+        "pw91lda": "pw91lda",
+        "vwn_1": "vwn_1",
+        "vwn_1_rpa": "vwn_1_rpa",
+        "vwn_2": "vwn_2",
+        "vwn_3": "vwn_3",
+        "vwn_4": "vwn_4",
+        "vwn_5": "vwn_5",
+    },
 }
 
 SYN_BASIS_SETS = {
     "sto3g": [],
     "mini": [],
     "minis": [],
     "minix": [],
@@ -1620,14 +1694,75 @@
         "blyp": "blyp",
         "b3lyp": "b3lyp",
         "pbe": "pbe",
         "pw91": "pw91",
         "revpbe": "revpbe",
         "rpbe": "rpbe",
     },
+    "nwchem": {  # Values are correct, keys need to be checked! - Zarko
+        "hf": "hf",
+        "rohf": "rohf",
+        "uhf": "uhf",
+        # exchange-correlation functionals
+        "acm": "acm",
+        "b3lyp": "b3lyp",
+        "becke97": "becke97",
+        "becke971": "becke97-1",
+        "becke972": "becke97-2",
+        "becke973": "becke97-3",
+        "becke97d": "becke97-d",
+        "becke97gga1": "becke97gga1",
+        "becke98": "becke98",
+        "beckehandh": "beckehandh",
+        "bop": "bop",
+        "dldf": "dldf",
+        "ft97": "ft97",
+        "hcth": "hcth",
+        "hcth120": "hcth120",
+        "hcth147": "hcth147",
+        "hcth147tz2p": "hcth147@tz2p",
+        "hcth407": "hcth407",
+        "hcthp14": "hcthp14",
+        "hle16": "hle16",
+        "htch407p": "htch407p",
+        "m052x": "m05-2x",
+        "m06L": "m06-L",
+        "m08hx": "m08-hx",
+        "m08so": "m08-so",
+        "m11": "m11",
+        "m11l": "m11-l",
+        "mpw1k": "mpw1k",
+        "pbe0": "pbe0",
+        "pbeop": "pbeop",
+        "r2scan": "r2scan",
+        "r2scan0": "r2scan0",
+        "r2scanl": "r2scanl",
+        "revm06": "revm06",
+        "revm06L": "revm06-L",
+        "rscan": "rscan",
+        "scan": "scan",
+        "scanl": "scanl",
+        "sogga": "sogga",
+        "sogga11": "sogga11",
+        "sogga11x": "sogga11-x",
+        "wb97x": "wb97x",
+        "wb97xd3": "wb97x-d3",
+        "ncap": "ncap",
+        "bb1k": "bb1k",
+        "m05": "m05",
+        "m06": "m06",
+        "m062x": "m06-2x",
+        "m06hf": "m06-hf",
+        "mpw1b95": "mpw1b95",
+        "mpwb1k": "mpwb1k",
+        "pw6b95": "pw6b95",
+        "pwb6k": "pwb6k",
+        "vs98": "vs98",
+        "xctpssh": "xctpssh",
+    },
 }
 
 SOFTWARE_BASIS_SETS = {
     "orca": {
         "sto3g": "STO-3G",
         "mini": "MINI",
         "minis": "MINIS",
@@ -2063,14 +2198,281 @@
     },
     "psi4": {
         "sto3g": "sto-3g",
         "631g": "6-31G",
         "ccpvdz": "cc-pVDZ",
         "def2tzvp": "def2-tzvp",
     },
+    "nwchem": {
+        "321++g": "3-21++G",
+        "321++gd": "3-21++G*",
+        "321g": "3-21G",
+        "321gd": "3-21G*",
+        "321gsp": "3-21GSP",
+        "422gsp": "4-22GSP",
+        "431g": "4-31G",
+        "631++g": "6-31++G",
+        "631++gd": "6-31++G*",
+        "631++gdp": "6-31++G**",
+        "631+gdp": "6-31+G*",
+        "6311++g2d2p": "6-311++G(2d,2p)",
+        "6311++g3df3pd": "6-311++G(3df,3pd)",
+        "6311++gdp": "6-311++G**",
+        "6311+gd": "6-311+G*",
+        "6311g": "6-311G",
+        "6311g2df2pd": "6-311G(2df,2pd)",
+        "6311gd": "6-311G*",
+        "6311gdp": "6-311G**",
+        "631g": "6-31G",
+        "631gblaudeau": "6-31G-Blaudeau",
+        "631g3df3pd": "6-31G(3df,3pd)",
+        "631gd": "6-31G*",
+        "631g*blaudeau": "6-31G*-Blaudeau",
+        "631gdp": "6-31G**",
+        "ahlrichspvdz": '"Ahlrichs pVDZ"',
+        "ahlrichstzv": '"Ahlrichs TZV"',
+        "ahlrichsvdz": '"Ahlrichs VDZ"',
+        "ahlrichsvtz": '"Ahlrichs VTZ"',
+        "anorcc": "ANO-RCC",
+        "aprccpvq+dz": "apr-cc-pV(Q+d)Z",
+        "augccpcv5z": "aug-cc-pCV5Z",
+        "augccpcvdz": "aug-cc-pCVDZ",
+        "augccpcvqz": "aug-cc-pCVQZ",
+        "augccpcvt+dz": "aug-cc-pCV(T+d)Z",
+        "augccpcvtz": "aug-cc-pCVTZ",
+        "augccpv5+dz": "aug-cc-pV(5+d)Z",
+        "augccpv5z": "aug-cc-pV5Z",
+        "augccpv6+dz": "aug-cc-pV(6+d)Z",
+        "augccpv6z": "aug-cc-pV6Z",
+        "augccpvd+dz": "aug-cc-pV(D+d)Z",
+        "augccpvdz": "aug-cc-pVDZ",
+        "augccpvq+dz": "aug-cc-pV(Q+d)Z",
+        "augccpvqz": "aug-cc-pVQZ",
+        "augccpvt+dz": "aug-cc-pV(T+d)Z",
+        "augccpvtz": "aug-cc-pVTZ",
+        "augccpvtzj": "aug-cc-pVTZ-J",
+        "augccpwcv5z": "aug-cc-pwCV5Z",
+        "augccpwcv5znr": "aug-cc-pwCV5Z-NR",
+        "augccpwcvdz": "aug-cc-pwCVDZ",
+        "augccpwcvqz": "aug-cc-pwCVQZ",
+        "augccpwcvqznr": "aug-cc-pwCVQZ-NR",
+        "augccpwcvtz": "aug-cc-pwCVTZ",
+        "augccpwcvtznr": "aug-cc-pwCVTZ-NR",
+        "augmccpv5z": "aug-mcc-pV5Z",
+        "augmccpv6z": "aug-mcc-pV6Z",
+        "augmccpv7z": "aug-mcc-pV7Z",
+        "augmccpv8z": "aug-mcc-pV8Z",
+        "augmccpvqz": "aug-mcc-pVQZ",
+        "augmccpvtz": "aug-mcc-pVTZ",
+        "augpc0": "aug-pc-0",
+        "augpc1": "aug-pc-1",
+        "augpc2": "aug-pc-2",
+        "augpc3": "aug-pc-3",
+        "augpc4": "aug-pc-4",
+        "augpcj0": "aug-pcJ-0",
+        "augpcj0_2006": "aug-pcJ-0_2006",
+        "augpcj1": "aug-pcJ-1",
+        "augpcj1_2006": "aug-pcJ-1_2006",
+        "augpcj2": "aug-pcJ-2",
+        "augpcj2_2006": "aug-pcJ-2_2006",
+        "augpcj3": "aug-pcJ-3",
+        "augpcj3_2006": "aug-pcJ-3_2006",
+        "augpcj4": "aug-pcJ-4",
+        "augpcj4_2006": "aug-pcJ-4_2006",
+        "augpcs0": "aug-pcS-0",
+        "augpcs1": "aug-pcS-1",
+        "augpcs2": "aug-pcS-2",
+        "augpcs3": "aug-pcS-3",
+        "augpcs4": "aug-pcS-4",
+        "augpv7z": "aug-pV7Z",
+        "b2basissetforzn": '"B2 basis set for Zn"',
+        "bauschlicherano": '"Bauschlicher ANO"',
+        "binningcurtisssv": '"Binning/Curtiss SV"',
+        "binningcurtisssvp": '"Binning/Curtiss SVP"',
+        "binningcurtissvtz": '"Binning/Curtiss VTZ"',
+        "binningcurtissvtzp": '"Binning/Curtiss VTZP"',
+        "ccpcv5z": "cc-pCV5Z",
+        "ccpcv6z": "cc-pCV6Z",
+        "ccpcv6zold": "cc-pCV6Z(old)",
+        "ccpcvdz": "cc-pCVDZ",
+        "ccpcvdzold": "cc-pCVDZ(old)",
+        "ccpcvqz": "cc-pCVQZ",
+        "ccpcvqzold": "cc-pCVQZ(old)",
+        "ccpcvtz": "cc-pCVTZ",
+        "ccpcvtzold": "cc-pCVTZ(old)",
+        "ccpv5+dz": "cc-pV(5+d)Z",
+        "ccpv5z": "cc-pV5Z",
+        "ccpv6+dz": "cc-pV(6+d)Z",
+        "ccpv6z": "cc-pV6Z",
+        "ccpv8z": "cc-pV8Z",
+        "ccpv9z": "cc-pV9Z",
+        "ccpvd+dz": "cc-pV(D+d)Z",
+        "ccpvdz": "cc-pVDZ",
+        "ccpvdzsegopt": "cc-pVDZ(seg-opt)",
+        "ccpvq+dz": "cc-pV(Q+d)Z",
+        "ccpvqz": "cc-pVQZ",
+        "ccpvqzsegopt": "cc-pVQZ(seg-opt)",
+        "ccpvt+dz": "cc-pV(T+d)Z",
+        "ccpvtz": "cc-pVTZ",
+        "ccpvtzsegopt": "cc-pVTZ(seg-opt)",
+        "ccpwcv5z": "cc-pwCV5Z",
+        "ccpwcv5zcoreset": '"cc-pwCV5Z Core Set"',
+        "ccpwcv5znr": "cc-pwCV5Z-NR",
+        "ccpwcvdz": "cc-pwCVDZ",
+        "ccpwcvqz": "cc-pwCVQZ",
+        "ccpwcvqznr": "cc-pwCVQZ-NR",
+        "ccpwcvtz": "cc-pwCVTZ",
+        "ccpwcvtznr": "cc-pwCVTZ-NR",
+        "ccemd2": "ccemd-2",
+        "ccemd3": "ccemd-3",
+        "ccjpv5z": "ccJ-pV5Z",
+        "ccjpvdz": "ccJ-pVDZ",
+        "ccjpvqz": "ccJ-pVQZ",
+        "ccjpvtz": "ccJ-pVTZ",
+        "coemd2": "coemd-2",
+        "coemd3": "coemd-3",
+        "coemd4": "coemd-4",
+        "coemdref": "coemd-ref",
+        "cvtz": "CVTZ",
+        "daugccpv5z": "d-aug-cc-pV5Z",
+        "daugccpv6z": "d-aug-cc-pV6Z",
+        "daugccpvdz": "d-aug-cc-pVDZ",
+        "daugccpvqz": "d-aug-cc-pVQZ",
+        "daugccpvtz": "d-aug-cc-pVTZ",
+        "def2qzvp": "Def2-QZVP",
+        "def2qzvpd": "Def2-QZVPD",
+        "def2svp": "Def2-SVP",
+        "def2svpd": "Def2-SVPD",
+        "def2tzvp": "Def2-TZVP",
+        "def2tzvpd": "Def2-TZVPD",
+        "dhfqzvp": "dhf-QZVP",
+        "dhfsvp": "dhf-SV(P)",
+        "dhftzvp": "dhf-TZVP",
+        "dunninghaydoublerydberg": '"Dunning-Hay Double Rydberg"',
+        "dunninghayrydberg": '"Dunning-Hay Rydberg"',
+        "dz+doublerydbergdunninghay": '"DZ + Double Rydberg (Dunning-Hay)"',
+        "dz+rydberg(dunning)": '"DZ + Rydberg (Dunning)"',
+        "dz(dunning)": '"DZ (Dunning)"',
+        "dzp+rydberg(dunning)": '"DZP + Rydberg (Dunning)"',
+        "dzp(dunning)": '"DZP (Dunning)"',
+        "dzq": "DZQ",
+        "dzvp2(dftorbital)": '"DZVP2 (DFT Orbital)"',
+        "dzvp(dftorbital)": '"DZVP (DFT Orbital)"',
+        "fellermisc.cvdz": '"Feller Misc. CVDZ"',
+        "fellermisc.cvqz": '"Feller Misc. CVQZ"',
+        "fellermisc.cvtz": '"Feller Misc. CVTZ"',
+        "gamesspvtz": '"GAMESS PVTZ"',
+        "gamessvtz": '"GAMESS VTZ"',
+        "igloii": "IGLO-II",
+        "igloiii": "IGLO-III",
+        "julccpvd+dz": "jul-cc-pV(D+d)Z",
+        "julccpvq+dz": "jul-cc-pV(Q+d)Z",
+        "julccpvt+dz": "jul-cc-pV(T+d)Z",
+        "junccpvd+dz": "jun-cc-pV(D+d)Z",
+        "junccpvq+dz": "jun-cc-pV(Q+d)Z",
+        "junccpvt+dz": "jun-cc-pV(T+d)Z",
+        "lanl08": "LANL08",
+        "lanl08+": "LANL08+",
+        "lanl08d": "LANL08d",
+        "lanl08(f)": "LANL08(f)",
+        "lanl2[10s8p7d3f2g]": "Lanl2-[10s8p7d3f2g]",
+        "lanl2[5s4p4d2f]": "Lanl2-[5s4p4d2f]",
+        "lanl2[6s4p4d2f]": "Lanl2-[6s4p4d2f]",
+        "lanl2dz+1d1f": "Lanl2DZ+1d1f",
+        "lanl2dz+2s2p2d2f": "Lanl2DZ+2s2p2d2f",
+        "lanl2tz": "LANL2TZ",
+        "lanl2tz+": "LANL2TZ+",
+        "lanl2tz(f)": "LANL2TZ(f)",
+        "m631g": "m6-31G",
+        "m631gd": "m6-31G*",
+        "maugccpvd+dz": "maug-cc-pV(D+d)Z",
+        "maugccpvdz": "maug-cc-pVDZ",
+        "maugccpvq+dz": "maug-cc-pV(Q+d)Z",
+        "maugccpvqz": "maug-cc-pVQZ",
+        "maugccpvt+dz": "maug-cc-pV(T+d)Z",
+        "maugccpvtz": "maug-cc-pVTZ",
+        "mayccpvq+dz": "may-cc-pV(Q+d)Z",
+        "mayccpvt+dz": "may-cc-pV(T+d)Z",
+        "mcleanchandlervtz": '"McLean/Chandler VTZ"',
+        "mg3s": "MG3S",
+        "midi!": "MIDI!",
+        "midi(huzinaga)": '"MIDI (Huzinaga)"',
+        "mini(huzinaga)": '"MINI (Huzinaga)"',
+        "mini(scaled)": '"MINI (Scaled)"',
+        "modifiedlanl2dz": '"modified LANL2DZ"',
+        "nasaamesano": '"NASA Ames ANO"',
+        "nasaamesano2": '"NASA Ames ANO2"',
+        "nasaamesccpcv5z": '"NASA Ames cc-pCV5Z"',
+        "nasaamesccpcvqz": '"NASA Ames cc-pCVQZ"',
+        "nasaamesccpcvtz": '"NASA Ames cc-pCVTZ"',
+        "nasaamesccpv5z": '"NASA Ames cc-pV5Z"',
+        "nasaamesccpvqz": '"NASA Ames cc-pVQZ"',
+        "nasaamesccpvtz": '"NASA Ames cc-pVTZ"',
+        "partridgeuncontracted1": '"Partridge Uncontracted 1"',
+        "partridgeuncontracted2": '"Partridge Uncontracted 2"',
+        "partridgeuncontracted3": '"Partridge Uncontracted 3"',
+        "partridgeuncontracted4": '"Partridge Uncontracted 4"',
+        "pc0": "pc-0",
+        "pc1": "pc-1",
+        "pc2": "pc-2",
+        "pc3": "pc-3",
+        "pc4": "pc-4",
+        "pcemd2": "pcemd-2",
+        "pcemd3": "pcemd-3",
+        "pcemd4": "pcemd-4",
+        "pcj0": "pcJ-0",
+        "pcj0_2006": "pcJ-0_2006",
+        "pcj1": "pcJ-1",
+        "pcj1_2006": "pcJ-1_2006",
+        "pcj2": "pcJ-2",
+        "pcj2_2006": "pcJ-2_2006",
+        "pcj3": "pcJ-3",
+        "pcj3_2006": "pcJ-3_2006",
+        "pcj4": "pcJ-4",
+        "pcj4_2006": "pcJ-4_2006",
+        "pcs0": "pcS-0",
+        "pcs1": "pcS-1",
+        "pcs2": "pcS-2",
+        "pcs3": "pcS-3",
+        "pcs4": "pcS-4",
+        "psbkjc": "pSBKJC",
+        "ptmdzp": '"Pt - mDZP"',
+        "pv6z": "pV6Z",
+        "pv7z": "pV7Z",
+        "roos_ano_dz": "Roos_ANO_DZ",
+        "roos_ano_tz": "Roos_ANO_TZ",
+        "roosaugmenteddoublezetaano": '"Roos Augmented Double Zeta ANO"',
+        "roosaugmentedtriplezetaano": '"Roos Augmented Triple Zeta ANO"',
+        "s321g": "s3-21G",
+        "s321gd": "s3-21G*",
+        "s631g": "s6-31G",
+        "s631gd": "s6-31G*",
+        "sadlejpvtz": '"Sadlej pVTZ"',
+        "sdbaugccpvqz": "SDB-aug-cc-pVQZ",
+        "sdbaugccpvtz": "SDB-aug-cc-pVTZ",
+        "sdbccpvqz": "SDB-cc-pVQZ",
+        "sdbccpvtz": "SDB-cc-pVTZ",
+        "sto2g": "STO-2G",
+        "sto3g": "STO-3G",
+        "sto3gd": "STO-3G*",
+        "sto6g": "STO-6G",
+        "sv+doublerydbergdunninghay": '"SV + Double Rydberg (Dunning-Hay)"',
+        "sv+rydbergdunninghay": '"SV + Rydberg (Dunning-Hay)"',
+        "svdunninghay": '"SV (Dunning-Hay)"',
+        "svp+rydbergdunninghay": '"SVP + Rydberg (Dunning-Hay)"',
+        "svpdunninghay": '"SVP (Dunning-Hay)"',
+        "tz(dunning)": '"TZ (Dunning)"',
+        "tzvp(dftorbital)": '"TZVP (DFT Orbital)"',
+        "ugbs": "UGBS",
+        "unccemdref": "un-ccemd-ref",
+        "unpcemdref": "un-pcemd-ref",
+        "wachters+f": "Wachters+f",
+        "wtbs": "WTBS",
+        "z3pol": "Z3Pol",
+    },
 }
 
 SOFTWARE_SOLVENTS = {
     "gaussian": {
         "water": "water",
         "acetonitrile": "acetonitrile",
         "methanol": "methanol",
@@ -2479,15 +2881,15 @@
     "d3": [
         "b1b95",
         "b2gp-plyp",
         "b3lyp",
         "b97-d",
         "bhlyp",  # BHandHLYP?
         "blyp",
-        "bp86",  # ?
+        "bp86",  # ? yes in nwchem
         "bpbe",  # HISSbPBE?
         "mpwlyp",
         "pbe",
         "pbe0",
         "pw6b95",
         "pwb6k",  # ?
         "revpbe",
@@ -2561,7 +2963,19 @@
         "revpbe38",  # ?
         "revpbe",
         "rpw86pbe",
         "tpss0",
         "tpss",
     ],
 }
+SOFTWARE_MULTIPLICITY = {
+    "nwchem": {
+        1: "singlet",
+        2: "doublet",
+        3: "triplet",
+        4: "quartet",
+        5: "quintet",
+        6: "sextet",
+        7: "septet",
+        8: "octet",
+    }
+}
```

### Comparing `ccinput-1.8.1/ccinput/documentation.py` & `ccinput-1.9.0/ccinput/documentation.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/drivers/pysis.py` & `ccinput-1.9.0/ccinput/drivers/pysis.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/packages/gaussian.py` & `ccinput-1.9.0/ccinput/packages/gaussian.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/packages/orca.py` & `ccinput-1.9.0/ccinput/packages/orca.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/packages/psi4.py` & `ccinput-1.9.0/ccinput/packages/psi4.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/packages/qchem.py` & `ccinput-1.9.0/ccinput/packages/qchem.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/packages/xtb.py` & `ccinput-1.9.0/ccinput/packages/xtb.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/presets.py` & `ccinput-1.9.0/ccinput/presets.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/tests/test_calculation.py` & `ccinput-1.9.0/ccinput/tests/test_calculation.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/tests/test_cli.py` & `ccinput-1.9.0/ccinput/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/tests/test_gaussian.py` & `ccinput-1.9.0/ccinput/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/tests/test_orca.py` & `ccinput-1.9.0/ccinput/tests/test_orca.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/tests/test_psi4.py` & `ccinput-1.9.0/ccinput/tests/test_psi4.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/tests/test_pysis.py` & `ccinput-1.9.0/ccinput/tests/test_pysis.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/tests/test_qchem.py` & `ccinput-1.9.0/ccinput/tests/test_qchem.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/tests/test_structures.py` & `ccinput-1.9.0/ccinput/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/tests/test_xtb.py` & `ccinput-1.9.0/ccinput/tests/test_xtb.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/tests/testing_utilities.py` & `ccinput-1.9.0/ccinput/tests/testing_utilities.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/utilities.py` & `ccinput-1.9.0/ccinput/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,51 +238,67 @@
     if trust_me:
         warn(f"Using unknown solvent '{solvent}'")
         return solvent
     else:
         raise InvalidParameter(f"Unknown solvent: '{solvent}'")
 
 
-def is_exchange_correlation_combination(method):
-    for x in EXCHANGE_FUNCTIONALS:
+def is_exchange_correlation_combination(method, software):
+    fill = ""
+    if software == "nwchem":
+        fill = " "
+    for x in EXCHANGE_FUNCTIONALS[software]:
         if method[: len(x)] == x:
-            if method[len(x) :] in CORRELATION_FUNCTIONALS:
+            if method[len(x) :] in CORRELATION_FUNCTIONALS[software]:
                 return (
-                    EXCHANGE_FUNCTIONALS[method[: len(x)]]
-                    + CORRELATION_FUNCTIONALS[method[len(x) :]]
+                    EXCHANGE_FUNCTIONALS[software][method[: len(x)]]
+                    + fill
+                    + CORRELATION_FUNCTIONALS[software][method[len(x) :]]
                 )
     return False
 
 
 def get_method(method, software):
     try:
         abs_method = get_abs_method(method)
     except InvalidParameter:
         if software == "gaussian":
-            # As far as I know, this kind of specification does not apply to ORCA
+            # As far as I know, this kind of specification does not apply to ORCA *** But it does to nwchem - Zarko***
             if method.lower()[0] in ["u", "r"]:
                 try:
                     abs_method = get_abs_method(method[1:])
                 except InvalidParameter:
                     pass
                 else:
                     if abs_method in SOFTWARE_METHODS[software]:
                         return (
                             method[0].upper() + SOFTWARE_METHODS[software][abs_method]
                         )
 
-                xc_check = is_exchange_correlation_combination(method.lower()[1:])
+                xc_check = is_exchange_correlation_combination(
+                    method.lower()[1:], software
+                )
                 if isinstance(xc_check, str):
                     return method[0].upper() + xc_check
 
-            xc_check = is_exchange_correlation_combination(method.lower())
+            xc_check = is_exchange_correlation_combination(method.lower(), software)
             if isinstance(xc_check, str):
                 return xc_check
-        warn(f"Unknown method '{method}'")
+            warn(f"Unknown method '{method}'")
+        if software == "nwchem":
+            # nwchem also supports combination of functionals
+            if len(method.split()) == 2:
+                xc_check = is_exchange_correlation_combination(
+                    indexify(method), "nwchem"
+                )
+                if isinstance(xc_check, str):
+                    return xc_check
+            warn(f"Unknown method '{method}'")
         return method
+
     else:
         if abs_method not in SOFTWARE_METHODS[software]:
             warn(f"Unknown method for this package: '{method}'")
             return method
 
         return SOFTWARE_METHODS[software][abs_method]
 
@@ -318,17 +334,15 @@
     return SOFTWARE_SOLVENTS[software][abs_solvent]
 
 
 def has_dispersion_parameters(method, version="d3"):
     try:
         _method = get_abs_method(method)
     except InvalidParameter:
-        warn(
-            "Unknown method, could not verify if dispersion parameters are available for it"
-        )
+        warn("Could not verify if dispersion parameters are available for this method")
         return True  # Don't print a second warning
 
     if _method in FUNCTIONALS_WITH_DISPERSION_PARAMETERS[version]:
         return True
     return False
```

### Comparing `ccinput-1.8.1/ccinput/verify_sanity.py` & `ccinput-1.9.0/ccinput/verify_sanity.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput/wrapper.py` & `ccinput-1.9.0/ccinput/wrapper.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/ccinput.egg-info/PKG-INFO` & `ccinput-1.9.0/ccinput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccinput
-Version: 1.8.1
+Version: 1.9.0
 Summary: Computational Chemistry Input Generator
 Home-page: http://github.com/cyllab/ccinput
 Author: Raphaël Robidas
 Author-email: Raphael.Robidas@USherbrooke.ca
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ccinput-1.8.1/ccinput.egg-info/SOURCES.txt` & `ccinput-1.9.0/ccinput.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/setup.py` & `ccinput-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.1/versioneer.py` & `ccinput-1.9.0/versioneer.py`

 * *Files identical despite different names*

