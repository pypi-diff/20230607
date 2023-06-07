# Comparing `tmp/seqlike-1.5.1.tar.gz` & `tmp/seqlike-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqlike-1.5.1.tar", last modified: Thu Feb  9 20:31:27 2023, max compression
+gzip compressed data, was "seqlike-1.5.2.tar", last modified: Wed Jun  7 17:26:59 2023, max compression
```

## Comparing `seqlike-1.5.1.tar` & `seqlike-1.5.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:31:27.121758 seqlike-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-02-09 20:31:15.000000 seqlike-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-02-09 20:31:27.117758 seqlike-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-02-09 20:31:15.000000 seqlike-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-09 20:31:15.000000 seqlike-1.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:31:27.117758 seqlike-1.5.1/seqlike/
--rw-r--r--   0 runner    (1001) docker     (123)    33845 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/AlignCommandline.py
--rw-r--r--   0 runner    (1001) docker     (123)   592752 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/FreeMono.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/Mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/MutationSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42630 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/SeqLike.py
--rw-r--r--   0 runner    (1001) docker     (123)    21270 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/SeqLikeAccessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/SequenceLike.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/alignment_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/alignment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/alphabets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/codon_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/draw_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:31:27.117758 seqlike-1.5.1/seqlike/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/utils/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/utils/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-02-09 20:31:15.000000 seqlike-1.5.1/seqlike/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 20:31:18.000000 seqlike-1.5.1/seqlike/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:31:27.117758 seqlike-1.5.1/seqlike.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-02-09 20:31:27.000000 seqlike-1.5.1/seqlike.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-02-09 20:31:27.000000 seqlike-1.5.1/seqlike.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:31:27.000000 seqlike-1.5.1/seqlike.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-09 20:31:27.000000 seqlike-1.5.1/seqlike.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-09 20:31:27.000000 seqlike-1.5.1/seqlike.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 20:31:27.121758 seqlike-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-02-09 20:31:18.000000 seqlike-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:31:27.117758 seqlike-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_Mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22160 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_SeqLike.py
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_SeqLikeAccessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_SeqLike_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_SeqLike_conversion_to_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_SeqLike_magic_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_SeqLike_to_other_seq_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_SequenceLike.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_aaSeqLike_ntSeqLike.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_codon_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_draw_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-09 20:31:15.000000 seqlike-1.5.1/tests/test_identify_alphabet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:26:59.488390 seqlike-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-07 17:26:42.000000 seqlike-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-06-07 17:26:59.488390 seqlike-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-06-07 17:26:42.000000 seqlike-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-07 17:26:42.000000 seqlike-1.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:26:59.484389 seqlike-1.5.2/seqlike/
+-rw-r--r--   0 runner    (1001) docker     (123)    33845 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/AlignCommandline.py
+-rw-r--r--   0 runner    (1001) docker     (123)   592752 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/FreeMono.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/Mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/MutationSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42630 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/SeqLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21270 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/SeqLikeAccessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/SequenceLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/alignment_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/alignment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/alphabets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/codon_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/draw_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:26:59.484389 seqlike-1.5.2/seqlike/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/utils/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/utils/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-07 17:26:42.000000 seqlike-1.5.2/seqlike/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 17:26:49.000000 seqlike-1.5.2/seqlike/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:26:59.484389 seqlike-1.5.2/seqlike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-06-07 17:26:59.000000 seqlike-1.5.2/seqlike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-07 17:26:59.000000 seqlike-1.5.2/seqlike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:26:59.000000 seqlike-1.5.2/seqlike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 17:26:59.000000 seqlike-1.5.2/seqlike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 17:26:59.000000 seqlike-1.5.2/seqlike.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 17:26:59.488390 seqlike-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-06-07 17:26:49.000000 seqlike-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:26:59.488390 seqlike-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_Mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22160 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_SeqLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_SeqLikeAccessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_SeqLike_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_SeqLike_conversion_to_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_SeqLike_magic_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_SeqLike_to_other_seq_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_SequenceLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_aaSeqLike_ntSeqLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_codon_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_draw_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 17:26:42.000000 seqlike-1.5.2/tests/test_identify_alphabet.py
```

### Comparing `seqlike-1.5.1/LICENSE` & `seqlike-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/PKG-INFO` & `seqlike-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqlike
-Version: 1.5.1
+Version: 1.5.2
 Home-page: https://github.com/modernatx/seqlike
 Project-URL: Documentation, https://modernatx.github.io/seqlike
 Project-URL: Source Code, https://github.com/modernatx/seqlike
 Project-URL: Issue Tracker, https://github.com/modernatx/seqlike/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seqlike Version: 1.5.1 Home-page: https://
