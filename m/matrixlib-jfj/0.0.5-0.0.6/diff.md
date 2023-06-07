# Comparing `tmp/matrixlib_jfj-0.0.5.tar.gz` & `tmp/matrixlib_jfj-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrixlib_jfj-0.0.5.tar", last modified: Wed Jun  7 03:18:05 2023, max compression
+gzip compressed data, was "matrixlib_jfj-0.0.6.tar", last modified: Wed Jun  7 15:36:56 2023, max compression
```

## Comparing `matrixlib_jfj-0.0.5.tar` & `matrixlib_jfj-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 03:18:05.715081 matrixlib_jfj-0.0.5/
--rw-r--r--   0 runner    (1000) runner    (1000)    35148 2023-06-06 20:50:00.000000 matrixlib_jfj-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 03:18:05.719081 matrixlib_jfj-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-06-06 20:36:36.000000 matrixlib_jfj-0.0.5/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)     1014 2023-06-07 01:46:06.000000 matrixlib_jfj-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      965 2023-06-07 03:18:05.719081 matrixlib_jfj-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)       65 2023-06-07 01:15:59.000000 matrixlib_jfj-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 03:18:05.711081 matrixlib_jfj-0.0.5/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 03:18:05.715081 matrixlib_jfj-0.0.5/src/matrixlib_jfj/
--rw-r--r--   0 runner    (1000) runner    (1000)      960 2023-06-07 03:17:46.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13699 2023-06-07 03:15:46.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj/matrix.py
--rw-r--r--   0 runner    (1000) runner    (1000)      270 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj/utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)      213 2023-06-07 01:45:54.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj/vector.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-07 03:18:05.715081 matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1096 2023-06-07 03:18:05.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      371 2023-06-07 03:18:05.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-07 03:18:05.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2023-06-07 03:18:05.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-06-07 03:18:05.000000 matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 15:36:56.952968 matrixlib_jfj-0.0.6/
+-rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0     1116 2023-06-07 15:36:56.952968 matrixlib_jfj-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1003 2023-06-07 15:36:56.961941 matrixlib_jfj-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:36:56.838302 matrixlib_jfj-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 15:36:56.917518 matrixlib_jfj-0.0.6/src/matrixlib_jfj/
+-rw-rw-rw-   0        0        0      960 2023-06-07 15:36:41.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj/__init__.py
+-rw-rw-rw-   0        0        0    13782 2023-06-07 15:36:32.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj/matrix.py
+-rw-rw-rw-   0        0        0      461 2023-06-07 15:32:43.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj/utils.py
+-rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj/vector.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:36:56.949972 matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/
+-rw-rw-rw-   0        0        0     1116 2023-06-07 15:36:56.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-06-07 15:36:56.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 15:36:56.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-07 15:36:56.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 15:36:56.000000 matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/top_level.txt
```

### Comparing `matrixlib_jfj-0.0.5/LICENSE.md` & `matrixlib_jfj-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.5/PKG-INFO` & `matrixlib_jfj-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: matrixlib_jfj
-Version: 0.0.5
-Summary: A library that deals with matrix and vector operations.
-Author: Jemma Starecki
-Author-email: Jemma Starecki <starecki.j@shaw.ca>
-License: GNU General Public License v3 (GPLv3)
-Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
-Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <4,>=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Matrixlib
-A basic library for matrix and vector operations. Any feedback is highly encouraged. I enjoy trying to create modules and programs that work with mathematical functions and data. I also like looking into higher end modules and researching the processes and programs they use to perform tasks. Any feedback will be taken and acted upon.
+Metadata-Version: 2.1
+Name: matrixlib_jfj
+Version: 0.0.6
+Summary: A library that deals with matrix and vector operations.
+Author: Jemma Starecki
+Author-email: Jemma Starecki <starecki.j@shaw.ca>
+License: GNU General Public License v3 (GPLv3)
+Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
+Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: <4,>=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Matrixlib
+A basic library for matrix and vector operations. Any feedback is highly encouraged. I enjoy trying to create modules and programs that work with mathematical functions and data. I also like looking into higher end modules and researching the processes and programs they use to perform tasks. Any feedback will be taken and acted upon.
```

### Comparing `matrixlib_jfj-0.0.5/pyproject.toml` & `matrixlib_jfj-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.0.5/setup.cfg` & `matrixlib_jfj-0.0.6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,63 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6d61 7472 6978 6c69 625f 6a66 6a0a  = matrixlib_jfj.
-00000020: 7665 7273 696f 6e20 3d20 6174 7472 3a20  version = attr: 
-00000030: 6d61 7472 6978 6c69 625f 6a66 6a2e 5f5f  matrixlib_jfj.__
-00000040: 7665 7273 696f 6e5f 5f0a 6465 7363 7269  version__.descri
-00000050: 7074 696f 6e20 3d20 4120 6c69 6272 6172  ption = A librar
-00000060: 7920 7468 6174 2064 6561 6c73 2077 6974  y that deals wit
-00000070: 6820 6d61 7472 6978 2061 6e64 2076 6563  h matrix and vec
-00000080: 746f 7220 6f70 6572 6174 696f 6e73 2e0a  tor operations..
-00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000a0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-000000b0: 6d64 0a6c 6f6e 675f 6465 7363 7269 7074  md.long_descript
-000000c0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000000d0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-000000e0: 0a6c 6963 656e 7365 203d 2047 4e55 2047  .license = GNU G
-000000f0: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
-00000100: 6365 6e73 6520 7633 2028 4750 4c76 3329  cense v3 (GPLv3)
-00000110: 0a61 7574 686f 7220 3d20 4a65 6d6d 6120  .author = Jemma 
-00000120: 5374 6172 6563 6b69 0a61 7574 686f 725f  Starecki.author_
-00000130: 656d 6169 6c20 3d20 7374 6172 6563 6b69  email = starecki
-00000140: 2e6a 4073 6861 772e 6361 0a63 6c61 7373  .j@shaw.ca.class
-00000150: 6966 6965 7273 203d 200a 0944 6576 656c  ifiers = ..Devel
-00000160: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000170: 2033 202d 2041 6c70 6861 0a09 496e 7465   3 - Alpha..Inte
-00000180: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-00000190: 2044 6576 656c 6f70 6572 730a 094c 6963   Developers..Lic
-000001a0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-000001b0: 6f76 6564 203a 3a20 474e 5520 4765 6e65  oved :: GNU Gene
-000001c0: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
-000001d0: 7365 2076 3320 2847 504c 7633 290a 094f  se v3 (GPLv3)..O
-000001e0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-000001f0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000200: 740a 0950 726f 6772 616d 6d69 6e67 204c  t..Programming L
-00000210: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000220: 6e20 3a3a 2033 2e31 300a 7079 7468 6f6e  n :: 3.10.python
-00000230: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000240: 3130 2c20 3c34 0a70 726f 6a65 6374 5f75  10, <4.project_u
-00000250: 726c 7320 3d20 0a09 686f 6d65 7061 6765  rls = ..homepage
-00000260: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000270: 622e 636f 6d2f 4a65 6d6d 6146 726f 6d4a  b.com/JemmaFromJ
-00000280: 7570 6974 6572 2f4d 6174 7269 786c 6962  upiter/Matrixlib
-00000290: 0a09 4973 7375 6520 5472 6163 6b65 7220  ..Issue Tracker 
-000002a0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-000002b0: 2e63 6f6d 2f4a 656d 6d61 4672 6f6d 4a75  .com/JemmaFromJu
-000002c0: 7069 7465 722f 4d61 7472 6978 6c69 622f  piter/Matrixlib/
-000002d0: 6973 7375 6573 0a0a 5b6f 7074 696f 6e73  issues..[options
-000002e0: 5d0a 696e 636c 7564 655f 7072 6f6a 6563  ].include_projec
-000002f0: 745f 6461 7461 203d 2054 7275 650a 696e  t_data = True.in
-00000300: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-00000310: 2066 696c 653a 2072 6571 7569 7265 6d65   file: requireme
-00000320: 6e74 732e 7478 740a 7061 636b 6167 655f  nts.txt.package_
-00000330: 6469 7220 3d20 0a09 3d20 7372 630a 7061  dir = ..= src.pa
-00000340: 636b 6167 6573 203d 2066 696e 643a 0a0a  ckages = find:..
-00000350: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000360: 732e 6669 6e64 5d0a 7768 6572 6520 3d20  s.find].where = 
-00000370: 7372 630a 0a5b 6f70 7469 6f6e 732e 7061  src..[options.pa
-00000380: 636b 6167 655f 6461 7461 5d0a 706f 7368  ckage_data].posh
-00000390: 203d 200a 0922 6461 7461 2f2a 220a 0a5b   = .."data/*"..[
-000003a0: 6567 675f 696e 666f 5d0a 7461 675f 6275  egg_info].tag_bu
-000003b0: 696c 6420 3d20 0a74 6167 5f64 6174 6520  ild = .tag_date 
-000003c0: 3d20 300a 0a                             = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 206d 6174 7269 786c 6962 5f6a 666a   = matrixlib_jfj
+00000020: 0d0a 7665 7273 696f 6e20 3d20 6174 7472  ..version = attr
+00000030: 3a20 6d61 7472 6978 6c69 625f 6a66 6a2e  : matrixlib_jfj.
+00000040: 5f5f 7665 7273 696f 6e5f 5f0d 0a64 6573  __version__..des
+00000050: 6372 6970 7469 6f6e 203d 2041 206c 6962  cription = A lib
+00000060: 7261 7279 2074 6861 7420 6465 616c 7320  rary that deals 
+00000070: 7769 7468 206d 6174 7269 7820 616e 6420  with matrix and 
+00000080: 7665 6374 6f72 206f 7065 7261 7469 6f6e  vector operation
+00000090: 732e 0d0a 6c6f 6e67 5f64 6573 6372 6970  s...long_descrip
+000000a0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
+000000b0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
+000000c0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
+000000d0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
+000000e0: 6b64 6f77 6e0d 0a6c 6963 656e 7365 203d  kdown..license =
+000000f0: 2047 4e55 2047 656e 6572 616c 2050 7562   GNU General Pub
+00000100: 6c69 6320 4c69 6365 6e73 6520 7633 2028  lic License v3 (
+00000110: 4750 4c76 3329 0d0a 6175 7468 6f72 203d  GPLv3)..author =
+00000120: 204a 656d 6d61 2053 7461 7265 636b 690d   Jemma Starecki.
+00000130: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
+00000140: 7374 6172 6563 6b69 2e6a 4073 6861 772e  starecki.j@shaw.
+00000150: 6361 0d0a 636c 6173 7369 6669 6572 7320  ca..classifiers 
+00000160: 3d20 0d0a 0944 6576 656c 6f70 6d65 6e74  = ...Development
+00000170: 2053 7461 7475 7320 3a3a 2033 202d 2041   Status :: 3 - A
+00000180: 6c70 6861 0d0a 0949 6e74 656e 6465 6420  lpha...Intended 
+00000190: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+000001a0: 6c6f 7065 7273 0d0a 094c 6963 656e 7365  lopers...License
+000001b0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000001c0: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
+000001d0: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
+000001e0: 3320 2847 504c 7633 290d 0a09 4f70 6572  3 (GPLv3)...Oper
+000001f0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000200: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
+00000210: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000220: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000230: 3a3a 2033 2e31 300d 0a70 7974 686f 6e5f  :: 3.10..python_
+00000240: 7265 7175 6972 6573 203d 203e 3d33 2e31  requires = >=3.1
+00000250: 302c 203c 340d 0a70 726f 6a65 6374 5f75  0, <4..project_u
+00000260: 726c 7320 3d20 0d0a 0968 6f6d 6570 6167  rls = ...homepag
+00000270: 6520 3d20 6874 7470 733a 2f2f 6769 7468  e = https://gith
+00000280: 7562 2e63 6f6d 2f4a 656d 6d61 4672 6f6d  ub.com/JemmaFrom
+00000290: 4a75 7069 7465 722f 4d61 7472 6978 6c69  Jupiter/Matrixli
+000002a0: 620d 0a09 4973 7375 6520 5472 6163 6b65  b...Issue Tracke
+000002b0: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
+000002c0: 7562 2e63 6f6d 2f4a 656d 6d61 4672 6f6d  ub.com/JemmaFrom
+000002d0: 4a75 7069 7465 722f 4d61 7472 6978 6c69  Jupiter/Matrixli
+000002e0: 622f 6973 7375 6573 0d0a 0d0a 5b6f 7074  b/issues....[opt
+000002f0: 696f 6e73 5d0d 0a69 6e63 6c75 6465 5f70  ions]..include_p
+00000300: 726f 6a65 6374 5f64 6174 6120 3d20 5472  roject_data = Tr
+00000310: 7565 0d0a 696e 7374 616c 6c5f 7265 7175  ue..install_requ
+00000320: 6972 6573 203d 2066 696c 653a 2072 6571  ires = file: req
+00000330: 7569 7265 6d65 6e74 732e 7478 740d 0a70  uirements.txt..p
+00000340: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
+00000350: 3d20 7372 630d 0a70 6163 6b61 6765 7320  = src..packages 
+00000360: 3d20 6669 6e64 3a0d 0a0d 0a5b 6f70 7469  = find:....[opti
+00000370: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000380: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+00000390: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+000003a0: 6167 655f 6461 7461 5d0d 0a70 6f73 6820  age_data]..posh 
+000003b0: 3d20 0d0a 0922 6461 7461 2f2a 220d 0a0d  = ..."data/*"...
+000003c0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000003d0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000003e0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `matrixlib_jfj-0.0.5/src/matrixlib_jfj/__init__.py` & `matrixlib_jfj-0.0.6/src/matrixlib_jfj/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
  	print(transposed) # Output:
 
  	0 0 0\n
 	0 0 0\n
  	6 0 0
 
-Version: 0.0.5
+Version: 0.0.6
 
 Author: Jemma Starecki
 
 Made By <a href="https://github.com/JemmaFromJupiter" target="_blank">JemmaFromJupiter</a> On Github.
 """
 from __future__ import annotations
 from . import matrix
 from . import vector
 from . import utils
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 __author__ = "JemmaFromJupiter"
 
 __all__ = [
 	"matrix",
 	"vector",
 	"utils"
 ]
```

