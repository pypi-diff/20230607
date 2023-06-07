# Comparing `tmp/REaLTabFormer-0.1.1.tar.gz` & `tmp/REaLTabFormer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "REaLTabFormer-0.1.1.tar", last modified: Tue Feb  7 02:20:58 2023, max compression
+gzip compressed data, was "REaLTabFormer-0.1.2.tar", last modified: Wed Jun  7 20:08:25 2023, max compression
```

## Comparing `REaLTabFormer-0.1.1.tar` & `REaLTabFormer-0.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.633348 REaLTabFormer-0.1.1/
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.621491 REaLTabFormer-0.1.1/.github/
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.624903 REaLTabFormer-0.1.1/.github/workflows/
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1035 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/.github/workflows/book.yml
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1856 2023-02-06 02:24:24.000000 REaLTabFormer-0.1.1/.gitignore
--rw-r--r--   0 avsolatorio   (501) staff       (20)     3042 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/.pre-commit-config.yaml
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.625077 REaLTabFormer-0.1.1/.vscode/
--rw-r--r--   0 avsolatorio   (501) staff       (20)      254 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/.vscode/settings.json
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1075 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/LICENSE
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1263 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/Makefile
--rw-r--r--   0 avsolatorio   (501) staff       (20)    11403 2023-02-07 02:20:58.633011 REaLTabFormer-0.1.1/PKG-INFO
--rw-r--r--   0 avsolatorio   (501) staff       (20)     9409 2023-02-07 02:17:37.000000 REaLTabFormer-0.1.1/README.md
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.625240 REaLTabFormer-0.1.1/colab/
--rw-r--r--   0 avsolatorio   (501) staff       (20)   264453 2023-02-07 02:17:12.000000 REaLTabFormer-0.1.1/colab/REaLTabFormer_GeoValidator_Example.ipynb
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.625958 REaLTabFormer-0.1.1/devtools/
--rw-r--r--   0 avsolatorio   (501) staff       (20)      723 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/devtools/print_env.sh
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.626673 REaLTabFormer-0.1.1/docs/
--rw-r--r--   0 avsolatorio   (501) staff       (20)      538 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/docs/_config.yml
--rw-r--r--   0 avsolatorio   (501) staff       (20)      155 2023-02-06 02:25:45.000000 REaLTabFormer-0.1.1/docs/_toc.yml
--rw-r--r--   0 avsolatorio   (501) staff       (20)       21 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/docs/requirements.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)      122 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/environment.yml
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.628424 REaLTabFormer-0.1.1/img/
--rw-r--r--   0 avsolatorio   (501) staff       (20)   123234 2023-02-06 22:11:22.000000 REaLTabFormer-0.1.1/img/CA-housing-raw-samples.png
--rw-r--r--   0 avsolatorio   (501) staff       (20)   126314 2023-02-06 22:11:52.000000 REaLTabFormer-0.1.1/img/CA-housing-validated-samples.png
--rw-r--r--   0 avsolatorio   (501) staff       (20)   490438 2023-02-06 19:49:48.000000 REaLTabFormer-0.1.1/img/REalTabFormer_Final_EQ.png
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1364 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/pyproject.toml
--rw-r--r--   0 avsolatorio   (501) staff       (20)       38 2023-02-07 02:20:58.633420 REaLTabFormer-0.1.1/setup.cfg
--rw-r--r--   0 avsolatorio   (501) staff       (20)      129 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/setup.py
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.622194 REaLTabFormer-0.1.1/src/
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.629964 REaLTabFormer-0.1.1/src/REaLTabFormer.egg-info/
--rw-r--r--   0 avsolatorio   (501) staff       (20)    11403 2023-02-07 02:20:58.000000 REaLTabFormer-0.1.1/src/REaLTabFormer.egg-info/PKG-INFO
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1134 2023-02-07 02:20:58.000000 REaLTabFormer-0.1.1/src/REaLTabFormer.egg-info/SOURCES.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)        1 2023-02-07 02:20:58.000000 REaLTabFormer-0.1.1/src/REaLTabFormer.egg-info/dependency_links.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)      133 2023-02-07 02:20:58.000000 REaLTabFormer-0.1.1/src/REaLTabFormer.egg-info/requires.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)       14 2023-02-07 02:20:58.000000 REaLTabFormer-0.1.1/src/REaLTabFormer.egg-info/top_level.txt
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.631874 REaLTabFormer-0.1.1/src/realtabformer/
--rw-r--r--   0 avsolatorio   (501) staff       (20)        6 2023-02-07 02:17:14.000000 REaLTabFormer-0.1.1/src/realtabformer/VERSION
--rw-r--r--   0 avsolatorio   (501) staff       (20)      504 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/src/realtabformer/__init__.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)      272 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/src/realtabformer/__main__.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)    24266 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/src/realtabformer/data_utils.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)    66554 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/src/realtabformer/realtabformer.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)    29165 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/src/realtabformer/rtf_analyze.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     3233 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/src/realtabformer/rtf_datacollator.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)      843 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/src/realtabformer/rtf_exceptions.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)    41526 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/src/realtabformer/rtf_sampler.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     7983 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/src/realtabformer/rtf_trainer.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1961 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/src/realtabformer/rtf_validators.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)      297 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/test_requirements.txt
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.622337 REaLTabFormer-0.1.1/tests/
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-02-07 02:20:58.632706 REaLTabFormer-0.1.1/tests/realtabformer/
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1310 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/tests/realtabformer/fixtures.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)    10899 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/tests/realtabformer/test_data_utils.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     7648 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/tests/realtabformer/test_realtabformer.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1724 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/tests/realtabformer/test_rtf_sampler.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)       88 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.1/trufflehog-ignore.txt
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.780517 REaLTabFormer-0.1.2/
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.764886 REaLTabFormer-0.1.2/.github/
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.767679 REaLTabFormer-0.1.2/.github/workflows/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1035 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/.github/workflows/book.yml
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1856 2023-02-06 02:24:24.000000 REaLTabFormer-0.1.2/.gitignore
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     3042 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/.pre-commit-config.yaml
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.767825 REaLTabFormer-0.1.2/.vscode/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      254 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/.vscode/settings.json
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1075 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/LICENSE
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1263 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/Makefile
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    11419 2023-06-07 20:08:25.780318 REaLTabFormer-0.1.2/PKG-INFO
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     9425 2023-02-08 20:37:30.000000 REaLTabFormer-0.1.2/README.md
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.767976 REaLTabFormer-0.1.2/colab/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)   264453 2023-02-08 20:37:53.000000 REaLTabFormer-0.1.2/colab/REaLTabFormer_GeoValidator_Example.ipynb
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.768278 REaLTabFormer-0.1.2/devtools/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      723 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/devtools/print_env.sh
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.768677 REaLTabFormer-0.1.2/docs/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      538 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/docs/_config.yml
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      155 2023-02-06 02:25:45.000000 REaLTabFormer-0.1.2/docs/_toc.yml
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       21 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/docs/requirements.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      122 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/environment.yml
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.769276 REaLTabFormer-0.1.2/img/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)   123234 2023-02-06 22:11:22.000000 REaLTabFormer-0.1.2/img/CA-housing-raw-samples.png
+-rw-r--r--   0 avsolatorio   (501) staff       (20)   126314 2023-02-06 22:11:52.000000 REaLTabFormer-0.1.2/img/CA-housing-validated-samples.png
+-rw-r--r--   0 avsolatorio   (501) staff       (20)   490438 2023-02-06 19:49:48.000000 REaLTabFormer-0.1.2/img/REalTabFormer_Final_EQ.png
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1364 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/pyproject.toml
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       38 2023-06-07 20:08:25.780560 REaLTabFormer-0.1.2/setup.cfg
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      129 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/setup.py
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.765446 REaLTabFormer-0.1.2/src/
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.770260 REaLTabFormer-0.1.2/src/REaLTabFormer.egg-info/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    11419 2023-06-07 20:08:25.000000 REaLTabFormer-0.1.2/src/REaLTabFormer.egg-info/PKG-INFO
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1134 2023-06-07 20:08:25.000000 REaLTabFormer-0.1.2/src/REaLTabFormer.egg-info/SOURCES.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)        1 2023-06-07 20:08:25.000000 REaLTabFormer-0.1.2/src/REaLTabFormer.egg-info/dependency_links.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      133 2023-06-07 20:08:25.000000 REaLTabFormer-0.1.2/src/REaLTabFormer.egg-info/requires.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       14 2023-06-07 20:08:25.000000 REaLTabFormer-0.1.2/src/REaLTabFormer.egg-info/top_level.txt
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.776389 REaLTabFormer-0.1.2/src/realtabformer/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)        6 2023-06-07 20:04:14.000000 REaLTabFormer-0.1.2/src/realtabformer/VERSION
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      504 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/src/realtabformer/__init__.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      272 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/src/realtabformer/__main__.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    24285 2023-03-20 16:29:07.000000 REaLTabFormer-0.1.2/src/realtabformer/data_utils.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    66742 2023-02-08 20:37:30.000000 REaLTabFormer-0.1.2/src/realtabformer/realtabformer.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    29164 2023-02-08 20:37:30.000000 REaLTabFormer-0.1.2/src/realtabformer/rtf_analyze.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     3233 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/src/realtabformer/rtf_datacollator.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      843 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/src/realtabformer/rtf_exceptions.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    41581 2023-02-08 20:37:30.000000 REaLTabFormer-0.1.2/src/realtabformer/rtf_sampler.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     7983 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/src/realtabformer/rtf_trainer.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1960 2023-02-08 20:37:30.000000 REaLTabFormer-0.1.2/src/realtabformer/rtf_validators.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      297 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/test_requirements.txt
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.765567 REaLTabFormer-0.1.2/tests/
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-06-07 20:08:25.780037 REaLTabFormer-0.1.2/tests/realtabformer/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1310 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/tests/realtabformer/fixtures.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    10899 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/tests/realtabformer/test_data_utils.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     7648 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/tests/realtabformer/test_realtabformer.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1724 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/tests/realtabformer/test_rtf_sampler.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       88 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.2/trufflehog-ignore.txt
```

### Comparing `REaLTabFormer-0.1.1/.github/workflows/book.yml` & `REaLTabFormer-0.1.2/.github/workflows/book.yml`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/.gitignore` & `REaLTabFormer-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/.pre-commit-config.yaml` & `REaLTabFormer-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/LICENSE` & `REaLTabFormer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/Makefile` & `REaLTabFormer-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/PKG-INFO` & `REaLTabFormer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REaLTabFormer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A novel method for generating tabular and relational data using language models.
 Author-email: "Aivin V. Solatorio" <asolatorio@worldbank.org>
 License: MIT License
         
         Copyright (c) 2022 Aivin V. Solatorio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,29 +33,30 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href="https://colab.research.google.com/github/avsolatorio/RealTabFormer/blob/main/colab/REaLTabFormer_GeoValidator_Example.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
-# RealTabFormer
+# REaLTabFormer
 
 The REaLTabFormer (Realistic Relational and Tabular Data using Transformers) offers a unified framework for synthesizing tabular data of different types. A sequence-to-sequence (Seq2Seq) model is used for generating synthetic relational datasets. The REaLTabFormer model for a non-relational tabular data uses GPT-2, and can be used out-of-the-box to model any tabular data with independent observations.
 <br>
 <br>
 <p align="center">
-<img src="https://github.com/avsolatorio/RealTabFormer/raw/main/img/REalTabFormer_Final_EQ.png" style="width:50%"/>
+<img src="https://github.com/avsolatorio/RealTabFormer/raw/main/img/REalTabFormer_Final_EQ.png" style="width:75%"/>
 </p>
 <p align="center">
 <strong>REaLTabFormer: Generating Realistic Relational and Tabular Data using Transformers</strong>
 <br>
 <a href="https://arxiv.org/abs/2302.02041">Paper on ArXiv</a>
 </p>
 <br>
-Tabular data is a common form of organizing data. Multiple models are available to generate synthetic tabular datasets where observations are independent, but few have the ability to produce relational datasets. Modeling relational data is challenging as it requires modeling both a "parent" table and its relationships across tables. We introduce REaLTabFormer (Realistic Relational and Tabular Transformer), a tabular and relational synthetic data generation model. It first creates a parent table using an autoregressive GPT-2 model, then generates the relational dataset conditioned on the parent table using a sequence-to-sequence (Seq2Seq) model. We implement target masking to prevent data copying and propose the $Q_\delta$ statistic and statistical bootstrapping to detect overfitting. Experiments using real-world datasets show that REaLTabFormer captures the relational structure better than a baseline model. REaLTabFormer also achieves state-of-the-art results on prediction tasks, "out-of-the-box", for large non-relational datasets without needing fine-tuning.
+<!---
+Tabular data is a common form of organizing data. Multiple models are available to generate synthetic tabular datasets where observations are independent, but few have the ability to produce relational datasets. Modeling relational data is challenging as it requires modeling both a "parent" table and its relationships across tables. We introduce REaLTabFormer (Realistic Relational and Tabular Transformer), a tabular and relational synthetic data generation model. It first creates a parent table using an autoregressive GPT-2 model, then generates the relational dataset conditioned on the parent table using a sequence-to-sequence (Seq2Seq) model. We implement target masking to prevent data copying and propose the $Q_\delta$ statistic and statistical bootstrapping to detect overfitting. Experiments using real-world datasets show that REaLTabFormer captures the relational structure better than a baseline model. REaLTabFormer also achieves state-of-the-art results on prediction tasks, "out-of-the-box", for large non-relational datasets without needing fine-tuning. --->
 
 
 ## Installation
 
 REaLTabFormer is available on PyPi and can be easily installed with [pip](https://pypi.org/project/pip/) (Python version >= 3.7):
 
 ```bash
