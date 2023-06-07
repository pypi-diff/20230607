# Comparing `tmp/dynamic_overload-0.1.0.tar.gz` & `tmp/dynamic_overload-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_overload-0.1.0.tar", last modified: Wed Jun  7 10:52:13 2023, max compression
+gzip compressed data, was "dynamic_overload-0.2.0.tar", last modified: Wed Jun  7 15:31:27 2023, max compression
```

## Comparing `dynamic_overload-0.1.0.tar` & `dynamic_overload-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 10:52:13.223152 dynamic_overload-0.1.0/
--rw-rw-rw-   0        0        0     1090 2021-09-19 20:06:17.000000 dynamic_overload-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3005 2023-06-07 10:52:13.224152 dynamic_overload-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1946 2023-06-07 10:19:49.000000 dynamic_overload-0.1.0/README.md
--rw-rw-rw-   0        0        0       99 2023-06-06 17:58:02.000000 dynamic_overload-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1556 2023-06-07 10:52:13.227151 dynamic_overload-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2021-09-19 19:56:34.000000 dynamic_overload-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:52:13.143530 dynamic_overload-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 10:52:13.167158 dynamic_overload-0.1.0/src/dynamic_overload/
--rw-rw-rw-   0        0        0      102 2023-06-07 10:45:02.000000 dynamic_overload-0.1.0/src/dynamic_overload/__init__.py
--rw-rw-rw-   0        0        0    13472 2023-06-07 10:45:22.000000 dynamic_overload-0.1.0/src/dynamic_overload/overload.py
--rw-rw-rw-   0        0        0        0 2022-10-22 20:59:42.000000 dynamic_overload-0.1.0/src/dynamic_overload/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-07 10:52:13.213292 dynamic_overload-0.1.0/src/dynamic_overload.egg-info/
--rw-rw-rw-   0        0        0     3005 2023-06-07 10:52:13.000000 dynamic_overload-0.1.0/src/dynamic_overload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-06-07 10:52:13.000000 dynamic_overload-0.1.0/src/dynamic_overload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 10:52:13.000000 dynamic_overload-0.1.0/src/dynamic_overload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 18:16:42.000000 dynamic_overload-0.1.0/src/dynamic_overload.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       52 2023-06-07 10:52:13.000000 dynamic_overload-0.1.0/src/dynamic_overload.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-07 10:52:13.000000 dynamic_overload-0.1.0/src/dynamic_overload.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 10:52:13.219144 dynamic_overload-0.1.0/tests/
--rw-rw-rw-   0        0        0     4333 2023-06-07 10:29:45.000000 dynamic_overload-0.1.0/tests/test_classes.py
--rw-rw-rw-   0        0        0     1545 2023-06-07 09:08:47.000000 dynamic_overload-0.1.0/tests/test_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:31:27.718242 dynamic_overload-0.2.0/
+-rw-rw-rw-   0        0        0     1090 2021-09-19 20:06:17.000000 dynamic_overload-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3033 2023-06-07 15:31:27.718242 dynamic_overload-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1973 2023-06-07 15:29:48.000000 dynamic_overload-0.2.0/README.md
+-rw-rw-rw-   0        0        0       99 2023-06-06 17:58:02.000000 dynamic_overload-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1902 2023-06-07 15:31:27.724255 dynamic_overload-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       73 2021-09-19 19:56:34.000000 dynamic_overload-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:31:27.668385 dynamic_overload-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 15:31:27.692414 dynamic_overload-0.2.0/src/dynamic_overload/
+-rw-rw-rw-   0        0        0      102 2023-06-07 10:45:02.000000 dynamic_overload-0.2.0/src/dynamic_overload/__init__.py
+-rw-rw-rw-   0        0        0    13521 2023-06-07 14:25:27.000000 dynamic_overload-0.2.0/src/dynamic_overload/overload.py
+-rw-rw-rw-   0        0        0        0 2022-10-22 20:59:42.000000 dynamic_overload-0.2.0/src/dynamic_overload/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-07 15:31:27.712241 dynamic_overload-0.2.0/src/dynamic_overload.egg-info/
+-rw-rw-rw-   0        0        0     3033 2023-06-07 15:31:27.000000 dynamic_overload-0.2.0/src/dynamic_overload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-06-07 15:31:27.000000 dynamic_overload-0.2.0/src/dynamic_overload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 15:31:27.000000 dynamic_overload-0.2.0/src/dynamic_overload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 18:16:42.000000 dynamic_overload-0.2.0/src/dynamic_overload.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       76 2023-06-07 15:31:27.000000 dynamic_overload-0.2.0/src/dynamic_overload.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-07 15:31:27.000000 dynamic_overload-0.2.0/src/dynamic_overload.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 15:31:27.716243 dynamic_overload-0.2.0/tests/
+-rw-rw-rw-   0        0        0     4335 2023-06-07 14:01:04.000000 dynamic_overload-0.2.0/tests/test_classes.py
+-rw-rw-rw-   0        0        0     1547 2023-06-07 13:12:26.000000 dynamic_overload-0.2.0/tests/test_functions.py
```

### Comparing `dynamic_overload-0.1.0/LICENSE` & `dynamic_overload-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_overload-0.1.0/PKG-INFO` & `dynamic_overload-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_overload
-Version: 0.1.0
+Version: 0.2.0
 Summary: A basic package that allows to overload functions and class functions dynamically depending on the input types.
 Home-page: https://github.com/ferranSanchezLlado/dynamic_overload.git
 Author: Ferran Sanchez Llado
 Author-email: ferransll@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -15,27 +15,29 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Dynamic Overload
 
 Dynamic Overload is a python package that allows you to overload functions and classes using dynamic dispatch depending on the type of the arguments. This allows you to write more readable code and avoid using isinstance and type checks.
 
 The package also detects collisions between the overloads and warns the user about them without breaking the code. In case of collision, the first overload is used. So, its recomended that you put the most specific overloads first before the more general ones.
 
 ## Installation
 