+Metadata-Version: 2.1 Name: seqlike Version: 1.5.2 Home-page: https://
 github.com/modernatx/seqlike Project-URL: Documentation, https://
 modernatx.github.io/seqlike Project-URL: Source Code, https://github.com/
 modernatx/seqlike Project-URL: Issue Tracker, https://github.com/modernatx/
 seqlike/issues Classifier: Intended Audience :: Science/Research Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `seqlike-1.5.1/README.md` & `seqlike-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/pyproject.toml` & `seqlike-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/AlignCommandline.py` & `seqlike-1.5.2/seqlike/AlignCommandline.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/FreeMono.ttf` & `seqlike-1.5.2/seqlike/FreeMono.ttf`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/Mutation.py` & `seqlike-1.5.2/seqlike/Mutation.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/MutationSet.py` & `seqlike-1.5.2/seqlike/MutationSet.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/SeqLike.py` & `seqlike-1.5.2/seqlike/SeqLike.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/SeqLikeAccessor.py` & `seqlike-1.5.2/seqlike/SeqLikeAccessor.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/SequenceLike.py` & `seqlike-1.5.2/seqlike/SequenceLike.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/alignment_commands.py` & `seqlike-1.5.2/seqlike/alignment_commands.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/alignment_utils.py` & `seqlike-1.5.2/seqlike/alignment_utils.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/alphabets.py` & `seqlike-1.5.2/seqlike/alphabets.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/codon_tables.py` & `seqlike-1.5.2/seqlike/codon_tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,21 +75,21 @@
     "TTG": "L",
     "TTT": "F",
     "NNN": "X",
     "---": "-",
 }
 
 # https://github.com/Edinburgh-Genome-Foundry/codon-usage-tables/blob/master/codon_usage_data/tables/h_sapiens_9606.csv
-human_codon_table = get_codons_table("h_sapiens_9606")
+human_codon_table = get_codons_table("h_sapiens_9606").copy()
 
 # https://github.com/Edinburgh-Genome-Foundry/codon-usage-tables/blob/master/codon_usage_data/tables/s_cerevisiae_4932.csv
-yeast_codon_table = get_codons_table("s_cerevisiae_4932")
+yeast_codon_table = get_codons_table("s_cerevisiae_4932").copy()
 
 # https://github.com/Edinburgh-Genome-Foundry/codon-usage-tables/blob/master/codon_usage_data/tables/e_coli_316407.csv