@@ -170,14 +171,15 @@
 
 The REaLTabFormer framework provides an interface to easily build observation validators for filtering invalid synthetic samples. We show an example of using the `GeoValidator` below. The chart on the left shows the distribution of the generated latitude and longitude without validation. The chart on the right shows the synthetic samples with observations that have been validated using the `GeoValidator` with the California boundary. Still, even when we did not optimally train the model for generating this, the invalid samples (falling outside of the boundary) are scarce from the generated data with no validator.
 
 <div align=center>
     <img src="https://github.com/avsolatorio/RealTabFormer/raw/main/img/CA-housing-raw-samples.png" style="width:35%; padding-right:5%;"/>
     <img src="https://github.com/avsolatorio/RealTabFormer/raw/main/img/CA-housing-validated-samples.png" style="width:35%; padding-left:5%;"/>
 </div>
+<br>
 
 ```Python
 # !pip install geopandas &> /dev/null
 # !pip install realtabformer &> /dev/null
 # !git clone https://github.com/joncutrer/geopandas-tutorial.git &> /dev/null
 import geopandas
 import seaborn as sns
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: REaLTabFormer Version: 0.1.1 Summary: A novel
+Metadata-Version: 2.1 Name: REaLTabFormer Version: 0.1.2 Summary: A novel
 method for generating tabular and relational data using language models.
 Author-email: "Aivin V. Solatorio"
 worldbank.org> License: MIT License Copyright (c) 2022 Aivin V. Solatorio
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -19,42 +19,28 @@
 avsolatorio/REaLTabFormer Project-URL: Documentation, https://
 avsolatorio.github.io/REaLTabFormer/ Keywords: REaLTabFormer,deep
 learning,tabular data,transformers,data generation,seq2seq model,synthetic
 data,pytorch,language models,synthetic data generation Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE [Open_In_Colab] #
-RealTabFormer The REaLTabFormer (Realistic Relational and Tabular Data using
+REaLTabFormer The REaLTabFormer (Realistic Relational and Tabular Data using
 Transformers) offers a unified framework for synthesizing tabular data of
 different types. A sequence-to-sequence (Seq2Seq) model is used for generating
 synthetic relational datasets. The REaLTabFormer model for a non-relational
 tabular data uses GPT-2, and can be used out-of-the-box to model any tabular
 data with independent observations.
 
           [https://github.com/avsolatorio/RealTabFormer/raw/main/img/
                           REalTabFormer_Final_EQ.png]
      REaLTabFormer: Generating Realistic Relational and Tabular Data using
                                  Transformers
                                 Paper_on_ArXiv
 
-Tabular data is a common form of organizing data. Multiple models are available
-to generate synthetic tabular datasets where observations are independent, but
-few have the ability to produce relational datasets. Modeling relational data
-is challenging as it requires modeling both a "parent" table and its
-relationships across tables. We introduce REaLTabFormer (Realistic Relational
-and Tabular Transformer), a tabular and relational synthetic data generation
-model. It first creates a parent table using an autoregressive GPT-2 model,
-then generates the relational dataset conditioned on the parent table using a
-sequence-to-sequence (Seq2Seq) model. We implement target masking to prevent
-data copying and propose the $Q_\delta$ statistic and statistical bootstrapping
-to detect overfitting. Experiments using real-world datasets show that
-REaLTabFormer captures the relational structure better than a baseline model.
-REaLTabFormer also achieves state-of-the-art results on prediction tasks, "out-
-of-the-box", for large non-relational datasets without needing fine-tuning. ##
-Installation REaLTabFormer is available on PyPi and can be easily installed
+ ## Installation REaLTabFormer is available on PyPi and can be easily installed
 with [pip](https://pypi.org/project/pip/) (Python version >= 3.7): ```bash pip
 install realtabformer ``` ## Usage We show examples of using the REaLTabFormer
 for modeling and generating synthetic data from a trained model. ###
 REaLTabFormer for regular tabular data ```Python # pip install realtabformer
 import pandas as pd from realtabformer import REaLTabFormer df = pd.read_csv
 ("foo.csv") # NOTE: Remove any unique identifiers in the # data that you don't
 want to be modeled. # Non-relational or parent table. rtf_model = REaLTabFormer