+Requires python 3.10 or higher
+
 ```bash
 pip install dynamic-overload
 ```
 
 ## Usage
 
 For functions:
@@ -96,9 +98,7 @@
 assert Integer('1').x == 1
 assert Integer(1.0).x == 1
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
-```
-
```

### Comparing `dynamic_overload-0.1.0/README.md` & `dynamic_overload-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 Dynamic Overload is a python package that allows you to overload functions and classes using dynamic dispatch depending on the type of the arguments. This allows you to write more readable code and avoid using isinstance and type checks.
 
 The package also detects collisions between the overloads and warns the user about them without breaking the code. In case of collision, the first overload is used. So, its recomended that you put the most specific overloads first before the more general ones.
 
 ## Installation
 
+Requires python 3.10 or higher
+
 ```bash
 pip install dynamic-overload
 ```
 
 ## Usage
 
 For functions:
@@ -70,9 +72,7 @@
 assert Integer('1').x == 1
 assert Integer(1.0).x == 1
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
-```
-
```

### Comparing `dynamic_overload-0.1.0/setup.cfg` & `dynamic_overload-0.2.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -10,89 +10,110 @@
 00000090: 6e20 7468 6520 696e 7075 7420 7479 7065  n the input type
 000000a0: 732e 0d0a 6c6f 6e67 5f64 6573 6372 6970  s...long_descrip
 000000b0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 000000c0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000d0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
 000000e0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
 000000f0: 6b64 6f77 6e0d 0a76 6572 7369 6f6e 203d  kdown..version =
