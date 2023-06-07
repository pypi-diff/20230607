# Comparing `tmp/clipol-5.tar.gz` & `tmp/clipol-6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipol-5.tar", last modified: Tue Jun  6 17:04:01 2023, max compression
+gzip compressed data, was "clipol-6.tar", last modified: Wed Jun  7 15:34:19 2023, max compression
```

## Comparing `clipol-5.tar` & `clipol-6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 17:04:01.364250 clipol-5/
--rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 17:04:01.364250 clipol-5/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)     3608 2020-12-08 21:30:42.000000 clipol-5/README
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 17:04:01.360250 clipol-5/clipol.egg-info/
--rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-06 17:04:01.000000 clipol-5/clipol.egg-info/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)      396 2023-06-06 17:04:01.000000 clipol-5/clipol.egg-info/SOURCES.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-06 17:04:01.000000 clipol-5/clipol.egg-info/dependency_links.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        5 2023-06-06 17:04:01.000000 clipol-5/clipol.egg-info/top_level.txt
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-06 17:04:01.364250 clipol-5/idl/
--rw-rw-r--   0 coco      (1000) coco      (1000)      358 2023-06-06 11:16:00.000000 clipol-5/idl/ace.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      623 2023-06-06 11:16:00.000000 clipol-5/idl/bm3d.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      545 2023-06-06 13:51:32.000000 clipol-5/idl/dctdenoise.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      758 2023-06-06 15:32:45.000000 clipol-5/idl/ffdnet.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      280 2020-12-08 23:32:50.000000 clipol-5/idl/lsd.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      996 2023-06-06 13:02:24.000000 clipol-5/idl/msdctd.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      597 2023-06-06 14:02:48.000000 clipol-5/idl/nlbayes.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      380 2023-06-06 11:16:00.000000 clipol-5/idl/nlm.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      209 2023-06-06 11:16:00.000000 clipol-5/idl/phs.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      441 2020-12-08 18:01:47.000000 clipol-5/idl/scb.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      379 2023-06-06 11:16:00.000000 clipol-5/idl/tvdenoise.Dockerfile
--rw-rw-r--   0 coco      (1000) coco      (1000)      303 2020-12-08 23:21:23.000000 clipol-5/idl/tvl1.Dockerfile
--rwxrwxr-x   0 coco      (1000) coco      (1000)    18437 2023-06-06 17:03:48.000000 clipol-5/ipol.py
--rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-06 17:04:01.364250 clipol-5/setup.cfg
--rw-rw-r--   0 coco      (1000) coco      (1000)      643 2023-06-06 17:03:55.000000 clipol-5/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-07 15:34:19.236396 clipol-6/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-07 15:34:19.236396 clipol-6/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5382 2023-06-07 14:47:16.000000 clipol-6/README
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-07 15:34:19.236396 clipol-6/clipol.egg-info/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      518 2023-06-07 15:34:19.000000 clipol-6/clipol.egg-info/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)      396 2023-06-07 15:34:19.000000 clipol-6/clipol.egg-info/SOURCES.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-07 15:34:19.000000 clipol-6/clipol.egg-info/dependency_links.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        5 2023-06-07 15:34:19.000000 clipol-6/clipol.egg-info/top_level.txt
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-07 15:34:19.236396 clipol-6/idl/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      543 2023-06-07 15:25:08.000000 clipol-6/idl/ace.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      769 2023-06-07 15:32:52.000000 clipol-6/idl/bm3d.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      545 2023-06-06 13:51:32.000000 clipol-6/idl/dctdenoise.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      758 2023-06-06 15:32:45.000000 clipol-6/idl/ffdnet.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      280 2020-12-08 23:32:50.000000 clipol-6/idl/lsd.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      996 2023-06-06 13:02:24.000000 clipol-6/idl/msdctd.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      677 2023-06-07 15:27:57.000000 clipol-6/idl/nlbayes.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      482 2023-06-07 15:14:38.000000 clipol-6/idl/nlm.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      283 2023-06-07 14:25:58.000000 clipol-6/idl/phs.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      441 2020-12-08 18:01:47.000000 clipol-6/idl/scb.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      564 2023-06-07 15:26:26.000000 clipol-6/idl/tvdenoise.Dockerfile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      376 2023-06-07 14:25:05.000000 clipol-6/idl/tvl1.Dockerfile
+-rwxrwxr-x   0 coco      (1000) coco      (1000)    18450 2023-06-07 15:33:48.000000 clipol-6/ipol.py
+-rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-07 15:34:19.236396 clipol-6/setup.cfg
+-rw-rw-r--   0 coco      (1000) coco      (1000)      643 2023-06-07 15:33:55.000000 clipol-6/setup.py
```

### Comparing `clipol-5/PKG-INFO` & `clipol-6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipol
-Version: 5
+Version: 6
 Summary: python interface to some IPOL journal algorithms
 Home-page: https://git.sr.ht/~coco/clipol
 Author: Enric Meinhardt-Llopis
 Author-email: enric.meinhardt@ens-paris-saclay.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `clipol-5/clipol.egg-info/PKG-INFO` & `clipol-6/clipol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipol
-Version: 5
+Version: 6
 Summary: python interface to some IPOL journal algorithms
 Home-page: https://git.sr.ht/~coco/clipol
 Author: Enric Meinhardt-Llopis
 Author-email: enric.meinhardt@ens-paris-saclay.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `clipol-5/idl/bm3d.Dockerfile` & `clipol-6/idl/nlbayes.Dockerfile`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-NAME bm3d
-TITLE An Analysis and Implementation of the BM3D Image Denoising Method
-AUTHORS Marc Lebrun
-SRC http://www.ipol.im/pub/art/2012/l-bm3d/revisions/2021-02-20/bm3d_src.tar.gz
+NAME nlbayes
+TITLE Implementation of the "Non-Local Bayes" (NL-Bayes) Image Denoising Algorithm
+AUTHORS Marc Lebrun, Antoni Buades, Jean-Michel Morel
+SRC http://www.ipol.im/pub/art/2013/16/./revisions/2021-02-20/nl-bayes_20130617.tar.gz
 
+BUILD sed '/stdio/a#include <string.h>' -i Utilities/io_png.c  # missing header
 BUILD make
-BUILD cp BM3Ddenoising $BIN/bm3d
+BUILD cp NL_Bayes $BIN/nlbayes
 
 INPUT in image
 INPUT sigma number 10    # denoiser sigma
 OUTPUT out image
 
-# note: we call bm3d with default arguments and without any diagnostic output
-# note2: the documentation line of the revised BM3Ddenoising executable is
+# note: the documentation line of the revised source code executable is
 # wrong (the add-noise selector and the value of sigma being reversed)
-RUN bm3d $in $sigma 0 /dev/null /dev/null $out /dev/null /dev/null /dev/null 1 bior 0 dct 1 opp
+RUN nlbayes $in $sigma 0 /dev/null $out /dev/null /dev/null /dev/null ImBiasBasic /dev/null 1 0 1
```