@@ -94,14 +80,15 @@
 shows the synthetic samples with observations that have been validated using
 the `GeoValidator` with the California boundary. Still, even when we did not
 optimally train the model for generating this, the invalid samples (falling
 outside of the boundary) are scarce from the generated data with no validator.
   [https://github.com/avsolatorio/RealTabFormer/raw/main/img/CA-housing-raw-
   samples.png] [https://github.com/avsolatorio/RealTabFormer/raw/main/img/CA-
                         housing-validated-samples.png]
+
 ```Python # !pip install geopandas &> /dev/null # !pip install realtabformer &>
 /dev/null # !git clone https://github.com/joncutrer/geopandas-tutorial.git &> /
 dev/null import geopandas import seaborn as sns import matplotlib.pyplot as plt
 from realtabformer import REaLTabFormer from realtabformer import
 rtf_validators as rtf_val from shapely.geometry import Polygon, LineString,
 Point, MultiPolygon from sklearn.datasets import fetch_california_housing def
 plot_sf(data, samples, title=None): xlims = (-126, -113.5) ylims = (31, 43)
```

### Comparing `REaLTabFormer-0.1.1/README.md` & `REaLTabFormer-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 <a href="https://colab.research.google.com/github/avsolatorio/RealTabFormer/blob/main/colab/REaLTabFormer_GeoValidator_Example.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
-# RealTabFormer
+# REaLTabFormer
 
 The REaLTabFormer (Realistic Relational and Tabular Data using Transformers) offers a unified framework for synthesizing tabular data of different types. A sequence-to-sequence (Seq2Seq) model is used for generating synthetic relational datasets. The REaLTabFormer model for a non-relational tabular data uses GPT-2, and can be used out-of-the-box to model any tabular data with independent observations.
 <br>
 <br>
 <p align="center">
