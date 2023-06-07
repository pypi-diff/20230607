# Comparing `tmp/sempler-0.2.8.tar.gz` & `tmp/sempler-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/juan/ETH/sempler/dist/.tmp-da_s477_/sempler-0.2.8.tar", last modified: Thu Dec  8 16:28:23 2022, max compression
+gzip compressed data, was "/home/juan/ETH/sempler/dist/.tmp-wctds1vd/sempler-0.2.9.tar", last modified: Thu Dec  8 16:41:26 2022, max compression
```

## Comparing `sempler-0.2.8.tar` & `sempler-0.2.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:28:23.000000 sempler-0.2.8/
--rw-rw-r--   0 juan      (1000) juan      (1000)     2848 2022-12-08 16:27:35.000000 sempler-0.2.8/CHANGES.txt
--rw-r--r--   0 juan      (1000) juan      (1000)     1521 2021-01-31 14:39:23.000000 sempler-0.2.8/LICENSE.txt
--rw-r--r--   0 juan      (1000) juan      (1000)       42 2020-04-24 17:02:02.000000 sempler-0.2.8/MANIFEST.in
--rw-rw-r--   0 juan      (1000) juan      (1000)     3022 2022-12-08 16:28:23.000000 sempler-0.2.8/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     2703 2022-12-08 15:06:14.000000 sempler-0.2.8/README.md
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:28:23.000000 sempler-0.2.8/docs/
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:28:23.000000 sempler-0.2.8/docs/build/
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:28:23.000000 sempler-0.2.8/docs/build/html/
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:28:23.000000 sempler-0.2.8/docs/build/html/_sources/
--rw-rw-r--   0 juan      (1000) juan      (1000)      428 2021-01-31 14:39:23.000000 sempler-0.2.8/docs/build/html/_sources/anm.rst.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)     2599 2022-11-29 09:55:02.000000 sempler-0.2.8/docs/build/html/_sources/drfnet.rst.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       87 2021-01-31 14:39:23.000000 sempler-0.2.8/docs/build/html/_sources/generators.rst.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)     3322 2022-11-29 09:55:02.000000 sempler-0.2.8/docs/build/html/_sources/index.rst.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)      623 2021-01-31 14:39:23.000000 sempler-0.2.8/docs/build/html/_sources/lganm.rst.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)      566 2021-01-31 14:39:23.000000 sempler-0.2.8/docs/build/html/_sources/normal_distribution.rst.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       51 2022-12-08 16:27:35.000000 sempler-0.2.8/docs/requirements.txt
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:28:23.000000 sempler-0.2.8/drf/
--rw-rw-r--   0 juan      (1000) juan      (1000)       22 2022-11-29 09:55:02.000000 sempler-0.2.8/drf/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6583 2022-12-08 16:27:35.000000 sempler-0.2.8/drf/code.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:28:23.000000 sempler-0.2.8/sempler/
--rw-rw-r--   0 juan      (1000) juan      (1000)      123 2022-11-29 09:55:02.000000 sempler-0.2.8/sempler/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     8531 2022-07-14 16:58:02.000000 sempler-0.2.8/sempler/anm.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1706 2022-07-14 16:58:02.000000 sempler-0.2.8/sempler/functions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    10597 2022-07-14 16:58:02.000000 sempler-0.2.8/sempler/generators.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    10520 2022-07-14 16:58:21.000000 sempler-0.2.8/sempler/lganm.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2037 2022-07-14 16:58:02.000000 sempler-0.2.8/sempler/noise.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14394 2022-07-14 16:58:02.000000 sempler-0.2.8/sempler/normal_distribution.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     3811 2022-11-29 09:55:02.000000 sempler-0.2.8/sempler/plot.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    11915 2022-12-08 16:27:35.000000 sempler-0.2.8/sempler/semi.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:28:23.000000 sempler-0.2.8/sempler/test/
--rw-r--r--   0 juan      (1000) juan      (1000)        0 2020-04-24 17:02:02.000000 sempler-0.2.8/sempler/test/__init__.py
--rw-r--r--   0 juan      (1000) juan      (1000)     5637 2021-01-31 14:39:23.000000 sempler-0.2.8/sempler/test/test_anm.py
--rw-r--r--   0 juan      (1000) juan      (1000)     2025 2021-01-31 14:39:23.000000 sempler-0.2.8/sempler/test/test_api.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5025 2022-07-14 16:58:02.000000 sempler-0.2.8/sempler/test/test_generators.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    16891 2022-11-29 09:55:02.000000 sempler-0.2.8/sempler/test/test_lganm.py
--rw-r--r--   0 juan      (1000) juan      (1000)    18683 2021-01-31 14:39:23.000000 sempler-0.2.8/sempler/test/test_normal_distribution.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2712 2022-11-29 09:55:02.000000 sempler-0.2.8/sempler/test/test_semi.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     9266 2022-11-29 09:55:02.000000 sempler-0.2.8/sempler/test/test_utils.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14143 2022-11-29 09:55:02.000000 sempler-0.2.8/sempler/utils.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:28:23.000000 sempler-0.2.8/sempler.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     3022 2022-12-08 16:28:23.000000 sempler-0.2.8/sempler.egg-info/PKG-INFO
--rw-r--r--   0 juan      (1000) juan      (1000)      930 2022-12-08 16:28:23.000000 sempler-0.2.8/sempler.egg-info/SOURCES.txt
--rw-r--r--   0 juan      (1000) juan      (1000)        1 2022-12-08 16:28:23.000000 sempler-0.2.8/sempler.egg-info/dependency_links.txt
--rw-r--r--   0 juan      (1000) juan      (1000)       40 2022-12-08 16:28:23.000000 sempler-0.2.8/sempler.egg-info/requires.txt
--rw-r--r--   0 juan      (1000) juan      (1000)       12 2022-12-08 16:28:23.000000 sempler-0.2.8/sempler.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2022-12-08 16:28:23.000000 sempler-0.2.8/setup.cfg
--rw-rw-r--   0 juan      (1000) juan      (1000)      544 2022-12-08 16:27:38.000000 sempler-0.2.8/setup.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:41:26.000000 sempler-0.2.9/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2918 2022-12-08 16:41:04.000000 sempler-0.2.9/CHANGES.txt
+-rw-r--r--   0 juan      (1000) juan      (1000)     1521 2021-01-31 14:39:23.000000 sempler-0.2.9/LICENSE.txt
+-rw-r--r--   0 juan      (1000) juan      (1000)       42 2020-04-24 17:02:02.000000 sempler-0.2.9/MANIFEST.in
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3022 2022-12-08 16:41:26.000000 sempler-0.2.9/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2703 2022-12-08 15:06:14.000000 sempler-0.2.9/README.md
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:41:26.000000 sempler-0.2.9/docs/
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:41:26.000000 sempler-0.2.9/docs/build/
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:41:26.000000 sempler-0.2.9/docs/build/html/
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:41:26.000000 sempler-0.2.9/docs/build/html/_sources/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      428 2021-01-31 14:39:23.000000 sempler-0.2.9/docs/build/html/_sources/anm.rst.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2455 2022-12-08 16:27:35.000000 sempler-0.2.9/docs/build/html/_sources/drfnet.rst.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       87 2021-01-31 14:39:23.000000 sempler-0.2.9/docs/build/html/_sources/generators.rst.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3698 2022-12-08 16:27:35.000000 sempler-0.2.9/docs/build/html/_sources/index.rst.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)      623 2021-01-31 14:39:23.000000 sempler-0.2.9/docs/build/html/_sources/lganm.rst.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)      566 2021-01-31 14:39:23.000000 sempler-0.2.9/docs/build/html/_sources/normal_distribution.rst.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       51 2022-12-08 16:27:35.000000 sempler-0.2.9/docs/requirements.txt
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:41:26.000000 sempler-0.2.9/drf/
+-rw-rw-r--   0 juan      (1000) juan      (1000)       22 2022-11-29 09:55:02.000000 sempler-0.2.9/drf/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6583 2022-12-08 16:27:35.000000 sempler-0.2.9/drf/code.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:41:26.000000 sempler-0.2.9/sempler/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      123 2022-11-29 09:55:02.000000 sempler-0.2.9/sempler/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     8531 2022-07-14 16:58:02.000000 sempler-0.2.9/sempler/anm.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1706 2022-07-14 16:58:02.000000 sempler-0.2.9/sempler/functions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    10597 2022-07-14 16:58:02.000000 sempler-0.2.9/sempler/generators.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    10520 2022-07-14 16:58:21.000000 sempler-0.2.9/sempler/lganm.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2037 2022-07-14 16:58:02.000000 sempler-0.2.9/sempler/noise.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14394 2022-07-14 16:58:02.000000 sempler-0.2.9/sempler/normal_distribution.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3811 2022-11-29 09:55:02.000000 sempler-0.2.9/sempler/plot.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    11919 2022-12-08 16:41:04.000000 sempler-0.2.9/sempler/semi.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:41:26.000000 sempler-0.2.9/sempler/test/
+-rw-r--r--   0 juan      (1000) juan      (1000)        0 2020-04-24 17:02:02.000000 sempler-0.2.9/sempler/test/__init__.py
+-rw-r--r--   0 juan      (1000) juan      (1000)     5637 2021-01-31 14:39:23.000000 sempler-0.2.9/sempler/test/test_anm.py
+-rw-r--r--   0 juan      (1000) juan      (1000)     2025 2021-01-31 14:39:23.000000 sempler-0.2.9/sempler/test/test_api.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5025 2022-07-14 16:58:02.000000 sempler-0.2.9/sempler/test/test_generators.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    16891 2022-11-29 09:55:02.000000 sempler-0.2.9/sempler/test/test_lganm.py
+-rw-r--r--   0 juan      (1000) juan      (1000)    18683 2021-01-31 14:39:23.000000 sempler-0.2.9/sempler/test/test_normal_distribution.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2712 2022-11-29 09:55:02.000000 sempler-0.2.9/sempler/test/test_semi.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     9266 2022-11-29 09:55:02.000000 sempler-0.2.9/sempler/test/test_utils.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14143 2022-11-29 09:55:02.000000 sempler-0.2.9/sempler/utils.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2022-12-08 16:41:26.000000 sempler-0.2.9/sempler.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     3022 2022-12-08 16:41:26.000000 sempler-0.2.9/sempler.egg-info/PKG-INFO
+-rw-r--r--   0 juan      (1000) juan      (1000)      930 2022-12-08 16:41:26.000000 sempler-0.2.9/sempler.egg-info/SOURCES.txt
+-rw-r--r--   0 juan      (1000) juan      (1000)        1 2022-12-08 16:41:26.000000 sempler-0.2.9/sempler.egg-info/dependency_links.txt
+-rw-r--r--   0 juan      (1000) juan      (1000)       40 2022-12-08 16:41:26.000000 sempler-0.2.9/sempler.egg-info/requires.txt
+-rw-r--r--   0 juan      (1000) juan      (1000)       12 2022-12-08 16:41:26.000000 sempler-0.2.9/sempler.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2022-12-08 16:41:26.000000 sempler-0.2.9/setup.cfg
+-rw-rw-r--   0 juan      (1000) juan      (1000)      544 2022-12-08 16:41:06.000000 sempler-0.2.9/setup.py
```

### Comparing `sempler-0.2.8/CHANGES.txt` & `sempler-0.2.9/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+v0.2.9, 2022-12-08
+-- Adapted docstrings
+-- Fixed bug in sempler.semi
 v0.2.8, 2022-12-08
 -- Fixed issues with readthedocs build: in drf/code.py, do not break if R package "drf" is not installed
 v0.2.7, 2022-12-08
 -- Fixed bad import in sempler.semi
 -- Added pandas and rpy2 as mandatory dependencies
 v0.2.6, 2022-12-08
 -- Added drf package to setup index
