# Comparing `tmp/bahire-hasab-0.2.6.tar.gz` & `tmp/bahire-hasab-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bahire-hasab-0.2.6.tar", last modified: Wed May 31 19:00:12 2023, max compression
+gzip compressed data, was "bahire-hasab-0.2.7.tar", last modified: Wed Jun  7 07:45:21 2023, max compression
```

## Comparing `bahire-hasab-0.2.6.tar` & `bahire-hasab-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:00:12.504729 bahire-hasab-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 18:59:59.000000 bahire-hasab-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-31 19:00:12.504729 bahire-hasab-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-31 18:59:59.000000 bahire-hasab-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-31 18:59:59.000000 bahire-hasab-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:00:12.504729 bahire-hasab-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-31 18:59:59.000000 bahire-hasab-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:00:12.500728 bahire-hasab-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:00:12.504729 bahire-hasab-0.2.6/src/bahire_hasab/
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-31 18:59:59.000000 bahire-hasab-0.2.6/src/bahire_hasab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:00:12.504729 bahire-hasab-0.2.6/src/bahire_hasab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-31 19:00:12.000000 bahire-hasab-0.2.6/src/bahire_hasab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-31 19:00:12.000000 bahire-hasab-0.2.6/src/bahire_hasab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:00:12.000000 bahire-hasab-0.2.6/src/bahire_hasab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 19:00:12.000000 bahire-hasab-0.2.6/src/bahire_hasab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:21.651998 bahire-hasab-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 07:45:10.000000 bahire-hasab-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-07 07:45:21.651998 bahire-hasab-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-07 07:45:10.000000 bahire-hasab-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 07:45:10.000000 bahire-hasab-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 07:45:21.651998 bahire-hasab-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-07 07:45:10.000000 bahire-hasab-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:21.647998 bahire-hasab-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:21.651998 bahire-hasab-0.2.7/src/bahire_hasab/
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-06-07 07:45:10.000000 bahire-hasab-0.2.7/src/bahire_hasab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-06-07 07:45:10.000000 bahire-hasab-0.2.7/src/bahire_hasab/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:45:21.651998 bahire-hasab-0.2.7/src/bahire_hasab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-07 07:45:21.000000 bahire-hasab-0.2.7/src/bahire_hasab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-07 07:45:21.000000 bahire-hasab-0.2.7/src/bahire_hasab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:45:21.000000 bahire-hasab-0.2.7/src/bahire_hasab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 07:45:21.000000 bahire-hasab-0.2.7/src/bahire_hasab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 07:45:21.000000 bahire-hasab-0.2.7/src/bahire_hasab.egg-info/top_level.txt
```

### Comparing `bahire-hasab-0.2.6/LICENSE` & `bahire-hasab-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.6/PKG-INFO` & `bahire-hasab-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.2.6
+Version: 0.2.7
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.6 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.7 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
 workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
 hasab/actions/workflows/python-publish.yml) - A python module for calculating
```

### Comparing `bahire-hasab-0.2.6/README.md` & `bahire-hasab-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.6/src/bahire_hasab/__init__.py` & `bahire-hasab-0.2.7/src/bahire_hasab/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # -*-coding:utf8;-*-
 # created by Hundera Awoke
 # May 28, 2023
+
+import logging
+from functools import cached_property
+
 class BahireHasab:
     """Object for  finding the Holidays and lents in the Ethiopian Calendar
     Written by: Hundera Awoke
     Year : 2023 G.C.
     Copyright(c) 2023
     """
-
     TINTE_METIK = 49 % 30
     TINTE_ABEKTE = 161 % 30
     WERAT = [
         "መስከረም",
         "ጥቅምት",
         "ኅዳር",
         "ታኅሣስ",
@@ -40,73 +43,106 @@
         "ዕርገት",
         "በዓለ ሀምሳ",
         "ጾመ ሐዋርያት",
         "ጾመ ድኅነት",
     ]
 
     ELETE_KEN = ["ረቡዕ", "ሐሙስ", "አርብ", "ቅዳሜ", "እሑድ", "ሰኞ", "ማክሰኞ"]
-
-    def __init__(self, year):
+    def __init__(self, year, logger=None):
         self.year = year if year else 2016
-
+        self.logger = logger or logging.getLogger(__name__)
+        self.logger.debug(f"Initializing Bahre Hasab: Year: {year}")
+        self.already_logged =False
+        
+    
     @property
     def wengelawi(self) -> str:
         """A function for findin the Wengelawi."""
+        self.logger.debug(f"Calculating wengelawi for year: {self.year}")
         _ = self.WENGELAWI[(self.year + 5500) % 4]
+        self.logger.debug(f"Wengelawi of {self.year} is {_}")
         return _
 
-    @property
+    @cached_property
     def medeb(self) -> int:
         """A function for finding medeb used in other calculations."""