### Comparing `clipol-5/idl/dctdenoise.Dockerfile` & `clipol-6/idl/dctdenoise.Dockerfile`

 * *Files identical despite different names*

### Comparing `clipol-5/idl/ffdnet.Dockerfile` & `clipol-6/idl/ffdnet.Dockerfile`

 * *Files identical despite different names*

### Comparing `clipol-5/idl/msdctd.Dockerfile` & `clipol-6/idl/msdctd.Dockerfile`

 * *Files identical despite different names*

### Comparing `clipol-5/ipol.py` & `clipol-6/ipol.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,18 +92,18 @@
 	singular_entries = ("NAME", "TITLE", "SRC", "AUTHORS")
 	linewise_entries = ("RUN", "BUILD")
 	keyed_sections = ("INPUT", "OUTPUT")
 
 	# parse the input file into the tree "p"
 	f = f if f.endswith(".Dockerfile") else f"{f}.Dockerfile"
 	for l in open(f, "r").read().split("\n"):
-		l = l.partition("#")[0].strip()    # remove comments
+		l = l.partition(" #")[0].strip()    # remove comments
 		if len(l) < 4: continue
 		k = l.partition(" ")[0]
-		v = l.partition(" ")[2]
+		v = l.partition(" ")[2].lstrip(" ")
 		if k in singular_entries:
 			p[k] = v
 		else:
 			p.setdefault(k,[]).append(v)
 
 	# turn the keyed sections intro key,value pairs
 	# the "key" is the ID of the parameter
@@ -636,10 +636,10 @@
 	idls = os.listdir(f"{IPOL_CONFIG}/idl")
 	idls = [ x[:-11] if x.endswith(".Dockerfile") else x for x in idls ]
 	for i in idls:
 		export_article_interface(i)
 
 
 # API
-version = 5
+version = 6
 
 # vim: sw=8 ts=8 sts=0 noexpandtab:
```

### Comparing `clipol-5/setup.py` & `clipol-6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def data_files():
 	import glob
 	return glob.glob("idl/*.Dockerfile")
 
 setuptools.setup(
 	name = "clipol",
-	version = "5",
+	version = "6",
 	author = "Enric Meinhardt-Llopis",
 	author_email = "enric.meinhardt@ens-paris-saclay.fr",
 	description = "python interface to some IPOL journal algorithms",
 	url = "https://git.sr.ht/~coco/clipol",
 	classifiers = [
 		"Operating System :: OS Independent",
 		"License :: OSI Approved :: GNU Affero General Public License v3",
```