```

### Comparing `sempler-0.2.8/LICENSE.txt` & `sempler-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/PKG-INFO` & `sempler-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sempler
-Version: 0.2.8
+Version: 0.2.9
 Summary: Sample from general structural causal models (SCMs).
 Home-page: https://github.com/juangamella/sempler
 Author: Juan L Gamella
 Author-email: juangamella@gmail.com
 License: BSD 3-Clause License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `sempler-0.2.8/README.md` & `sempler-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/docs/build/html/_sources/drfnet.rst.txt` & `sempler-0.2.9/docs/build/html/_sources/drfnet.rst.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,20 @@
     author={Gamella, Juan L. and Taeb, Armeen and Heinze-Deml, Christina and B\"uhlmann, Peter},
     journal={arXiv preprint arXiv:2211.14897},
     year={2022}
   }
 
 As input, the procedure takes a directed acyclic graph over some variables and a dataset consisting of their observations under different environments. The data can also be "observational", that is, from a single environment. The procedure then fits a non-parametric Bayesian network, where the conditional distributions entailed by the graph are approximated via distributional random forests :ref:`[2]<references class>`. Once fitted, you can sample from this collection of forests to produce a new, semi-synthetic dataset that respects acyclicity, causal sufficiency, and the conditional independence relationships entailed by the given graph, while its marginal and conditional distributions closely resemble those of the original dataset :ref:`[1, figure 4]<references class>`.
 
-**Additional dependencies**
+**Additional R dependencies**
 
-To run this procedure you will need additional dependencies, which are not required for the rest of sempler's functionality. In particular,
+For now, only an `R` implementation of distributional random forests [2] is available. Thus, to run the procedure you will additionally need
 
-- you will need an installation of `R`; you can find an installation guide `here <https://rstudio-education.github.io/hopr/starting.html>`__
+- an `R` installation; you can find an installation guide `here <https://rstudio-education.github.io/hopr/starting.html>`__
 - the `R` package ``drf``, which you can install by typing ``install.packages("drf")`` in an R terminal