-        medeb = (self.year + 5500) % 19
-        return medeb
+        _medeb = (self.year + 5500) % 19
+        already_logged = None
+        if already_logged==None:
+            already_logged = self.already_logged
+        if not already_logged:
+            self.logger.debug(f"Medeb Value returned: {_medeb}")
+            already_logged=True
+        return _medeb
 
-    @property
+    @cached_property
     def wenber(self) -> int:
         """A function for finding Wenber of the year."""
-        wenber = self.medeb - 1
-        return wenber if self.medeb else 18
+        _wenber = self.medeb -1
+        already_logged = self.already_logged
+        if not already_logged:
+            self.logger.debug(f"Wenber Returned {_wenber}")
+            already_logged = True
+        return _wenber if self.medeb else 18
 
-    @property
+    @cached_property
     def abekte(self) -> int:
         """A function for finding the abekte used for other calculations."""
-        abekte = self.wenber * self.TINTE_ABEKTE
-        if abekte > 30:
-            abekte %= 30
-        return abekte if abekte else 30
+        _abekte = self.wenber * self.TINTE_ABEKTE
+        if _abekte > 30:
+            _abekte %= 30
+        self.logger.debug(f"Returned Abekte: {_abekte}")
+        return _abekte if _abekte else 30
 
     @property
     def metene_rabiet(self) -> int:
         """A function for finding metene rabiet"""
         _m = (self.year + 5500) // 4
+        self.logger.debug(f"Calculated metene rabiet :{_m}")
         return _m
 
-    @property
+    @cached_property
     def metk(self) -> int:
         """A function for determinig metk used in other calculations."""
         _m = self.wenber * self.TINTE_METIK
+        already_logged = self.already_logged
+        if not already_logged:
+            self.logger.debug(f"Calulated metk: {_m}")
+            already_logged = True
+        self.already_logged = False
         return _m % 30 if _m else 30
 
     @property
     def beale_metk(self) -> str:
         """A function for finding the date of beale metk used for other calculations."""
         metk = self.metk
+        # self.logger.debug(f"Getting the metk: {metk}")
+        # already_logged = self.already_logged
         if 15 <= metk <= 30:
             beale_metk = f"መስከረም {self.metk}"
         elif 2 <= metk <= 14:
             beale_metk = f"ጥቅምት {self.metk}"
+        # if not already_logged:
+        #     self.logger.debug(f"Returned beale metk: {beale_metk}")
+        #     already_logged = True
         return beale_metk
-
     def elete_ken(self, elet) -> str:
         """A function for determinig the day name of the given date in Ethiopian Calendar. Input in mm/dd format"""
         elet = [i for i in elet.split()]
         atsfe_wer = (self.WERAT.index(elet[0]) + 1) * 2
         tnete_yon = (self.metene_rabiet + self.year + 5500) % 7 - 1
+        already_logged = self.already_logged
+        if not already_logged:
+            self.logger.debug(f"Getting elet :{elet}")
+            self.logger.debug(f"Getting atsfewer: {atsfe_wer}")
+            self.logger.debug(f"Getting tnteyon: {tnete_yon}")
+            already_logged = True
         ken = int(elet[-1])
         _ = (ken + tnete_yon + atsfe_wer) % 7
+        self.logger.debug(f"Returning elete_ken: {_}")
         return self.ELETAT[_]
 
     @property
     def new_year(self):
         """A function for determining the day of the Ethiopian New year not the date but its name."""
         amete_alem = self.year + 5500
         _ = (amete_alem + self.metene_rabiet + 2) % 7
@@ -132,25 +168,27 @@
             _w = "ጥር"
         else:
             _w = "የካቲት"
         return f"{_w} {_mh}"
 
     def atswamat_webealat(self, beal) -> str:
         """A function for finding the respective events or Bealat in Ethiopian Calendar."""
+        self.logger.debug(f"Calculating the date of : {beal}")
         _bt = self.BEALAT_TEWSAK[self.BEALAT.index(beal)]
         if _bt == 0:
             return self.neneweh
         _nw, _nk = [_ for _ in self.neneweh.split()]
         _nk = int(_nk)
         _bk = _nk + _bt
         if _bk % 30 == 0:
             _bw = self.WERAT[self.WERAT.index(_nw) + (_bk // 30) - 1]
         else:
             _bw = self.WERAT[self.WERAT.index(_nw) + (_bk // 30)]
         _bk = _bk % 30 if _bk % 30 else 30
+        self.logger.debug(f"Returned: {_bw} {_bk}")
         return f"{_bw} {_bk}"
 
     @property
     def abiy_tsom(self):
         """A Function for finding the day of enterance of the Great lent according to the Ethiopian Calendar."""
         return self.atswamat_webealat(beal=self.BEALAT[1])
```

### Comparing `bahire-hasab-0.2.6/src/bahire_hasab.egg-info/PKG-INFO` & `bahire-hasab-0.2.7/src/bahire_hasab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.2.6
+Version: 0.2.7
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.6 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.7 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
 workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
 hasab/actions/workflows/python-publish.yml) - A python module for calculating
```