-ecoli_codon_table = get_codons_table("e_coli_316407")
+ecoli_codon_table = get_codons_table("e_coli_316407").copy()
 
 random_codon_table = {
     "*": {"TAA": 0.33, "TAG": 0.33, "TGA": 0.33},
     "A": {"GCA": 0.25, "GCC": 0.25, "GCG": 0.25, "GCT": 0.25},
     "C": {"TGC": 0.50, "TGT": 0.50},
     "D": {"GAC": 0.50, "GAT": 0.50},
     "E": {"GAA": 0.50, "GAG": 0.50},
```

### Comparing `seqlike-1.5.1/seqlike/draw_utils.py` & `seqlike-1.5.2/seqlike/draw_utils.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/encoders.py` & `seqlike-1.5.2/seqlike/encoders.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/utils/constructor.py` & `seqlike-1.5.2/seqlike/utils/constructor.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/utils/sequences.py` & `seqlike-1.5.2/seqlike/utils/sequences.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike/utils/validation.py` & `seqlike-1.5.2/seqlike/utils/validation.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/seqlike.egg-info/PKG-INFO` & `seqlike-1.5.2/seqlike.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqlike
-Version: 1.5.1
+Version: 1.5.2
 Home-page: https://github.com/modernatx/seqlike
 Project-URL: Documentation, https://modernatx.github.io/seqlike
 Project-URL: Source Code, https://github.com/modernatx/seqlike
 Project-URL: Issue Tracker, https://github.com/modernatx/seqlike/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seqlike Version: 1.5.1 Home-page: https://
+Metadata-Version: 2.1 Name: seqlike Version: 1.5.2 Home-page: https://
 github.com/modernatx/seqlike Project-URL: Documentation, https://
 modernatx.github.io/seqlike Project-URL: Source Code, https://github.com/
 modernatx/seqlike Project-URL: Issue Tracker, https://github.com/modernatx/
 seqlike/issues Classifier: Intended Audience :: Science/Research Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `seqlike-1.5.1/seqlike.egg-info/SOURCES.txt` & `seqlike-1.5.2/seqlike.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/setup.py` & `seqlike-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 test_requires = [
     "pytest",
     "pytest-regtest",
 ]
 
 setup(
     name="seqlike",
-    version="1.5.1",
+    version="1.5.2",
     packages=find_packages(),  # https://stackoverflow.com/a/22442340
     cmdclass={"install": InstallWrapper},
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/modernatx/seqlike",
     project_urls={
         "Documentation": "https://modernatx.github.io/seqlike",
```

### Comparing `seqlike-1.5.1/tests/test_Mutation.py` & `seqlike-1.5.2/tests/test_Mutation.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/tests/test_SeqLike.py` & `seqlike-1.5.2/tests/test_SeqLike.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/tests/test_SeqLikeAccessor.py` & `seqlike-1.5.2/tests/test_SeqLikeAccessor.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/tests/test_SeqLike_alignment.py` & `seqlike-1.5.2/tests/test_SeqLike_alignment.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/tests/test_SeqLike_conversion_to_numerical.py` & `seqlike-1.5.2/tests/test_SeqLike_conversion_to_numerical.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/tests/test_SeqLike_magic_methods.py` & `seqlike-1.5.2/tests/test_SeqLike_magic_methods.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/tests/test_SeqLike_to_other_seq_formats.py` & `seqlike-1.5.2/tests/test_SeqLike_to_other_seq_formats.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/tests/test_SequenceLike.py` & `seqlike-1.5.2/tests/test_SequenceLike.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/tests/test_aaSeqLike_ntSeqLike.py` & `seqlike-1.5.2/tests/test_aaSeqLike_ntSeqLike.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/tests/test_assets.py` & `seqlike-1.5.2/tests/test_assets.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/tests/test_codon_tables.py` & `seqlike-1.5.2/tests/test_codon_tables.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 
+from python_codon_tables import get_codons_table
 from seqlike import aaSeqLike
 from seqlike.codon_tables import (
     codon_table_to_codon_map,
     human_codon_table,
     ecoli_codon_table,
     sort_codon_table_by_frequency,
 )
@@ -28,7 +29,15 @@
     codon = aaSeqLike(letter).back_translate(codon_map=human_codon_map)
     assert list(human_codon_table[letter])[0] == str(codon)
 
     # deterministic sorted
     human_codon_map = codon_table_to_codon_map(sort_codon_table_by_frequency(human_codon_table))
     codon = aaSeqLike(letter).back_translate(codon_map=human_codon_map)
     assert sorted(human_codon_table[letter].items(), key=lambda x: x[1], reverse=True)[0][0] == str(codon)
+
+
+@pytest.mark.parametrize("codon_table_name", ["h_sapiens_9606", "s_cerevisiae_4932"])
+def test_codon_table(codon_table_name):
+    assert ''.join(sorted(human_codon_table.keys())) == '*-ACDEFGHIKLMNPQRSTVWXY'
+
+    codons_table = get_codons_table(codon_table_name)
+    assert ''.join(sorted(codons_table.keys())) == '*ACDEFGHIKLMNPQRSTVWY'
```

### Comparing `seqlike-1.5.1/tests/test_draw_utils.py` & `seqlike-1.5.2/tests/test_draw_utils.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/tests/test_encoders.py` & `seqlike-1.5.2/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `seqlike-1.5.1/tests/test_identify_alphabet.py` & `seqlike-1.5.2/tests/test_identify_alphabet.py`

 * *Files identical despite different names*

