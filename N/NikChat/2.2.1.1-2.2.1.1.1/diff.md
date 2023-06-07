# Comparing `tmp/NikChat-2.2.1.1.tar.gz` & `tmp/NikChat-2.2.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikChat-2.2.1.1.tar", last modified: Tue Jun  6 01:11:51 2023, max compression
+gzip compressed data, was "NikChat-2.2.1.1.1.tar", last modified: Wed Jun  7 03:21:10 2023, max compression
```

## Comparing `NikChat-2.2.1.1.tar` & `NikChat-2.2.1.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 01:11:51.364853 NikChat-2.2.1.1/
--rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.2.1.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-06 01:11:51.335853 NikChat-2.2.1.1/NikChat/
--rw-rw-rw-   0        0        0        0 2023-06-06 01:09:19.000000 NikChat-2.2.1.1/NikChat/__init__.py
--rw-rw-rw-   0        0        0     3233 2023-06-06 01:07:44.000000 NikChat-2.2.1.1/NikChat/chatbot.py
--rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.2.1.1/NikChat/results.py
--rw-rw-rw-   0        0        0     2382 2023-06-06 01:06:27.000000 NikChat-2.2.1.1/NikChat/training.py
-drwxrwxrwx   0        0        0        0 2023-06-06 01:11:51.363855 NikChat-2.2.1.1/NikChat.egg-info/
--rw-rw-rw-   0        0        0     1680 2023-06-06 01:11:51.000000 NikChat-2.2.1.1/NikChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-06 01:11:51.000000 NikChat-2.2.1.1/NikChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 01:11:51.000000 NikChat-2.2.1.1/NikChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 01:11:51.000000 NikChat-2.2.1.1/NikChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1680 2023-06-06 01:11:51.365853 NikChat-2.2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-05-24 05:16:40.000000 NikChat-2.2.1.1/README.md
--rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.2.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      635 2023-06-06 01:11:51.367853 NikChat-2.2.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 03:21:10.708798 NikChat-2.2.1.1.1/
+-rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.2.1.1.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-07 03:21:10.604471 NikChat-2.2.1.1.1/NikChat/
+-rw-rw-rw-   0        0        0     3233 2023-06-07 03:15:23.000000 NikChat-2.2.1.1.1/NikChat/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.2.1.1.1/NikChat/results.py
+-rw-rw-rw-   0        0        0     2382 2023-06-06 01:06:27.000000 NikChat-2.2.1.1.1/NikChat/training.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:21:10.692131 NikChat-2.2.1.1.1/NikChat.egg-info/
+-rw-rw-rw-   0        0        0     1682 2023-06-07 03:21:10.000000 NikChat-2.2.1.1.1/NikChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-07 03:21:10.000000 NikChat-2.2.1.1.1/NikChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 03:21:10.000000 NikChat-2.2.1.1.1/NikChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-07 03:21:10.000000 NikChat-2.2.1.1.1/NikChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1682 2023-06-07 03:21:10.710798 NikChat-2.2.1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-05-24 05:16:40.000000 NikChat-2.2.1.1.1/README.md
+-rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.2.1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      637 2023-06-07 03:21:10.728424 NikChat-2.2.1.1.1/setup.cfg
```

### Comparing `NikChat-2.2.1.1/LICENSE` & `NikChat-2.2.1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NikChat-2.2.1.1/NikChat/chatbot.py` & `NikChat-2.2.1.1.1/NikChat/__init__.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.2.1.1/NikChat/results.py` & `NikChat-2.2.1.1.1/NikChat/results.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.2.1.1/NikChat/training.py` & `NikChat-2.2.1.1.1/NikChat/training.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.2.1.1/NikChat.egg-info/PKG-INFO` & `NikChat-2.2.1.1.1/NikChat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.2.1.1
+Version: 2.2.1.1.1
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NikChat-2.2.1.1/PKG-INFO` & `NikChat-2.2.1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.2.1.1
+Version: 2.2.1.1.1
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NikChat-2.2.1.1/README.md` & `NikChat-2.2.1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `NikChat-2.2.1.1/setup.cfg` & `NikChat-2.2.1.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204e 696b 4368 6174 0d0a 7665 7273   = NikChat..vers
-00000020: 696f 6e20 3d20 322e 322e 312e 310d 0a61  ion = 2.2.1.1..a
-00000030: 7574 686f 7220 3d20 4e69 6b68 696c 2054  uthor = Nikhil T
-00000040: 616d 7661 6461 2028 4e69 6b68 696c 6f64  amvada (Nikhilod
-00000050: 656f 6e31 290d 0a61 7574 686f 725f 656d  eon1)..author_em
-00000060: 6169 6c20 3d20 6e69 6b68 696c 7461 6d76  ail = nikhiltamv
-00000070: 6164 6140 676d 6169 6c2e 636f 6d0d 0a64  ada@gmail.com..d
-00000080: 6573 6372 6970 7469 6f6e 203d 2041 2066  escription = A f
-00000090: 756c 6c2d 666c 6564 6765 6420 6368 6174  ull-fledged chat
-000000a0: 626f 7420 6465 7369 676e 6564 2074 6f20  bot designed to 
-000000b0: 6265 2069 6e63 6f72 7065 7261 7465 6420  be incorperated 
-000000c0: 696e 746f 206f 7468 6572 2070 726f 6a65  into other proje
-000000d0: 6374 732e 2028 5370 6565 6473 206f 6620  cts. (Speeds of 
-000000e0: 302e 3120 7365 636f 6e64 7329 0d0a 6c6f  0.1 seconds)..lo
-000000f0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
-00000100: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
-00000110: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-00000120: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
-00000130: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
-00000140: 0a68 6f6d 655f 7061 6765 203d 2068 7474  .home_page = htt
-00000150: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000160: 4e69 6b68 696c 6f64 656f 6e31 2f4e 696b  Nikhilodeon1/Nik
-00000170: 4368 6174 0d0a 636c 6173 7369 6669 6572  Chat..classifier
-00000180: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
-00000190: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001a0: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
-000001b0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-000001c0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-000001d0: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
-000001e0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-000001f0: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
-00000200: 696f 6e73 5d0d 0a70 6163 6b61 6765 7320  ions]..packages 
-00000210: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
-00000220: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
-00000230: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
-00000240: 655f 6461 7461 203d 2054 7275 650d 0a0d  e_data = True...
-00000250: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000260: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000270: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000020: 696f 6e20 3d20 322e 322e 312e 312e 310d  ion = 2.2.1.1.1.
+00000030: 0a61 7574 686f 7220 3d20 4e69 6b68 696c  .author = Nikhil
+00000040: 2054 616d 7661 6461 2028 4e69 6b68 696c   Tamvada (Nikhil
+00000050: 6f64 656f 6e31 290d 0a61 7574 686f 725f  odeon1)..author_
+00000060: 656d 6169 6c20 3d20 6e69 6b68 696c 7461  email = nikhilta
+00000070: 6d76 6164 6140 676d 6169 6c2e 636f 6d0d  mvada@gmail.com.
+00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
+00000090: 2066 756c 6c2d 666c 6564 6765 6420 6368   full-fledged ch
+000000a0: 6174 626f 7420 6465 7369 676e 6564 2074  atbot designed t
+000000b0: 6f20 6265 2069 6e63 6f72 7065 7261 7465  o be incorperate
+000000c0: 6420 696e 746f 206f 7468 6572 2070 726f  d into other pro
+000000d0: 6a65 6374 732e 2028 5370 6565 6473 206f  jects. (Speeds o
+000000e0: 6620 302e 3120 7365 636f 6e64 7329 0d0a  f 0.1 seconds)..
+000000f0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000100: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+00000110: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+00000120: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+00000130: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+00000140: 6e0d 0a68 6f6d 655f 7061 6765 203d 2068  n..home_page = h
+00000150: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000160: 6d2f 4e69 6b68 696c 6f64 656f 6e31 2f4e  m/Nikhilodeon1/N
+00000170: 696b 4368 6174 0d0a 636c 6173 7369 6669  ikChat..classifi
+00000180: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
+00000190: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000001a0: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
+000001b0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000001c0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+000001d0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
+000001e0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+000001f0: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
+00000200: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
+00000210: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
+00000220: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000230: 2e38 0d0a 696e 636c 7564 655f 7061 636b  .8..include_pack
+00000240: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
+00000250: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000260: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000270: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

