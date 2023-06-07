# Comparing `tmp/hlann-0.0.2-py3-none-any.whl.zip` & `tmp/hlann-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 88084 bytes, number of entries: 32
+Zip file size: 88046 bytes, number of entries: 32
 -rw-r--r--  2.0 unx    22757 b- defN 23-May-30 16:37 hlann/allotype.py
 -rw-r--r--  2.0 unx     6214 b- defN 23-Apr-11 20:16 hlann/allotype_match.py
 -rw-r--r--  2.0 unx     8971 b- defN 23-Apr-11 20:16 hlann/annotation.py
 -rw-r--r--  2.0 unx    51370 b- defN 23-May-30 16:17 hlann/dataset.py
 -rw-r--r--  2.0 unx     7260 b- defN 23-May-30 16:37 hlann/features.py
 -rw-r--r--  2.0 unx     2704 b- defN 23-Apr-11 20:16 hlann/gene_features.py
 -rw-r--r--  2.0 unx     2542 b- defN 23-Apr-11 20:16 hlann/gene_parser.py
@@ -23,12 +23,12 @@
 -rw-r--r--  2.0 unx    12920 b- defN 23-Apr-11 20:16 hlann/sequence.py
 -rw-r--r--  2.0 unx     2337 b- defN 23-May-30 16:37 hlann/sequence_feat_searched.py
 -rw-r--r--  2.0 unx     3452 b- defN 23-May-30 16:37 hlann/sequence_features.py
 -rw-r--r--  2.0 unx     5819 b- defN 23-May-30 16:37 hlann/sequence_match.py
 -rw-r--r--  2.0 unx    33474 b- defN 23-Jun-05 16:18 hlann/sequence_search.py
 -rw-r--r--  2.0 unx     5529 b- defN 23-May-30 16:37 hlann/snp.py
 -rw-r--r--  2.0 unx     3173 b- defN 23-Apr-11 20:16 hlann/util.py
--rw-r--r--  2.0 unx     9507 b- defN 23-Jun-07 19:13 hlann-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 19:13 hlann-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-07 19:13 hlann-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2485 b- defN 23-Jun-07 19:13 hlann-0.0.2.dist-info/RECORD
-32 files, 317790 bytes uncompressed, 84210 bytes compressed:  73.5%
+-rw-r--r--  2.0 unx     9387 b- defN 23-Jun-07 19:45 hlann-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 19:45 hlann-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-07 19:45 hlann-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2485 b- defN 23-Jun-07 19:45 hlann-0.0.3.dist-info/RECORD
+32 files, 317670 bytes uncompressed, 84172 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -78,20 +78,20 @@
 
 Filename: hlann/snp.py
 Comment: 
 
 Filename: hlann/util.py
 Comment: 
 
-Filename: hlann-0.0.2.dist-info/METADATA
+Filename: hlann-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: hlann-0.0.2.dist-info/WHEEL
+Filename: hlann-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: hlann-0.0.2.dist-info/top_level.txt
+Filename: hlann-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: hlann-0.0.2.dist-info/RECORD
+Filename: hlann-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `hlann-0.0.2.dist-info/METADATA` & `hlann-0.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlann
-Version: 0.0.2
+Version: 0.0.3
 Summary: HLA Annotation (HLAnn) Python package for annotating HLA
 Author: NMDP Bioinformatics
 Author-email: <rsajulga@nmdp.org>
 License: LGPL 3.0
 Keywords: hlann
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -26,24 +26,21 @@
 Requires-Dist: biopython (==1.77)
 Requires-Dist: click (<=8.0.4)
 Requires-Dist: connexion[swagger-ui] (>=2.12.0)
 Requires-Dist: editdistance (>=0.6.0)
 Requires-Dist: Flask-Cors (==3.0.10)
 Requires-Dist: inflect (==6.0.2)
 Requires-Dist: openpyxl (==3.0.10)
-Requires-Dist: matplotlib (==3.6.2)
 Requires-Dist: protobuf (==3.20.0)
 Requires-Dist: py-ard (==0.8.0)
 Requires-Dist: py2neo (==2021.0.1)
 Requires-Dist: PyHamcrest (==1.9.0)
 Requires-Dist: regex (==2022.3.2)
 Requires-Dist: SQLAlchemy (==1.4.41)
 Requires-Dist: SQLAlchemy-Utils (==0.38.3)
-Requires-Dist: streamlit (>=1.15.0)
-Requires-Dist: streamlit-aggrid (>=0.2.3.post2)
 
 # HLA Annotation Pipeline
 
 # Table of Contents
 - [Background](#background-)
 - [Tools](#tools-)
     - [Python Package](#python-package-)
```

## Comparing `hlann-0.0.2.dist-info/RECORD` & `hlann-0.0.3.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 hlann/sequence.py,sha256=1ZcslEmS0rumpd6Hy4eZcgE73vBEuGunv6ILSZ1nqGQ,12920
 hlann/sequence_feat_searched.py,sha256=Lm7HmC7dxEKGC6k-c0e3gvvWkFPuMxl_RIAplgeCQI4,2337
 hlann/sequence_features.py,sha256=CMRrdtvnj8C48EYFVC37Etd2BSHXbFo6qOBOECupiqc,3452
 hlann/sequence_match.py,sha256=VKwwaCTtBYkOwqaitcyDqQZq-P95I8JPfiK3EBpc3A4,5819
 hlann/sequence_search.py,sha256=SITOpWX6NRZ_bfeJ0KWsW1ze134S-QFSl7eaNB7sP3U,33474
 hlann/snp.py,sha256=WP2SmnSnKEp0QfSoEwNkRBtPW7KN4-oYIlUecj-H3Ok,5529
 hlann/util.py,sha256=Y42Ilr43G2AXxoDP7BbSr3lYx8VxwuPFYvSihZBAEU0,3173
-hlann-0.0.2.dist-info/METADATA,sha256=PLOpiMerYtDOUT7GWtHDn7_Gfp29naSRvECxlzSf940,9507
-hlann-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-hlann-0.0.2.dist-info/top_level.txt,sha256=jNc77jtAw0Hs775tbJXvzjqMWcLHqND-5rtumVJeREM,6
-hlann-0.0.2.dist-info/RECORD,,
+hlann-0.0.3.dist-info/METADATA,sha256=qjGzE14eRrb-Ba2bNGueqMGzjyo2Wjrge3VCXHwHEz0,9387
+hlann-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hlann-0.0.3.dist-info/top_level.txt,sha256=jNc77jtAw0Hs775tbJXvzjqMWcLHqND-5rtumVJeREM,6
+hlann-0.0.3.dist-info/RECORD,,
```