### Comparing `matrixlib_jfj-0.0.5/src/matrixlib_jfj/matrix.py` & `matrixlib_jfj-0.0.6/src/matrixlib_jfj/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 from typing import Union, Optional
 import math
 import random as r
-"""from . import vector
-from . import utils"""
+import numpy as np
+from . import vector
+from . import utils
 
 class Matrix(list):
 	"""Initialises a Matrix that can be used for numerous things
 
 Parameters
 ----------
 rowcols (Union[tuple, list]) : The how many rows and columns are in the matrix.
@@ -106,14 +107,19 @@
 		result.append("+-" + center_space + "-+")
 		result.insert(0, "+-" + center_space + "-+\n")
 		return "".join(result)
 
 	def __repr__(self):
 		return self
 	
+	def rank(self):
+		raise NotImplementedError("Function Not Implemented")
+
+
+	
 	def fill(self, val: Union[int, float]):
 		"""
 		Fill the Matrix with a specified value.
 
  		Parameters
 	 	----------
 	 	val (Union[int, float]) : The value to fill the Matrix with.
@@ -323,15 +329,15 @@
 		if len(self) != len(self[0]):
 			raise ValueError("Matrix Must Be Square")
 		if self.shape == (1, 1):
 			return self[0][0]
 		if self.shape == (2, 2):
 			return (self.get_value(0, 0) * self.get_value(1, 1)) - (self.get_value(0, 1) * self.get_value(1, 0))
 
