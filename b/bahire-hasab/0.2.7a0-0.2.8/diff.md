# Comparing `tmp/bahire-hasab-0.2.7a0.tar.gz` & `tmp/bahire-hasab-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bahire-hasab-0.2.7a0.tar", last modified: Wed Jun  7 07:52:17 2023, max compression
+gzip compressed data, was "bahire-hasab-0.2.8.tar", last modified: Wed Jun  7 08:50:19 2023, max compression
```

## Comparing `bahire-hasab-0.2.7a0.tar` & `bahire-hasab-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:52:17.038201 bahire-hasab-0.2.7a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 07:52:01.000000 bahire-hasab-0.2.7a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-07 07:52:17.034201 bahire-hasab-0.2.7a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-07 07:52:01.000000 bahire-hasab-0.2.7a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 07:52:01.000000 bahire-hasab-0.2.7a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 07:52:17.038201 bahire-hasab-0.2.7a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-07 07:52:01.000000 bahire-hasab-0.2.7a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:52:17.034201 bahire-hasab-0.2.7a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:52:17.034201 bahire-hasab-0.2.7a0/src/bahire_hasab/
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-06-07 07:52:01.000000 bahire-hasab-0.2.7a0/src/bahire_hasab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-07 07:52:01.000000 bahire-hasab-0.2.7a0/src/bahire_hasab/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:52:17.034201 bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-07 07:52:17.000000 bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-07 07:52:17.000000 bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:52:17.000000 bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 07:52:17.000000 bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 07:52:17.000000 bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:50:19.388286 bahire-hasab-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 08:50:08.000000 bahire-hasab-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-07 08:50:19.388286 bahire-hasab-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-07 08:50:08.000000 bahire-hasab-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 08:50:08.000000 bahire-hasab-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 08:50:19.388286 bahire-hasab-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-07 08:50:08.000000 bahire-hasab-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:50:19.388286 bahire-hasab-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:50:19.388286 bahire-hasab-0.2.8/src/bahire_hasab/
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-07 08:50:08.000000 bahire-hasab-0.2.8/src/bahire_hasab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-07 08:50:08.000000 bahire-hasab-0.2.8/src/bahire_hasab/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:50:19.388286 bahire-hasab-0.2.8/src/bahire_hasab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-07 08:50:19.000000 bahire-hasab-0.2.8/src/bahire_hasab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-07 08:50:19.000000 bahire-hasab-0.2.8/src/bahire_hasab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:50:19.000000 bahire-hasab-0.2.8/src/bahire_hasab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 08:50:19.000000 bahire-hasab-0.2.8/src/bahire_hasab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 08:50:19.000000 bahire-hasab-0.2.8/src/bahire_hasab.egg-info/top_level.txt
```

### Comparing `bahire-hasab-0.2.7a0/LICENSE` & `bahire-hasab-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.7a0/PKG-INFO` & `bahire-hasab-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.2.7a0
+Version: 0.2.8
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
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.7a0 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.8 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
 workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
 hasab/actions/workflows/python-publish.yml) - A python module for calculating