-00000100: 2030 2e31 2e30 0d0a 6175 7468 6f72 203d   0.1.0..author =
+00000100: 2030 2e32 2e30 0d0a 6175 7468 6f72 203d   0.2.0..author =
 00000110: 2046 6572 7261 6e20 5361 6e63 6865 7a20   Ferran Sanchez 
 00000120: 4c6c 6164 6f0d 0a61 7574 686f 725f 656d  Llado..author_em
 00000130: 6169 6c20 3d20 6665 7272 616e 736c 6c40  ail = ferransll@
 00000140: 676d 6169 6c2e 636f 6d0d 0a75 726c 203d  gmail.com..url =
 00000150: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000160: 636f 6d2f 6665 7272 616e 5361 6e63 6865  com/ferranSanche
 00000170: 7a4c 6c61 646f 2f64 796e 616d 6963 5f6f  zLlado/dynamic_o
 00000180: 7665 726c 6f61 642e 6769 740d 0a6c 6963  verload.git..lic
 00000190: 656e 7365 203d 204d 4954 0d0a 6c69 6365  ense = MIT..lice
-000001a0: 6e73 655f 6669 6c65 203d 204c 4943 454e  nse_file = LICEN
-000001b0: 5345 0d0a 7265 6164 6d65 203d 2052 4541  SE..readme = REA
-000001c0: 444d 452e 6d64 0d0a 706c 6174 666f 726d  DME.md..platform
-000001d0: 7320 3d20 616e 790d 0a63 6c61 7373 6966  s = any..classif
-000001e0: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
-000001f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000200: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-00000210: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000220: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000230: 3a20 3320 3a3a 204f 6e6c 790d 0a09 4c69  : 3 :: Only...Li
-00000240: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000250: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-00000260: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
-00000270: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000280: 6465 7065 6e64 656e 740d 0a09 4465 7665  dependent...Deve
-00000290: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
-000002a0: 3a20 3320 2d20 416c 7068 610d 0a09 496e  : 3 - Alpha...In
-000002b0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-000002c0: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
-000002d0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-000002e0: 6520 3a3a 2053 6369 656e 6365 2f52 6573  e :: Science/Res
-000002f0: 6561 7263 680d 0a09 546f 7069 6320 3a3a  earch...Topic ::
-00000300: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
-00000310: 6e65 6572 696e 670d 0a09 546f 7069 6320  neering...Topic 
-00000320: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000330: 6c6f 706d 656e 740d 0a09 546f 7069 6320  lopment...Topic 
-00000340: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000350: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
-00000360: 7269 6573 0d0a 0954 6f70 6963 203a 3a20  ries...Topic :: 
-00000370: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
-00000380: 6d65 6e74 203a 3a20 4c69 6272 6172 6965  ment :: Librarie
-00000390: 7320 3a3a 2050 7974 686f 6e20 4d6f 6475  s :: Python Modu
-000003a0: 6c65 730d 0a09 5479 7069 6e67 203a 3a20  les...Typing :: 
-000003b0: 5479 7065 640d 0a0d 0a5b 6f70 7469 6f6e  Typed....[option
-000003c0: 735d 0d0a 7061 636b 6167 6573 203d 2066  s]..packages = f
-000003d0: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-000003e0: 7569 7265 7320 3d20 3e3d 332e 360d 0a70  uires = >=3.6..p
-000003f0: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
-00000400: 3d73 7263 0d0a 7a69 705f 7361 6665 203d  =src..zip_safe =
-00000410: 206e 6f0d 0a0d 0a5b 6f70 7469 6f6e 732e   no....[options.
-00000420: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-00000430: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
-00000440: 6f70 7469 6f6e 732e 6578 7472 6173 5f72  options.extras_r
-00000450: 6571 7569 7265 5d0d 0a74 6573 7469 6e67  equire]..testing
-00000460: 203d 200d 0a09 7079 7465 7374 3e3d 362e   = ...pytest>=6.
-00000470: 300d 0a09 7079 7465 7374 2d63 6f76 3e3d  0...pytest-cov>=
-00000480: 322e 3130 0d0a 0966 6c61 6b65 383e 3d33  2.10...flake8>=3
-00000490: 2e39 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .9....[options.p
-000004a0: 6163 6b61 6765 5f64 6174 615d 0d0a 6479  ackage_data]..dy
-000004b0: 6e61 6d69 635f 6f76 6572 6c6f 6164 203d  namic_overload =
-000004c0: 2070 792e 7479 7065 640d 0a0d 0a5b 666c   py.typed....[fl
-000004d0: 616b 6538 5d0d 0a6d 6178 2d6c 696e 652d  ake8]..max-line-
-000004e0: 6c65 6e67 7468 203d 2031 3630 0d0a 6578  length = 160..ex
-000004f0: 7465 6e64 2d69 676e 6f72 6520 3d20 4532  tend-ignore = E2
-00000500: 3033 2c20 4638 3131 0d0a 0d0a 5b70 796c  03, F811....[pyl
-00000510: 696e 742e 464f 524d 4154 5d0d 0a6d 6178  int.FORMAT]..max
-00000520: 2d6c 696e 652d 6c65 6e67 7468 203d 2031  -line-length = 1
-00000530: 3630 0d0a 0d0a 5b63 6f76 6572 6167 653a  60....[coverage:
-00000540: 7265 706f 7274 5d0d 0a73 6b69 705f 656d  report]..skip_em
-00000550: 7074 7920 3d20 7472 7565 0d0a 6f6d 6974  pty = true..omit
-00000560: 203d 202a 2f6d 6169 6e2e 7079 0d0a 6578   = */main.py..ex
-00000570: 636c 7564 655f 6c69 6e65 7320 3d20 0d0a  clude_lines = ..
-00000580: 0970 6173 730d 0a09 7072 6167 6d61 3a20  .pass...pragma: 
-00000590: 6e6f 2063 6f76 6572 0d0a 0964 6566 205f  no cover...def _
-000005a0: 5f72 6570 725f 5f0d 0a09 6465 6620 5f5f  _repr__...def __
-000005b0: 7374 725f 5f0d 0a09 6966 205f 5f6e 616d  str__...if __nam
-000005c0: 655f 5f20 3d3d 202e 5f5f 6d61 696e 5f5f  e__ == .__main__
-000005d0: 2e3a 0d0a 0969 6620 5459 5045 5f43 4845  .:...if TYPE_CHE
-000005e0: 434b 494e 473a 0d0a 0d0a 5b65 6767 5f69  CKING:....[egg_i
-000005f0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-00000600: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-00000610: 0d0a 0d0a                                ....
+000001a0: 6e73 655f 6669 6c65 7320 3d20 4c49 4345  nse_files = LICE
+000001b0: 4e53 450d 0a72 6561 646d 6520 3d20 5245  NSE..readme = RE
+000001c0: 4144 4d45 2e6d 640d 0a70 6c61 7466 6f72  ADME.md..platfor
+000001d0: 6d73 203d 2061 6e79 0d0a 636c 6173 7369  ms = any..classi
+000001e0: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
+000001f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000200: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
+00000210: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000220: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000230: 3a3a 2033 203a 3a20 4f6e 6c79 0d0a 094c  :: 3 :: Only...L
+00000240: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000250: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000260: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
+00000270: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+00000280: 6e64 6570 656e 6465 6e74 0d0a 0944 6576  ndependent...Dev
+00000290: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
+000002a0: 3a3a 2033 202d 2041 6c70 6861 0d0a 0949  :: 3 - Alpha...I
+000002b0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+000002c0: 203a 3a20 4465 7665 6c6f 7065 7273 0d0a   :: Developers..
+000002d0: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+000002e0: 6365 203a 3a20 5363 6965 6e63 652f 5265  ce :: Science/Re
+000002f0: 7365 6172 6368 0d0a 0954 6f70 6963 203a  search...Topic :
+00000300: 3a20 5363 6965 6e74 6966 6963 2f45 6e67  : Scientific/Eng
+00000310: 696e 6565 7269 6e67 0d0a 0954 6f70 6963  ineering...Topic
+00000320: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
+00000330: 656c 6f70 6d65 6e74 0d0a 0954 6f70 6963  elopment...Topic
+00000340: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
+00000350: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
+00000360: 6172 6965 730d 0a09 546f 7069 6320 3a3a  aries...Topic ::
+00000370: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
+00000380: 706d 656e 7420 3a3a 204c 6962 7261 7269  pment :: Librari
+00000390: 6573 203a 3a20 5079 7468 6f6e 204d 6f64  es :: Python Mod
+000003a0: 756c 6573 0d0a 0954 7970 696e 6720 3a3a  ules...Typing ::
+000003b0: 2054 7970 6564 0d0a 0d0a 5b6f 7074 696f   Typed....[optio
+000003c0: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
+000003d0: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
+000003e0: 7175 6972 6573 203d 203e 3d33 2e31 300d  quires = >=3.10.
+000003f0: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
+00000400: 0a09 3d73 7263 0d0a 7a69 705f 7361 6665  ..=src..zip_safe
+00000410: 203d 206e 6f0d 0a0d 0a5b 6f70 7469 6f6e   = no....[option
+00000420: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000430: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+00000440: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+00000450: 5f72 6571 7569 7265 5d0d 0a74 6573 7469  _require]..testi
+00000460: 6e67 203d 200d 0a09 7079 7465 7374 3e3d  ng = ...pytest>=
+00000470: 362e 300d 0a09 7079 7465 7374 2d63 6f76  6.0...pytest-cov
+00000480: 3e3d 322e 3130 0d0a 0966 6c61 6b65 383e  >=2.10...flake8>
+00000490: 3d33 2e39 0d0a 0970 796c 696e 743e 3d32  =3.9...pylint>=2
+000004a0: 2e38 0d0a 096d 7970 793e 3d30 2e38 3132  .8...mypy>=0.812
+000004b0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+000004c0: 6b61 6765 5f64 6174 615d 0d0a 6479 6e61  kage_data]..dyna
+000004d0: 6d69 635f 6f76 6572 6c6f 6164 203d 2070  mic_overload = p
+000004e0: 792e 7479 7065 640d 0a0d 0a5b 666c 616b  y.typed....[flak
+000004f0: 6538 5d0d 0a6d 6178 2d6c 696e 652d 6c65  e8]..max-line-le
+00000500: 6e67 7468 203d 2031 3630 0d0a 6578 7465  ngth = 160..exte
+00000510: 6e64 2d69 676e 6f72 6520 3d20 4532 3033  nd-ignore = E203
+00000520: 2c20 4638 3131 0d0a 0d0a 5b70 796c 696e  , F811....[pylin
+00000530: 742e 464f 524d 4154 5d0d 0a6d 6178 2d6c  t.FORMAT]..max-l
+00000540: 696e 652d 6c65 6e67 7468 203d 2031 3630  ine-length = 160
+00000550: 0d0a 0d0a 5b6d 7970 795d 0d0a 7079 7468  ....[mypy]..pyth
+00000560: 6f6e 5f76 6572 7369 6f6e 203d 2033 2e31  on_version = 3.1
+00000570: 300d 0a77 6172 6e5f 7265 7475 726e 5f61  0..warn_return_a
+00000580: 6e79 203d 2054 7275 650d 0a77 6172 6e5f  ny = True..warn_
+00000590: 756e 7573 6564 5f63 6f6e 6669 6773 203d  unused_configs =
+000005a0: 2054 7275 650d 0a64 6973 616c 6c6f 775f   True..disallow_
+000005b0: 756e 7479 7065 645f 6465 6673 203d 2054  untyped_defs = T
+000005c0: 7275 650d 0a64 6973 616c 6c6f 775f 696e  rue..disallow_in
+000005d0: 636f 6d70 6c65 7465 5f64 6566 7320 3d20  complete_defs = 
+000005e0: 5472 7565 0d0a 6368 6563 6b5f 756e 7479  True..check_unty
+000005f0: 7065 645f 6465 6673 203d 2054 7275 650d  ped_defs = True.
+00000600: 0a73 7472 6963 745f 6f70 7469 6f6e 616c  .strict_optional
+00000610: 203d 2054 7275 650d 0a77 6172 6e5f 7265   = True..warn_re
+00000620: 6475 6e64 616e 745f 6361 7374 7320 3d20  dundant_casts = 
+00000630: 5472 7565 0d0a 7761 726e 5f75 6e75 7365  True..warn_unuse
+00000640: 645f 6967 6e6f 7265 7320 3d20 5472 7565  d_ignores = True
+00000650: 0d0a 6e6f 5f69 6d70 6c69 6369 745f 6f70  ..no_implicit_op
+00000660: 7469 6f6e 616c 203d 2054 7275 650d 0a69  tional = True..i
+00000670: 676e 6f72 655f 6d69 7373 696e 675f 696d  gnore_missing_im
+00000680: 706f 7274 7320 3d20 5472 7565 0d0a 0d0a  ports = True....
+00000690: 5b63 6f76 6572 6167 653a 7265 706f 7274  [coverage:report
+000006a0: 5d0d 0a73 6b69 705f 656d 7074 7920 3d20  ]..skip_empty = 
+000006b0: 7472 7565 0d0a 6f6d 6974 203d 202a 2f6d  true..omit = */m
+000006c0: 6169 6e2e 7079 0d0a 6578 636c 7564 655f  ain.py..exclude_
+000006d0: 6c69 6e65 7320 3d20 0d0a 0970 6173 730d  lines = ...pass.
+000006e0: 0a09 7072 6167 6d61 3a20 6e6f 2063 6f76  ..pragma: no cov
+000006f0: 6572 0d0a 0964 6566 205f 5f72 6570 725f  er...def __repr_
+00000700: 5f0d 0a09 6465 6620 5f5f 7374 725f 5f0d  _...def __str__.
+00000710: 0a09 6966 205f 5f6e 616d 655f 5f20 3d3d  ..if __name__ ==
+00000720: 202e 5f5f 6d61 696e 5f5f 2e3a 0d0a 0969   .__main__.:...i
+00000730: 6620 5459 5045 5f43 4845 434b 494e 473a  f TYPE_CHECKING:
+00000740: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000750: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000760: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `dynamic_overload-0.1.0/src/dynamic_overload/overload.py` & `dynamic_overload-0.2.0/src/dynamic_overload/overload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ This module provides the core functionality for dynamic_overload. """
 # https://peps.python.org/pep-3124/
-from typing import Any, Callable, TypeVar, Generic
+from typing import Any, Callable, TypeVar, Generic, Dict, Type, Tuple, List
 from types import UnionType
 from inspect import signature, Signature, Parameter, BoundArguments
 import warnings
 
 
 # message, category, filename, lineno, line=None
 warnings.formatwarning = (
@@ -17,15 +17,15 @@
 
 
 class ConflictingOverloadWarning(Warning):
     """Raised when two or more overload functions have the similar signatures that could result in a collision.
     Default behavior is to ignore the warning and use the first overload function that matches the arguments."""
 
 
-class OverloadDict(dict[str, Any]):
+class OverloadDict(Dict[str, Any]):
     """A dictionary that allows overloading of methods. Other than that, it behaves like a normal dictionary."""
 
     def __setitem__(self, key: str, value: Any) -> None:
         if not callable(value):
             super().__setitem__(key, value)
             return
 
@@ -34,35 +34,36 @@
             super().__setitem__(key, OverloadItem(value))
         elif isinstance(current_value, OverloadItem):
             current_value.append(value)
         else:
             raise TypeError(f"Overloaded method {key} must be a function")
 
 
-def _score_type_hint(arg: Any, hint: type) -> int:
+def _score_type_hint(arg: Any, hint: Type) -> int:
     """Returns a score based on how well the argument matches the type hint.
 
     Returns -1 if the argument does not match the type hint.
     Returns 0 if the type hint is Any or not specified.
     Returns 1 if the argument matches the type hint (including Union types).
     """
     # Remove parameterized types (e.g. List[int] -> List)
     if hasattr(hint, "__origin__"):
         hint = hint.__origin__
 
     if hint is Parameter.empty or hint is Any:
         return 0
 
-    if isinstance(arg, hint):
-        return 1
-    # Handle Union types and Optional types
     if isinstance(hint, UnionType):
         for subhint in hint.__args__:
-            if isinstance(arg, subhint):
+            if _score_type_hint(arg, subhint) > 0:
                 return 1
+        return -1
+
+    if isinstance(arg, hint):
+        return 1
     return -1  # no match
 
 
 def _score_any_type_hint(arg: Any, param: Parameter) -> int:
     """Returns a score based on how well the argument matches the type hint.
     This function can handle *args and **kwargs.
 
@@ -158,18 +159,18 @@
     This class is not meant to be used directly. Instead, use the `OverloadMeta` metaclass to create overloaded methods.
     """
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         instance: T,
-        owner_cls: type[T],
+        owner_cls: Type[T],
         name: str,
-        overload_list: list[Callable],
-        signatures: list[Signature],
+        overload_list: List[Callable],
+        signatures: List[Signature],
     ) -> None:
         """Initializes the dispatcher."""
         self.instance = instance
         self.owner_cls = owner_cls
         self.name = name
         self.overload_list = overload_list
         self.signatures = signatures
@@ -197,15 +198,15 @@
             func = self.best_match(*args, **kwargs)
         except NoMatchingOverloadException:
             pass
         else:
             return func(self.instance, *args, **kwargs)
 
         # no matching overload in owner class, check next in line
-        super_instance = super(self.owner_cls, self.instance)  # type: ignore
+        super_instance = super(self.owner_cls, self.instance)
         super_call = getattr(super_instance, self.name, None)
         if super_call is not None:
             try:
                 return super_call(*args, **kwargs)
             except TypeError:
                 pass
         raise NoMatchingOverloadException()
@@ -214,15 +215,15 @@
 class FunctionOverloadDispatcher:
     """A class that dispatches overloaded functions based on the arguments. This dispatcher is intended to be used
     with functions that are not bound to a specific instance of a class.
 
     This class is not meant to be used directly. Instead, use the `overload` decorator.
     """
 
-    def __init__(self, name: str, overload_list: list[Callable], signatures: list[Signature]) -> None:
+    def __init__(self, name: str, overload_list: List[Callable], signatures: List[Signature]) -> None:
         """Initializes the dispatcher."""
         self.name = name
         self.overload_list = overload_list
         self.signatures = signatures
 
     def best_match(self, *args: Any, **kwargs: Any) -> Callable:
         """Returns the best matching overload based on the arguments."""
@@ -243,20 +244,20 @@
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         """Calls the best matching overload."""
         func = self.best_match(*args, **kwargs)
         return func(*args, **kwargs)
 
 
-class OverloadItem:
+class OverloadItem(Generic[T]):
     """A class that represents an overloaded method or function."""
 
     name: str
-    overloads: list[Callable]
-    signatures: list[Signature]
+    overloads: List[Callable]
+    signatures: List[Signature]
 
     def __init__(self, func: Callable) -> None:
         """Initializes the overload item."""
         self.name = func.__name__
         self.overloads = [func]
         self.signatures = [signature(func)]
 
@@ -274,15 +275,15 @@
                     f"Overload collision: {func.__name__}, {sig} with {existing_sig}. "
                     "In case of conflict on runtime, the first overload will be used.",
                     ConflictingOverloadWarning,
                 )
         self.overloads.append(func)
         self.signatures.append(sig)
 
-    def __get__(self, instance, owner_cls):
+    def __get__(self, instance: T, owner_cls: Type[T]) -> BoundOverloadDispatcher[T]:
         """Returns a bound dispatcher for instance methods, or a dispatcher for static/class methods."""
         return BoundOverloadDispatcher(instance, owner_cls, self.name, self.overloads, self.signatures)
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         """Calls the function overload dispatcher."""
         return FunctionOverloadDispatcher(self.name, self.overloads, self.signatures)(*args, **kwargs)
 
@@ -302,29 +303,29 @@
         return f"Overloaded function '{self.name}' with {len(self)} signatures:\n" + items
 
 
 class OverloadMeta(type):
     """A metaclass that allows overloading methods and functions."""
 
     @classmethod
-    def __prepare__(mcs, _name: str, _bases: tuple[type, ...], /, **_kwargs: Any) -> OverloadDict:
+    def __prepare__(mcs, _name: str, _bases: Tuple[type, ...], /, **_kwargs: Any) -> OverloadDict:
         """Returns a dictionary that allows overloading."""
         return OverloadDict()
 
     def __new__(mcs, name: str, bases: tuple, namespace: OverloadDict, **kwargs: Any) -> Any:
         """Creates a new class with overloaded methods and functions."""
         return super().__new__(mcs, name, bases, namespace, **kwargs)
 
 
 # pylint: disable=too-few-public-methods
 class Overload(metaclass=OverloadMeta):
     """A class that allows overloading methods and functions."""
 
 
-_overload_functions: dict[str, OverloadItem] = {}
+_overload_functions: Dict[str, OverloadItem] = {}
 """A dictionary that maps function names to their overloads. Used by the `overload` decorator."""
 
 
 def overload(func: Callable) -> Callable:
     """A decorator that allows overloading functions."""
     name = f"{func.__module__}.{func.__qualname__}"
     if name not in _overload_functions:
```

### Comparing `dynamic_overload-0.1.0/src/dynamic_overload.egg-info/PKG-INFO` & `dynamic_overload-0.2.0/src/dynamic_overload.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-overload
-Version: 0.1.0
+Version: 0.2.0
 Summary: A basic package that allows to overload functions and class functions dynamically depending on the input types.
 Home-page: https://github.com/ferranSanchezLlado/dynamic_overload.git
 Author: Ferran Sanchez Llado
 Author-email: ferransll@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -15,27 +15,29 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Dynamic Overload
 
 Dynamic Overload is a python package that allows you to overload functions and classes using dynamic dispatch depending on the type of the arguments. This allows you to write more readable code and avoid using isinstance and type checks.
 
 The package also detects collisions between the overloads and warns the user about them without breaking the code. In case of collision, the first overload is used. So, its recomended that you put the most specific overloads first before the more general ones.
 
 ## Installation
 
+Requires python 3.10 or higher
+
 ```bash
 pip install dynamic-overload
 ```
 
 ## Usage
 
 For functions:
@@ -96,9 +98,7 @@
 assert Integer('1').x == 1
 assert Integer(1.0).x == 1
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
-```
-
```

### Comparing `dynamic_overload-0.1.0/tests/test_classes.py` & `dynamic_overload-0.2.0/tests/test_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dynamic_overload import OverloadMeta, Overload
 from dynamic_overload.overload import ConflictingOverloadWarning, NoMatchingOverloadException
+
 import pytest
 
 
 class Test(metaclass=OverloadMeta):
     __test__ = False  # disables pytest collection
     x: int | str | float | None
     y: float | None
```

### Comparing `dynamic_overload-0.1.0/tests/test_functions.py` & `dynamic_overload-0.2.0/tests/test_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dynamic_overload import overload
-from typing import Iterable
 from dynamic_overload.overload import NoMatchingOverloadException
+
 import pytest
+from typing import Iterable
 
 
 @overload
 def flatten(x: int) -> Iterable[int]:
     """Flatten an integer."""
     yield x
```