-		raise NotImplementedError("This Function Hasnt Been Implemented yet")
+		raise NotImplementedError("Function Not Implemented Yet.")
 			
 	
 	def __hash__(self):
 		return hash(tuple(map(tuple, self)))
 
 	def __add__(self, other: Union[Matrix, int, float]) -> Matrix:
 		if isinstance(other, Matrix):
@@ -518,8 +524,8 @@
 					if self[i][j] == other[i][j]:
 						return False
 			return True
 		else:
 			return False
 		
 	def max(self):
-		return max(self.flatten())
+		return max(max(self, key=max))
```

### Comparing `matrixlib_jfj-0.0.5/src/matrixlib_jfj.egg-info/PKG-INFO` & `matrixlib_jfj-0.0.6/src/matrixlib_jfj.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: matrixlib-jfj
-Version: 0.0.5
-Summary: A library that deals with matrix and vector operations.
-Author: Jemma Starecki
-Author-email: Jemma Starecki <starecki.j@shaw.ca>
-License: GNU General Public License v3 (GPLv3)
-Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
-Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <4,>=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Matrixlib
-A basic library for matrix and vector operations. Any feedback is highly encouraged. I enjoy trying to create modules and programs that work with mathematical functions and data. I also like looking into higher end modules and researching the processes and programs they use to perform tasks. Any feedback will be taken and acted upon.
+Metadata-Version: 2.1
+Name: matrixlib-jfj
+Version: 0.0.6
+Summary: A library that deals with matrix and vector operations.
+Author: Jemma Starecki
+Author-email: Jemma Starecki <starecki.j@shaw.ca>
+License: GNU General Public License v3 (GPLv3)
+Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
+Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: <4,>=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Matrixlib
+A basic library for matrix and vector operations. Any feedback is highly encouraged. I enjoy trying to create modules and programs that work with mathematical functions and data. I also like looking into higher end modules and researching the processes and programs they use to perform tasks. Any feedback will be taken and acted upon.
```