-<img src="https://github.com/avsolatorio/RealTabFormer/raw/main/img/REalTabFormer_Final_EQ.png" style="width:50%"/>
+<img src="https://github.com/avsolatorio/RealTabFormer/raw/main/img/REalTabFormer_Final_EQ.png" style="width:75%"/>
 </p>
 <p align="center">
 <strong>REaLTabFormer: Generating Realistic Relational and Tabular Data using Transformers</strong>
 <br>
 <a href="https://arxiv.org/abs/2302.02041">Paper on ArXiv</a>
 </p>
 <br>
-Tabular data is a common form of organizing data. Multiple models are available to generate synthetic tabular datasets where observations are independent, but few have the ability to produce relational datasets. Modeling relational data is challenging as it requires modeling both a "parent" table and its relationships across tables. We introduce REaLTabFormer (Realistic Relational and Tabular Transformer), a tabular and relational synthetic data generation model. It first creates a parent table using an autoregressive GPT-2 model, then generates the relational dataset conditioned on the parent table using a sequence-to-sequence (Seq2Seq) model. We implement target masking to prevent data copying and propose the $Q_\delta$ statistic and statistical bootstrapping to detect overfitting. Experiments using real-world datasets show that REaLTabFormer captures the relational structure better than a baseline model. REaLTabFormer also achieves state-of-the-art results on prediction tasks, "out-of-the-box", for large non-relational datasets without needing fine-tuning.
+<!---
+Tabular data is a common form of organizing data. Multiple models are available to generate synthetic tabular datasets where observations are independent, but few have the ability to produce relational datasets. Modeling relational data is challenging as it requires modeling both a "parent" table and its relationships across tables. We introduce REaLTabFormer (Realistic Relational and Tabular Transformer), a tabular and relational synthetic data generation model. It first creates a parent table using an autoregressive GPT-2 model, then generates the relational dataset conditioned on the parent table using a sequence-to-sequence (Seq2Seq) model. We implement target masking to prevent data copying and propose the $Q_\delta$ statistic and statistical bootstrapping to detect overfitting. Experiments using real-world datasets show that REaLTabFormer captures the relational structure better than a baseline model. REaLTabFormer also achieves state-of-the-art results on prediction tasks, "out-of-the-box", for large non-relational datasets without needing fine-tuning. --->
 
 
 ## Installation
 
 REaLTabFormer is available on PyPi and can be easily installed with [pip](https://pypi.org/project/pip/) (Python version >= 3.7):
 
 ```bash
@@ -133,14 +134,15 @@
 
 The REaLTabFormer framework provides an interface to easily build observation validators for filtering invalid synthetic samples. We show an example of using the `GeoValidator` below. The chart on the left shows the distribution of the generated latitude and longitude without validation. The chart on the right shows the synthetic samples with observations that have been validated using the `GeoValidator` with the California boundary. Still, even when we did not optimally train the model for generating this, the invalid samples (falling outside of the boundary) are scarce from the generated data with no validator.
 
 <div align=center>
     <img src="https://github.com/avsolatorio/RealTabFormer/raw/main/img/CA-housing-raw-samples.png" style="width:35%; padding-right:5%;"/>
     <img src="https://github.com/avsolatorio/RealTabFormer/raw/main/img/CA-housing-validated-samples.png" style="width:35%; padding-left:5%;"/>
 </div>
+<br>
 
 ```Python
 # !pip install geopandas &> /dev/null
 # !pip install realtabformer &> /dev/null
 # !git clone https://github.com/joncutrer/geopandas-tutorial.git &> /dev/null
 import geopandas
 import seaborn as sns
```

#### html2text {}

```diff
@@ -1,35 +1,21 @@
-[Open_In_Colab] # RealTabFormer The REaLTabFormer (Realistic Relational and
+[Open_In_Colab] # REaLTabFormer The REaLTabFormer (Realistic Relational and
 Tabular Data using Transformers) offers a unified framework for synthesizing
 tabular data of different types. A sequence-to-sequence (Seq2Seq) model is used
 for generating synthetic relational datasets. The REaLTabFormer model for a
 non-relational tabular data uses GPT-2, and can be used out-of-the-box to model
 any tabular data with independent observations.
 
           [https://github.com/avsolatorio/RealTabFormer/raw/main/img/
                           REalTabFormer_Final_EQ.png]
      REaLTabFormer: Generating Realistic Relational and Tabular Data using
                                  Transformers
                                 Paper_on_ArXiv
 