```

### Comparing `bahire-hasab-0.2.7a0/README.md` & `bahire-hasab-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.7a0/setup.py` & `bahire-hasab-0.2.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open("./README.md", "r") as file:
     long_description = file.read()
 setup(
     name="bahire-hasab",
     author="Hundera Awoke",
-    version="0.2.7a",
+    version="0.2.8",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="hunderaweke@gmail.com",
     url="https://github.com/hunderaweke/bahire-hasab",
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=[],
     keywords="bahire_hasab",
-    entry_points ={
-        'console_scripts':[
+    entry_points={
+        "console_scripts": [
             "bahire-hasab=bahire_hasab.__main__:main",
         ]
-    }
+    },
 )
```

### Comparing `bahire-hasab-0.2.7a0/src/bahire_hasab/__init__.py` & `bahire-hasab-0.2.8/src/bahire_hasab/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*-coding:utf8;-*-
 # created by Hundera Awoke
 # May 28, 2023
 
 import logging
 from functools import cached_property
 
+
 class BahireHasab:
     """Object for  finding the Holidays and lents in the Ethiopian Calendar
     Written by: Hundera Awoke
     Year : 2023 G.C.
     Copyright(c) 2023
     """
+
     TINTE_METIK = 49 % 30
     TINTE_ABEKTE = 161 % 30
     WERAT = [
         "መስከረም",
         "ጥቅምት",
         "ኅዳር",
         "ታኅሣስ",
@@ -43,76 +45,63 @@
         "ዕርገት",
         "በዓለ ሀምሳ",
         "ጾመ ሐዋርያት",
         "ጾመ ድኅነት",
     ]
 
     ELETE_KEN = ["ረቡዕ", "ሐሙስ", "አርብ", "ቅዳሜ", "እሑድ", "ሰኞ", "ማክሰኞ"]
+
     def __init__(self, year, logger=None):
         self.year = year if year else 2016
         self.logger = logger or logging.getLogger(__name__)
         self.logger.debug(f"Initializing Bahre Hasab: Year: {year}")
-        self.already_logged =False
-        
-    
+
     @property
     def wengelawi(self) -> str:
         """A function for findin the Wengelawi."""
         self.logger.debug(f"Calculating wengelawi for year: {self.year}")
         _ = self.WENGELAWI[(self.year + 5500) % 4]
         self.logger.debug(f"Wengelawi of {self.year} is {_}")
         return _
 
     @cached_property
     def medeb(self) -> int:
         """A function for finding medeb used in other calculations."""
         _medeb = (self.year + 5500) % 19
-        already_logged = None
-        if already_logged==None:
-            already_logged = self.already_logged
-        if not already_logged:
-            self.logger.debug(f"Medeb Value returned: {_medeb}")
-            already_logged=True
+        self.logger.debug(f"Medeb Value returned: {_medeb}")
         return _medeb
 
     @cached_property
     def wenber(self) -> int:
         """A function for finding Wenber of the year."""
-        _wenber = self.medeb -1
-        already_logged = self.already_logged
-        if not already_logged:
-            self.logger.debug(f"Wenber Returned {_wenber}")
-            already_logged = True
+        _wenber = self.medeb - 1
+        self.logger.debug(f"Wenber Returned {_wenber}")
         return _wenber if self.medeb else 18
 
     @cached_property
     def abekte(self) -> int:
         """A function for finding the abekte used for other calculations."""
         _abekte = self.wenber * self.TINTE_ABEKTE
         if _abekte > 30:
             _abekte %= 30
         self.logger.debug(f"Returned Abekte: {_abekte}")
         return _abekte if _abekte else 30
 
-    @property
+    @cached_property
     def metene_rabiet(self) -> int:
         """A function for finding metene rabiet"""
         _m = (self.year + 5500) // 4
         self.logger.debug(f"Calculated metene rabiet :{_m}")
         return _m
 
     @cached_property
     def metk(self) -> int:
         """A function for determinig metk used in other calculations."""
         _m = self.wenber * self.TINTE_METIK
-        already_logged = self.already_logged
-        if not already_logged:
-            self.logger.debug(f"Calulated metk: {_m}")
-            already_logged = True
-        self.already_logged = False
+        self.logger.debug(f"Calulated metk: {_m}")
         return _m % 30 if _m else 30
 
     @property
     def beale_metk(self) -> str:
         """A function for finding the date of beale metk used for other calculations."""
         metk = self.metk
         # self.logger.debug(f"Getting the metk: {metk}")
@@ -121,57 +110,58 @@
             beale_metk = f"መስከረም {self.metk}"
         elif 2 <= metk <= 14:
             beale_metk = f"ጥቅምት {self.metk}"
         # if not already_logged:
         #     self.logger.debug(f"Returned beale metk: {beale_metk}")
         #     already_logged = True
         return beale_metk
+
     def elete_ken(self, elet) -> str:
         """A function for determinig the day name of the given date in Ethiopian Calendar. Input in mm/dd format"""
         elet = [i for i in elet.split()]
         atsfe_wer = (self.WERAT.index(elet[0]) + 1) * 2
         tnete_yon = (self.metene_rabiet + self.year + 5500) % 7 - 1
-        already_logged = self.already_logged
-        if not already_logged:
-            self.logger.debug(f"Getting elet :{elet}")
-            self.logger.debug(f"Getting atsfewer: {atsfe_wer}")
-            self.logger.debug(f"Getting tnteyon: {tnete_yon}")
-            already_logged = True
+        self.logger.debug(f"Getting elet :{elet}")
+        self.logger.debug(f"Getting atsfewer: {atsfe_wer}")
+        self.logger.debug(f"Getting tnteyon: {tnete_yon}")
         ken = int(elet[-1])
         _ = (ken + tnete_yon + atsfe_wer) % 7
         self.logger.debug(f"Returning elete_ken: {_}")
         return self.ELETAT[_]
 
-    @property
+    @cached_property
     def new_year(self):
         """A function for determining the day of the Ethiopian New year not the date but its name."""
         amete_alem = self.year + 5500
         _ = (amete_alem + self.metene_rabiet + 2) % 7
+        self.logger.debug(f"Returned new_year: {_}")
         return self.ELETAT[_]
 
     @property
     def mebaja_hamer(self):
         """A function for finding mebaja hamer important for other calculations."""
         _mh = self.metk + self.ELET_TEWSAK.get(self.elete_ken(self.beale_metk))
+        self.logger.debug(f"Returned Mebaja Hamer: {_mh}")
         return _mh
 
-    @property
+    @cached_property
     def neneweh(self) -> str:
         """A function for finding the date of Nenewh Lent."""
         _l = [i for i in self.beale_metk.split()]
         _mh = self.mebaja_hamer
         if _mh > 30:
             _w = "የካቲት"
             _mh %= 30
         elif self.metk == 30 or self.metk == 0:
             _w = "የካቲት"
         elif _l[0] == "መስከረም":
             _w = "ጥር"
         else:
             _w = "የካቲት"
+        self.logger.debug(f"Returned neneweh: {_w} {_mh}")
         return f"{_w} {_mh}"
 
     def atswamat_webealat(self, beal) -> str:
         """A function for finding the respective events or Bealat in Ethiopian Calendar."""
         self.logger.debug(f"Calculating the date of : {beal}")
         _bt = self.BEALAT_TEWSAK[self.BEALAT.index(beal)]
         if _bt == 0:
```

### Comparing `bahire-hasab-0.2.7a0/src/bahire_hasab/__main__.py` & `bahire-hasab-0.2.8/src/bahire_hasab/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python3
 
-from tabulate import tabulate
-import datetime
 import argparse
-from bahire_hasab import BahireHasab
-import logging 
+import datetime
+import logging
 
+from tabulate import tabulate
+
+from bahire_hasab import BahireHasab
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Prints the dates of lents and holidays in a year for Ethiopian Calendar.",
         formatter_class=argparse.MetavarTypeHelpFormatter,
+        # add_help=False,
     )
     parser.add_argument(
         "Year",
         default=None,
         type=int,
         help="Assings the year for the table",
         nargs="?",
@@ -89,35 +91,37 @@
     parser.add_argument(
         "-td",
         "--tsome-dhnet",
         help="Prints the day of Tsome Dhnet in Ethiopia Calendar.",
         action="store_true",
     )
     parser.add_argument(
-        '-l',
-        '--log-level',
+        "-l",
+        "--log-level",
         help="Loglever setter for the cli.",
-        choices=['debug', 'info', 'warning', 'error', 'critical'],
-        default='info',
+        choices=["debug", "info", "warning", "error", "critical"],
+        default="info",
+        type=str.lower,
     )
     args: argparse.Namespace = parser.parse_args()
 
     log_level = args.log_level.upper()
-    
-    logging.basicConfig(format='%(asctime)s | %(funcName)s | %(message)s ', datefmt='%d-%b-%y %H:%M:%S', level=log_level)
+
+    logging.basicConfig(
+        format="%(asctime)s | %(funcName)s | %(message)s ",
+        datefmt="%d-%b-%y %H:%M:%S",
+        level=log_level if log_level else "INFO",
+    )
 
     logger = logging.getLogger(__name__)
     # --------------------------------------------
     if args.Year == None:
         year = BahireHasab(datetime.datetime.now().year - 8)
     else:
-        try:
-            year = BahireHasab(args.Year, logger=logger)
-        except:
-            logging.exception(f"{args.Year} caused an Error please try again by using integer.")
+        year = BahireHasab(args.Year, logger=logger)
     arguments = [
         "new_year",
         "tsome_neneweh",
         "abiy_tsome",
         "debre_zeyt",
         "hosaena",
         "siklet",
@@ -170,16 +174,15 @@
         year.beale_hamsa,
         year.tsome_hawaryat,
         year.tsome_dhnet,
     ]
     table = zip(name, value)
     # --------------------------------------------
     if args.all:
-        print(tabulate(table, headers=heading,tablefmt="simple_grid"));
- 
-    for a, m in zip(arguments, methods):
-        if getattr(args, a):
-            print(getattr(year, m))
+        print(tabulate(table, headers=heading, tablefmt="simple_grid"))
+    for _a, _m in zip(arguments, methods):
+        if getattr(args, _a):
+            print(getattr(year, _m))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bahire-hasab-0.2.7a0/src/bahire_hasab.egg-info/PKG-INFO` & `bahire-hasab-0.2.8/src/bahire_hasab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.2.7a0
+Version: 0.2.8
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
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.7a0 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.8 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
 workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
 hasab/actions/workflows/python-publish.yml) - A python module for calculating
```