-- the python packages ``pandas`` and ``rpy2``, which you can install by executing ``pip install rpy2 pandas`` in a suitable shell
 
 The class is documented below.
   
 .. autoclass:: sempler.DRFNet
    :members:
 
 .. _references class:
```

### Comparing `sempler-0.2.8/docs/build/html/_sources/index.rst.txt` & `sempler-0.2.9/docs/build/html/_sources/index.rst.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,17 +11,20 @@
     journal={arXiv preprint arXiv:2211.14897},
     year={2022}
   }
 
 Overview
 --------
 
-The semi-synthetic data generation procedure is implemented in the class :class:`sempler.DRFNet`.
+The semi-synthetic data generation procedure is implemented in the class :class:`sempler.DRFNet`. For now, only an `R` implementation of distributional random forests [2] is available. Thus, to run the procedure you will additionally need
 
-Additionally, you can generate purely synthetic data from general structural causal models with additive noise. Two classes are defined for this purpose.
+- an `R` installation; you can find an installation guide `here <https://rstudio-education.github.io/hopr/starting.html>`__
+- the `R` package ``drf``, which you can install by typing ``install.packages("drf")`` in an R terminal
+
+Sempler also allows you can generate purely synthetic data from general structural causal models with additive noise. Two classes are defined for this purpose.
 
 - :class:`sempler.ANM` is for general (acyclic) additive noise SCMs. Any assignment function is possible, as are the distributions of the noise terms.
 - :class:`sempler.LGANM` is for linear Gaussian SCMs. While this is also possible with :class:`sempler.ANM`, this class simplifies the interface and offers the additional functionality of sampling "in the population setting", i.e. by returning a symbolic gaussian distribution (see :func:`sempler.LGANM.sample` and :class:`sempler.NormalDistribution`).
 
 To allow for random generation of SCMs and interventional distributions, the module :class:`sempler.generators` contains functions to sample random DAGs and intervention targets.
  
 ------