-Tabular data is a common form of organizing data. Multiple models are available
-to generate synthetic tabular datasets where observations are independent, but
-few have the ability to produce relational datasets. Modeling relational data
-is challenging as it requires modeling both a "parent" table and its
-relationships across tables. We introduce REaLTabFormer (Realistic Relational
-and Tabular Transformer), a tabular and relational synthetic data generation
-model. It first creates a parent table using an autoregressive GPT-2 model,
-then generates the relational dataset conditioned on the parent table using a
-sequence-to-sequence (Seq2Seq) model. We implement target masking to prevent
-data copying and propose the $Q_\delta$ statistic and statistical bootstrapping
-to detect overfitting. Experiments using real-world datasets show that
-REaLTabFormer captures the relational structure better than a baseline model.
-REaLTabFormer also achieves state-of-the-art results on prediction tasks, "out-
-of-the-box", for large non-relational datasets without needing fine-tuning. ##
-Installation REaLTabFormer is available on PyPi and can be easily installed
+ ## Installation REaLTabFormer is available on PyPi and can be easily installed
 with [pip](https://pypi.org/project/pip/) (Python version >= 3.7): ```bash pip
 install realtabformer ``` ## Usage We show examples of using the REaLTabFormer
 for modeling and generating synthetic data from a trained model. ###
 REaLTabFormer for regular tabular data ```Python # pip install realtabformer
 import pandas as pd from realtabformer import REaLTabFormer df = pd.read_csv
 ("foo.csv") # NOTE: Remove any unique identifiers in the # data that you don't
 want to be modeled. # Non-relational or parent table. rtf_model = REaLTabFormer
@@ -69,14 +55,15 @@
 shows the synthetic samples with observations that have been validated using
 the `GeoValidator` with the California boundary. Still, even when we did not
 optimally train the model for generating this, the invalid samples (falling
 outside of the boundary) are scarce from the generated data with no validator.
   [https://github.com/avsolatorio/RealTabFormer/raw/main/img/CA-housing-raw-
   samples.png] [https://github.com/avsolatorio/RealTabFormer/raw/main/img/CA-
                         housing-validated-samples.png]
+
 ```Python # !pip install geopandas &> /dev/null # !pip install realtabformer &>
 /dev/null # !git clone https://github.com/joncutrer/geopandas-tutorial.git &> /
 dev/null import geopandas import seaborn as sns import matplotlib.pyplot as plt
 from realtabformer import REaLTabFormer from realtabformer import
 rtf_validators as rtf_val from shapely.geometry import Polygon, LineString,
 Point, MultiPolygon from sklearn.datasets import fetch_california_housing def
 plot_sf(data, samples, title=None): xlims = (-126, -113.5) ylims = (31, 43)
```

### Comparing `REaLTabFormer-0.1.1/colab/REaLTabFormer_GeoValidator_Example.ipynb` & `REaLTabFormer-0.1.2/colab/REaLTabFormer_GeoValidator_Example.ipynb`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/devtools/print_env.sh` & `REaLTabFormer-0.1.2/devtools/print_env.sh`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/docs/_config.yml` & `REaLTabFormer-0.1.2/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/img/CA-housing-raw-samples.png` & `REaLTabFormer-0.1.2/img/CA-housing-raw-samples.png`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/img/CA-housing-validated-samples.png` & `REaLTabFormer-0.1.2/img/CA-housing-validated-samples.png`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/img/REalTabFormer_Final_EQ.png` & `REaLTabFormer-0.1.2/img/REalTabFormer_Final_EQ.png`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/pyproject.toml` & `REaLTabFormer-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/src/REaLTabFormer.egg-info/PKG-INFO` & `REaLTabFormer-0.1.2/src/REaLTabFormer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REaLTabFormer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A novel method for generating tabular and relational data using language models.
 Author-email: "Aivin V. Solatorio" <asolatorio@worldbank.org>
 License: MIT License
         
         Copyright (c) 2022 Aivin V. Solatorio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,29 +33,30 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href="https://colab.research.google.com/github/avsolatorio/RealTabFormer/blob/main/colab/REaLTabFormer_GeoValidator_Example.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
-# RealTabFormer
+# REaLTabFormer
 
 The REaLTabFormer (Realistic Relational and Tabular Data using Transformers) offers a unified framework for synthesizing tabular data of different types. A sequence-to-sequence (Seq2Seq) model is used for generating synthetic relational datasets. The REaLTabFormer model for a non-relational tabular data uses GPT-2, and can be used out-of-the-box to model any tabular data with independent observations.
 <br>
 <br>
 <p align="center">
-<img src="https://github.com/avsolatorio/RealTabFormer/raw/main/img/REalTabFormer_Final_EQ.png" style="width:50%"/>
+<img src="https://github.com/avsolatorio/RealTabFormer/raw/main/img/REalTabFormer_Final_EQ.png" style="width:75%"/>
 </p>
 <p align="center">
 <strong>REaLTabFormer: Generating Realistic Relational and Tabular Data using Transformers</strong>
 <br>
 <a href="https://arxiv.org/abs/2302.02041">Paper on ArXiv</a>
 </p>
 <br>
-Tabular data is a common form of organizing data. Multiple models are available to generate synthetic tabular datasets where observations are independent, but few have the ability to produce relational datasets. Modeling relational data is challenging as it requires modeling both a "parent" table and its relationships across tables. We introduce REaLTabFormer (Realistic Relational and Tabular Transformer), a tabular and relational synthetic data generation model. It first creates a parent table using an autoregressive GPT-2 model, then generates the relational dataset conditioned on the parent table using a sequence-to-sequence (Seq2Seq) model. We implement target masking to prevent data copying and propose the $Q_\delta$ statistic and statistical bootstrapping to detect overfitting. Experiments using real-world datasets show that REaLTabFormer captures the relational structure better than a baseline model. REaLTabFormer also achieves state-of-the-art results on prediction tasks, "out-of-the-box", for large non-relational datasets without needing fine-tuning.
+<!---
+Tabular data is a common form of organizing data. Multiple models are available to generate synthetic tabular datasets where observations are independent, but few have the ability to produce relational datasets. Modeling relational data is challenging as it requires modeling both a "parent" table and its relationships across tables. We introduce REaLTabFormer (Realistic Relational and Tabular Transformer), a tabular and relational synthetic data generation model. It first creates a parent table using an autoregressive GPT-2 model, then generates the relational dataset conditioned on the parent table using a sequence-to-sequence (Seq2Seq) model. We implement target masking to prevent data copying and propose the $Q_\delta$ statistic and statistical bootstrapping to detect overfitting. Experiments using real-world datasets show that REaLTabFormer captures the relational structure better than a baseline model. REaLTabFormer also achieves state-of-the-art results on prediction tasks, "out-of-the-box", for large non-relational datasets without needing fine-tuning. --->
 
 
 ## Installation
 
 REaLTabFormer is available on PyPi and can be easily installed with [pip](https://pypi.org/project/pip/) (Python version >= 3.7):
 
 ```bash
@@ -170,14 +171,15 @@
 
 The REaLTabFormer framework provides an interface to easily build observation validators for filtering invalid synthetic samples. We show an example of using the `GeoValidator` below. The chart on the left shows the distribution of the generated latitude and longitude without validation. The chart on the right shows the synthetic samples with observations that have been validated using the `GeoValidator` with the California boundary. Still, even when we did not optimally train the model for generating this, the invalid samples (falling outside of the boundary) are scarce from the generated data with no validator.
 
 <div align=center>
     <img src="https://github.com/avsolatorio/RealTabFormer/raw/main/img/CA-housing-raw-samples.png" style="width:35%; padding-right:5%;"/>
     <img src="https://github.com/avsolatorio/RealTabFormer/raw/main/img/CA-housing-validated-samples.png" style="width:35%; padding-left:5%;"/>
 </div>
+<br>
 
 ```Python
 # !pip install geopandas &> /dev/null
 # !pip install realtabformer &> /dev/null
 # !git clone https://github.com/joncutrer/geopandas-tutorial.git &> /dev/null
 import geopandas
 import seaborn as sns
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: REaLTabFormer Version: 0.1.1 Summary: A novel
+Metadata-Version: 2.1 Name: REaLTabFormer Version: 0.1.2 Summary: A novel
 method for generating tabular and relational data using language models.
 Author-email: "Aivin V. Solatorio"
 worldbank.org> License: MIT License Copyright (c) 2022 Aivin V. Solatorio
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -19,42 +19,28 @@
 avsolatorio/REaLTabFormer Project-URL: Documentation, https://
 avsolatorio.github.io/REaLTabFormer/ Keywords: REaLTabFormer,deep
 learning,tabular data,transformers,data generation,seq2seq model,synthetic
 data,pytorch,language models,synthetic data generation Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE [Open_In_Colab] #
-RealTabFormer The REaLTabFormer (Realistic Relational and Tabular Data using
+REaLTabFormer The REaLTabFormer (Realistic Relational and Tabular Data using
 Transformers) offers a unified framework for synthesizing tabular data of
 different types. A sequence-to-sequence (Seq2Seq) model is used for generating
 synthetic relational datasets. The REaLTabFormer model for a non-relational
 tabular data uses GPT-2, and can be used out-of-the-box to model any tabular
 data with independent observations.
 
           [https://github.com/avsolatorio/RealTabFormer/raw/main/img/
                           REalTabFormer_Final_EQ.png]
      REaLTabFormer: Generating Realistic Relational and Tabular Data using
                                  Transformers
                                 Paper_on_ArXiv
 
-Tabular data is a common form of organizing data. Multiple models are available
-to generate synthetic tabular datasets where observations are independent, but
-few have the ability to produce relational datasets. Modeling relational data
-is challenging as it requires modeling both a "parent" table and its
-relationships across tables. We introduce REaLTabFormer (Realistic Relational
-and Tabular Transformer), a tabular and relational synthetic data generation
-model. It first creates a parent table using an autoregressive GPT-2 model,
-then generates the relational dataset conditioned on the parent table using a
-sequence-to-sequence (Seq2Seq) model. We implement target masking to prevent
-data copying and propose the $Q_\delta$ statistic and statistical bootstrapping
-to detect overfitting. Experiments using real-world datasets show that
-REaLTabFormer captures the relational structure better than a baseline model.
-REaLTabFormer also achieves state-of-the-art results on prediction tasks, "out-
-of-the-box", for large non-relational datasets without needing fine-tuning. ##
-Installation REaLTabFormer is available on PyPi and can be easily installed
+ ## Installation REaLTabFormer is available on PyPi and can be easily installed
 with [pip](https://pypi.org/project/pip/) (Python version >= 3.7): ```bash pip
 install realtabformer ``` ## Usage We show examples of using the REaLTabFormer
 for modeling and generating synthetic data from a trained model. ###
 REaLTabFormer for regular tabular data ```Python # pip install realtabformer
 import pandas as pd from realtabformer import REaLTabFormer df = pd.read_csv
 ("foo.csv") # NOTE: Remove any unique identifiers in the # data that you don't
 want to be modeled. # Non-relational or parent table. rtf_model = REaLTabFormer
@@ -94,14 +80,15 @@
 shows the synthetic samples with observations that have been validated using
 the `GeoValidator` with the California boundary. Still, even when we did not
 optimally train the model for generating this, the invalid samples (falling
 outside of the boundary) are scarce from the generated data with no validator.
   [https://github.com/avsolatorio/RealTabFormer/raw/main/img/CA-housing-raw-
   samples.png] [https://github.com/avsolatorio/RealTabFormer/raw/main/img/CA-
                         housing-validated-samples.png]
+
 ```Python # !pip install geopandas &> /dev/null # !pip install realtabformer &>
 /dev/null # !git clone https://github.com/joncutrer/geopandas-tutorial.git &> /
 dev/null import geopandas import seaborn as sns import matplotlib.pyplot as plt
 from realtabformer import REaLTabFormer from realtabformer import
 rtf_validators as rtf_val from shapely.geometry import Polygon, LineString,
 Point, MultiPolygon from sklearn.datasets import fetch_california_housing def
 plot_sf(data, samples, title=None): xlims = (-126, -113.5) ylims = (31, 43)
```

### Comparing `REaLTabFormer-0.1.1/src/REaLTabFormer.egg-info/SOURCES.txt` & `REaLTabFormer-0.1.2/src/REaLTabFormer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/src/realtabformer/data_utils.py` & `REaLTabFormer-0.1.2/src/realtabformer/data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,15 +488,15 @@
         if _col_transform_data is None:
             # This means that no transform data is available
             # before the processing.
             col_transform_data[c] = transform_data
         series.name = col_name
         processed_series.append(series)
 
-    processed_df = pd.concat(processed_series, axis=1)
+    processed_df = pd.concat([pd.DataFrame()] + processed_series, axis=1)
 
     if not processed_df.empty:
         # Combine the processed numeric and datetime data.
         processed_df = pd.concat(
             [
                 tokenize_numeric_col(processed_df[col], nparts=numeric_nparts)
                 for col in processed_df.columns
```

### Comparing `REaLTabFormer-0.1.1/src/realtabformer/realtabformer.py` & `REaLTabFormer-0.1.2/src/realtabformer/realtabformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,17 @@
 def _validate_get_device(device: str) -> str:
     if torch.cuda.device_count() == 0:
         if torch.backends.mps.is_available():
             _device = "mps"
         else:
             _device = "cpu"
 
-        warnings.warn(f"The device={device} is not available, using device={_device} instead.")
+        warnings.warn(
+            f"The device={device} is not available, using device={_device} instead."
+        )
         device = _device
 
     return device
 
 
 class REaLTabFormer:
     def __init__(
@@ -863,20 +865,22 @@
             # `RuntimeError: CUDA error: device-side assert triggered`
             assert self.relational_max_length
             if (
                 coder_name == "decoder"
                 and coder.n_positions < self.relational_max_length
             ):
                 coder.n_positions = 128 + self.relational_max_length
-            elif coder_name == "encoder" and coder.n_positions < len(
-                self.vocab[coder_name]["column_token_ids"]
-            ):
-                coder.n_positions = 128 + len(
-                    self.vocab[coder_name]["column_token_ids"]
-                )
+            elif coder_name == "encoder" and getattr(
+                coder, "n_positions", getattr(coder, "max_position_embeddings")
+            ) < len(self.vocab[coder_name]["column_token_ids"]):
+                positions = 128 + len(self.vocab[coder_name]["column_token_ids"])
+                try:
+                    coder.n_positions = positions
+                except:
+                    coder.max_position_embeddings = positions
 
         # This must be set to True for the EncoderDecoderModel to work at least
         # with GPT2 as the decoder.
         self.relational_config.decoder.add_cross_attention = True
 
     def _fit_relational(
         self, out_df: pd.DataFrame, in_df: pd.DataFrame, join_on: str, device="cuda"
```

### Comparing `REaLTabFormer-0.1.1/src/realtabformer/rtf_analyze.py` & `REaLTabFormer-0.1.2/src/realtabformer/rtf_analyze.py`

 * *Files 0% similar despite different names*

```diff
@@ -739,9 +739,8 @@
         self,
         data_id: str,
         model_type: str,
         categorical: bool,
         target_col: str,
         target_pos_val: Any = None,
     ) -> None:
-
         pass
```

### Comparing `REaLTabFormer-0.1.1/src/realtabformer/rtf_datacollator.py` & `REaLTabFormer-0.1.2/src/realtabformer/rtf_datacollator.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/src/realtabformer/rtf_exceptions.py` & `REaLTabFormer-0.1.2/src/realtabformer/rtf_exceptions.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/src/realtabformer/rtf_sampler.py` & `REaLTabFormer-0.1.2/src/realtabformer/rtf_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         column_dtypes: Dict,
         column_has_missing: Dict,
         drop_na_cols: List,
         col_transform_data: Dict,
         random_state: Optional[int] = 1029,
         device="cuda",
     ) -> None:
-
         self.model_type = model_type
         self.vocab = vocab
         self.processed_columns = processed_columns
         self.col_size = col_size  # relational_col_size or tabular_col_size
         self.col_idx_ids = col_idx_ids
         self.max_length = max_length  # relational_max_length or tabular_max_length
 
@@ -252,15 +251,14 @@
                 _samples = _samples.numpy()
             else:
                 _samples = _samples.cpu().numpy()
 
         return _samples
 
     def _validate_synth_sample(self, synth_sample: pd.DataFrame) -> pd.DataFrame:
-
         # Validate data
         valid_mask = []
 
         # Validate that the generated value for a column is correct.
         # Use the column identifier as basis for the validation.
         # Is this useful when we actually filter the vocabulary
         # during generation???
@@ -371,15 +369,14 @@
     def _processes_sample(
         self,
         sample_outputs: np.ndarray,
         vocab: Dict,
         relate_ids: Optional[List[Any]] = None,
         validator: Optional[ObservationValidator] = None,
     ) -> pd.DataFrame:
-
         assert isinstance(sample_outputs, np.ndarray)
 
         def _decode_tokens(s):
             # No need to remove [BOS] and [EOS] tokens
             # here, it will be handled later.
             return [vocab["id2token"][i] for i in s]
 
@@ -600,15 +597,14 @@
         constrain_tokens_gen: Optional[bool] = True,
         validator: Optional[ObservationValidator] = None,
         continuous_empty_limit: int = 10,
         suppress_tokens: Optional[List[int]] = None,
         forced_decoder_ids: Optional[List[List[int]]] = None,
         **generate_kwargs,
     ) -> pd.DataFrame:
-
         device = torch.device(device)
 
         if self.model.device != device:
             self.model = self.model.to(device)
 
         self.model.eval()
         synth_df = []
@@ -889,32 +885,35 @@
 
             # Create a fixed-size matrix to store the data filled with [PAD] token ids.
             samples = np.ones((input_df.shape[0], self.max_length))
             samples *= self.vocab["decoder"]["token2id"][SpecialTokens.PAD]
             start = 0
 
             if isinstance(related_num, str) and related_num in input_df.columns:
-                init_min_max_length = self._get_min_max_length(input_df[related_num].max())
+                init_min_max_length = self._get_min_max_length(
+                    input_df[related_num].max()
+                )
 
                 if init_min_max_length["max_length"] > samples.shape[1]:
-                    samples = np.ones((input_df.shape[0], init_min_max_length["max_length"]))
+                    samples = np.ones(
+                        (input_df.shape[0], init_min_max_length["max_length"])
+                    )
                     samples *= self.vocab["decoder"]["token2id"][SpecialTokens.PAD]
 
                 _input_unique_ids = []
                 input_df = input_df.copy()
 
                 # Make sure that we couple the `input_unique_ids` with
                 # its intended data when sorting and grouping.
                 input_df[NQ_COL] = input_unique_ids
                 input_df.sort_values(related_num, ascending=True, inplace=True)
 
                 for related_num, _input_df in input_df.groupby(related_num):
                     _input_unique_ids.append(_input_df.pop(NQ_COL))
-                    generate_kwargs.update(
-                        self._get_min_max_length(related_num))
+                    generate_kwargs.update(self._get_min_max_length(related_num))
 
                     for _samples in self._sample_input_batch(
                         input_df=_input_df,
                         gen_batch=gen_batch,
                         device=device,
                         constrain_tokens_gen=constrain_tokens_gen,
                         suppress_tokens=suppress_tokens,
@@ -924,20 +923,21 @@
                         end = start + len(_samples)
 
                         samples[start:end, : _samples.shape[1]] = _samples
                         start = end
 
                 input_unique_ids = pd.concat(_input_unique_ids)
             else:
-                generate_kwargs.update(
-                    self._get_min_max_length(related_num))
+                generate_kwargs.update(self._get_min_max_length(related_num))
 
                 if generate_kwargs["max_length"] > samples.shape[1]:
                     # Create a fixed-size matrix to store the data filled with [PAD] token ids.
-                    samples = np.ones((input_df.shape[0], generate_kwargs["max_length"]))
+                    samples = np.ones(
+                        (input_df.shape[0], generate_kwargs["max_length"])
+                    )
                     samples *= self.vocab["decoder"]["token2id"][SpecialTokens.PAD]
 
                 for _samples in self._sample_input_batch(
                     input_df=input_df,
                     gen_batch=gen_batch,
                     device=device,
                     constrain_tokens_gen=constrain_tokens_gen,
@@ -977,17 +977,15 @@
                 min_length = min_length + ((self.col_size + 2) * related_num)
                 max_length = min_length + 1
             else:
                 raise ValueError(
                     "The `related_num` must be greater than or equal to zero."
                 )
 
-        return dict(
-            min_length=min_length,
-            max_length=max_length)
+        return dict(min_length=min_length, max_length=max_length)
 
     def _sample_input_batch(
         self,
         input_df: Optional[pd.DataFrame] = None,
         gen_batch: Optional[int] = 128,
         device: Optional[str] = "cuda",
         constrain_tokens_gen: Optional[bool] = True,
```

### Comparing `REaLTabFormer-0.1.1/src/realtabformer/rtf_trainer.py` & `REaLTabFormer-0.1.2/src/realtabformer/rtf_trainer.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/src/realtabformer/rtf_validators.py` & `REaLTabFormer-0.1.2/src/realtabformer/rtf_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
         self.min_val = min_val
         self.max_val = max_val
 
     def validate(  # type: ignore
         self, val: Union[float, int, np.number], *args: Any, **kwargs: Any
     ) -> bool:
-
         return self.min_val <= val <= self.max_val
 
 
 class GeoValidator(ValidatorBase):
     def __init__(self, geo_bound: Union[Polygon, MultiPolygon]) -> None:
         super().__init__()
```

### Comparing `REaLTabFormer-0.1.1/tests/realtabformer/fixtures.py` & `REaLTabFormer-0.1.2/tests/realtabformer/fixtures.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/tests/realtabformer/test_data_utils.py` & `REaLTabFormer-0.1.2/tests/realtabformer/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/tests/realtabformer/test_realtabformer.py` & `REaLTabFormer-0.1.2/tests/realtabformer/test_realtabformer.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.1/tests/realtabformer/test_rtf_sampler.py` & `REaLTabFormer-0.1.2/tests/realtabformer/test_rtf_sampler.py`

 * *Files identical despite different names*

