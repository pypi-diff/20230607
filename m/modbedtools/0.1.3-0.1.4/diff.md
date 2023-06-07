# Comparing `tmp/modbedtools-0.1.3.tar.gz` & `tmp/modbedtools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modbedtools-0.1.3.tar", last modified: Fri May 19 14:59:00 2023, max compression
+gzip compressed data, was "modbedtools-0.1.4.tar", last modified: Wed Jun  7 04:31:37 2023, max compression
```

## Comparing `modbedtools-0.1.3.tar` & `modbedtools-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-05-19 14:59:00.850567 modbedtools-0.1.3/
--rw-r--r--   0 dli        (501) staff       (20)     1067 2023-01-18 19:28:55.000000 modbedtools-0.1.3/LICENSE
--rw-r--r--   0 dli        (501) staff       (20)     8637 2023-05-19 14:59:00.849970 modbedtools-0.1.3/PKG-INFO
--rw-r--r--   0 dli        (501) staff       (20)     8192 2023-05-19 14:57:30.000000 modbedtools-0.1.3/README.md
-drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-05-19 14:59:00.847374 modbedtools-0.1.3/modbed/
--rw-r--r--   0 dli        (501) staff       (20)        0 2023-01-18 19:31:33.000000 modbedtools-0.1.3/modbed/__init__.py
--rw-r--r--   0 dli        (501) staff       (20)     6620 2023-05-15 19:56:33.000000 modbedtools-0.1.3/modbed/modbed.py
--rw-r--r--   0 dli        (501) staff       (20)       22 2023-05-19 14:58:46.000000 modbedtools-0.1.3/modbed/version.py
--rwxr-xr-x   0 dli        (501) staff       (20)     3224 2023-05-13 03:59:08.000000 modbedtools-0.1.3/modbedtools
-drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-05-19 14:59:00.849464 modbedtools-0.1.3/modbedtools.egg-info/
--rw-r--r--   0 dli        (501) staff       (20)     8637 2023-05-19 14:59:00.000000 modbedtools-0.1.3/modbedtools.egg-info/PKG-INFO
--rw-r--r--   0 dli        (501) staff       (20)      266 2023-05-19 14:59:00.000000 modbedtools-0.1.3/modbedtools.egg-info/SOURCES.txt
--rw-r--r--   0 dli        (501) staff       (20)        1 2023-05-19 14:59:00.000000 modbedtools-0.1.3/modbedtools.egg-info/dependency_links.txt
--rw-r--r--   0 dli        (501) staff       (20)        6 2023-05-19 14:59:00.000000 modbedtools-0.1.3/modbedtools.egg-info/requires.txt
--rw-r--r--   0 dli        (501) staff       (20)        7 2023-05-19 14:59:00.000000 modbedtools-0.1.3/modbedtools.egg-info/top_level.txt
--rw-r--r--   0 dli        (501) staff       (20)       38 2023-05-19 14:59:00.850689 modbedtools-0.1.3/setup.cfg
--rw-r--r--   0 dli        (501) staff       (20)      771 2023-01-18 19:33:05.000000 modbedtools-0.1.3/setup.py
+drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-06-07 04:31:37.010157 modbedtools-0.1.4/
+-rw-r--r--   0 dli        (501) staff       (20)     1067 2023-01-18 19:28:55.000000 modbedtools-0.1.4/LICENSE
+-rw-r--r--   0 dli        (501) staff       (20)     8715 2023-06-07 04:31:37.009622 modbedtools-0.1.4/PKG-INFO
+-rw-r--r--   0 dli        (501) staff       (20)     8270 2023-06-06 19:11:20.000000 modbedtools-0.1.4/README.md
+drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-06-07 04:31:37.005105 modbedtools-0.1.4/modbed/
+-rw-r--r--   0 dli        (501) staff       (20)        0 2023-01-18 19:31:33.000000 modbedtools-0.1.4/modbed/__init__.py
+-rw-r--r--   0 dli        (501) staff       (20)     6715 2023-06-07 04:23:50.000000 modbedtools-0.1.4/modbed/modbed.py
+-rw-r--r--   0 dli        (501) staff       (20)       22 2023-06-07 04:27:13.000000 modbedtools-0.1.4/modbed/version.py
+-rwxr-xr-x   0 dli        (501) staff       (20)     3224 2023-05-13 03:59:08.000000 modbedtools-0.1.4/modbedtools
+drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-06-07 04:31:37.008826 modbedtools-0.1.4/modbedtools.egg-info/
+-rw-r--r--   0 dli        (501) staff       (20)     8715 2023-06-07 04:31:36.000000 modbedtools-0.1.4/modbedtools.egg-info/PKG-INFO
+-rw-r--r--   0 dli        (501) staff       (20)      266 2023-06-07 04:31:36.000000 modbedtools-0.1.4/modbedtools.egg-info/SOURCES.txt
+-rw-r--r--   0 dli        (501) staff       (20)        1 2023-06-07 04:31:36.000000 modbedtools-0.1.4/modbedtools.egg-info/dependency_links.txt
+-rw-r--r--   0 dli        (501) staff       (20)        6 2023-06-07 04:31:36.000000 modbedtools-0.1.4/modbedtools.egg-info/requires.txt
+-rw-r--r--   0 dli        (501) staff       (20)        7 2023-06-07 04:31:36.000000 modbedtools-0.1.4/modbedtools.egg-info/top_level.txt
+-rw-r--r--   0 dli        (501) staff       (20)       38 2023-06-07 04:31:37.010524 modbedtools-0.1.4/setup.cfg
+-rw-r--r--   0 dli        (501) staff       (20)      771 2023-01-18 19:33:05.000000 modbedtools-0.1.4/setup.py
```

### Comparing `modbedtools-0.1.3/LICENSE` & `modbedtools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modbedtools-0.1.3/PKG-INFO` & `modbedtools-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modbedtools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generate modbed track files for visualization on WashU Epigenome Browser
 Home-page: https://github.com/lidaof/modbedtools
 Author: Daofeng Li
 Author-email: lidaof@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,18 +25,18 @@
 ## installation
 
 Install through [pypi modbedtools project page](https://pypi.org/project/modbedtools/) (version number might change):
 
 ```sh
 $ pip install modbedtools
 Collecting modbedtools
-  Downloading modbedtools-0.1.0-py3-none-any.whl (6.8 kB)
+  Downloading modbedtools-0.1.3-py3-none-any.whl (8.8 kB)
 Requirement already satisfied: pysam in /opt/apps/python3/lib/python3.7/site-packages (from modbedtools) (0.19.1)
 Installing collected packages: modbedtools
-Successfully installed modbedtools-0.1.0
+Successfully installed modbedtools-0.1.3
 ```
 
 ## modbed format
 
 ```sh
 chr11   5173273 5195306 read_id score + -110,-266,-1459,-1780,-1840,-1842,-1848,-1865,-1928,-1936,... -396,-1543,-3222,-4195,-4319,-4692,-5352,-5366,-5523,-5838,...
 chr11   5174507 5194585 read_id score +  223,605,607,613,630,693,701,936,1761,3369,...  307,544,1280,2017,2859,2994,3116,3249,3790,3935,...
@@ -153,14 +153,16 @@
 
 Then the .gz and .gz.tbi files can be placed into any web server for hosting and the URL to the .gz file can be used for Visualization in [WashU Epigenome Browser](https://epigenomegateway.wustl.edu/).
 
 ## visualization
 
 In this tutorial, and we will use [hifi-test.modbed.gz](https://target.wustl.edu/dli/modbed/hifi-test.modbed.gz) for the next step by step tutorial.
 
+***(Please note this test data only contains methylation signal on chr11)***
+
 First we will go to the Browser by navigating your web browser to <https://epigenomegateway.wustl.edu/browser/>, click `hg38` for the genome.
 
 ![](https://github.com/lidaof/modbedtools/blob/main/img/m1.png?raw=true)
 
 In the test data, we will check methylation signal over *KDM2A* gene, we will use the gene search function, type in `KDM2A` and choose the first hit in refGene:
 
 ![](https://github.com/lidaof/modbedtools/blob/main/img/m2.png?raw=true)
```

### Comparing `modbedtools-0.1.3/README.md` & `modbedtools-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 ## installation
 
 Install through [pypi modbedtools project page](https://pypi.org/project/modbedtools/) (version number might change):
 
 ```sh
 $ pip install modbedtools
 Collecting modbedtools
-  Downloading modbedtools-0.1.0-py3-none-any.whl (6.8 kB)
+  Downloading modbedtools-0.1.3-py3-none-any.whl (8.8 kB)
 Requirement already satisfied: pysam in /opt/apps/python3/lib/python3.7/site-packages (from modbedtools) (0.19.1)
 Installing collected packages: modbedtools
-Successfully installed modbedtools-0.1.0
+Successfully installed modbedtools-0.1.3
 ```
 
 ## modbed format
 
 ```sh
 chr11   5173273 5195306 read_id score + -110,-266,-1459,-1780,-1840,-1842,-1848,-1865,-1928,-1936,... -396,-1543,-3222,-4195,-4319,-4692,-5352,-5366,-5523,-5838,...
 chr11   5174507 5194585 read_id score +  223,605,607,613,630,693,701,936,1761,3369,...  307,544,1280,2017,2859,2994,3116,3249,3790,3935,...
@@ -140,14 +140,16 @@
 
 Then the .gz and .gz.tbi files can be placed into any web server for hosting and the URL to the .gz file can be used for Visualization in [WashU Epigenome Browser](https://epigenomegateway.wustl.edu/).
 
 ## visualization
 
 In this tutorial, and we will use [hifi-test.modbed.gz](https://target.wustl.edu/dli/modbed/hifi-test.modbed.gz) for the next step by step tutorial.
 
+***(Please note this test data only contains methylation signal on chr11)***
+
 First we will go to the Browser by navigating your web browser to <https://epigenomegateway.wustl.edu/browser/>, click `hg38` for the genome.
 
 ![](https://github.com/lidaof/modbedtools/blob/main/img/m1.png?raw=true)
 
 In the test data, we will check methylation signal over *KDM2A* gene, we will use the gene search function, type in `KDM2A` and choose the first hit in refGene:
 
 ![](https://github.com/lidaof/modbedtools/blob/main/img/m2.png?raw=true)
```

### Comparing `modbedtools-0.1.3/modbed/modbed.py` & `modbedtools-0.1.4/modbed/modbed.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,23 +64,27 @@
                 modbase_unmet_string]
         return line
     else:
         return []
 
 
 def bam2mod(bamfile, outfile, cutoff=0.5, base='C', cpg=False):
-    bam = pysam.AlignmentFile(bamfile, 'rb', check_sq=False)
+    # remove 'rb' mode for auto-detect
+    bam = pysam.AlignmentFile(bamfile, check_sq=False)
+    hasIndex = False
     if os.path.exists(bamfile+'.bai'):
+        hasIndex = True
         num_reads = bam.count()  # this needs index
         print(f'[info] total reads: {num_reads}', file=sys.stderr)
     cpgtag = '.cpg' if cpg else ''
     outf = f'{outfile}{cpgtag}.modbed'
     print(f'[info] writing file {outf}', file=sys.stderr)
     with open(outf, "w") as out:
-        for read in bam.fetch(until_eof=True):  # this makes bam index optional
+        # this makes bam index optional
+        for read in bam.fetch(until_eof=(not hasIndex)):
             items = process_read(read, cutoff, base, cpg)
             if len(items):
                 # for output, need either has modified base or unmodified base
                 if items[3] != '.' or items[4] != '.':
                     line = '\t'.join(items)
                     out.write(line+'\n')
```

### Comparing `modbedtools-0.1.3/modbedtools` & `modbedtools-0.1.4/modbedtools`

 * *Files identical despite different names*

### Comparing `modbedtools-0.1.3/modbedtools.egg-info/PKG-INFO` & `modbedtools-0.1.4/modbedtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modbedtools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generate modbed track files for visualization on WashU Epigenome Browser
 Home-page: https://github.com/lidaof/modbedtools
 Author: Daofeng Li
 Author-email: lidaof@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,18 +25,18 @@
 ## installation
 
 Install through [pypi modbedtools project page](https://pypi.org/project/modbedtools/) (version number might change):
 
 ```sh
 $ pip install modbedtools
 Collecting modbedtools
-  Downloading modbedtools-0.1.0-py3-none-any.whl (6.8 kB)
+  Downloading modbedtools-0.1.3-py3-none-any.whl (8.8 kB)
 Requirement already satisfied: pysam in /opt/apps/python3/lib/python3.7/site-packages (from modbedtools) (0.19.1)
 Installing collected packages: modbedtools
-Successfully installed modbedtools-0.1.0
+Successfully installed modbedtools-0.1.3
 ```
 
 ## modbed format
 
 ```sh
 chr11   5173273 5195306 read_id score + -110,-266,-1459,-1780,-1840,-1842,-1848,-1865,-1928,-1936,... -396,-1543,-3222,-4195,-4319,-4692,-5352,-5366,-5523,-5838,...
 chr11   5174507 5194585 read_id score +  223,605,607,613,630,693,701,936,1761,3369,...  307,544,1280,2017,2859,2994,3116,3249,3790,3935,...
@@ -153,14 +153,16 @@
 
 Then the .gz and .gz.tbi files can be placed into any web server for hosting and the URL to the .gz file can be used for Visualization in [WashU Epigenome Browser](https://epigenomegateway.wustl.edu/).
 
 ## visualization
 
 In this tutorial, and we will use [hifi-test.modbed.gz](https://target.wustl.edu/dli/modbed/hifi-test.modbed.gz) for the next step by step tutorial.
 
+***(Please note this test data only contains methylation signal on chr11)***
+
 First we will go to the Browser by navigating your web browser to <https://epigenomegateway.wustl.edu/browser/>, click `hg38` for the genome.
 
 ![](https://github.com/lidaof/modbedtools/blob/main/img/m1.png?raw=true)
 
 In the test data, we will check methylation signal over *KDM2A* gene, we will use the gene search function, type in `KDM2A` and choose the first hit in refGene:
 
 ![](https://github.com/lidaof/modbedtools/blob/main/img/m2.png?raw=true)
```

### Comparing `modbedtools-0.1.3/setup.py` & `modbedtools-0.1.4/setup.py`

 * *Files identical despite different names*

