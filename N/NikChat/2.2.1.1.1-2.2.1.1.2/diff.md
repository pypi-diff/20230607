# Comparing `tmp/NikChat-2.2.1.1.1.tar.gz` & `tmp/NikChat-2.2.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikChat-2.2.1.1.1.tar", last modified: Wed Jun  7 03:21:10 2023, max compression
+gzip compressed data, was "NikChat-2.2.1.1.2.tar", last modified: Wed Jun  7 03:40:49 2023, max compression
```

## Comparing `NikChat-2.2.1.1.1.tar` & `NikChat-2.2.1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 03:21:10.708798 NikChat-2.2.1.1.1/
--rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.2.1.1.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-07 03:21:10.604471 NikChat-2.2.1.1.1/NikChat/
--rw-rw-rw-   0        0        0     3233 2023-06-07 03:15:23.000000 NikChat-2.2.1.1.1/NikChat/__init__.py
--rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.2.1.1.1/NikChat/results.py
--rw-rw-rw-   0        0        0     2382 2023-06-06 01:06:27.000000 NikChat-2.2.1.1.1/NikChat/training.py
-drwxrwxrwx   0        0        0        0 2023-06-07 03:21:10.692131 NikChat-2.2.1.1.1/NikChat.egg-info/
--rw-rw-rw-   0        0        0     1682 2023-06-07 03:21:10.000000 NikChat-2.2.1.1.1/NikChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-07 03:21:10.000000 NikChat-2.2.1.1.1/NikChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 03:21:10.000000 NikChat-2.2.1.1.1/NikChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 03:21:10.000000 NikChat-2.2.1.1.1/NikChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1682 2023-06-07 03:21:10.710798 NikChat-2.2.1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-05-24 05:16:40.000000 NikChat-2.2.1.1.1/README.md
--rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.2.1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      637 2023-06-07 03:21:10.728424 NikChat-2.2.1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 03:40:49.676564 NikChat-2.2.1.1.2/
+-rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.2.1.1.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-07 03:40:49.622655 NikChat-2.2.1.1.2/NikChat/
+-rw-rw-rw-   0        0        0     3382 2023-06-07 03:39:55.000000 NikChat-2.2.1.1.2/NikChat/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.2.1.1.2/NikChat/results.py
+-rw-rw-rw-   0        0        0     2382 2023-06-06 01:06:27.000000 NikChat-2.2.1.1.2/NikChat/training.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:40:49.670029 NikChat-2.2.1.1.2/NikChat.egg-info/
+-rw-rw-rw-   0        0        0     1682 2023-06-07 03:40:49.000000 NikChat-2.2.1.1.2/NikChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-07 03:40:49.000000 NikChat-2.2.1.1.2/NikChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 03:40:49.000000 NikChat-2.2.1.1.2/NikChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-07 03:40:49.000000 NikChat-2.2.1.1.2/NikChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1682 2023-06-07 03:40:49.677547 NikChat-2.2.1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-05-24 05:16:40.000000 NikChat-2.2.1.1.2/README.md
+-rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.2.1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      637 2023-06-07 03:40:49.681548 NikChat-2.2.1.1.2/setup.cfg
```

### Comparing `NikChat-2.2.1.1.1/LICENSE` & `NikChat-2.2.1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NikChat-2.2.1.1.1/NikChat/__init__.py` & `NikChat-2.2.1.1.2/NikChat/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             res = res
         return res
     except Exception as e:
         from os.path import exists
         if exists('words.pkl') == False:
             return 'Remember to use nikchat.init() before you use nikchat.NChat()'
         else:
-            return e
+            return e, " If your OS doesn't support automated downloads, please install the following libraries: nltk, numpy, tensorflow, wikipedia, bs4, geopy, geocoder"
         
 
 def init():
     from os.path import exists
     if exists('words.pkl') == False:
         import NikChat.training as traning
         traning.init()
```

### Comparing `NikChat-2.2.1.1.1/NikChat/results.py` & `NikChat-2.2.1.1.2/NikChat/results.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.2.1.1.1/NikChat/training.py` & `NikChat-2.2.1.1.2/NikChat/training.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.2.1.1.1/NikChat.egg-info/PKG-INFO` & `NikChat-2.2.1.1.2/NikChat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.2.1.1.1
+Version: 2.2.1.1.2
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nikchat - v1
 
 Nikchat, the inaugural version of a groundbreaking chatbot AI, signifies a pivotal advancement in conversational interfaces. Equipped with advanced AI algorithms and natural language processing capabilities, Nikchat excels in facilitating meaningful conversations. With its contextual understanding, emotion detection, and personalized responses, Nikchat foreshadows the transformative potential of conversational AI, promising enhanced communication and unparalleled user experiences.
```

### Comparing `NikChat-2.2.1.1.1/PKG-INFO` & `NikChat-2.2.1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.2.1.1.1
+Version: 2.2.1.1.2
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nikchat - v1
 
 Nikchat, the inaugural version of a groundbreaking chatbot AI, signifies a pivotal advancement in conversational interfaces. Equipped with advanced AI algorithms and natural language processing capabilities, Nikchat excels in facilitating meaningful conversations. With its contextual understanding, emotion detection, and personalized responses, Nikchat foreshadows the transformative potential of conversational AI, promising enhanced communication and unparalleled user experiences.
```

### Comparing `NikChat-2.2.1.1.1/README.md` & `NikChat-2.2.1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `NikChat-2.2.1.1.1/setup.cfg` & `NikChat-2.2.1.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204e 696b 4368 6174 0d0a 7665 7273   = NikChat..vers
-00000020: 696f 6e20 3d20 322e 322e 312e 312e 310d  ion = 2.2.1.1.1.
+00000020: 696f 6e20 3d20 322e 322e 312e 312e 320d  ion = 2.2.1.1.2.
 00000030: 0a61 7574 686f 7220 3d20 4e69 6b68 696c  .author = Nikhil
 00000040: 2054 616d 7661 6461 2028 4e69 6b68 696c   Tamvada (Nikhil
 00000050: 6f64 656f 6e31 290d 0a61 7574 686f 725f  odeon1)..author_
 00000060: 656d 6169 6c20 3d20 6e69 6b68 696c 7461  email = nikhilta
 00000070: 6d76 6164 6140 676d 6169 6c2e 636f 6d0d  mvada@gmail.com.
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000090: 2066 756c 6c2d 666c 6564 6765 6420 6368   full-fledged ch
@@ -29,12 +29,12 @@
 000001c0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
 000001d0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
 000001e0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
 000001f0: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
 00000200: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
 00000210: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
 00000220: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000230: 2e38 0d0a 696e 636c 7564 655f 7061 636b  .8..include_pack
+00000230: 2e36 0d0a 696e 636c 7564 655f 7061 636b  .6..include_pack
 00000240: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
 00000250: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
 00000260: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
 00000270: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

