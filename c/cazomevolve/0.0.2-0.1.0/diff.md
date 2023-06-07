# Comparing `tmp/cazomevolve-0.0.2.tar.gz` & `tmp/cazomevolve-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cazomevolve-0.0.2.tar", last modified: Thu Feb 23 10:34:38 2023, max compression
+gzip compressed data, was "cazomevolve-0.1.0.tar", last modified: Wed Jun  7 08:51:12 2023, max compression
```

## Comparing `cazomevolve-0.0.2.tar` & `cazomevolve-0.1.0.tar`

### file list

```diff
@@ -1,40 +1,69 @@
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-02-23 10:34:38.902732 cazomevolve-0.0.2/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1067 2023-02-07 13:59:17.000000 cazomevolve-0.0.2/LICENSE
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    23987 2023-02-23 10:34:38.902732 cazomevolve-0.0.2/PKG-INFO
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    23222 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/README.md
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-02-23 10:34:38.898732 cazomevolve-0.0.2/cazomevolve/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2065 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/cazomevolve/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-02-23 10:34:38.898732 cazomevolve-0.0.2/cazomevolve/cazome/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1517 2023-02-07 13:59:17.000000 cazomevolve-0.0.2/cazomevolve/cazome/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-02-23 10:34:38.898732 cazomevolve-0.0.2/cazomevolve/cazome/cazy/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.0.2/cazomevolve/cazome/cazy/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7708 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/cazomevolve/cazome/cazy/get_cazy_cazymes.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-02-23 10:34:38.898732 cazomevolve-0.0.2/cazomevolve/cazome/dbcan/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.0.2/cazomevolve/cazome/dbcan/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6487 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4308 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/cazomevolve/cazome/dbcan/invoke_dbcan.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-02-23 10:34:38.902732 cazomevolve-0.0.2/cazomevolve/cazome/explore/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1526 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/cazomevolve/cazome/explore/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7089 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/cazomevolve/cazome/explore/cazome_sizes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8669 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/cazomevolve/cazome/explore/identify_families.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8302 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/cazomevolve/cazome/explore/parse_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11754 2023-02-23 10:32:15.000000 cazomevolve-0.0.2/cazomevolve/cazome/explore/pca.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3181 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/cazomevolve/cazome/explore/plot.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6041 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/cazomevolve/cazome/explore/taxonomies.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-02-23 10:34:38.902732 cazomevolve-0.0.2/cazomevolve/genomes/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1540 2023-02-07 13:59:17.000000 cazomevolve-0.0.2/cazomevolve/genomes/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2255 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/cazomevolve/genomes/download_acc_genomes.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11667 2023-02-21 11:07:12.000000 cazomevolve-0.0.2/cazomevolve/genomes/download_genomes.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-02-23 10:34:38.902732 cazomevolve-0.0.2/cazomevolve/seq_diversity/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1787 2023-02-07 13:59:17.000000 cazomevolve-0.0.2/cazomevolve/seq_diversity/get_fam_seqs.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1624 2023-02-07 13:59:17.000000 cazomevolve-0.0.2/cazomevolve/seq_diversity/run_blastp.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1837 2023-02-07 13:59:17.000000 cazomevolve-0.0.2/cazomevolve/seq_diversity/run_diamond.sh
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-02-23 10:34:38.898732 cazomevolve-0.0.2/cazomevolve.egg-info/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    23987 2023-02-23 10:34:38.000000 cazomevolve-0.0.2/cazomevolve.egg-info/PKG-INFO
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1017 2023-02-23 10:34:38.000000 cazomevolve-0.0.2/cazomevolve.egg-info/SOURCES.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)        1 2023-02-23 10:34:38.000000 cazomevolve-0.0.2/cazomevolve.egg-info/dependency_links.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)      302 2023-02-23 10:34:38.000000 cazomevolve-0.0.2/cazomevolve.egg-info/entry_points.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       87 2023-02-23 10:34:38.000000 cazomevolve-0.0.2/cazomevolve.egg-info/requires.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       12 2023-02-23 10:34:38.000000 cazomevolve-0.0.2/cazomevolve.egg-info/top_level.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       38 2023-02-23 10:34:38.902732 cazomevolve-0.0.2/setup.cfg
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3673 2023-02-23 10:08:21.000000 cazomevolve-0.0.2/setup.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.643525 cazomevolve-0.1.0/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1067 2023-02-07 13:59:17.000000 cazomevolve-0.1.0/LICENSE
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    31182 2023-06-07 08:51:12.643525 cazomevolve-0.1.0/PKG-INFO
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    30417 2023-06-07 08:48:37.000000 cazomevolve-0.1.0/README.md
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.631525 cazomevolve-0.1.0/cazomevolve/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2094 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.635525 cazomevolve-0.1.0/cazomevolve/cazome/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1517 2023-02-07 13:59:17.000000 cazomevolve-0.1.0/cazomevolve/cazome/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.635525 cazomevolve-0.1.0/cazomevolve/cazome/cazy/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.1.0/cazomevolve/cazome/cazy/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1568 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/cazy/build_db.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6916 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/cazy/get_cazy_cazymes.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.635525 cazomevolve-0.1.0/cazomevolve/cazome/dbcan/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.1.0/cazomevolve/cazome/dbcan/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6148 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4375 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/dbcan/invoke_dbcan.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.639525 cazomevolve-0.1.0/cazomevolve/cazome/explore/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1527 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    17139 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/cazome_sizes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6409 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/cazy_classes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    16877 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/cazy_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    19882 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/cooccurring_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8670 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/identify_families.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3750 2023-05-18 10:26:39.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/ie_cazymes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11913 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/parse_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    17003 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/pca.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3181 2023-02-21 11:07:12.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/plot.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6041 2023-02-21 11:07:12.000000 cazomevolve-0.1.0/cazomevolve/cazome/explore/taxonomies.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.639525 cazomevolve-0.1.0/cazomevolve/genomes/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1540 2023-02-07 13:59:17.000000 cazomevolve-0.1.0/cazomevolve/genomes/__init__.py
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2382 2023-06-07 08:39:51.000000 cazomevolve-0.1.0/cazomevolve/genomes/download_acc_genomes.sh
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)    11257 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/genomes/download_genomes.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.639525 cazomevolve-0.1.0/cazomevolve/scripts/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1492 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1713 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/build_cazy_db.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2462 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/cazomevolve_script.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3130 2023-06-07 08:41:03.000000 cazomevolve-0.1.0/cazomevolve/scripts/download_acc_genomes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3063 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/get_fam_seqs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2064 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/run_fam_blast.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1969 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/run_fam_diamond.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.631525 cazomevolve-0.1.0/cazomevolve/scripts/tree/
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.639525 cazomevolve-0.1.0/cazomevolve/scripts/tree/ani/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2123 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/ani/build_anim_tree.R
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1123 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/ani/run_anim.sh
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.643525 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1863 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/align_scos.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1928 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/annotate_genomes.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1927 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/backtranslate.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6330 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/concatenate_cds.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5189 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/extract_cds.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1718 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/find_orthologues.sh
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2073 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.643525 cazomevolve-0.1.0/cazomevolve/seq_diversity/
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1790 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/seq_diversity/get_fam_seqs.sh
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1724 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/seq_diversity/run_blastp.sh
+-rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2036 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/seq_diversity/run_diamond.sh
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.643525 cazomevolve-0.1.0/cazomevolve/taxs/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1513 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/taxs/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11563 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/taxs/add_taxs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6982 2023-06-06 17:06:20.000000 cazomevolve-0.1.0/cazomevolve/taxs/ncbi.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-06-07 08:51:12.635525 cazomevolve-0.1.0/cazomevolve.egg-info/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    31182 2023-06-07 08:51:12.000000 cazomevolve-0.1.0/cazomevolve.egg-info/PKG-INFO
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2015 2023-06-07 08:51:12.000000 cazomevolve-0.1.0/cazomevolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)        1 2023-06-07 08:51:12.000000 cazomevolve-0.1.0/cazomevolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       76 2023-06-07 08:51:12.000000 cazomevolve-0.1.0/cazomevolve.egg-info/entry_points.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)      154 2023-06-07 08:51:12.000000 cazomevolve-0.1.0/cazomevolve.egg-info/requires.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       12 2023-06-07 08:51:12.000000 cazomevolve-0.1.0/cazomevolve.egg-info/top_level.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       38 2023-06-07 08:51:12.643525 cazomevolve-0.1.0/setup.cfg
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4127 2023-06-07 08:50:54.000000 cazomevolve-0.1.0/setup.py
```

### Comparing `cazomevolve-0.0.2/LICENSE` & `cazomevolve-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.0.2/PKG-INFO` & `cazomevolve-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,155 +1,269 @@
-Metadata-Version: 2.1
-Name: cazomevolve
-Version: 0.0.2
-Summary: A bioinforamtic package for investigating the evolution of CAZomes
-Author: Emma E. M. Hobbs
-Author-email: eemh1@st-andrews.ac.uk
-License: MIT
-Keywords: bioinforamtics protein
-Platform: Posix
-Platform: MacOS X
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cazomevolve
 