```

### Comparing `sempler-0.2.8/docs/build/html/_sources/lganm.rst.txt` & `sempler-0.2.9/docs/build/html/_sources/lganm.rst.txt`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/docs/build/html/_sources/normal_distribution.rst.txt` & `sempler-0.2.9/docs/build/html/_sources/normal_distribution.rst.txt`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/drf/code.py` & `sempler-0.2.9/drf/code.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/anm.py` & `sempler-0.2.9/sempler/anm.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/functions.py` & `sempler-0.2.9/sempler/functions.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/generators.py` & `sempler-0.2.9/sempler/generators.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/lganm.py` & `sempler-0.2.9/sempler/lganm.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/noise.py` & `sempler-0.2.9/sempler/noise.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/normal_distribution.py` & `sempler-0.2.9/sempler/normal_distribution.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/plot.py` & `sempler-0.2.9/sempler/plot.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/semi.py` & `sempler-0.2.9/sempler/semi.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 Please cite it if you use this procedure in your work.
 
 <TODO: Dependencies>
 """
 
 import numpy as np
 import drf
-import sempler.utils as utils
+import sempler.utils
 import copy
 import pandas as pd
 import time
 
 _GRAPH_TYPE_ERROR = "graph must be a 2-dimensional numpy.ndarray"
 _DATA_TYPE_ERROR = "data must be a list of 2-dimensional numpy.ndarray"
 _N_TYPE_ERROR = "n must be a positive int or list of positive ints"
@@ -243,15 +243,15 @@
                     # print(DRF.info())
                     self._random_forests[i, k] = DRF
         print(
             "Done in %0.2f seconds           " % (time.time() - start)
         ) if verbose else None
 
     def sample(self, n=None, random_state=None):
-        """Generate a sample from the fitted SCM.
+        """Generate a sample from the fitted Bayesian network.
 
         Parameters
         ----------
         n : int or list of ints or NoneType, default=None
             The desired sample size. If `None` the sample size from
             each environment matches that of the original
             data. Otherwise: either a single value (same number of
```

### Comparing `sempler-0.2.8/sempler/test/test_anm.py` & `sempler-0.2.9/sempler/test/test_anm.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/test/test_api.py` & `sempler-0.2.9/sempler/test/test_api.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/test/test_generators.py` & `sempler-0.2.9/sempler/test/test_generators.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/test/test_lganm.py` & `sempler-0.2.9/sempler/test/test_lganm.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/test/test_normal_distribution.py` & `sempler-0.2.9/sempler/test/test_normal_distribution.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/test/test_semi.py` & `sempler-0.2.9/sempler/test/test_semi.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/test/test_utils.py` & `sempler-0.2.9/sempler/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler/utils.py` & `sempler-0.2.9/sempler/utils.py`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/sempler.egg-info/PKG-INFO` & `sempler-0.2.9/sempler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sempler
-Version: 0.2.8
+Version: 0.2.9
 Summary: Sample from general structural causal models (SCMs).
 Home-page: https://github.com/juangamella/sempler
 Author: Juan L Gamella
 Author-email: juangamella@gmail.com
 License: BSD 3-Clause License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `sempler-0.2.8/sempler.egg-info/SOURCES.txt` & `sempler-0.2.9/sempler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sempler-0.2.8/setup.py` & `sempler-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="sempler",
-    version="0.2.8",
+    version="0.2.9",
     author="Juan L Gamella",
     author_email="juangamella@gmail.com",
     packages=["sempler", "sempler.test", "drf"],
     scripts=[],
     url="https://github.com/juangamella/sempler",
     license="BSD 3-Clause License",
     description="Sample from general structural causal models (SCMs).",
```