+[![DOI](https://zenodo.org/badge/367898306.svg)](https://zenodo.org/badge/latestdoi/367898306)
+[![Documentation Status](https://readthedocs.org/projects/cazomevolve/badge/?version=latest)](https://cazomevolve.readthedocs.io/en/latest/?badge=latest)
 [![Funding](https://img.shields.io/badge/Funding-EASTBio-blue)](http://www.eastscotbiodtp.ac.uk/)
 [![PhD licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/PhD_Project_Scripts/blob/master/LICENSE)
 ![Python](https://img.shields.io/badge/Python-v3.9.---orange)
 ![Research](https://img.shields.io/badge/Research-Bioinformatics-ff69b4)
 
-**Cazome** **Evolve** (`cazomevolve`) invetigates the evolution of CAZomes by:
-* searching for CAZy families that associated more than expected from their lineage
-* projecting the CAZome composition onto a plot
-* building a dendogram using distances calculated from the CAZome composition 
+`cazomevolve` ('cazome-evolve') is an application and Python3 package for the automated annotation and exploratory analysis of CAZyme complements (CAZomes) for a set of species and/or genomes of interest. Carbohydrate Active enZymes are a subset of proteins that generate, modify and/or degrade carbohydrates. CAZy (www.cazy.org) is the most comprehensive CAZyme database, grouping proteins by sequence similarity into CAZy families.
 
-This repo houses all scripts required for calculating, exploring and visually representing the covariance of CAZy family annotations within genomic assemblies.
+Use `cazomevolve` to explore:
 
-## Contents
+**CAZome sizes:**
+* Compare the number of CAZymes and CAZy families
+* Calculate the proportion of the proteome encompassed by the CAZome
+* Compute the CAZy family to CAZyme ratio
+
+**CAZy class frequencies:**
+* Calculate the number of CAZymes per CAZy class
+* Plot a proportional area plot of CAZy class frequency broken down by CAZy class and user defined group deliniations (e.g. by genus or species)
+
+**CAZy families:**
+* Explore **sequence diversity** within a set of CAZy families:
+  * Run all-vs-all sequence comparison analyses
+  * Cluster the sequences by degree of sequence similarity
+  * Generate clustermaps of sequence identity, BLAST-score ratio, and coverage
+* Explore **CAZy family frequencies**:
+  * Compute the number of CAZymes per CAZy family
+  * Identify **lineage or group specific families** - e.g. genus or species specific families
+  * Identify **core CAZomes** - families that appear in all genomes
+  * Cluster genomes by CAZy family frequencies using **hierarchical clustering:**
+    * Generate annotated clustermaps of CAZy family frequencies
+    * Build a dendogram using distances calculated from the CAZome composition
+    * Construct tanglegrams to compare CAZy family dendrogram to a ANI-dendrogram or phylogenetic tree
+
+**Always co-occurring families:**
+* Identity CAZy families that are always present in the CAZome together
+* Find lineage or group specific groups of co-occurring families 
+* Construct an upset plot of co-occurring families
+* Calculate the number of genomes each group of co-occurring families appear in
+
+**Principal component analysis (PCA):**
+* Use PCA to idenify overal trends in the large and complex data set
+* Project genomes onto use selected principal components (PCs)
+* Construct loadings plots to explore correlation between CAZy families and PCs
+* Identify relationships between groups of CAZy families
+* Explore associations between CAZy families and lineage, phenotype, and niche adaptation
+
+**Co-evolving CAZy families:**
+* Generate the input file tab delimited list of genomes and CAZy families required by [`coinfinder`]() (Whelan _et al._)
+* Optionally add taxonomic data to the tab delimited list, to include taxa in the `coinfinder` output
+* Reconstruct phylogenetic trees to be used as input by `coinfinder`:
+  * Reconstruct a multi-gene phylogenetic tree using [`RaxML-ng`]()
+  * Construct an ANI-based dendrogram
+* Use `coinfinder` to identify CAZy families that appear together in a genome **more often than expected by lienage and chance**
+
+> Kozlov AM, Darriba D, Flouri T, Morel B, Stamatakis A. RAxML-NG: a fast, scalable and user-friendly tool for maximum likelihood phylogenetic inference. Bioinformatics. 2019 Nov 1;35(21):4453-4455. doi: 10.1093/bioinformatics/btz305.
+> Whelan FJ, Rusilowicz M, McInerney JO. Coinfinder: detecting significant associations and dissociations in pangenomes. Microb Genom. 2020 Mar;6(3):e000338. doi: 10.1099/mgen.0.000338. Epub 2020 Feb 24.
 
-1. [Overview](#Overview)
-2. [Installation](#Installation)
-    - [Requirements](#Requirements)
-3. [Current Developments](#Current)
-3. [Directories](#Directories)
-        
-## Overview
-
-Carbohydrate Active enZymes are a subset of proteins that generate, modify and/or degrade carbohydrates. CAZy (www.cazy.org) is the most comprehensive CAZyme database, grouping proteins by sequence similarity into CAZy families. **C**azy **F**amily co**V**ariance **investigator** (`cfv_investigator`) investigates the covariance of CAZy family annotations within proteomes across all species annotated by CAZy, and evaluates taxonomic specific covaraince of CAZy families.
-
-`cazomevolve` is a bioinformatic package (still in development) for:
-1. Retrieving of genomic accessions from which proteins catalogued within CAZy are derived from, and the associated taxonomic data of the source organism
-2. Tracking frequency of CAZy family annotations for all genomic assemblies identified in step 1
-3. Calculation of covariance of CAZy family annotations across all genomic assemblies identified in step 1, and for taxonomic specific groups (at the kingdom, genus and species taxonomic level)
-4. Generating dataframes of the number of CAZymes per CAZy family for each genomic assembly
-5. Generating a presence/absence matrix for each CAZy family in each genomic assembly
+## Documentation
 
-<p>&nbsp;</p>
+`cazomevolve` uses bash-script based workflow management. A summary of this workflow is provided in this README.
+
+Please see the [full documeentation including tutorials at ReadTheDocs]().
+
+An analysis using `cazomevolve` can be found [here](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto), which includes a README-walkthrough and all output files.
+
+## Contents
+
+1. [cazomevolve](#cazomevolve)
+2. [Documentation](#documentation)
+3. [Installation](#installation)
 
 ## Installation
 
+### PyPi
+
+The easiest way to install `cazomeolve` is via PyPi
+
+```bash
+pip install cazomevolve
+```
+
+### From source
+
 1. Create a virtual environment with dependencies, then activate the environment - _where venv_name is an chosen name for the virtual environment_
-`conda create -n <venv_name> python=3.9`   
-`conda activate <venv_name>`
+```bash
+conda create -n cazomevolve python=3.9
+conda activate cazomevolve
+```
 
 2. Clone the repository
-`git clone https://github.com/HobnobMancer/cazomevolve.git`
-
-3. Install pyrewton
-`pip3 install -e <path to directory containing setup.py file>`   
-Do not forget to use the **-e** option when install using pip3, otherwise each time pyrewton is invoked a ModuleNotFound error will be raised. Pass the path to the **directory** containign the setup.py file not the path to the setup.py file; if you are currently in the root directory of the repoistory where the file is located, simply use '.' to indicate the current working directory.
+```bash
+git clone https://github.com/HobnobMancer/cazomevolve.git
+pip install cazomevolve/.
+```
 
 <p>&nbsp;</p>
 
 ## Requirements
 
+### Essential
+
 POISx or Mac OS, or linux emulator   
-Python version 3.8+   
+Python version 3.8+
 Miniconda3 or Anaconda managed microenvironment, incorporated code checkers are included in list form in 'requirements.txt'.   
 Miniconda3 environment file is also available in the GitHub repository: 'environment.yml'.   
 For all required Python libraries please read 'requirements.txt'. 
 
-* [`ncbi-genome-download`](https://github.com/kblin/ncbi-genome-download/)
+The following packages are required by the core `cazomevolve` application, and their installation is handled by the `setup.py` file:
+* [`adjustText`](https://adjusttext.readthedocs.io/en/latest/)
+* [`biopython`](https://biopython.org/)
+* [`cazy_webscraper`](https://github.com/HobnobMancer/cazy_webscraper)
+* [`jupyter](https://jupyter.org/)
+* [`ncbi-genome-download`](https://pypi.org/project/ncbi-genome-download/)
+* [`numpy`](https://numpy.org/)
+* [`pandas`](https://pandas.pydata.org/)
 * [`saintBioutils`](https://github.com/HobnobMancer/saintBioutils)
+* [`seaborn`](https://seaborn.pydata.org/)
+* [`sklearn`](https://scikit-learn.org/stable/index.html) / `scikit-learn`
+* [`tqdm`](https://pypi.org/project/tqdm/)
+* [`upsetplot`](https://pypi.org/project/UpSetPlot/)
+
+### Optional
+
+The following packages are optional can installation instructions can be found in their respective repositories:
+
+**dbCAN:**
+
+To expand the data set beyond those CAZomes only listed in CAZy (**highly recommended!**) `dbCAN` must also be installed.
+
+Note: _`dbCAN` and `cazomevolve` can be installed in the same or separate virtual environments._
+
+**dbCAN version 3 and 4:**
+The CAZyme classifier `dbCAN` versions >= 3.0.6 can be installed via Conda (recommended). The full installation instructions are found [here](https://github.com/linnabrown/run_dbcan/tree/c9bad4835b2bc1a9685d693237f1d6a9d56ff3a1), and must be followed to ensure all additional database files are downloaded and compiled correctly.
+
+**dbCAN version 2:**
+The installation instructions for dbCAN v==2.0.11 can be found [here](https://github.com/linnabrown/run_dbcan/tree/fde6d7225441ef3d4cb29ea29e39cfdcc41d8b19).
 
-<p>&nbsp;</p>
 
+**`coinfinder`: Identify CAZy families that co-occurr more often than expected by lineage and chance:**
+* [`coinfinder`](https://github.com/fwhelan/coinfinder) >= v1.2.0
 
+Note: _`coinfinder` requires Python v3.6, we recommend installing and running `coinfinder` in a separate venv to `cazomevolve`
+
+**Construct an ANI-based dendrogram:**
+* [`pyani`](https://github.com/widdowquinn/pyani) >= version 0.3.0-alpha
+* [`R`](https://www.r-project.org/)
+
+**Reconstruct a multi-gene phylogenetic tree:**
+* [`MAFFT`](https://mafft.cbrc.jp/alignment/software/)
+* [`Orthofinder`](https://github.com/davidemms/OrthoFinder)
+* [`Prodigal`](https://github.com/hyattpd/Prodigal)
+* [`RaxML-ng`](https://github.com/amkozlov/raxml-ng)
+* [`T-coffee`](https://tcoffee.crg.eu/)
+
+<p>&nbsp;</p>
 
 # Method
 
-# Explore sequence diversity in CAZy families
+## Construct a local CAZyme database
+
+Download all CAZyme records from CAZy, and compile the records into a local SQLite3 database using `cazy_webscraper`:
+```bash
+cazy_webscraper <user-email-address> -o <desired-path-for-db>
+```
+
+## Explore sequence diversity in CAZy families
 
 Presuming a local CAZyme database has already been generated using `cazy_webscraper`:
 
-1. Generate a multisequence FASTA file for each CAZy family of interest using the bash script `get_fam_seqs.sh`, which 
-takes 4 positional arguments:
+1. Generate a multisequence FASTA file for each CAZy family of interest using the bash script `get_fam_seqs.sh`, which takes 4 positional arguments:
 
 * email address
 * path to a local cazyme db
 * name(s) of families of interest (separate with a single comma)
 * path to an output dir (do not include terminal /)
 
+```bash
+cazomevolve get_fam_seqs \
+  <email> \
+  <cazy_db> \
+  <fam1,fam2,fam3> \
+  <path to outdir>
+```
+
+* The output dir will be created by `cazy_webscraper` - it will not delete exsiting content in the outdir unless their is a FASTA file with the same name
+* Creates one output FASTA file per CAZy family
+
 Or use `cazy_webscraper` directly to create a multisequence FASTA file containing the protein sequences of interst
 
-2. Run all-vs-all sequence analysis for each multisequence FASTA file. Use the `run_blastp.sh` script to use BLASTP+ or the `run_diamond.sh` script to use DIAMOND (recommend for large families of >1000 proteins sequences)
+## Run all-vs-all analysis
+
+Run all-vs-all sequence analysis for each multisequence FASTA file, using BLAST or DIAMOND (recommend for large families of >1000 proteins sequences).
+
+The output directories will be created by `cazomevolve` - existing data in the existing output directories will **not** be deleted.
 
-`run_blastp.sh` takes 2 positional arguments:
+**Using BLASTP:**
+Use the `run_fam_blast` subcommand, which takes 2 positional arguments:
 * Path to the input FASTA file
 * Path for the output TSV file
 
-`run_diamond.sh` takes 3 positional arguments:
+```bash
+cazomevolve run_fam_blast \
+  <input fasta file> \
+  <output TSV file> 
+```
+
+**Using DIAMOND: (recommended for large datasets):**
+Use the `run_fam_diamond` subcommand, which takes 3 positional arguments:
 * Path to the input FASTA file
-* Path to build the DIAMOND database at
-* Path for the output TSV file
+* Path where to create a diamond db 
+* Path to write out output matrix
+
+```bash
+cazomevolve run_fam_diamond \
+  <input fasta file> \
+  <diamond db path> \
+  <output TSV file> 
+```
 
-Both scripts are located in `cazomevolve/seq_diversity/` directory.
+## Visualise the sequence diversity
 
-3. Visualise the results using the `jupyter notebook` template located at `cazomevolve/seq_diversity/explore_seq_diversity.ipynb`. This generates clustermaps and heatmaps that plot the proteins in the same order as the generated clustermap.
+Visualise the results using the `jupyter notebook` template located at `cazomevolve/seq_diversity/explore_seq_diversity.ipynb`. This generates clustermaps and heatmaps that plot the proteins in the same order as the generated clustermap.
+
+All functions used in the notebook are available, and can be imported from, `cazomevolve`, specifically the module `cazomevolve.seq_diversity.explore`.
 
 We recommend using the [BLAST Score Ratio (BSR)](https://widdowquinn.github.io/2018-03-06-ibioic/02-sequence_databases/05-blast_for_rbh.html#Normalised-bit-score,-and-coverage) to generate a clustermap, then generate heatmaps of the percentage identity (pident) and query coverage (qcov) so the proteins are plotted in the same order for the 3 plots and thus facilitates comparing between the three.
 
 Optionally, redundant protein sequences can be removed, and proteins of interest (mannually defined by the user) and functionally/structurally characterised proteins can be annotated on the plots, to facilitate identifying the degree of characterisation across a family.
 
-# Download genomes
+<p>&nbsp;</p>
+<p>&nbsp;</p>
+
+# Annotate the CAZome
+
+## Download genomes
 
-To download the genomic assemblies, use either method [A] or [B]
+The genomes to be download can be specified by [A] their genomic accessions, or [B] by specifying a taxa of interest (using a taxa of any level).
 
-## [A] Already have a list of genomic version accessions
+### [A] Genomic accessions
 
-If you already have a list of genomic version accessions in a plain text file, using the Python package `ncbi-genome-download` to download the genomic assemblies genomic (`.fna`) and proteome (`.faa`) sequence files.
+If you have a list of genomic version accessions in a plain text file, `cazomevolve` can use the Python package `ncbi-genome-download` to download the genomic assemblies genomic (`.fna`) and proteome (`.faa`) sequence files.
 
-The `cazevolve_download_acc_genomes` configures using `ncbi-genome-download`. The command takes 4 positional arguments and 1 optional argument:
+Using the `download_acc_genomes` subcommand, which takes 4 positional arguments and 1 optional argument:
 
 **Positional arguments:**
 1. Path to file containing list of accessions (with a unique genome accession per row)
 2. Path to output directory (will be created by `cazevolve_download_acc_genomes`)
 3. File options - a comma-separated list, e.g. "fasta,assembly-report": Choose from: ['genbank', 'fasta', 'rm', 'features', 'gff', 'protein-fasta', 'genpept', 'wgs', 'cds-fasta', 'rna-fna', 'rna-fasta', 'assembly-report', 'assembly-stats', 'all']
 4. Download Refseq ('refseq') or GenBank ('genbank') assemblies
 
 **Optional arguments:**
 1. Assembly level. Default 'all'. Comma separated list. Choose from: ['all', 'complete', 'chromosome', 'scaffold', 'contig']
 
-**Download the genomes in `.fna` and `faa` format.**
+**Downloads the genomes in `.fna` and `faa` format.**
 
-## [B] Retrieve all genomic assemblies associated with a specific term
+### [B] Taxa
 
-To download load all genomic assemblies associated with a term of interest, such as `Pectobacteriaceae` (so as to download all Pectobacteriaceae assemblies), use the command`cazevolve_download_genomes`.
+To download load all genomic assemblies associated with a term of interest, such as `Pectobacteriaceae` (so as to download all Pectobacteriaceae assemblies), use the subcommand `download_genomes`, which takes 4 arguments:
 
-**The command takes 4 requires arguments:**
 1. User email address (required by NCBI)
 2. The terms of interest. Comma-separated list, e.g. 'Pectobacterium,Dickeya'
 3. The file formats to download the genomic assemblies in. ['genomic' - downloads genomic.fna seq files, 'protein' - downloads protein.faa seq files]"
 4. Path to an output directory (this will be built by `cazomevolve`).
 
 By default if the output directory exists, `cazomevolve` will crash. To write to an existing output directory use the `-f`/`--force` flag. By default, `cazomevolve` will delete all existing data in the existing output directory. To retain the data available in the existing output directory use the `-n`/`--nodelete` flag.
 
@@ -162,42 +276,50 @@
 ``-f``, ``--force`` - Force file over writting (default: False)
 ``-l - log file name, --log log file name
                         Defines log file name and/or path (default: None)
 ``-n``, ``--nodelete`` - enable/disable deletion of exisiting files (default: False)
 ``--timeout`` TIMEOUT - time in seconds before connection times out (default: 30)
 ``-v``, ``--verbose`` - Set logger level to 'INFO' (default: False)
 
-# Annotate CAZomes
+## Annotate CAZomes
 
-To retrieve the most comprehensive annotation of the CAZome, the (widely considered) canonical classifications from CAZy retrieved using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) (Hobbs _et al.,_ 2022), combined with predicted CAZy family annotations from [`dbCAN`](https://github.com/linnabrown/run_dbcan) (Zhang _et al._ 2018).
+To retrieve the most comprehensive annotation of the CAZome, we recommend using the (widely considered) canonical classifications from CAZy retrieved using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) (Hobbs _et al.,_ 2022), combined with predicted CAZy family annotations from [`dbCAN`](https://github.com/linnabrown/run_dbcan) (Zhang _et al._ 2018).
 
 > Emma E. M. Hobbs, Tracey M. Gloster, Leighton Pritchard; cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets, BioRxiv, 3 December 2022, https://doi.org/10.1101/2022.12.02.518825
 
 > Han Zhang, Tanner Yohe, Le Huang, Sarah Entwistle, Peizhi Wu, Zhenglu Yang, Peter K Busk, Ying Xu, Yanbin Yin; dbCAN2: a meta server for automated carbohydrate-active enzyme annotation, Nucleic Acids Research, Volume 46, Issue W1, 2 July 2018, Pages W95–W101, https://doi.org/10.1093/nar/gky418
 
 ## Build a local CAZyme database using `cazy_webscraper`
 
 To include 'canonical' CAZy family classifications from CAZy, download all data from the CAZy database and compile the data into a local CAZyme database using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) (Hobbs _et al., 2022).
 
 > cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets
 Emma E. M. Hobbs, Tracey M. Gloster, Leighton Pritchard
 bioRxiv 2022.12.02.518825; doi: https://doi.org/10.1101/2022.12.02.518825
 
+The `cazomevolve` subcommand `build_cazy_db` to coordinate uisng `cazy_webscraper`:
+```bash
+cazomevolve build_cazy_db \
+  <email> \
+  <desired db path>
+```
+
+Or you can use `cazy_webscraper` directly
 ```bash
 cazy_webscraper \
     <email> \
     -o <db file output path>
 ```
 
 ## Retrieve CAZy annotations
 
-Use `cazomevolve` to query the protein version accessions in the downloaded protein FASTA files against the local CAZyme db, to retrieve the 'canonical' CAZy family classifications, using the `cazevolve_get_cazy_cazymes` command.
+The `get_cazy_cazymes` subcommand to coordinate `cazomevolve` to query the protein version accessions in the downloaded protein FASTA files against the local CAZyme db, to retrieve the 'canonical' CAZy family classifications:
 
 ```bash
-cazevolve_get_cazy_cazymes \
+cazomevolve get_cazy_cazymes \
     <path to dir containing protein FASTA files> \
     <path to local cazyme database> \
     <path to dir to write out protein sequences NOT in the local db> \
     <path to write out tab delimited lists of CAZy families and genomic accessions> \
     <path to write out tab delimited lists of CAZy families, genomic accessions and protein accessions> \
 ```
 
@@ -227,41 +349,44 @@
   -n, --nodelete        enable/disable deletion of exisiting files (default: False)
   --sql_echo            Set verbose SQLite3 logging (default: False)
   -v, --verbose         Set logger level to 'INFO' (default: False)
 ```
 
 ## Invoke dbCAN
 
-_`eCAMI` is memory intensive. We recommend using the maximum availalbe RAM. 445 Pseudomonas proteomes on 64GB RAM, 8-core XX processor takes 4 days to run dbCAN._
+_`eCAMI` is memory intensive. We recommend using the maximum availalbe RAM._
 
-`dbCAN` can be automated to parse all FASTA files in a directory (e.g. all download protein FASTA files or FASTA files of proteins not in a local CAZyme database), using `cazomveolve`, specifically, the `cazevolve_run_dbcan` command.
+`dbCAN` can be automated to parse all FASTA files in a directory (e.g. all download protein FASTA files or FASTA files of proteins not in a local CAZyme database), using the `cazomveolve`, subcommand `run_dbcan` command.
 
 ```bash
-cazevolve_run_dbcan \
+cazomevolve run_dbcan \
     <path to dir containing FASTA files> \
     <path to output directory> 
 ```
 
-The ouput directory will be created by `cazevolve_run_dbcan`. Inside the output directory, for each FASTA file parsed by `dbCAN` an output subdirectory will be created (named after the genomic version accession) and will contain the output from `dbCAN` for the respective protein FASTA file.
+The ouput directory will be created by `run_dbcan`. 
+
+Inside the output directory, for each FASTA file parsed by `dbCAN` an output subdirectory will be created (named after the genomic version accession) and will contain the output from `dbCAN` for the respective protein FASTA file.
 
 Optional args:
 ```bash
 options:
   -h, --help            show this help message and exit
-  -V2--version_2        Use dbCAN version 2 NOT 3 (default: False)
+  -V2--version_2        Use dbCAN version 2 NOT 3/4 (default: False)
   -f, --force           Force file over writting (default: False)
   -l log file name, --log log file name
                         Defines log file name and/or path (default: None)
   -n, --nodelete        enable/disable deletion of exisiting files (default: False)
   -v, --verbose         Set logger level to 'INFO' (default: False)
 ```
 
 ## Retrieve dbCAN annotations
 
-After running dbCAN, `cazomevolve` can iterate through the output subdirectories created by `cazevolve_run_dbcan` and compile the data into two tab delimited lists, containing:
+After running dbCAN, use the `cazomevolve` subcommand `get_dbcan_cazymes` to iterate through the output subdirectories created by `cazomevolve run_dbcan` and compile the data into two tab delimited lists, containing:
+
 1. Listing the CAZy family accession and genomic accession per line
 ```bash
 fam1    genome1
 fam2    genome1
 fam1    genome2
 fam3    genome2
 ```
@@ -269,15 +394,15 @@
 ```bash
 fam1    genome1 protein1
 fam2    genome1 protein1
 fam1    genome2 protein2
 fam3    genome2 protein3
 ```
 
-If paths to the tab delimited lists created by `cazevolve_get_cazy_cazymes` are provided, the dbCAN classifications will be **added** the existing tab delimited lists, and will not **overwrite** the data in the files (make sure to include the `-f`/`--force` and `-n`/`--nodelete` flags when wanting to add data to existing tab delimited files).
+If paths to the tab delimited lists created by `cazomevolve get_cazy_cazymes` are provided, the dbCAN classifications will be **added** the existing tab delimited lists, and will not **overwrite** the data in the files (make sure to include the `-f`/`--force` and `-n`/`--nodelete` flags when wanting to add data to existing tab delimited files).
 
 ```bash
 cazevolve_get_dbcan_cazymes \
     <path to dbCAN output dir (contining output subdirs)> \
     <path to write out tab delimited lists of CAZy families and genomic accessions> \
     <path to write out tab delimited lists of CAZy families, genomic accessions and protein accessions>
 ```
@@ -291,183 +416,231 @@
                         Defines log file name and/or path (default: None)
   -n, --nodelete        enable/disable deletion of exisiting files (default: False)
   --sql_echo            Set verbose SQLite3 logging (default: False)
   -v, --verbose         Set logger level to 'INFO' (default: False)
   -v2, --version_2      Parse the data from dbCAN version 2 (default: False, parse data from dbCAN version 3)
 ```
 
-# Reconstruct a phylogenetic tree using a baysian approach
-
-# Calculate ANI and construct a dendrogram
-
 # Explore the CAZome composition
 
 The module `cazomevolve.cazome.explore` contains functions for exploring the CAZome annotated by `cazomevolve`. These are:
 
 ```python
-from cazomevolve.cazome.explore import (
-    cazome_sizes,
-    identify_families,
-    parse_data,
-    pca,
-    plot,
-    taxonomies,
+# loading and parsing data
+from cazomevolve.cazome.explore.parse_data import (
+    load_fgp_data,
+    load_tax_data,
+    add_tax_data_from_tax_df,
+    add_tax_column_from_row_index,
+)
+
+# functions for exploring the sizes of CAZomes
+from cazomevolve.cazome.explore.cazome_sizes import (
+    calc_proteome_representation,
+    count_items_in_cazome,
+    get_proteome_sizes,
+    count_cazyme_fam_ratio,
+)
+
+# explore the frequency of CAZymes per CAZy class
+from cazomevolve.cazome.explore.cazy_classes import calculate_class_sizes
+
+# explore the frequencies of CAZy families and identify the co-cazome
+from cazomevolve.cazome.explore.cazy_families import (
+    build_fam_freq_df,
+    build_row_colours,
+    build_family_clustermap,
+    identify_core_cazome,
+    plot_fam_boxplot,
+    build_fam_mean_freq_df,
+    get_group_specific_fams,
+    build_family_clustermap_multi_legend,
 )
 
-# parse the output from cazomevolve tab delimited lists
-parse_data.get_dbcan_fams_data()
-parse_data.build_fam_freq_df()
-parse_data.index_df()  # index genome, genus and species to be row names
-
-# add taxonomic information for taxonomic context
-taxonomies.add_tax_info()
-taxonomies.get_gtdb_db_tax_dict()  # in development
-taxonomies.get_gtdb_search_tax_dict()
-taxonomies.get_ncbi_tax_dict()  # in development
-taxonomies.get_group_sample_sizes()  # returns the number of genomes per group (genus or species)
-
-# summarise the size of the cazomes
-cazome_sizes.get_cazome_size_df()
-cazome_sizes.get_proteome_size()
-cazome_sizes.get_cazome_proportion_df()
-cazome_sizes.get_num_of_fams_per_group()
-
-# identify the core CAZome, i.e. families that appear in every genome
-identify_families.identify_core_cazome()
-identify_families.get_core_fam_freqs()
-
-# identify families that are specific to a group (i.e. genus or species)
-identify_families.get_group_specific_fams()
-
-# identity families that always appear together 
-identify_families.get_cooccurring_fams()  # across all genomes
-identify_families.get_grps_cooccurring_fams()  # in a specific group (i.e. genus or species)
-
-# visually summarise the data
-plot.get_clustermap()  # clustermap of cazy family freqs - potentially add clustering by cazy class freqs
-
-# perform and visualise PCA
-pca.perform_pca()
-pca.plot_explained_variance()
-pca.plot_spree()
-pca.plot_pca()  # project genomes onto PCs
-pca.plot_loadings()
+# functions to identify and explore CAZy families that are always present together
+from cazomevolve.cazome.explore.cooccurring_families import (
+    identify_cooccurring_fams_corrM,
+    calc_cooccuring_fam_freqs,
+    identify_cooccurring_fam_pairs,
+    add_to_upsetplot_membership,
+    build_upsetplot,
+    get_upsetplot_grps,
+    add_upsetplot_grp_freqs,
+    build_upsetplot_matrix,
+)
+
+# functions to perform PCA
+from cazomevolve.cazome.explore.pca import (
+    perform_pca,
+    plot_explained_variance,
+    plot_scree,
+    plot_pca,
+    plot_loadings,
+)
 ```
 
+Two example jupyter notebooks are available which demonstrate using `cazomevolve` to explore, interogate, compare and visualise the CAZyme complement:
+
+1. Notebook exploring the CAZomes of _Pectobacteriaceae_
+    * [Notebook](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto/blob/master/notebooks/explore_pectobact_cazomes.ipynb)
+    * [Website](https://hobnobmancer.github.io/SI_Hobbs_et_al_2023_Pecto/notebooks/explore_pectobact_cazomes.html)
+2. Notebook exploring the CAZomes of _Pectobacterium_ and _Dickeya_
+    * [Notebook](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto/blob/master/notebooks/explore_pecto_dic_cazomes.ipynb)
+    * [Website](https://hobnobmancer.github.io/SI_Hobbs_et_al_2023_Pecto/notebooks/explore_pecto_dic_cazomes.html)
+
+
 # Identify networks of co-evolving CAZy families using `coinfinder`
 
+Any phylogentic tree written in Newick format can be used by `coinfinder`. To help out those new to phylogenetics, `cazomevovle` includes two sets of bash scripts for two alternative methods for creating trees.
 
+## Maximumlikelihood multi-gene tree
 
+To reconstruct a multi-gene phylogenetic tree, we recommend following the method presented in [Hugouviux-Corre-Pattat et al.](https://pure.strath.ac.uk/ws/portalfiles/portal/124038859/Hugouvieux_Cotte_Pattat_etal_IJSEM_2021_Proposal_for_the_creation_of_a_new_genus_Musicola_gen_nov_reclassification_of_Dickeya_paradisiaca.pdf). The specific method they used can be found in the [SI](https://widdowquinn.github.io/SI_Hugouvieux-Cotte-Pattat_2021/).
 
+To facilitate reconstructing the phylogenetic tree, `cazomevolve` includes a series of bash scripts which are available in the repository to coordinate the process.
 
+An example of using very similar scripts can be found in [Hobbs et al](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto).
 
-## Reconstruct the phylogenetic tree
+### CDS prediction
 
-### A baysian based approach
+To ensure consistency of nomenclature and support back threading the nucleotides sequences onto aligned single-copy orthologues, reannotate all prokaryotic and archaea genomes using [`prodigal`](https://github.com/hyattpd/Prodigal)
 
-### A distance based approach
+> Hyatt D, Chen GL, Locascio PF, Land ML, Larimer FW, Hauser LJ. Prodigal: prokaryotic gene recognition and translation initiation site identification. BMC Bioinformatics. 2010 Mar 8;11:119. doi: 10.1186/1471-2105-11-119. PMID: 20211023; PMCID: PMC2848648.
 
-## Annotate the CAZomes
+```bash
+scripts/tree/phylo/annotate_genomes.sh \
+  <output dir>
+```
 
-### Option 1: Using `cazomevolve` and `cazy_webscraper`
+The output directory is created by the bash script
 
-#### Step 1: Using CAZy -- retrieve the canonical classifications
+The annotate features were written to the following directories:  
+Proteins: `.../proteins`  
+CDS: `.../cds`  
+GBK: `.../gbk`  
 
-Use the Python script `cazomevolve/cazome/cazy/get_cazy_cazymes.py`, or the command `cevolve_get_cazy_cazymes` to retrieve the CAZy family classifications for proteins extracted from the genomic assemblies, and write two files of tab delimited list of the:
-1. <fam> <genomic accession>
-2. <fam> <genomic accession> <protein accession>
 
-The required args are:
-1. Path to the directory containing the FASTA protein sequences files
-2. Path to the local CAZyme database compiled using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/)
-3. Path to an output directory to write out the protein sequences of proteins not listed in the local CAZyme database
-4. Path to write out the tab delimited list of CAZy family annotations and associated genomic assembly accessions
-5. Path to write out the tab delimited list of CAZy family annotations and associated genome and protein accessions 
+### Identify Single Copy Orthologues (SCOs)
 
-`cazomevolve` will build all necessary output directories.
+Orthologues present in the genomes are identified using [`orthofinder`](https://github.com/davidemms/OrthoFinder).
 
-#### Step 2: Using dbCAN --- retrieve predicted classifications
+> Emms, D.M. and Kelly, S. (2019) OrthoFinder: phylogenetic orthology inference for comparative genomics. [Genome Biology 20:238](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1832-y)
 
-Use the Python script `cazomevolve/cazome/invoke_dbcan.py` to use `dbCAN` to predicte the CAZymes in each FASTA file of protein sequences.
+```bash
+scripts/tree/phylo/find_orthologues.sh \
+ <Path to .../proteins dir created by annotate_genomes.sh> \
+ <path to output dir>
+```
+
+The output dir will be created by orthofinder.
+
+### Multiple Sequence Alignment
+
+Each collection of single-copy orthologous was aligned using [`MAFFT`](https://mafft.cbrc.jp/alignment/software/).
+
+The output from `MAFFT` (the aligned files) are placed in the `data/pecto_dic/tree/sco_proteins_aligned` directory.
+
+```bash
+scripts/tree/phylo/align_scos.sh <path to dir containing SCO seqs from orthofinder>
+```
 
-2 positional arguments are required:
-1. Input dir: path to directory containing all FASTA files of protein sequences
-2. Output dir: path to write out all dbCAN output files. One subdir is created in the output dir for each FASTA file parsed by `dbCAN`
+### Collect Single-Copy Orthologues CDS sequences
 
-By default `dbCAN` version >= 3.0.4 is used (which uses `HMMER`, `DIAMOND` and `eCAMI`). To use `dbCAN` version 2.0.11 (which uses `HMMER`, `DIAMOND` and `Hotpep`) add the `-V2` or `--version_2` flag.
+The CDS sequences corresponding to each set of single-copy orthologues are identified and extracted with the Python script `extract_cds.py`. 
 
-To extract the CAZy family predictions from `dbCAN` version 2 and/or 3, use the Python script `cazomevolve/cazome/get_dbcan_cazymes.py`, which will write out the CAZy family annotations to a tab delimited list. 
+```bash
+python3 scripts/tree/phylo/extract_cds.py \
+  <Path to 'Single_Copy_Orthologue_Sequences' in the orthofinder output dir> \
+  <Path to CDS sequence annotated by Prodigal> \
+  <Output dir>
+```
 
-Two positional arguments are required:
-1. dbCAN dir: path to output dir from `invoke_dbcan<num>.py`
-2. Path to write out tab delimited list - this may already exist and contain the CAZy family annotations from the local CAZyme database. The script will add the predicted CAZy family annotaitons from the `dbCAN` to the existing file. If a file does not already exist, a new file will be created.
+The output directory will be created by the script.
 
-### Option 2: Using `pyrewton` and `cazy_webscraper`
+The output is a set of unaligned CDS sequences corresponding to each single-copy orthologue, which are 
+placed in the `data/pecto_dic/tree/sco_cds` directory
 
-You can use the Python package [`pyrewton`](https://hobnobmancer.github.io/pyrewton/) to annotate the CAZome for a set of genomic assemblies, using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) and `dbCAN` [Zhange et al., 2018]. `pyrewton` compiles the canconical and predicted CAZyme classifications into a local SQLite3 database.
+### Back-translate Aligned Single-Copy Orthologues
 
-> Han Zhang, Tanner Yohe, Le Huang, Sarah Entwistle, Peizhi Wu, Zhenglu Yang, Peter K Busk, Ying Xu, Yanbin Yin, dbCAN2: a meta server for automated carbohydrate-active enzyme annotation, Nucleic Acids Research, Volume 46, Issue W1, 2 July 2018, Pages W95–W101, https://doi.org/10.1093/nar/gky418
+The single-copy orthologue CDS sequences are threaded onto the corresponding aligned protein sequences using [`t-coffee`](http://www.tcoffee.org/Projects/tcoffee/), coordinated using the `backtranslate.sh` script.
 
-To retrieve the CAZy family annotations associated with each genomic assembly, execute the following sql command against the local CAZome database compiled using `pyrewton`:
-```sql
+> T-Coffee: A novel method for multiple sequence alignments. Notredame, Higgins, Heringa, JMB, 302(205-217)2000
 
+```bash
+scripts/tree/phylo/backtranslate.sh \
+  <path to dir containing protein MSA from MAFFT> \
+  <output dir - will contain codon MSA>
 ```
-Export the resulting table as a `tsv` file or tab delimited list.
 
-## Find networks of co-evolving CAZy families
-    
-Use the Python package `coinfinder` ([Whelan et al., 2020](https://www.microbiologyresearch.org/content/journal/mgen/10.1099/mgen.0.000338)) to identify networks of co-evolving CAZy families.
+The output dir will be made by the bash script.
 
-> Fiona J. Whelan, Martin Rusilowicz, & James O. McInerney. "Coinfinder: detecting significant associations and dissociations in pangenomes." doi: https://doi.org/10.1099/mgen.0.000338
-    
-See the `coinfinder` [documentation](https://github.com/fwhelan/coinfinder) for details.
-    
-To customise the resulting phylogenetic tree and heatmap, edit the R script `network.R` in `coinfinder`.
+### Concatenating CDS into a Multigene Alignment
 
-## Build a presence/abensce and CAZy family number matrices
+The threaded single-copy orthologue CDS sequences were concatenated into a single sequence per input organism using the Python script `concatenate_cds.py`. To reproduce this, execute the script from this directory with:
 
-## Build dendograms based upon CAZome compositions, and compare against the phylogenetic tree
+```bash
+python3 scripts/tree/phylo/concatenate_cds.py \
+  <Path to genome dir> \
+  <Path to CDS sequence annotated by Prodigal> \
+  <Output dir>
+```
 
-## Map genome and CAZome distances onto a plot
+Two files are generated, a FASTA file with the concatenated multigene sequences, and a partition file allowing a different set of model parameters to be fit to each gene in phylogenetic reconstruction.
 
-## Directories
+### Phylogenetic reconstruction
 
-Below is a directory plan of this repository, followed by a brief overview of each directories role , to facilitate navigation through the repository.
+To reconstruct the phylogenetic tree, the bash script `raxml_ng_build_tree.sh` is used, and is run from the root of this repository. This executes a series of [`raxml-ng`](https://github.com/amkozlov/raxml-ng) commands.
 
-### **assets**
+All genes are considered as separate partitions in the reconstuction, 
+with parameters estimated  for the model recommended by `raxml-ng check`.
 
-Directory containing all files needed for the GitHub page, created for easy access to accompanying Jupyter notebooks.
+Tree reconstructions are placed in the output directory. The best estimate tree is listed in `03_infer.raxml.bestTree`. 
 
-### **docs**
+> Alexey M. Kozlov, Diego Darriba, Tomáš Flouri, Benoit Morel, and Alexandros Stamatakis (2019) RAxML-NG: A fast, scalable, and user-friendly tool for maximum likelihood phylogenetic inference. Bioinformatics, btz305 [doi:10.1093/bioinformatics/btz305](https://doi.org/10.1093/bioinformatics/btz305)
 
-Directory containing files to build documentation hosted at ReadTheDocs.
+```bash
+scripts/tree/phylo/raxml_ng_build_tree.sh \
+ <path to contenated fasta file> \
+ <path to partition file> \
+ <path to output dir>
+```
 
-### **notebooks**
+The output directory is created by the script
 
-Directory containing all Jupyter notebooks, and html copies used for easier in-browser viewing via the GitHub pages. These notebooks include the data outputs from using `cfv_investigator`, how to use the package and how the package works.
+## A distance based approach
 
-### **tests**
+An alternative approach is to calculate genome distances from the Average Nucleotide Identity (ANI).
 
-Directory containing all `pytest` files for testing `pyrewton`, including subdirectories for test inputs and targets. Each module/submodule has its own specific test input and target subdirectory.
+The software package `pyani` [Pritchard et al.](https://doi.org/10.1039/C5AY02550H) can be used to calculate the ANI between all possible pairs of genomes, for a set of given genomes.
 
-### **cazomevolve**
+> Pritchard et al. (2016) "Genomics and taxonomy in diagnostics for food security: soft-rotting enterobacterial plant pathogens" Anal. Methods 8, 12-24
 
-Directory containing all `pyrewton` program modules (including all submodules and Python scripts).
-<p>&nbsp;</p>
+An example of using `pyani` to generate a ANI-based dendrogram can be found in [Hobbs et al.](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto/)
 
-## Modules
+The installation instructions for [`pyani`](https://github.com/widdowquinn/pyani)can be found in its [GitHub repo](https://github.com/widdowquinn/pyani). We recommend using >= version 0.3.0-alpha.
 
-_Please find more detailed documentation at for operation and troubleshooting at [Read the Docs](https://phd-project-scripts.readthedocs.io/en/latest/)_
+`cazomevolve` includes bash scripts to coordinate using `pyani`:
 
-This is an overview of the functionalities of each module within `pyrewton`, as well as basics of operation. For more detailed documentation on the operation of each module and indiviudal Python scripts please see the documentation at [Read the Docs](https://phd-project-scripts.readthedocs.io/en/latest/)
+```bash
+scripts/tree/ani/run_anim.sh \
+  <pyani and log file output directory> \
+  <dir containing genome .faa seqs> \
+  <plot and matrix output dir>
+```
 
-### **utilities**
+The R script `build_anim_tree.R` (in `scripts/tree/ani/`) can be used and modified to create to infer genome distances from the all-vs-all ANI analysis and construct a dendrogram from the distances.
 
-Contains all functions that are called from other Python scripts for building command-line parsers and loggers. Includes the submodule **file_io**, which contains functions that are called from other Python scripts for handling directories and files in `pyrewton`, including retrieving program inputs and creating output directories.
+## Find networks of co-evolving CAZy families
+    
+Use the Python package `coinfinder` ([Whelan et al., 2020](https://www.microbiologyresearch.org/content/journal/mgen/10.1099/mgen.0.000338)) to identify networks of co-evolving CAZy families.
 
-### **ncbi**
+> Fiona J. Whelan, Martin Rusilowicz, & James O. McInerney. "Coinfinder: detecting significant associations and dissociations in pangenomes." doi: https://doi.org/10.1099/mgen.0.000338
+    
+See the `coinfinder` [documentation](https://github.com/fwhelan/coinfinder) for details.
+    
+To customise the resulting phylogenetic tree and heatmap, edit the R script `network.R` in `coinfinder`.
 
-Modules that are involved in retrieving handling data from NCBI. This includes retrieval of genomic accession numbers and source organism taxonomic data.
+An example of where this is done can be found in [Hobbs _et al._ SI information on the exploration of _Pectobacteriaceae_ CAZomes](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto).
 
-### **covariance**
+# Build dendograms based upon CAZome compositions, and compare against the phylogenetic tree
 
-Modules that build the data set required for calculating the covariance, calculate the covariance of CAZy family annotations for all genomic accessions retrieved and taxonomic specific groups.
+....
```

### Comparing `cazomevolve-0.0.2/cazomevolve/__init__.py` & `cazomevolve-0.1.0/cazomevolve/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,28 +39,30 @@
 # SOFTWARE.
 """Bioinforamtic package for exploring the evolution of CAZomes"""
 
 
 import logging
 
 
-__version__ = "0.0.2"
+__version__ = "0.1.0"
 
+__citation__ = "???"
 
-def closing_message(job):
+
+def closing_message(job, args):
     """Write closing messsage to terminal
     
     :param job: str, name of module run
     :param args: CLI arguments parser
     """
     logging.basicConfig(level=logging.INFO)
     logger = logging.getLogger(__name__)
 
     message = f"""
     =====================cazomevolve: {job}=====================
-    Version: {VERSION_INFO}
+    Version: {__version__}
     """
 
     if args.verbose:
         logger.info(message)
     else:
         print(message)
```

### Comparing `cazomevolve-0.0.2/cazomevolve/cazome/__init__.py` & `cazomevolve-0.1.0/cazomevolve/cazome/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.0.2/cazomevolve/cazome/cazy/__init__.py` & `cazomevolve-0.1.0/cazomevolve/cazome/cazy/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.0.2/cazomevolve/cazome/cazy/get_cazy_cazymes.py` & `cazomevolve-0.1.0/cazomevolve/cazome/cazy/get_cazy_cazymes.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,45 +36,31 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Retrieve CAZy canoncial CAZyme classifications"""
 
 
-import json
 import logging
 import re
 import sys
 
-from pathlib import Path
 from typing import List, Optional
 
 from Bio import SeqIO
 from cazy_webscraper.sql.sql_orm import get_db_connection, Session, Genbank, CazyFamily
 from cazy_webscraper.sql.sql_interface.get_data.get_table_dicts import get_gbk_table_dict
 from saintBioutils.utilities.file_io import make_output_directory
-from saintBioutils.utilities.logger import config_logger
+from saintBioutils.utilities.file_io.get_paths import get_file_paths
 from tqdm import tqdm
 
 from cazomevolve import closing_message
-from cazomevolve.utilities.parsers.get_cazy_parser import build_parser
 
 
-def main(argv: Optional[List[str]] = None, logger: Optional[logging.Logger] = None):
-    if argv is None:
-        parser = build_parser()
-        args = parser.parse_args()
-    else:
-        parser = build_parser(argv)
-        args = parser.parse_args()
-
-    if logger is None:
-        config_logger(args)
-    logger = logging.getLogger(__name__)
-
+def main(args: Optional[List[str]] = None, logger: Optional[logging.Logger] = None):
     if str(args.output_dir.parent) != ".":
         make_output_directory(args.output_dir, args.force, args.nodelete)
 
     if str(args.fam_genome_list.parent) != ".":
         make_output_directory(args.fam_genome_list.parent, args.force, args.nodelete)
 
     if str(args.fam_genome_protein_list.parent) != ".":
@@ -83,54 +69,33 @@
         else:
             make_output_directory(args.fam_genome_protein_list.parent, args.force, args.nodelete)
 
     # connect to the local CAZyme db
     connection = get_db_connection(args.database, args.sql_echo, False)
 
     # retrieve path to protein FASTA files
-    fasta_files_paths, number_of_files = get_fasta_paths(args)
-
-    gbk_table_dict = get_gbk_table_dict(connection)
-
-    for fasta_path in tqdm(fasta_files_paths, desc="Getting CAZy annotations", total=number_of_files):
-        get_cazy_annotations(fasta_path, gbk_table_dict, args, connection)
-
-    closing_message('Get CAZy CAZymes')
-
-
-def get_fasta_paths(args):
-    """Retrieve paths to fasta files created by extract_proteins_genomes.py.
-    :param args: cmd-line args parser
-    Return two lists, one of path to FASTA files contain sequences, one of empty FASTA files.
-    """
-    logger = logging.getLogger(__name__)
-
-    # retrieve all files from directory
-    files_in_entries = (
-        entry for entry in Path(args.input_dir).iterdir() if (
-            entry.is_file() and entry.name.endswith(".fasta")
-        )
-    )
+    fasta_files_paths = get_file_paths(args.input_dir, suffixes=['.fasta', '.faa'])
 
-    file_list = [
-        entry for entry in Path(args.input_dir).iterdir() if (
-            entry.is_file() and entry.name.endswith(".fasta")
-        )
-    ]
-
-    if len(file_list) == 0:
+    if len(fasta_files_paths) == 0:
         logger.error(
             f"Found 0 fasta files in {args.input_dir}\n"
             "Check the path is correct. Terminating program"
         )
         sys.exit(1)
 
-    logger.warning(f"Retrieved {len(file_list)} FASTA files")
+    logger.warning(f"Retrieved {len(fasta_files_paths)} FASTA files")
+
+    logger.warning("Parsing CAZy db Genbanks table into dict")
+    gbk_table_dict = get_gbk_table_dict(connection)
+    logger.warning("Loading the GenBanks annotations into dict")
+
+    for fasta_path in tqdm(fasta_files_paths, desc="Getting CAZy annotations"):
+        get_cazy_annotations(fasta_path, gbk_table_dict, args, connection)
 
-    return files_in_entries, len(file_list)
+    closing_message('Get CAZy CAZymes', args)
 
 
 def get_cazy_annotations(fasta_path, gbk_table_dict, args, connection):
     """Get the CAZy family annotations for each fasta file.
 
     Move empty fasta files to directory used as input for dbCAN.
 
@@ -144,68 +109,68 @@
     logger = logging.getLogger(__name__)
 
     # compile path to write out non-CAZy annotated proteins
     output_path = args.output_dir / fasta_path.name
 
     # extract genomic accession from the file name
     try:
-        genomic_accession = re.findall(r"GCF_\d+\.\d+\.", fasta_path.name)[0]
-        genomic_accession = genomic_accession
+        genomic_accession = re.findall(r"GCF_\d+\.\d{1,5}", fasta_path.name)[0]
     except IndexError:
         try:
-            genomic_accession = re.findall(r"GCA_\d+\.\d+\.", fasta_path.name)[0]
-            genomic_accession = genomic_accession
+            genomic_accession = re.findall(r"GCA_\d+\.\d{1,5}", fasta_path.name)[0]
         except IndexError:
             logger.warning(
                 f"Could not retrieve genomic accession from\n{fasta_path}\n"
                 "Skipping FASTA file"
             )
             return
 
-    genomic_accession = genomic_accession[:-1]
-
-    in_cazy, not_in_cazy = set(), []
-
     cazy_accessions = set(list(gbk_table_dict.keys()))  # gbk accessions in the local db
 
+    # load sequences in proteome FASTA file into dict
     fasta_seqs = {}  # {protein acc: seq record}
     for record in SeqIO.parse(fasta_path, "fasta"):
         fasta_seqs[record.id] = record
 
     fasta_accessions = set(list(fasta_seqs.keys()))
-    print(f"Loaded {len(fasta_accessions)} seq IDs from {fasta_path}")
+    logger.warning(f"Loaded {len(fasta_accessions)} seq IDs from {fasta_path.name}")
+
+    acc_in_cazy, acc_not_in_cazy = set(), set()  # ensure they are reset to 0
 
     acc_in_cazy = cazy_accessions & fasta_accessions
-    print(f"Found {len(acc_in_cazy)} proteins in local CAZyme db")
+    logger.warning(f"Found {len(acc_in_cazy)} proteins in local CAZyme db")
 
-    acc_not_in_cazy = fasta_accessions.difference(in_cazy)
-    print(f"{len(acc_not_in_cazy)} proteins no in the local CAZyme db")
+    acc_not_in_cazy = fasta_accessions.difference(acc_in_cazy)
+    logger.warning(f"{len(acc_not_in_cazy)} proteins not in the local CAZyme db")
 
-    if len(not_in_cazy) != 0:
+    if len(acc_not_in_cazy) != 0:
+        # gather seqs of prot not in cazy and write to a FASTA file
         not_in_cazy_seqs = []
         for acc in acc_not_in_cazy:
             not_in_cazy_seqs.append(fasta_seqs[acc])
         SeqIO.write(not_in_cazy_seqs, output_path, "fasta")
 
-    if len(in_cazy) != 0:
+    if len(acc_in_cazy) != 0:
+        # compile data to write the tab delimited lists
         fam_genome_data = ""
         fam_genome_protein_data = ""
         
-        for prot_acc in tqdm(in_cazy, desc="Retrieving CAZy family annotaions from the local CAZyme database"):
+        for prot_acc in tqdm(acc_in_cazy, desc="Retrieving CAZy family annotaions from the local CAZyme database"):
             with Session(bind=connection) as session:
                 fam_query = session.query(Genbank, CazyFamily).\
                     join(CazyFamily, Genbank.families).\
                     filter(Genbank.genbank_accession == prot_acc).\
                     all()
 
                 for result in fam_query:
                     fam = result[1].family
                     fam_genome_data += f"{fam}\t{genomic_accession}\n"
                     fam_genome_protein_data += f"{fam}\t{genomic_accession}\t{prot_acc}\n"
 
+        # write out data
         with open(args.fam_genome_list, "a") as fh:
             fh.write(fam_genome_data)
         
         with open(args.fam_genome_protein_list, "a") as fh:
             fh.write(fam_genome_protein_data)
 
     return
```

### Comparing `cazomevolve-0.0.2/cazomevolve/cazome/dbcan/__init__.py` & `cazomevolve-0.1.0/cazomevolve/cazome/dbcan/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.0.2/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py` & `cazomevolve-0.1.0/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 # -*- coding: utf-8 -*-
 # (c) University of St Andrews 2022
 # (c) University of Strathclyde 2022
 # (c) James Hutton Institute 2022
 # Author:
 # Emma E. M. Hobbs
 
-# Contact
+# ContactC                                    
 # eemh1@st-andrews.ac.uk
 
 # Emma E. M. Hobbs,
 # Biomolecular Sciences Building,
 # University of St Andrews,
 # North Haugh Campus,
 # St Andrews,
 # KY16 9ST
 # Scotland,
 # UK
-
+#
 # The MIT License
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
@@ -37,39 +37,27 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Parse output from dbCAN version 2"""
 
 
 import logging
+import pandas as pd
 import re
 
 from tqdm import tqdm
 from typing import List, Optional
 
 from saintBioutils.utilities.file_io import make_output_directory
 from saintBioutils.utilities.file_io.get_paths import get_dir_paths
-from saintBioutils.utilities.logger import config_logger
 
 from cazomevolve import closing_message
-from cazomevolve.utilities.parsers.get_dbcan_parser import build_parser
-
 
-def main(argv: Optional[List[str]] = None, logger: Optional[logging.Logger] = None):
-    if argv is None:
-        parser = build_parser()
-        args = parser.parse_args()
-    else:
-        parser = build_parser(argv)
-        args = parser.parse_args
-    
-    if logger is None:
-        config_logger(args)
-    logger = logging.getLogger(__name__)
 
+def main(args: Optional[List[str]] = None, logger: Optional[logging.Logger] = None):
     # make output dir if necessary
     if str(args.fam_genome_list.parent) != ".":
         make_output_directory(args.fam_genome_list.parent, args.force, args.nodelete)
 
     if str(args.fam_genome_protein_list.parent) != ".":
         if str(args.fam_genome_list.parent) == str(args.fam_genome_protein_list.parent):
             make_output_directory(args.fam_genome_protein_list.parent, True, True)
@@ -78,15 +66,15 @@
 
     # get path to output directories from dbCAN
     output_dirs = get_dir_paths(args.dbcan_dir)
 
     for output_dir in tqdm(output_dirs, desc="Parsing dbCAN output dirs"):
         get_family_annotations(output_dir, args)
 
-    closing_message('Get dbCAN CAZymes')
+    closing_message('Get dbCAN CAZymes', args)
 
 
 def get_family_annotations(output_dir, args):
     """Extract CAZy family annotations from the dbCAN output
     
     Extracted famly annotations are added to the tab delimited list
 
@@ -97,38 +85,41 @@
     logger = logging.getLogger(__name__)
 
     genomic_accession = output_dir.name
     
     fam_annotations = {}  # {protein accession: {fams}} -- a single protein can appear on multiple lines
 
     try:
-        with open((output_dir/"overview.txt"), "r") as fh:
-            overview_file = fh.read().splitlines()
+        df = pd.read_table(output_dir/"overview.txt")
     except FileNotFoundError:
         logger.error(f"Could not find overview.txt file in {output_dir.name}\nSkipping output dir")
         return
+
+    # drop rows were #ofTools = 1
+    df = df[df['#ofTools'] != 1]
     
-    for line in tqdm(overview_file[1:], desc=f"Parsing {output_dir.name}"):
-        line = line.split("\t")
+    for ri in tqdm(range(len(df)), desc=f"Parsing {output_dir.name}"):
+        row = df.iloc[ri]
 
-        protein_accession = line[0]
+        protein_accession = row['Gene ID']
 
-        hmmer_fams = get_tool_fams(line[1])
-        hotpep_fams = get_tool_fams(line[2])
-        diamond_fams = get_tool_fams(line[3])
+        hmmer_fams = get_tool_fams(row[1])
+        hotpep_fams = get_tool_fams(row[2])
+        diamond_fams = get_tool_fams(row[3])
 
         # get the fams at least two tools agreed upon
         dbcan_fams = get_dbcan_consensus(hmmer_fams, hotpep_fams, diamond_fams)
 
-        try:
-            fam_annotations[protein_accession]
-            for fam in dbcan_fams:
-                fam_annotations[protein_accession].add(fam)
-        except KeyError:
-            fam_annotations[protein_accession] = dbcan_fams
+        if len(dbcan_fams) > 0:
+            try:
+                fam_annotations[protein_accession]
+                for fam in dbcan_fams:
+                    fam_annotations[protein_accession].add(fam)
+            except KeyError:
+                fam_annotations[protein_accession] = dbcan_fams
     
     with open(args.fam_genome_list, 'a') as fh:
         for protein_acc in tqdm(fam_annotations, desc="Adding fam-genome annotations to tab delim list"):
             protein_fams = fam_annotations[protein_acc]
             for fam in protein_fams:
                 fh.write(f"{fam}\t{genomic_accession}\n")
 
@@ -174,18 +165,14 @@
     Return set
     """
     hmmer_hotpep = hmmer_fams & hotpep_fams
     hmmer_diamond = hmmer_fams & diamond_fams
     hotpep_diamond = hotpep_fams & diamond_fams
     all_tools = hmmer_fams & diamond_fams & hotpep_fams
 
-    dbcan_consensus = list(
-        set(
-            list(all_tools) + list(hotpep_diamond) + list(hmmer_diamond) + list(hmmer_hotpep)
-            )
-        )
+    dbcan_consensus = list(all_tools.union(hmmer_hotpep, hmmer_diamond, hotpep_diamond))
     
     return dbcan_consensus
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cazomevolve-0.0.2/cazomevolve/cazome/dbcan/invoke_dbcan.py` & `cazomevolve-0.1.0/cazomevolve/cazome/dbcan/invoke_dbcan.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,56 +38,57 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Script for invoking dbCAN"""
 
 
 import re
 import subprocess
+import logging
 
 from tqdm import tqdm
+from typing import List, Optional
 
 from saintBioutils.utilities.file_io import make_output_directory
 from saintBioutils.utilities.file_io import get_paths
 
 from cazomevolve import closing_message
-from cazomevolve.utilities.parsers.invoke_dbcan_parser import build_parser
 
 
-def main():
-    parser = build_parser()
-    args = parser.parse_args()
-
+def main(args: Optional[List[str]] = None, logger: Optional[logging.Logger] = None):
     make_output_directory(args.output_dir, args.force, args.nodelete)
 
     # get the path to every FASTA to be parsed by dbCAN
     fasta_files_paths = list(set(get_paths.get_file_paths(args.input_dir, suffixes=['fasta', 'faa'])))
     fasta_files_paths.sort()
     print(f"Retrieved {len(fasta_files_paths)} fasta files from {args.input_dir}")
 
     for fasta_path in tqdm(fasta_files_paths, desc="Running dbCAN"):
         # define path to output dir that will house output for this specific input FASTA file
         # extract genomic accession from the file name, and name output dir after the accession
         try:
-            genomic_accession = re.findall(r"GCa_\d+\.\d+", fasta_path.name)[0]
+            genomic_accession = re.findall(r"GCF_\d+\.\d{1,5}", fasta_path.name)[0]
         except IndexError:
             try:
-                genomic_accession = re.findall(r"GCF_\d+\.\d+", fasta_path.name)[0]
+                genomic_accession = re.findall(r"GCA_\d+\.\d{1,5}", fasta_path.name)[0]
             except IndexError:
-                print(f"Could not get find genomic accession in {fasta_path.name}\nSkipping assembly\n")
-                continue
+                logger.warning(
+                    f"Could not retrieve genomic accession from\n{fasta_path}\n"
+                    "Skipping FASTA file"
+                )
+                return
         
         output_dir = args.output_dir / genomic_accession
 
         if output_dir.exists():
             print(f"Already parsed {genomic_accession}\nSKIIIP")
             continue
 
         invoke_dbcan(fasta_path, output_dir, args)
 
-    closing_message('Invoke dbCAN')
+    closing_message('Invoke dbCAN', args)
 
 
 def invoke_dbcan(input_path, out_dir, args):
     """Invoke the prediction tool (run-)dbCAN.
 
     :param input_path: path to input FASTA file
     :param out_dir: path to output directory for input FASTA file query
```

### Comparing `cazomevolve-0.0.2/cazomevolve/cazome/explore/__init__.py` & `cazomevolve-0.1.0/cazomevolve/cazome/explore/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""Module containing functions for exploring the composition and size of the CAZome"""
+"""Module containing functions for exploring the composition and size of the CAZome"""
```

### Comparing `cazomevolve-0.0.2/cazomevolve/cazome/explore/identify_families.py` & `cazomevolve-0.1.0/cazomevolve/cazome/explore/identify_families.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 
 import pandas as pd
 
 from tqdm import tqdm
 
 
+
 def identify_core_cazome(df):
     """Identify families that are present in every genome
     
     :param df: pandas df, cazy fam freq df
     
     Return list of CAZy families"""
     core_cazome = []
```

### Comparing `cazomevolve-0.0.2/cazomevolve/cazome/explore/parse_data.py` & `cazomevolve-0.1.0/cazomevolve/cazome/explore/parse_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -45,14 +45,143 @@
 from copy import copy
 from collections import Counter
 
 from tqdm import tqdm
 from saintBioutils.utilities.file_io.get_paths import get_dir_paths
 
 
+def load_fgp_data(fgp_file):
+    """Load data from the fgp (fam - genome - protein) tab delimited file from cazomevolve.
+
+    :param fgp_file: str/Path, path to fgp_file
+
+    Return pandas df with columns 'Family', 'Genome' and 'Protein' (containing the protein id/accession)
+    """
+    fgp_df = pd.read_table(fgp_file, header=None)
+    fgp_df.columns = ['Family', 'Genome', 'Protein']
+
+    return fgp_df
+
+
+def add_tax_column_from_row_index(df, tax_rank, tax_index):
+    """Add a column listing the tax for each row in a family frequency df
+    where the tax info is in the row index
+    
+    :param df: df to add tax data to
+    :param tax_rank: str, name of the tax rank, to be used as new column name
+    :param tax_index: int, index of tax info in the row name/index to be added to the new column
+    
+    Return df with a new column add
+    """
+    new_col = []
+    
+    for i in range(len(df)):
+        tax = df.iloc[i].name[tax_index]
+        new_col.append(tax)
+        
+    df[tax_rank] = new_col
+    
+    return df
+
+
+def load_tax_data(
+    tax_csv_path,
+    kingdom=False,
+    phylum=False,
+    tax_class=False,
+    tax_order=False,
+    tax_family=False,
+    genus=False,
+    species=False,
+):
+    """Load tax data compiled by cazomevolve into a pandas df
+
+    :param tax_csv_path: str/Path to csv file of genome, tax_rank, tax_rank
+        e.g. 'Genome', 'Genus', 'Species'
+    The remaining params are bool checks for lineage ranks included in the tax data file
+    
+    Return df of genome, tax_rank, tax_rank,  e.g. 'Genome', 'Genus', 'Species'
+    """
+    tax_df = pd.read_csv(tax_csv_path)
+    
+    col_names = ['Genome']
+    if kingdom:
+        col_names.append('Kingdom')
+    if phylum:
+        col_names.append('Phylun')
+    if tax_class:
+        col_names.append('Class')
+    if tax_order:
+        col_names.append('Order')
+    if genus:
+        col_names.append('Genus')
+    if species:
+        col_names.append('Species')
+
+    try:
+        tax_df = tax_df.drop('Unnamed: 0', axis=1)  #'Unnamed: 0' from pandas indexes
+    except:
+        pass
+
+    for colname in tax_df.columns:
+        if colname not in col_names:
+            tax_df = tax_df.drop(colname, axis=1)
+
+    return tax_df
+
+
+def add_tax_data_from_tax_df(
+    df,
+    tax_df,
+    kingdom=False,
+    phylum=False,
+    tax_class=False,
+    tax_order=False,
+    tax_family=False,
+    genus=False,
+    species=False,
+):
+    """Extract tax data from the tax df and add to the df (e.g. the gfp_df)
+    
+    :param df: pandas df, df to add tax data to
+    :param df: pandas df containing tax data, with one column called 'Genome'
+        and one column per tax rank
+    The remaining params are bool checks for lineage ranks to be added to 
+    the df
+    
+    Return df with new taxonomy columns
+    """
+    tax_ranks = []
+    if kingdom:
+        tax_ranks.append('Kingdom')
+    if phylum:
+        tax_ranks.append('Phylun')
+    if tax_class:
+        tax_ranks.append('Class')
+    if tax_order:
+        tax_ranks.append('Order')
+    if genus:
+        tax_ranks.append('Genus')
+    if species:
+        tax_ranks.append('Species')
+    if len(tax_ranks) == 0:
+        print('No tax ranks listed to be added to df')
+        return df
+    
+    for tax_rank in tax_ranks:
+        new_col = []
+        for ri in tqdm(range(len(df)), desc=f"Collecting {tax_rank} data"):
+            # retrieve the row in the tax_df containing the corresponding genome information
+            tax_row = tax_df[tax_df['Genome'] == df.iloc[ri]['Genome']]
+            new_col.append(tax_row[tax_rank].values[0])
+        df[tax_rank] = new_col
+        
+    return df
+
+
 def get_dbcan_fams_data(dbcan_dir, fam_g_path, fam_g_p_path):
     """Retrieve all CAZy families predicted by dbCAN and their frequencies.
     
     Removes EC numbers, domain ranges and subfams (retains fam of the subfam) 
     using parse_dbcan_tool().
     Writes out tab delimited lists using write_tab_files().
     
@@ -62,15 +191,15 @@
     
     Return
     * all_fams: a set of all CAZy families
     * fam_freq: Dict {genomic acc: Counter(cazy fam)}
     * cazome_sizes: Dict {genomic_acc: {'CAZymes': (num of CAZymes (num unique protein acc))}}
     """
     # get paths to all dbCAN output dirs
-    dbcan_dir_paths = get_dir_paths(dbcan_output_dir)
+    dbcan_dir_paths = get_dir_paths(dbcan_dir)
     
     all_fams = set()
     fam_freqs = {}  # genomic acc: Counter objects
     cazome_sizes = {}  # genome: {cazymes: int}
 
     for dir_path in tqdm(dbcan_dir_paths, desc="Parsing dbCAN output files"):
         genomic_acc = dir_path.name.split("_")[0] + '_' + dir_path.name.split("_")[1]
```

### Comparing `cazomevolve-0.0.2/cazomevolve/cazome/explore/plot.py` & `cazomevolve-0.1.0/cazomevolve/cazome/explore/plot.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.0.2/cazomevolve/cazome/explore/taxonomies.py` & `cazomevolve-0.1.0/cazomevolve/cazome/explore/taxonomies.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.0.2/cazomevolve/genomes/__init__.py` & `cazomevolve-0.1.0/cazomevolve/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.0.2/cazomevolve/genomes/download_acc_genomes.sh` & `cazomevolve-0.1.0/cazomevolve/genomes/download_acc_genomes.sh`

 * *Files 11% similar despite different names*

```diff
@@ -46,18 +46,19 @@
 # $1 path to file listing the accessions, with a unique genome accession per row
 # $2 output directory to write out the genomes to
 # $3 file options - A comma-separated list of formats is also possible. For example: "fasta,assembly-report". Choose from:
 # ['genbank', 'fasta', 'rm', 'features', 'gff', 'protein-fasta', 'genpept', 'wgs', 'cds-fasta', 'rna-fna', 'rna-fasta', 'assembly-report', 'assembly-stats', 'all']
 # $4 refseq or genbank
 # $5 assembly level, default all, ['all', 'complete', 'chromosome', 'scaffold', 'contig']
 
-ARG5=${5: 'all'}
-
-mkdir -p $2
+echo "Running ncbi-genome-download"
+echo "Citation: Blin et al. (2017) ncbi-genome-download, Follow link (ctrl + click)"
 
 ncbi-genome-download \
     all \
     --section $4 \
     --formats $3 \
     --assembly-levels $5 \
     --assembly-accessions $1 \
-    --output-folder $2
+    --output-folder $2 \
+    --verbose \
+    --flat-output
```

### Comparing `cazomevolve-0.0.2/cazomevolve/genomes/download_genomes.py` & `cazomevolve-0.1.0/cazomevolve/genomes/download_genomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,48 +34,36 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Retrieve all genomic assembly accessions descendent from a taxonomy node"""
 
+
 import logging
 import re
 import time
 
 from typing import List, Optional
 
 from socket import timeout
 from Bio import Entrez
 from saintBioutils.utilities.file_io import make_output_directory
-from saintBioutils.utilities.logger import config_logger
 from tqdm import tqdm
 from urllib.request import urlopen
 from urllib.error import HTTPError, URLError
 
 from cazomevolve import closing_message
-from cazomevolve.utilities.parsers.download_genomes_parser import build_parser
 
 
-def main(argv: Optional[List[str]] = None, logger: Optional[logging.Logger] = None):
+def main(args: Optional[List[str]] = None, logger: Optional[logging.Logger] = None):
     """Coordinate the retrieval of protein annotations from GenBank (.gbff) files.
     Including building parser, logger and output directory.
     Return dataframe of protein data.
     """
-    if argv is None:
-        parser = build_parser()
-        args = parser.parse_args()
-    else:
-        parser = build_parser(argv)
-        args = parser.parse_args()
-
-    if logger is None:
-        config_logger(args)
-    logger = logging.getLogger(__name__)
-
     make_output_directory(args.output_dir, args.force, args.nodelete)
 
     Entrez.email = args.email
 
     uid_lists = []
 
     for term in tqdm(((args.terms).split(",")), desc="Searching NCBI with terms"):
```

### Comparing `cazomevolve-0.0.2/cazomevolve/seq_diversity/get_fam_seqs.sh` & `cazomevolve-0.1.0/cazomevolve/seq_diversity/get_fam_seqs.sh`

 * *Files 0% similar despite different names*

```diff
@@ -51,9 +51,9 @@
 # get the seqs from NCBI
 cw_get_genbank_seqs $2 $1 --families $3
 
 IFS=',' read -ra user_families <<< "$3"
 
 for FAM in "${user_families[@]}"
 do
-    cw_extract_db_seqs $2 genbank $FAM --fasta_file $4/$FAM".seqs.fasta"
+    cw_extract_db_seqs $2 genbank $FAM --fasta_file $4/$FAM".seqs.fasta" -n
 done
```

### Comparing `cazomevolve-0.0.2/cazomevolve/seq_diversity/run_blastp.sh` & `cazomevolve-0.1.0/cazomevolve/seq_diversity/run_blastp.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env bash
+#!/usr/bin/ bash
 #
 # (c) University of St Andrews 2020-2021
 # (c) University of Strathclyde 2020-2021
 # (c) James Hutton Institute 2020-2021
 #
 # Author:
 # Emma E. M. Hobbs
@@ -40,12 +41,19 @@
 # SOFTWARE.
 
 # run_blastp.sh
 
 # $1 input FASTA file
 # $2 output file
 
+FILE_NAME=${2##*/}
+mkdir -p "${2%$FILE_NAME}"
+
+echo "Running BLASTP"
+
 blastp \
   -query $1 \
   -subject $1 \
   -out $2 \
   -outfmt "6 qseqid sseqid qlen slen length pident qcov scov evalue bitscore"
+
+echo "Done"
```

### Comparing `cazomevolve-0.0.2/cazomevolve/seq_diversity/run_diamond.sh` & `cazomevolve-0.1.0/cazomevolve/seq_diversity/run_diamond.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env bash
+#!/usr/bin/ bash
 #
 # (c) University of St Andrews 2020-2021
 # (c) University of Strathclyde 2020-2021
 # (c) James Hutton Institute 2020-2021
 #
 # Author:
 # Emma E. M. Hobbs
@@ -37,28 +38,38 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # run_diamond.sh
 
-# $1 cazy family
-# $2 input FASTA file
-# $3 diamond db to be created
-# $4 output file
+# $1 input FASTA file
+# $2 diamond db to be created
+# $3 output file
+
+echo "$1**$2***$3"
+
+FILE_NAME=${3##*/}
+mkdir -p "${3%$FILE_NAME}"
+echo "***********$FILE_NAME"
+FILE_NAME=${2##*/}
+mkdir -p "${2%$FILE_NAME}"
+echo "**************************$FILE_NAME"
+
 
 # build db
 echo 'Building database'
 diamond makedb \
-    --in $2 \
-    --db $3
+    --in $1 \
+    --db $2
 
 # run diamond
 echo 'Running DIAMOND'
 diamond blastp \
-    --db $3 \
-    --query $2 \
-    --out $4 \
+    --db $2 \
+    --query $1 \
+    --out $3 \
     --outfmt 6 qseqid sseqid qlen slen length pident evalue bitscore \
     --evalue 10 \
     --max-target-seqs 0
 
+echo "Done"
```

### Comparing `cazomevolve-0.0.2/cazomevolve.egg-info/PKG-INFO` & `cazomevolve-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cazomevolve
-Version: 0.0.2
+Version: 0.1.0
 Summary: A bioinforamtic package for investigating the evolution of CAZomes
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics protein
 Platform: Posix
 Platform: MacOS X
@@ -18,138 +18,274 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cazomevolve
 
+[![DOI](https://zenodo.org/badge/367898306.svg)](https://zenodo.org/badge/latestdoi/367898306)
+[![Documentation Status](https://readthedocs.org/projects/cazomevolve/badge/?version=latest)](https://cazomevolve.readthedocs.io/en/latest/?badge=latest)
 [![Funding](https://img.shields.io/badge/Funding-EASTBio-blue)](http://www.eastscotbiodtp.ac.uk/)
 [![PhD licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/PhD_Project_Scripts/blob/master/LICENSE)
 ![Python](https://img.shields.io/badge/Python-v3.9.---orange)
 ![Research](https://img.shields.io/badge/Research-Bioinformatics-ff69b4)
 
-**Cazome** **Evolve** (`cazomevolve`) invetigates the evolution of CAZomes by:
-* searching for CAZy families that associated more than expected from their lineage
-* projecting the CAZome composition onto a plot
-* building a dendogram using distances calculated from the CAZome composition 
+`cazomevolve` ('cazome-evolve') is an application and Python3 package for the automated annotation and exploratory analysis of CAZyme complements (CAZomes) for a set of species and/or genomes of interest. Carbohydrate Active enZymes are a subset of proteins that generate, modify and/or degrade carbohydrates. CAZy (www.cazy.org) is the most comprehensive CAZyme database, grouping proteins by sequence similarity into CAZy families.
 
-This repo houses all scripts required for calculating, exploring and visually representing the covariance of CAZy family annotations within genomic assemblies.
+Use `cazomevolve` to explore:
 
-## Contents
+**CAZome sizes:**
+* Compare the number of CAZymes and CAZy families
+* Calculate the proportion of the proteome encompassed by the CAZome
+* Compute the CAZy family to CAZyme ratio
+
+**CAZy class frequencies:**
+* Calculate the number of CAZymes per CAZy class
+* Plot a proportional area plot of CAZy class frequency broken down by CAZy class and user defined group deliniations (e.g. by genus or species)
+
+**CAZy families:**
+* Explore **sequence diversity** within a set of CAZy families:
+  * Run all-vs-all sequence comparison analyses
+  * Cluster the sequences by degree of sequence similarity
+  * Generate clustermaps of sequence identity, BLAST-score ratio, and coverage
+* Explore **CAZy family frequencies**:
+  * Compute the number of CAZymes per CAZy family
+  * Identify **lineage or group specific families** - e.g. genus or species specific families
+  * Identify **core CAZomes** - families that appear in all genomes
+  * Cluster genomes by CAZy family frequencies using **hierarchical clustering:**
+    * Generate annotated clustermaps of CAZy family frequencies
+    * Build a dendogram using distances calculated from the CAZome composition
+    * Construct tanglegrams to compare CAZy family dendrogram to a ANI-dendrogram or phylogenetic tree
+
+**Always co-occurring families:**
+* Identity CAZy families that are always present in the CAZome together
+* Find lineage or group specific groups of co-occurring families 
+* Construct an upset plot of co-occurring families
+* Calculate the number of genomes each group of co-occurring families appear in
+
+**Principal component analysis (PCA):**
+* Use PCA to idenify overal trends in the large and complex data set
+* Project genomes onto use selected principal components (PCs)
+* Construct loadings plots to explore correlation between CAZy families and PCs
+* Identify relationships between groups of CAZy families
+* Explore associations between CAZy families and lineage, phenotype, and niche adaptation
+
+**Co-evolving CAZy families:**
+* Generate the input file tab delimited list of genomes and CAZy families required by [`coinfinder`]() (Whelan _et al._)
+* Optionally add taxonomic data to the tab delimited list, to include taxa in the `coinfinder` output
+* Reconstruct phylogenetic trees to be used as input by `coinfinder`:
+  * Reconstruct a multi-gene phylogenetic tree using [`RaxML-ng`]()
+  * Construct an ANI-based dendrogram
+* Use `coinfinder` to identify CAZy families that appear together in a genome **more often than expected by lienage and chance**
+
+> Kozlov AM, Darriba D, Flouri T, Morel B, Stamatakis A. RAxML-NG: a fast, scalable and user-friendly tool for maximum likelihood phylogenetic inference. Bioinformatics. 2019 Nov 1;35(21):4453-4455. doi: 10.1093/bioinformatics/btz305.
+> Whelan FJ, Rusilowicz M, McInerney JO. Coinfinder: detecting significant associations and dissociations in pangenomes. Microb Genom. 2020 Mar;6(3):e000338. doi: 10.1099/mgen.0.000338. Epub 2020 Feb 24.
 
-1. [Overview](#Overview)
-2. [Installation](#Installation)
-    - [Requirements](#Requirements)
-3. [Current Developments](#Current)
-3. [Directories](#Directories)
-        
-## Overview
-
-Carbohydrate Active enZymes are a subset of proteins that generate, modify and/or degrade carbohydrates. CAZy (www.cazy.org) is the most comprehensive CAZyme database, grouping proteins by sequence similarity into CAZy families. **C**azy **F**amily co**V**ariance **investigator** (`cfv_investigator`) investigates the covariance of CAZy family annotations within proteomes across all species annotated by CAZy, and evaluates taxonomic specific covaraince of CAZy families.
-
-`cazomevolve` is a bioinformatic package (still in development) for:
-1. Retrieving of genomic accessions from which proteins catalogued within CAZy are derived from, and the associated taxonomic data of the source organism
-2. Tracking frequency of CAZy family annotations for all genomic assemblies identified in step 1
-3. Calculation of covariance of CAZy family annotations across all genomic assemblies identified in step 1, and for taxonomic specific groups (at the kingdom, genus and species taxonomic level)
-4. Generating dataframes of the number of CAZymes per CAZy family for each genomic assembly
-5. Generating a presence/absence matrix for each CAZy family in each genomic assembly
+## Documentation
 
-<p>&nbsp;</p>
+`cazomevolve` uses bash-script based workflow management. A summary of this workflow is provided in this README.
+
+Please see the [full documeentation including tutorials at ReadTheDocs]().
+
+An analysis using `cazomevolve` can be found [here](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto), which includes a README-walkthrough and all output files.
+
+## Contents
+
+1. [cazomevolve](#cazomevolve)
+2. [Documentation](#documentation)
+3. [Installation](#installation)
 
 ## Installation
 
+### PyPi
+
+The easiest way to install `cazomeolve` is via PyPi
+
+```bash
+pip install cazomevolve
+```
+
+### From source
+
 1. Create a virtual environment with dependencies, then activate the environment - _where venv_name is an chosen name for the virtual environment_
-`conda create -n <venv_name> python=3.9`   
-`conda activate <venv_name>`
+```bash
+conda create -n cazomevolve python=3.9
+conda activate cazomevolve
+```
 
 2. Clone the repository
-`git clone https://github.com/HobnobMancer/cazomevolve.git`
-
-3. Install pyrewton
-`pip3 install -e <path to directory containing setup.py file>`   
-Do not forget to use the **-e** option when install using pip3, otherwise each time pyrewton is invoked a ModuleNotFound error will be raised. Pass the path to the **directory** containign the setup.py file not the path to the setup.py file; if you are currently in the root directory of the repoistory where the file is located, simply use '.' to indicate the current working directory.
+```bash
+git clone https://github.com/HobnobMancer/cazomevolve.git
+pip install cazomevolve/.
+```
 
 <p>&nbsp;</p>
 
 ## Requirements
 
+### Essential
+
 POISx or Mac OS, or linux emulator   
-Python version 3.8+   
+Python version 3.8+
 Miniconda3 or Anaconda managed microenvironment, incorporated code checkers are included in list form in 'requirements.txt'.   
 Miniconda3 environment file is also available in the GitHub repository: 'environment.yml'.   
 For all required Python libraries please read 'requirements.txt'. 
 
-* [`ncbi-genome-download`](https://github.com/kblin/ncbi-genome-download/)
+The following packages are required by the core `cazomevolve` application, and their installation is handled by the `setup.py` file:
+* [`adjustText`](https://adjusttext.readthedocs.io/en/latest/)
+* [`biopython`](https://biopython.org/)
+* [`cazy_webscraper`](https://github.com/HobnobMancer/cazy_webscraper)
+* [`jupyter](https://jupyter.org/)
+* [`ncbi-genome-download`](https://pypi.org/project/ncbi-genome-download/)
+* [`numpy`](https://numpy.org/)
+* [`pandas`](https://pandas.pydata.org/)
 * [`saintBioutils`](https://github.com/HobnobMancer/saintBioutils)
+* [`seaborn`](https://seaborn.pydata.org/)
+* [`sklearn`](https://scikit-learn.org/stable/index.html) / `scikit-learn`
+* [`tqdm`](https://pypi.org/project/tqdm/)
+* [`upsetplot`](https://pypi.org/project/UpSetPlot/)
+
+### Optional
+
+The following packages are optional can installation instructions can be found in their respective repositories:
+
+**dbCAN:**
+
+To expand the data set beyond those CAZomes only listed in CAZy (**highly recommended!**) `dbCAN` must also be installed.
+
+Note: _`dbCAN` and `cazomevolve` can be installed in the same or separate virtual environments._
+
+**dbCAN version 3 and 4:**
+The CAZyme classifier `dbCAN` versions >= 3.0.6 can be installed via Conda (recommended). The full installation instructions are found [here](https://github.com/linnabrown/run_dbcan/tree/c9bad4835b2bc1a9685d693237f1d6a9d56ff3a1), and must be followed to ensure all additional database files are downloaded and compiled correctly.
+
+**dbCAN version 2:**
+The installation instructions for dbCAN v==2.0.11 can be found [here](https://github.com/linnabrown/run_dbcan/tree/fde6d7225441ef3d4cb29ea29e39cfdcc41d8b19).
 
-<p>&nbsp;</p>
 
+**`coinfinder`: Identify CAZy families that co-occurr more often than expected by lineage and chance:**
+* [`coinfinder`](https://github.com/fwhelan/coinfinder) >= v1.2.0
 
+Note: _`coinfinder` requires Python v3.6, we recommend installing and running `coinfinder` in a separate venv to `cazomevolve`
+
+**Construct an ANI-based dendrogram:**
+* [`pyani`](https://github.com/widdowquinn/pyani) >= version 0.3.0-alpha
+* [`R`](https://www.r-project.org/)
+
+**Reconstruct a multi-gene phylogenetic tree:**
+* [`MAFFT`](https://mafft.cbrc.jp/alignment/software/)
+* [`Orthofinder`](https://github.com/davidemms/OrthoFinder)
+* [`Prodigal`](https://github.com/hyattpd/Prodigal)
+* [`RaxML-ng`](https://github.com/amkozlov/raxml-ng)
+* [`T-coffee`](https://tcoffee.crg.eu/)
+
+<p>&nbsp;</p>
 
 # Method
 
-# Explore sequence diversity in CAZy families
+## Construct a local CAZyme database
+
+Download all CAZyme records from CAZy, and compile the records into a local SQLite3 database using `cazy_webscraper`:
+```bash
+cazy_webscraper <user-email-address> -o <desired-path-for-db>
+```
+
+## Explore sequence diversity in CAZy families
 
 Presuming a local CAZyme database has already been generated using `cazy_webscraper`:
 
-1. Generate a multisequence FASTA file for each CAZy family of interest using the bash script `get_fam_seqs.sh`, which 
-takes 4 positional arguments:
+1. Generate a multisequence FASTA file for each CAZy family of interest using the bash script `get_fam_seqs.sh`, which takes 4 positional arguments:
 
 * email address
 * path to a local cazyme db
 * name(s) of families of interest (separate with a single comma)
 * path to an output dir (do not include terminal /)
 
+```bash
+cazomevolve get_fam_seqs \
+  <email> \
+  <cazy_db> \
+  <fam1,fam2,fam3> \
+  <path to outdir>
+```
+
+* The output dir will be created by `cazy_webscraper` - it will not delete exsiting content in the outdir unless their is a FASTA file with the same name
+* Creates one output FASTA file per CAZy family
+
 Or use `cazy_webscraper` directly to create a multisequence FASTA file containing the protein sequences of interst
 
-2. Run all-vs-all sequence analysis for each multisequence FASTA file. Use the `run_blastp.sh` script to use BLASTP+ or the `run_diamond.sh` script to use DIAMOND (recommend for large families of >1000 proteins sequences)
+## Run all-vs-all analysis
+
+Run all-vs-all sequence analysis for each multisequence FASTA file, using BLAST or DIAMOND (recommend for large families of >1000 proteins sequences).
+
+The output directories will be created by `cazomevolve` - existing data in the existing output directories will **not** be deleted.
 
-`run_blastp.sh` takes 2 positional arguments:
+**Using BLASTP:**
+Use the `run_fam_blast` subcommand, which takes 2 positional arguments:
 * Path to the input FASTA file
 * Path for the output TSV file
 
-`run_diamond.sh` takes 3 positional arguments:
+```bash
+cazomevolve run_fam_blast \
+  <input fasta file> \
+  <output TSV file> 
+```
+
+**Using DIAMOND: (recommended for large datasets):**
+Use the `run_fam_diamond` subcommand, which takes 3 positional arguments:
 * Path to the input FASTA file
-* Path to build the DIAMOND database at
-* Path for the output TSV file
+* Path where to create a diamond db 
+* Path to write out output matrix
+
+```bash
+cazomevolve run_fam_diamond \
+  <input fasta file> \
+  <diamond db path> \
+  <output TSV file> 
+```
 
-Both scripts are located in `cazomevolve/seq_diversity/` directory.
+## Visualise the sequence diversity
 
-3. Visualise the results using the `jupyter notebook` template located at `cazomevolve/seq_diversity/explore_seq_diversity.ipynb`. This generates clustermaps and heatmaps that plot the proteins in the same order as the generated clustermap.
+Visualise the results using the `jupyter notebook` template located at `cazomevolve/seq_diversity/explore_seq_diversity.ipynb`. This generates clustermaps and heatmaps that plot the proteins in the same order as the generated clustermap.
+
+All functions used in the notebook are available, and can be imported from, `cazomevolve`, specifically the module `cazomevolve.seq_diversity.explore`.
 
 We recommend using the [BLAST Score Ratio (BSR)](https://widdowquinn.github.io/2018-03-06-ibioic/02-sequence_databases/05-blast_for_rbh.html#Normalised-bit-score,-and-coverage) to generate a clustermap, then generate heatmaps of the percentage identity (pident) and query coverage (qcov) so the proteins are plotted in the same order for the 3 plots and thus facilitates comparing between the three.
 
 Optionally, redundant protein sequences can be removed, and proteins of interest (mannually defined by the user) and functionally/structurally characterised proteins can be annotated on the plots, to facilitate identifying the degree of characterisation across a family.
 
-# Download genomes
+<p>&nbsp;</p>
+<p>&nbsp;</p>
+
+# Annotate the CAZome
+
+## Download genomes
 
-To download the genomic assemblies, use either method [A] or [B]
+The genomes to be download can be specified by [A] their genomic accessions, or [B] by specifying a taxa of interest (using a taxa of any level).
 
-## [A] Already have a list of genomic version accessions
+### [A] Genomic accessions
 
-If you already have a list of genomic version accessions in a plain text file, using the Python package `ncbi-genome-download` to download the genomic assemblies genomic (`.fna`) and proteome (`.faa`) sequence files.
+If you have a list of genomic version accessions in a plain text file, `cazomevolve` can use the Python package `ncbi-genome-download` to download the genomic assemblies genomic (`.fna`) and proteome (`.faa`) sequence files.
 
-The `cazevolve_download_acc_genomes` configures using `ncbi-genome-download`. The command takes 4 positional arguments and 1 optional argument:
+Using the `download_acc_genomes` subcommand, which takes 4 positional arguments and 1 optional argument:
 
 **Positional arguments:**
 1. Path to file containing list of accessions (with a unique genome accession per row)
 2. Path to output directory (will be created by `cazevolve_download_acc_genomes`)
 3. File options - a comma-separated list, e.g. "fasta,assembly-report": Choose from: ['genbank', 'fasta', 'rm', 'features', 'gff', 'protein-fasta', 'genpept', 'wgs', 'cds-fasta', 'rna-fna', 'rna-fasta', 'assembly-report', 'assembly-stats', 'all']
 4. Download Refseq ('refseq') or GenBank ('genbank') assemblies
 
 **Optional arguments:**
 1. Assembly level. Default 'all'. Comma separated list. Choose from: ['all', 'complete', 'chromosome', 'scaffold', 'contig']
 
-**Download the genomes in `.fna` and `faa` format.**
+**Downloads the genomes in `.fna` and `faa` format.**
 
-## [B] Retrieve all genomic assemblies associated with a specific term
+### [B] Taxa
 
-To download load all genomic assemblies associated with a term of interest, such as `Pectobacteriaceae` (so as to download all Pectobacteriaceae assemblies), use the command`cazevolve_download_genomes`.
+To download load all genomic assemblies associated with a term of interest, such as `Pectobacteriaceae` (so as to download all Pectobacteriaceae assemblies), use the subcommand `download_genomes`, which takes 4 arguments:
 
-**The command takes 4 requires arguments:**
 1. User email address (required by NCBI)
 2. The terms of interest. Comma-separated list, e.g. 'Pectobacterium,Dickeya'
 3. The file formats to download the genomic assemblies in. ['genomic' - downloads genomic.fna seq files, 'protein' - downloads protein.faa seq files]"
 4. Path to an output directory (this will be built by `cazomevolve`).
 
 By default if the output directory exists, `cazomevolve` will crash. To write to an existing output directory use the `-f`/`--force` flag. By default, `cazomevolve` will delete all existing data in the existing output directory. To retain the data available in the existing output directory use the `-n`/`--nodelete` flag.
 
@@ -162,42 +298,50 @@
 ``-f``, ``--force`` - Force file over writting (default: False)
 ``-l - log file name, --log log file name
                         Defines log file name and/or path (default: None)
 ``-n``, ``--nodelete`` - enable/disable deletion of exisiting files (default: False)
 ``--timeout`` TIMEOUT - time in seconds before connection times out (default: 30)
 ``-v``, ``--verbose`` - Set logger level to 'INFO' (default: False)
 
-# Annotate CAZomes
+## Annotate CAZomes
 
-To retrieve the most comprehensive annotation of the CAZome, the (widely considered) canonical classifications from CAZy retrieved using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) (Hobbs _et al.,_ 2022), combined with predicted CAZy family annotations from [`dbCAN`](https://github.com/linnabrown/run_dbcan) (Zhang _et al._ 2018).
+To retrieve the most comprehensive annotation of the CAZome, we recommend using the (widely considered) canonical classifications from CAZy retrieved using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) (Hobbs _et al.,_ 2022), combined with predicted CAZy family annotations from [`dbCAN`](https://github.com/linnabrown/run_dbcan) (Zhang _et al._ 2018).
 
 > Emma E. M. Hobbs, Tracey M. Gloster, Leighton Pritchard; cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets, BioRxiv, 3 December 2022, https://doi.org/10.1101/2022.12.02.518825
 
 > Han Zhang, Tanner Yohe, Le Huang, Sarah Entwistle, Peizhi Wu, Zhenglu Yang, Peter K Busk, Ying Xu, Yanbin Yin; dbCAN2: a meta server for automated carbohydrate-active enzyme annotation, Nucleic Acids Research, Volume 46, Issue W1, 2 July 2018, Pages W95–W101, https://doi.org/10.1093/nar/gky418
 
 ## Build a local CAZyme database using `cazy_webscraper`
 
 To include 'canonical' CAZy family classifications from CAZy, download all data from the CAZy database and compile the data into a local CAZyme database using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) (Hobbs _et al., 2022).
 
 > cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets
 Emma E. M. Hobbs, Tracey M. Gloster, Leighton Pritchard
 bioRxiv 2022.12.02.518825; doi: https://doi.org/10.1101/2022.12.02.518825
 
+The `cazomevolve` subcommand `build_cazy_db` to coordinate uisng `cazy_webscraper`:
+```bash
+cazomevolve build_cazy_db \
+  <email> \
+  <desired db path>
+```
+
+Or you can use `cazy_webscraper` directly
 ```bash
 cazy_webscraper \
     <email> \
     -o <db file output path>
 ```
 
 ## Retrieve CAZy annotations
 
-Use `cazomevolve` to query the protein version accessions in the downloaded protein FASTA files against the local CAZyme db, to retrieve the 'canonical' CAZy family classifications, using the `cazevolve_get_cazy_cazymes` command.
+The `get_cazy_cazymes` subcommand to coordinate `cazomevolve` to query the protein version accessions in the downloaded protein FASTA files against the local CAZyme db, to retrieve the 'canonical' CAZy family classifications:
 
 ```bash
-cazevolve_get_cazy_cazymes \
+cazomevolve get_cazy_cazymes \
     <path to dir containing protein FASTA files> \
     <path to local cazyme database> \
     <path to dir to write out protein sequences NOT in the local db> \
     <path to write out tab delimited lists of CAZy families and genomic accessions> \
     <path to write out tab delimited lists of CAZy families, genomic accessions and protein accessions> \
 ```
 
@@ -227,41 +371,44 @@
   -n, --nodelete        enable/disable deletion of exisiting files (default: False)
   --sql_echo            Set verbose SQLite3 logging (default: False)
   -v, --verbose         Set logger level to 'INFO' (default: False)
 ```
 
 ## Invoke dbCAN
 
-_`eCAMI` is memory intensive. We recommend using the maximum availalbe RAM. 445 Pseudomonas proteomes on 64GB RAM, 8-core XX processor takes 4 days to run dbCAN._
+_`eCAMI` is memory intensive. We recommend using the maximum availalbe RAM._
 
-`dbCAN` can be automated to parse all FASTA files in a directory (e.g. all download protein FASTA files or FASTA files of proteins not in a local CAZyme database), using `cazomveolve`, specifically, the `cazevolve_run_dbcan` command.
+`dbCAN` can be automated to parse all FASTA files in a directory (e.g. all download protein FASTA files or FASTA files of proteins not in a local CAZyme database), using the `cazomveolve`, subcommand `run_dbcan` command.
 
 ```bash
-cazevolve_run_dbcan \
+cazomevolve run_dbcan \
     <path to dir containing FASTA files> \
     <path to output directory> 
 ```
 
-The ouput directory will be created by `cazevolve_run_dbcan`. Inside the output directory, for each FASTA file parsed by `dbCAN` an output subdirectory will be created (named after the genomic version accession) and will contain the output from `dbCAN` for the respective protein FASTA file.
+The ouput directory will be created by `run_dbcan`. 
+
+Inside the output directory, for each FASTA file parsed by `dbCAN` an output subdirectory will be created (named after the genomic version accession) and will contain the output from `dbCAN` for the respective protein FASTA file.
 
 Optional args:
 ```bash
 options:
   -h, --help            show this help message and exit
-  -V2--version_2        Use dbCAN version 2 NOT 3 (default: False)
+  -V2--version_2        Use dbCAN version 2 NOT 3/4 (default: False)
   -f, --force           Force file over writting (default: False)
   -l log file name, --log log file name
                         Defines log file name and/or path (default: None)
   -n, --nodelete        enable/disable deletion of exisiting files (default: False)
   -v, --verbose         Set logger level to 'INFO' (default: False)
 ```
 
 ## Retrieve dbCAN annotations
 
-After running dbCAN, `cazomevolve` can iterate through the output subdirectories created by `cazevolve_run_dbcan` and compile the data into two tab delimited lists, containing:
+After running dbCAN, use the `cazomevolve` subcommand `get_dbcan_cazymes` to iterate through the output subdirectories created by `cazomevolve run_dbcan` and compile the data into two tab delimited lists, containing:
+
 1. Listing the CAZy family accession and genomic accession per line
 ```bash
 fam1    genome1
 fam2    genome1
 fam1    genome2
 fam3    genome2
 ```
@@ -269,15 +416,15 @@
 ```bash
 fam1    genome1 protein1
 fam2    genome1 protein1
 fam1    genome2 protein2
 fam3    genome2 protein3
 ```
 
-If paths to the tab delimited lists created by `cazevolve_get_cazy_cazymes` are provided, the dbCAN classifications will be **added** the existing tab delimited lists, and will not **overwrite** the data in the files (make sure to include the `-f`/`--force` and `-n`/`--nodelete` flags when wanting to add data to existing tab delimited files).
+If paths to the tab delimited lists created by `cazomevolve get_cazy_cazymes` are provided, the dbCAN classifications will be **added** the existing tab delimited lists, and will not **overwrite** the data in the files (make sure to include the `-f`/`--force` and `-n`/`--nodelete` flags when wanting to add data to existing tab delimited files).
 
 ```bash
 cazevolve_get_dbcan_cazymes \
     <path to dbCAN output dir (contining output subdirs)> \
     <path to write out tab delimited lists of CAZy families and genomic accessions> \
     <path to write out tab delimited lists of CAZy families, genomic accessions and protein accessions>
 ```
@@ -291,183 +438,231 @@
                         Defines log file name and/or path (default: None)
   -n, --nodelete        enable/disable deletion of exisiting files (default: False)
   --sql_echo            Set verbose SQLite3 logging (default: False)
   -v, --verbose         Set logger level to 'INFO' (default: False)
   -v2, --version_2      Parse the data from dbCAN version 2 (default: False, parse data from dbCAN version 3)
 ```
 
-# Reconstruct a phylogenetic tree using a baysian approach
-
-# Calculate ANI and construct a dendrogram
-
 # Explore the CAZome composition
 
 The module `cazomevolve.cazome.explore` contains functions for exploring the CAZome annotated by `cazomevolve`. These are:
 
 ```python
-from cazomevolve.cazome.explore import (
-    cazome_sizes,
-    identify_families,
-    parse_data,
-    pca,
-    plot,
-    taxonomies,
+# loading and parsing data
+from cazomevolve.cazome.explore.parse_data import (
+    load_fgp_data,
+    load_tax_data,
+    add_tax_data_from_tax_df,
+    add_tax_column_from_row_index,
+)
+
+# functions for exploring the sizes of CAZomes
+from cazomevolve.cazome.explore.cazome_sizes import (
+    calc_proteome_representation,
+    count_items_in_cazome,
+    get_proteome_sizes,
+    count_cazyme_fam_ratio,
+)
+
+# explore the frequency of CAZymes per CAZy class
+from cazomevolve.cazome.explore.cazy_classes import calculate_class_sizes
+
+# explore the frequencies of CAZy families and identify the co-cazome
+from cazomevolve.cazome.explore.cazy_families import (
+    build_fam_freq_df,
+    build_row_colours,
+    build_family_clustermap,
+    identify_core_cazome,
+    plot_fam_boxplot,
+    build_fam_mean_freq_df,
+    get_group_specific_fams,
+    build_family_clustermap_multi_legend,
 )
 
-# parse the output from cazomevolve tab delimited lists
-parse_data.get_dbcan_fams_data()
-parse_data.build_fam_freq_df()
-parse_data.index_df()  # index genome, genus and species to be row names
-
-# add taxonomic information for taxonomic context
-taxonomies.add_tax_info()
-taxonomies.get_gtdb_db_tax_dict()  # in development
-taxonomies.get_gtdb_search_tax_dict()
-taxonomies.get_ncbi_tax_dict()  # in development
-taxonomies.get_group_sample_sizes()  # returns the number of genomes per group (genus or species)
-
-# summarise the size of the cazomes
-cazome_sizes.get_cazome_size_df()
-cazome_sizes.get_proteome_size()
-cazome_sizes.get_cazome_proportion_df()
-cazome_sizes.get_num_of_fams_per_group()
-
-# identify the core CAZome, i.e. families that appear in every genome
-identify_families.identify_core_cazome()
-identify_families.get_core_fam_freqs()
-
-# identify families that are specific to a group (i.e. genus or species)
-identify_families.get_group_specific_fams()
-
-# identity families that always appear together 
-identify_families.get_cooccurring_fams()  # across all genomes
-identify_families.get_grps_cooccurring_fams()  # in a specific group (i.e. genus or species)
-
-# visually summarise the data
-plot.get_clustermap()  # clustermap of cazy family freqs - potentially add clustering by cazy class freqs
-
-# perform and visualise PCA
-pca.perform_pca()
-pca.plot_explained_variance()
-pca.plot_spree()
-pca.plot_pca()  # project genomes onto PCs
-pca.plot_loadings()
+# functions to identify and explore CAZy families that are always present together
+from cazomevolve.cazome.explore.cooccurring_families import (
+    identify_cooccurring_fams_corrM,
+    calc_cooccuring_fam_freqs,
+    identify_cooccurring_fam_pairs,
+    add_to_upsetplot_membership,
+    build_upsetplot,
+    get_upsetplot_grps,
+    add_upsetplot_grp_freqs,
+    build_upsetplot_matrix,
+)
+
+# functions to perform PCA
+from cazomevolve.cazome.explore.pca import (
+    perform_pca,
+    plot_explained_variance,
+    plot_scree,
+    plot_pca,
+    plot_loadings,
+)
 ```
 
+Two example jupyter notebooks are available which demonstrate using `cazomevolve` to explore, interogate, compare and visualise the CAZyme complement:
+
+1. Notebook exploring the CAZomes of _Pectobacteriaceae_
+    * [Notebook](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto/blob/master/notebooks/explore_pectobact_cazomes.ipynb)
+    * [Website](https://hobnobmancer.github.io/SI_Hobbs_et_al_2023_Pecto/notebooks/explore_pectobact_cazomes.html)
+2. Notebook exploring the CAZomes of _Pectobacterium_ and _Dickeya_
+    * [Notebook](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto/blob/master/notebooks/explore_pecto_dic_cazomes.ipynb)
+    * [Website](https://hobnobmancer.github.io/SI_Hobbs_et_al_2023_Pecto/notebooks/explore_pecto_dic_cazomes.html)
+
+
 # Identify networks of co-evolving CAZy families using `coinfinder`
 
+Any phylogentic tree written in Newick format can be used by `coinfinder`. To help out those new to phylogenetics, `cazomevovle` includes two sets of bash scripts for two alternative methods for creating trees.
 
+## Maximumlikelihood multi-gene tree
 
+To reconstruct a multi-gene phylogenetic tree, we recommend following the method presented in [Hugouviux-Corre-Pattat et al.](https://pure.strath.ac.uk/ws/portalfiles/portal/124038859/Hugouvieux_Cotte_Pattat_etal_IJSEM_2021_Proposal_for_the_creation_of_a_new_genus_Musicola_gen_nov_reclassification_of_Dickeya_paradisiaca.pdf). The specific method they used can be found in the [SI](https://widdowquinn.github.io/SI_Hugouvieux-Cotte-Pattat_2021/).
 
+To facilitate reconstructing the phylogenetic tree, `cazomevolve` includes a series of bash scripts which are available in the repository to coordinate the process.
 
+An example of using very similar scripts can be found in [Hobbs et al](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto).
 
-## Reconstruct the phylogenetic tree
+### CDS prediction
 
-### A baysian based approach
+To ensure consistency of nomenclature and support back threading the nucleotides sequences onto aligned single-copy orthologues, reannotate all prokaryotic and archaea genomes using [`prodigal`](https://github.com/hyattpd/Prodigal)
 
-### A distance based approach
+> Hyatt D, Chen GL, Locascio PF, Land ML, Larimer FW, Hauser LJ. Prodigal: prokaryotic gene recognition and translation initiation site identification. BMC Bioinformatics. 2010 Mar 8;11:119. doi: 10.1186/1471-2105-11-119. PMID: 20211023; PMCID: PMC2848648.
 
-## Annotate the CAZomes
+```bash
+scripts/tree/phylo/annotate_genomes.sh \
+  <output dir>
+```
 
-### Option 1: Using `cazomevolve` and `cazy_webscraper`
+The output directory is created by the bash script
 
-#### Step 1: Using CAZy -- retrieve the canonical classifications
+The annotate features were written to the following directories:  
+Proteins: `.../proteins`  
+CDS: `.../cds`  
+GBK: `.../gbk`  
 
-Use the Python script `cazomevolve/cazome/cazy/get_cazy_cazymes.py`, or the command `cevolve_get_cazy_cazymes` to retrieve the CAZy family classifications for proteins extracted from the genomic assemblies, and write two files of tab delimited list of the:
-1. <fam> <genomic accession>
-2. <fam> <genomic accession> <protein accession>
 
-The required args are:
-1. Path to the directory containing the FASTA protein sequences files
-2. Path to the local CAZyme database compiled using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/)
-3. Path to an output directory to write out the protein sequences of proteins not listed in the local CAZyme database
-4. Path to write out the tab delimited list of CAZy family annotations and associated genomic assembly accessions
-5. Path to write out the tab delimited list of CAZy family annotations and associated genome and protein accessions 
+### Identify Single Copy Orthologues (SCOs)
 
-`cazomevolve` will build all necessary output directories.
+Orthologues present in the genomes are identified using [`orthofinder`](https://github.com/davidemms/OrthoFinder).
 
-#### Step 2: Using dbCAN --- retrieve predicted classifications
+> Emms, D.M. and Kelly, S. (2019) OrthoFinder: phylogenetic orthology inference for comparative genomics. [Genome Biology 20:238](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1832-y)
 
-Use the Python script `cazomevolve/cazome/invoke_dbcan.py` to use `dbCAN` to predicte the CAZymes in each FASTA file of protein sequences.
+```bash
+scripts/tree/phylo/find_orthologues.sh \
+ <Path to .../proteins dir created by annotate_genomes.sh> \
+ <path to output dir>
+```
+
+The output dir will be created by orthofinder.
+
+### Multiple Sequence Alignment
+
+Each collection of single-copy orthologous was aligned using [`MAFFT`](https://mafft.cbrc.jp/alignment/software/).
+
+The output from `MAFFT` (the aligned files) are placed in the `data/pecto_dic/tree/sco_proteins_aligned` directory.
+
+```bash
+scripts/tree/phylo/align_scos.sh <path to dir containing SCO seqs from orthofinder>
+```
 
-2 positional arguments are required:
-1. Input dir: path to directory containing all FASTA files of protein sequences
-2. Output dir: path to write out all dbCAN output files. One subdir is created in the output dir for each FASTA file parsed by `dbCAN`
+### Collect Single-Copy Orthologues CDS sequences
 
-By default `dbCAN` version >= 3.0.4 is used (which uses `HMMER`, `DIAMOND` and `eCAMI`). To use `dbCAN` version 2.0.11 (which uses `HMMER`, `DIAMOND` and `Hotpep`) add the `-V2` or `--version_2` flag.
+The CDS sequences corresponding to each set of single-copy orthologues are identified and extracted with the Python script `extract_cds.py`. 
 
-To extract the CAZy family predictions from `dbCAN` version 2 and/or 3, use the Python script `cazomevolve/cazome/get_dbcan_cazymes.py`, which will write out the CAZy family annotations to a tab delimited list. 
+```bash
+python3 scripts/tree/phylo/extract_cds.py \
+  <Path to 'Single_Copy_Orthologue_Sequences' in the orthofinder output dir> \
+  <Path to CDS sequence annotated by Prodigal> \
+  <Output dir>
+```
 
-Two positional arguments are required:
-1. dbCAN dir: path to output dir from `invoke_dbcan<num>.py`
-2. Path to write out tab delimited list - this may already exist and contain the CAZy family annotations from the local CAZyme database. The script will add the predicted CAZy family annotaitons from the `dbCAN` to the existing file. If a file does not already exist, a new file will be created.
+The output directory will be created by the script.
 
-### Option 2: Using `pyrewton` and `cazy_webscraper`
+The output is a set of unaligned CDS sequences corresponding to each single-copy orthologue, which are 
+placed in the `data/pecto_dic/tree/sco_cds` directory
 
-You can use the Python package [`pyrewton`](https://hobnobmancer.github.io/pyrewton/) to annotate the CAZome for a set of genomic assemblies, using [`cazy_webscraper`](https://hobnobmancer.github.io/cazy_webscraper/) and `dbCAN` [Zhange et al., 2018]. `pyrewton` compiles the canconical and predicted CAZyme classifications into a local SQLite3 database.
+### Back-translate Aligned Single-Copy Orthologues
 
-> Han Zhang, Tanner Yohe, Le Huang, Sarah Entwistle, Peizhi Wu, Zhenglu Yang, Peter K Busk, Ying Xu, Yanbin Yin, dbCAN2: a meta server for automated carbohydrate-active enzyme annotation, Nucleic Acids Research, Volume 46, Issue W1, 2 July 2018, Pages W95–W101, https://doi.org/10.1093/nar/gky418
+The single-copy orthologue CDS sequences are threaded onto the corresponding aligned protein sequences using [`t-coffee`](http://www.tcoffee.org/Projects/tcoffee/), coordinated using the `backtranslate.sh` script.
 
-To retrieve the CAZy family annotations associated with each genomic assembly, execute the following sql command against the local CAZome database compiled using `pyrewton`:
-```sql
+> T-Coffee: A novel method for multiple sequence alignments. Notredame, Higgins, Heringa, JMB, 302(205-217)2000
 
+```bash
+scripts/tree/phylo/backtranslate.sh \
+  <path to dir containing protein MSA from MAFFT> \
+  <output dir - will contain codon MSA>
 ```
-Export the resulting table as a `tsv` file or tab delimited list.
 
-## Find networks of co-evolving CAZy families
-    
-Use the Python package `coinfinder` ([Whelan et al., 2020](https://www.microbiologyresearch.org/content/journal/mgen/10.1099/mgen.0.000338)) to identify networks of co-evolving CAZy families.
+The output dir will be made by the bash script.
 
-> Fiona J. Whelan, Martin Rusilowicz, & James O. McInerney. "Coinfinder: detecting significant associations and dissociations in pangenomes." doi: https://doi.org/10.1099/mgen.0.000338
-    
-See the `coinfinder` [documentation](https://github.com/fwhelan/coinfinder) for details.
-    
-To customise the resulting phylogenetic tree and heatmap, edit the R script `network.R` in `coinfinder`.
+### Concatenating CDS into a Multigene Alignment
 
-## Build a presence/abensce and CAZy family number matrices
+The threaded single-copy orthologue CDS sequences were concatenated into a single sequence per input organism using the Python script `concatenate_cds.py`. To reproduce this, execute the script from this directory with:
 
-## Build dendograms based upon CAZome compositions, and compare against the phylogenetic tree
+```bash
+python3 scripts/tree/phylo/concatenate_cds.py \
+  <Path to genome dir> \
+  <Path to CDS sequence annotated by Prodigal> \
+  <Output dir>
+```
 
-## Map genome and CAZome distances onto a plot
+Two files are generated, a FASTA file with the concatenated multigene sequences, and a partition file allowing a different set of model parameters to be fit to each gene in phylogenetic reconstruction.
 
-## Directories
+### Phylogenetic reconstruction
 
-Below is a directory plan of this repository, followed by a brief overview of each directories role , to facilitate navigation through the repository.
+To reconstruct the phylogenetic tree, the bash script `raxml_ng_build_tree.sh` is used, and is run from the root of this repository. This executes a series of [`raxml-ng`](https://github.com/amkozlov/raxml-ng) commands.
 
-### **assets**
+All genes are considered as separate partitions in the reconstuction, 
+with parameters estimated  for the model recommended by `raxml-ng check`.
 
-Directory containing all files needed for the GitHub page, created for easy access to accompanying Jupyter notebooks.
+Tree reconstructions are placed in the output directory. The best estimate tree is listed in `03_infer.raxml.bestTree`. 
 
-### **docs**
+> Alexey M. Kozlov, Diego Darriba, Tomáš Flouri, Benoit Morel, and Alexandros Stamatakis (2019) RAxML-NG: A fast, scalable, and user-friendly tool for maximum likelihood phylogenetic inference. Bioinformatics, btz305 [doi:10.1093/bioinformatics/btz305](https://doi.org/10.1093/bioinformatics/btz305)
 
-Directory containing files to build documentation hosted at ReadTheDocs.
+```bash
+scripts/tree/phylo/raxml_ng_build_tree.sh \
+ <path to contenated fasta file> \
+ <path to partition file> \
+ <path to output dir>
+```
 
-### **notebooks**
+The output directory is created by the script
 
-Directory containing all Jupyter notebooks, and html copies used for easier in-browser viewing via the GitHub pages. These notebooks include the data outputs from using `cfv_investigator`, how to use the package and how the package works.
+## A distance based approach
 
-### **tests**
+An alternative approach is to calculate genome distances from the Average Nucleotide Identity (ANI).
 
-Directory containing all `pytest` files for testing `pyrewton`, including subdirectories for test inputs and targets. Each module/submodule has its own specific test input and target subdirectory.
+The software package `pyani` [Pritchard et al.](https://doi.org/10.1039/C5AY02550H) can be used to calculate the ANI between all possible pairs of genomes, for a set of given genomes.
 
-### **cazomevolve**
+> Pritchard et al. (2016) "Genomics and taxonomy in diagnostics for food security: soft-rotting enterobacterial plant pathogens" Anal. Methods 8, 12-24
 
-Directory containing all `pyrewton` program modules (including all submodules and Python scripts).
-<p>&nbsp;</p>
+An example of using `pyani` to generate a ANI-based dendrogram can be found in [Hobbs et al.](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto/)
 
-## Modules
+The installation instructions for [`pyani`](https://github.com/widdowquinn/pyani)can be found in its [GitHub repo](https://github.com/widdowquinn/pyani). We recommend using >= version 0.3.0-alpha.
 
-_Please find more detailed documentation at for operation and troubleshooting at [Read the Docs](https://phd-project-scripts.readthedocs.io/en/latest/)_
+`cazomevolve` includes bash scripts to coordinate using `pyani`:
 
-This is an overview of the functionalities of each module within `pyrewton`, as well as basics of operation. For more detailed documentation on the operation of each module and indiviudal Python scripts please see the documentation at [Read the Docs](https://phd-project-scripts.readthedocs.io/en/latest/)
+```bash
+scripts/tree/ani/run_anim.sh \
+  <pyani and log file output directory> \
+  <dir containing genome .faa seqs> \
+  <plot and matrix output dir>
+```
 
-### **utilities**
+The R script `build_anim_tree.R` (in `scripts/tree/ani/`) can be used and modified to create to infer genome distances from the all-vs-all ANI analysis and construct a dendrogram from the distances.
 
-Contains all functions that are called from other Python scripts for building command-line parsers and loggers. Includes the submodule **file_io**, which contains functions that are called from other Python scripts for handling directories and files in `pyrewton`, including retrieving program inputs and creating output directories.
+## Find networks of co-evolving CAZy families
+    
+Use the Python package `coinfinder` ([Whelan et al., 2020](https://www.microbiologyresearch.org/content/journal/mgen/10.1099/mgen.0.000338)) to identify networks of co-evolving CAZy families.
 
-### **ncbi**
+> Fiona J. Whelan, Martin Rusilowicz, & James O. McInerney. "Coinfinder: detecting significant associations and dissociations in pangenomes." doi: https://doi.org/10.1099/mgen.0.000338
+    
+See the `coinfinder` [documentation](https://github.com/fwhelan/coinfinder) for details.
+    
+To customise the resulting phylogenetic tree and heatmap, edit the R script `network.R` in `coinfinder`.
 
-Modules that are involved in retrieving handling data from NCBI. This includes retrieval of genomic accession numbers and source organism taxonomic data.
+An example of where this is done can be found in [Hobbs _et al._ SI information on the exploration of _Pectobacteriaceae_ CAZomes](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto).
 
-### **covariance**
+# Build dendograms based upon CAZome compositions, and compare against the phylogenetic tree
 
-Modules that build the data set required for calculating the covariance, calculate the covariance of CAZy family annotations for all genomic accessions retrieved and taxonomic specific groups.
+....
```

