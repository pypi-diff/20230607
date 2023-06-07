# Comparing `tmp/cobamp-0.2.1.tar.gz` & `tmp/cobamp-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cobamp-0.2.1.tar", last modified: Tue Jan 24 16:00:51 2023, max compression
+gzip compressed data, was "dist\cobamp-0.2.2.tar", last modified: Wed Jun  7 08:09:18 2023, max compression
```

## Comparing `cobamp-0.2.1.tar` & `cobamp-0.2.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-01-24 16:00:51.000000 cobamp-0.2.1/
--rw-rw-rw-   0        0        0    35823 2023-01-24 10:04:44.000000 cobamp-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2901 2023-01-24 16:00:51.000000 cobamp-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2156 2023-01-24 10:04:44.000000 cobamp-0.2.1/README.rst
--rw-rw-rw-   0        0        0       23 2023-01-24 10:04:44.000000 cobamp-0.2.1/notice.txt
--rw-rw-rw-   0        0        0       42 2023-01-24 16:00:51.000000 cobamp-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1275 2023-01-24 15:57:54.000000 cobamp-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:00:50.000000 cobamp-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-01-24 16:00:50.000000 cobamp-0.2.1/src/cobamp/
--rw-rw-rw-   0        0        0       74 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:00:50.000000 cobamp-0.2.1/src/cobamp/algorithms/
--rw-rw-rw-   0        0        0      143 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/algorithms/__init__.py
--rw-rw-rw-   0        0        0    34563 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/algorithms/kshortest.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:00:50.000000 cobamp-0.2.1/src/cobamp/analysis/
--rw-rw-rw-   0        0        0       42 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/analysis/__init__.py
--rw-rw-rw-   0        0        0     1956 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/analysis/frequency.py
--rw-rw-rw-   0        0        0     6971 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/analysis/graph.py
--rw-rw-rw-   0        0        0     4302 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/analysis/plotting.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:00:50.000000 cobamp-0.2.1/src/cobamp/core/
--rw-rw-rw-   0        0        0       78 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/core/__init__.py
--rw-rw-rw-   0        0        0     4620 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/core/cb_analysis.py
--rw-rw-rw-   0        0        0    30906 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/core/linear_systems.py
--rw-rw-rw-   0        0        0    22499 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/core/models.py
--rw-rw-rw-   0        0        0    15401 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/core/optimization.py
--rw-rw-rw-   0        0        0     2147 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/core/transformer.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:00:50.000000 cobamp-0.2.1/src/cobamp/gpr/
--rw-rw-rw-   0        0        0       20 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/gpr/__init__.py
--rw-rw-rw-   0        0        0     5734 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/gpr/core.py
--rw-rw-rw-   0        0        0     5564 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/gpr/integration.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:00:50.000000 cobamp-0.2.1/src/cobamp/nullspace/
--rw-rw-rw-   0        0        0       43 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/nullspace/__init__.py
--rw-rw-rw-   0        0        0     1305 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/nullspace/nullspace.py
--rw-rw-rw-   0        0        0     9277 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/nullspace/subset_reduction.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:00:51.000000 cobamp-0.2.1/src/cobamp/utilities/
--rw-rw-rw-   0        0        0       76 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/utilities/__init__.py
--rw-rw-rw-   0        0        0      440 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/utilities/context.py
--rw-rw-rw-   0        0        0      628 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/utilities/file_io.py
--rw-rw-rw-   0        0        0      448 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/utilities/hash.py
--rw-rw-rw-   0        0        0     1555 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/utilities/linear_system_diagnostics.py
--rw-rw-rw-   0        0        0     2108 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/utilities/parallel.py
--rw-rw-rw-   0        0        0     4855 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/utilities/postfix_expressions.py
--rw-rw-rw-   0        0        0      820 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/utilities/printing.py
--rw-rw-rw-   0        0        0     4964 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/utilities/property_management.py
--rw-rw-rw-   0        0        0      919 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/utilities/set.py
--rw-rw-rw-   0        0        0      492 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/utilities/test.py
--rw-rw-rw-   0        0        0     3124 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/utilities/tree.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:00:51.000000 cobamp-0.2.1/src/cobamp/wrappers/
--rw-rw-rw-   0        0        0     1864 2023-01-24 10:15:05.000000 cobamp-0.2.1/src/cobamp/wrappers/__init__.py
--rw-rw-rw-   0        0        0     1964 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/wrappers/cobamp.py
--rw-rw-rw-   0        0        0     4030 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/wrappers/cobra.py
--rw-rw-rw-   0        0        0    10616 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/wrappers/core.py
--rw-rw-rw-   0        0        0      610 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/wrappers/external_wrappers.py
--rw-rw-rw-   0        0        0     1171 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/wrappers/framed.py
--rw-rw-rw-   0        0        0    12819 2023-01-24 10:04:44.000000 cobamp-0.2.1/src/cobamp/wrappers/method_wrappers.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:00:50.000000 cobamp-0.2.1/src/cobamp.egg-info/
--rw-rw-rw-   0        0        0     2901 2023-01-24 16:00:49.000000 cobamp-0.2.1/src/cobamp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1444 2023-01-24 16:00:50.000000 cobamp-0.2.1/src/cobamp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-24 16:00:49.000000 cobamp-0.2.1/src/cobamp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-01-24 16:00:49.000000 cobamp-0.2.1/src/cobamp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-24 16:00:49.000000 cobamp-0.2.1/src/cobamp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 08:09:18.188175 cobamp-0.2.2/
+-rw-rw-rw-   0        0        0    35823 2023-01-24 10:04:44.000000 cobamp-0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3296 2023-06-07 08:09:18.188175 cobamp-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2156 2023-01-24 10:04:44.000000 cobamp-0.2.2/README.rst
+-rw-rw-rw-   0        0        0       23 2023-01-24 10:04:44.000000 cobamp-0.2.2/notice.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 08:09:18.188175 cobamp-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2023-06-07 08:03:31.000000 cobamp-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:09:18.126635 cobamp-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 08:09:18.133641 cobamp-0.2.2/src/cobamp/
+-rw-rw-rw-   0        0        0       74 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:09:18.154177 cobamp-0.2.2/src/cobamp/algorithms/
+-rw-rw-rw-   0        0        0      143 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/algorithms/__init__.py
+-rw-rw-rw-   0        0        0    34563 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/algorithms/kshortest.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:09:18.157177 cobamp-0.2.2/src/cobamp/analysis/
+-rw-rw-rw-   0        0        0       42 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1956 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/analysis/frequency.py
+-rw-rw-rw-   0        0        0     6971 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/analysis/graph.py
+-rw-rw-rw-   0        0        0     4302 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/analysis/plotting.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:09:18.164175 cobamp-0.2.2/src/cobamp/core/
+-rw-rw-rw-   0        0        0       78 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/core/__init__.py
+-rw-rw-rw-   0        0        0     4620 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/core/cb_analysis.py
+-rw-rw-rw-   0        0        0    30906 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/core/linear_systems.py
+-rw-rw-rw-   0        0        0    22499 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/core/models.py
+-rw-rw-rw-   0        0        0    15401 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/core/optimization.py
+-rw-rw-rw-   0        0        0     2147 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/core/transformer.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:09:18.168185 cobamp-0.2.2/src/cobamp/gpr/
+-rw-rw-rw-   0        0        0       20 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/gpr/__init__.py
+-rw-rw-rw-   0        0        0     5734 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/gpr/core.py
+-rw-rw-rw-   0        0        0     5564 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/gpr/integration.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:09:18.171180 cobamp-0.2.2/src/cobamp/nullspace/
+-rw-rw-rw-   0        0        0       43 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/nullspace/__init__.py
+-rw-rw-rw-   0        0        0     1305 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/nullspace/nullspace.py
+-rw-rw-rw-   0        0        0     9277 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/nullspace/subset_reduction.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:09:18.181174 cobamp-0.2.2/src/cobamp/utilities/
+-rw-rw-rw-   0        0        0       76 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/utilities/__init__.py
+-rw-rw-rw-   0        0        0      440 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/utilities/context.py
+-rw-rw-rw-   0        0        0      628 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/utilities/file_io.py
+-rw-rw-rw-   0        0        0      448 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/utilities/hash.py
+-rw-rw-rw-   0        0        0     1555 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/utilities/linear_system_diagnostics.py
+-rw-rw-rw-   0        0        0     2108 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/utilities/parallel.py
+-rw-rw-rw-   0        0        0     4855 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/utilities/postfix_expressions.py
+-rw-rw-rw-   0        0        0      820 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/utilities/printing.py
+-rw-rw-rw-   0        0        0     4964 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/utilities/property_management.py
+-rw-rw-rw-   0        0        0      919 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/utilities/set.py
+-rw-rw-rw-   0        0        0      492 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/utilities/test.py
+-rw-rw-rw-   0        0        0     3124 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/utilities/tree.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:09:18.187174 cobamp-0.2.2/src/cobamp/wrappers/
+-rw-rw-rw-   0        0        0     1864 2023-01-24 10:15:05.000000 cobamp-0.2.2/src/cobamp/wrappers/__init__.py
+-rw-rw-rw-   0        0        0     1964 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/wrappers/cobamp.py
+-rw-rw-rw-   0        0        0     4030 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/wrappers/cobra.py
+-rw-rw-rw-   0        0        0    10616 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/wrappers/core.py
+-rw-rw-rw-   0        0        0      610 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/wrappers/external_wrappers.py
+-rw-rw-rw-   0        0        0     1171 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/wrappers/framed.py
+-rw-rw-rw-   0        0        0    12819 2023-01-24 10:04:44.000000 cobamp-0.2.2/src/cobamp/wrappers/method_wrappers.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:09:18.152177 cobamp-0.2.2/src/cobamp.egg-info/
+-rw-rw-rw-   0        0        0     3296 2023-06-07 08:09:18.000000 cobamp-0.2.2/src/cobamp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1444 2023-06-07 08:09:18.000000 cobamp-0.2.2/src/cobamp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 08:09:18.000000 cobamp-0.2.2/src/cobamp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-06-07 08:09:18.000000 cobamp-0.2.2/src/cobamp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-07 08:09:18.000000 cobamp-0.2.2/src/cobamp.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cobamp-0.2.1/LICENSE.txt` & `cobamp-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/PKG-INFO` & `cobamp-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,69 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: cobamp
-Version: 0.2.1
+Version: 0.2.2
 Summary: cobamp - pathway analysis methods for genome-scale metabolic models
 Home-page: https://github.com/BioSystemsUM/cobamp
 Author: Vítor Vieira
 Author-email: vvieira@ceb.uminho.pt
 License: GNU General Public License v3.0
+Description: |License| |PyPI version| |RTD version|
+        
+        CoBAMP
+        ============
+        
+        *CoBAMP* (Constraint-Based Analysis of Metabolic Pathways) is a Python package containing pathway analysis methods
+        for use with constraint-based metabolic models. The main purpose is to provide a framework that is both modular and
+        flexible enough to be integrated in other packages (such as cobrapy, framed or cameo) that already implement generic
+        data structures for metabolic models.
+        
+        CoBAMP depends on *optlang* (https://github.com/biosustain/optlang) for solving (mixed-integer) linear programming
+        problems, and thus, requires a compatible solver and Python dependency installed from the following list:
+        
+        -  `cplex <https://www-01.ibm.com/software/commerce/optimization/cplex-optimizer/>`__ (preferred)
+        -  `gurobi <http://www.gurobi.com>`__ (no explicit indicator variables)
+        -  `glpk <https://www.gnu.org/software/glpk/>`__ (no explicit indicator variables or solution pools)
+        
+        Current methods include:
+           -  Elementary flux modes: K-Shortest algorithm
+           -  Minimal cut sets: MCSEnumerator approach
+           -  Elementary flux patterns: K-Shortest algorithm
+        
+        
+        Documentation
+        ~~~~~~~~~~~~~
+        Documentation available at https://cobamp.readthedocs.io/
+        
+        
+        Instalation from PyPI (stable releases)
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        pip install cobamp
+        
+        
+        Credits and License
+        ~~~~~~~~~~~~~~~~~~~
+        
+        Developed at the Centre of Biological Engineering, University of Minho
+        
+        Please refer to this work through this `publication <https://doi.org/10.1093/bioinformatics/btz598>`__ by Vieira and Rocha (2019):
+        
+        - CoBAMP: a Python framework for metabolic pathway analysis in constraint-based models, *Bioinformatics*, btz598
+        
+        Released under the GNU Public License (version 3.0).
+        
+        
+        .. |License| image:: https://img.shields.io/badge/license-GPL%20v3.0-blue.svg
+           :target: https://opensource.org/licenses/GPL-3.0
+        .. |PyPI version| image:: https://badge.fury.io/py/cobamp.svg
+           :target: https://badge.fury.io/py/cobamp
+        .. |RTD version| image:: https://readthedocs.org/projects/cobamp/badge/?version=latest&style=plastic
+           :target: https://cobamp.readthedocs.io/ 
+        
 Keywords: pathway analysis metabolic model
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-License-File: LICENSE.txt
-License-File: notice.txt
-
-|License| |PyPI version| |RTD version|
-
-CoBAMP
-============
-
-*CoBAMP* (Constraint-Based Analysis of Metabolic Pathways) is a Python package containing pathway analysis methods
-for use with constraint-based metabolic models. The main purpose is to provide a framework that is both modular and
-flexible enough to be integrated in other packages (such as cobrapy, framed or cameo) that already implement generic
-data structures for metabolic models.
-
-CoBAMP depends on *optlang* (https://github.com/biosustain/optlang) for solving (mixed-integer) linear programming
-problems, and thus, requires a compatible solver and Python dependency installed from the following list:
-
--  `cplex <https://www-01.ibm.com/software/commerce/optimization/cplex-optimizer/>`__ (preferred)
--  `gurobi <http://www.gurobi.com>`__ (no explicit indicator variables)
--  `glpk <https://www.gnu.org/software/glpk/>`__ (no explicit indicator variables or solution pools)
-
-Current methods include:
-   -  Elementary flux modes: K-Shortest algorithm
-   -  Minimal cut sets: MCSEnumerator approach
-   -  Elementary flux patterns: K-Shortest algorithm
-
-
-Documentation
-~~~~~~~~~~~~~
-Documentation available at https://cobamp.readthedocs.io/
-
-
-Instalation from PyPI (stable releases)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-pip install cobamp
-
-
-Credits and License
-~~~~~~~~~~~~~~~~~~~
-
-Developed at the Centre of Biological Engineering, University of Minho
-
-Please refer to this work through this `publication <https://doi.org/10.1093/bioinformatics/btz598>`__ by Vieira and Rocha (2019):
-
-- CoBAMP: a Python framework for metabolic pathway analysis in constraint-based models, *Bioinformatics*, btz598
-
-Released under the GNU Public License (version 3.0).
-
-
-.. |License| image:: https://img.shields.io/badge/license-GPL%20v3.0-blue.svg
-   :target: https://opensource.org/licenses/GPL-3.0
-.. |PyPI version| image:: https://badge.fury.io/py/cobamp.svg
-   :target: https://badge.fury.io/py/cobamp
-.. |RTD version| image:: https://readthedocs.org/projects/cobamp/badge/?version=latest&style=plastic
-   :target: https://cobamp.readthedocs.io/
```

### Comparing `cobamp-0.2.1/README.rst` & `cobamp-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/setup.py` & `cobamp-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'cobamp',
-    version = '0.2.1',
+    version = '0.2.2',
     package_dir = {'':'src'},
     packages = find_packages('src'),
     install_requires = ["indexed==1.2.1",
                         "pandas==1.3.5",
                         "scipy==1.7.3",
                         "numpy==1.21.6",
                         "matplotlib==3.5.2",
                         "optlang==1.5.2",
                         "pathos==0.2.9",
-                        "boolean.py==4.0"],
+                        "boolean.py==3.8"],
 
     author = 'Vítor Vieira',
     author_email = 'vvieira@ceb.uminho.pt',
     description = 'cobamp - pathway analysis methods for genome-scale metabolic models',
     license = 'GNU General Public License v3.0',
     keywords = 'pathway analysis metabolic model',
     url = 'https://github.com/BioSystemsUM/cobamp',
```

### Comparing `cobamp-0.2.1/src/cobamp/algorithms/kshortest.py` & `cobamp-0.2.2/src/cobamp/algorithms/kshortest.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/analysis/frequency.py` & `cobamp-0.2.2/src/cobamp/analysis/frequency.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/analysis/graph.py` & `cobamp-0.2.2/src/cobamp/analysis/graph.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/analysis/plotting.py` & `cobamp-0.2.2/src/cobamp/analysis/plotting.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/core/cb_analysis.py` & `cobamp-0.2.2/src/cobamp/core/cb_analysis.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/core/linear_systems.py` & `cobamp-0.2.2/src/cobamp/core/linear_systems.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/core/models.py` & `cobamp-0.2.2/src/cobamp/core/models.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/core/optimization.py` & `cobamp-0.2.2/src/cobamp/core/optimization.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/core/transformer.py` & `cobamp-0.2.2/src/cobamp/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/gpr/core.py` & `cobamp-0.2.2/src/cobamp/gpr/core.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/gpr/integration.py` & `cobamp-0.2.2/src/cobamp/gpr/integration.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/nullspace/nullspace.py` & `cobamp-0.2.2/src/cobamp/nullspace/nullspace.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/nullspace/subset_reduction.py` & `cobamp-0.2.2/src/cobamp/nullspace/subset_reduction.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/utilities/file_io.py` & `cobamp-0.2.2/src/cobamp/utilities/file_io.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/utilities/linear_system_diagnostics.py` & `cobamp-0.2.2/src/cobamp/utilities/linear_system_diagnostics.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/utilities/parallel.py` & `cobamp-0.2.2/src/cobamp/utilities/parallel.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/utilities/postfix_expressions.py` & `cobamp-0.2.2/src/cobamp/utilities/postfix_expressions.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/utilities/printing.py` & `cobamp-0.2.2/src/cobamp/utilities/printing.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/utilities/property_management.py` & `cobamp-0.2.2/src/cobamp/utilities/property_management.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/utilities/set.py` & `cobamp-0.2.2/src/cobamp/utilities/set.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/utilities/tree.py` & `cobamp-0.2.2/src/cobamp/utilities/tree.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/wrappers/__init__.py` & `cobamp-0.2.2/src/cobamp/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/wrappers/cobamp.py` & `cobamp-0.2.2/src/cobamp/wrappers/cobamp.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/wrappers/cobra.py` & `cobamp-0.2.2/src/cobamp/wrappers/cobra.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/wrappers/core.py` & `cobamp-0.2.2/src/cobamp/wrappers/core.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/wrappers/external_wrappers.py` & `cobamp-0.2.2/src/cobamp/wrappers/external_wrappers.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/wrappers/framed.py` & `cobamp-0.2.2/src/cobamp/wrappers/framed.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp/wrappers/method_wrappers.py` & `cobamp-0.2.2/src/cobamp/wrappers/method_wrappers.py`

 * *Files identical despite different names*

### Comparing `cobamp-0.2.1/src/cobamp.egg-info/PKG-INFO` & `cobamp-0.2.2/src/cobamp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,69 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: cobamp
-Version: 0.2.1
+Version: 0.2.2
 Summary: cobamp - pathway analysis methods for genome-scale metabolic models
 Home-page: https://github.com/BioSystemsUM/cobamp
 Author: Vítor Vieira
 Author-email: vvieira@ceb.uminho.pt
 License: GNU General Public License v3.0
+Description: |License| |PyPI version| |RTD version|
+        
+        CoBAMP
+        ============
+        
+        *CoBAMP* (Constraint-Based Analysis of Metabolic Pathways) is a Python package containing pathway analysis methods
+        for use with constraint-based metabolic models. The main purpose is to provide a framework that is both modular and
+        flexible enough to be integrated in other packages (such as cobrapy, framed or cameo) that already implement generic
+        data structures for metabolic models.
+        
+        CoBAMP depends on *optlang* (https://github.com/biosustain/optlang) for solving (mixed-integer) linear programming
+        problems, and thus, requires a compatible solver and Python dependency installed from the following list:
+        
+        -  `cplex <https://www-01.ibm.com/software/commerce/optimization/cplex-optimizer/>`__ (preferred)
+        -  `gurobi <http://www.gurobi.com>`__ (no explicit indicator variables)
+        -  `glpk <https://www.gnu.org/software/glpk/>`__ (no explicit indicator variables or solution pools)
+        
+        Current methods include:
+           -  Elementary flux modes: K-Shortest algorithm
+           -  Minimal cut sets: MCSEnumerator approach
+           -  Elementary flux patterns: K-Shortest algorithm
+        
+        
+        Documentation
+        ~~~~~~~~~~~~~
+        Documentation available at https://cobamp.readthedocs.io/
+        
+        
+        Instalation from PyPI (stable releases)
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        pip install cobamp
+        
+        
+        Credits and License
+        ~~~~~~~~~~~~~~~~~~~
+        
+        Developed at the Centre of Biological Engineering, University of Minho
+        
+        Please refer to this work through this `publication <https://doi.org/10.1093/bioinformatics/btz598>`__ by Vieira and Rocha (2019):
+        
+        - CoBAMP: a Python framework for metabolic pathway analysis in constraint-based models, *Bioinformatics*, btz598
+        
+        Released under the GNU Public License (version 3.0).
+        
+        
+        .. |License| image:: https://img.shields.io/badge/license-GPL%20v3.0-blue.svg
+           :target: https://opensource.org/licenses/GPL-3.0
+        .. |PyPI version| image:: https://badge.fury.io/py/cobamp.svg
+           :target: https://badge.fury.io/py/cobamp
+        .. |RTD version| image:: https://readthedocs.org/projects/cobamp/badge/?version=latest&style=plastic
+           :target: https://cobamp.readthedocs.io/ 
+        
 Keywords: pathway analysis metabolic model
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-License-File: LICENSE.txt
-License-File: notice.txt
-
-|License| |PyPI version| |RTD version|
-
-CoBAMP
-============
-
-*CoBAMP* (Constraint-Based Analysis of Metabolic Pathways) is a Python package containing pathway analysis methods
-for use with constraint-based metabolic models. The main purpose is to provide a framework that is both modular and
-flexible enough to be integrated in other packages (such as cobrapy, framed or cameo) that already implement generic
-data structures for metabolic models.
-
-CoBAMP depends on *optlang* (https://github.com/biosustain/optlang) for solving (mixed-integer) linear programming
-problems, and thus, requires a compatible solver and Python dependency installed from the following list:
-
--  `cplex <https://www-01.ibm.com/software/commerce/optimization/cplex-optimizer/>`__ (preferred)
--  `gurobi <http://www.gurobi.com>`__ (no explicit indicator variables)
--  `glpk <https://www.gnu.org/software/glpk/>`__ (no explicit indicator variables or solution pools)
-
-Current methods include:
-   -  Elementary flux modes: K-Shortest algorithm
-   -  Minimal cut sets: MCSEnumerator approach
-   -  Elementary flux patterns: K-Shortest algorithm
-
-
-Documentation
-~~~~~~~~~~~~~
-Documentation available at https://cobamp.readthedocs.io/
-
-
-Instalation from PyPI (stable releases)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-pip install cobamp
-
-
-Credits and License
-~~~~~~~~~~~~~~~~~~~
-
-Developed at the Centre of Biological Engineering, University of Minho
-
-Please refer to this work through this `publication <https://doi.org/10.1093/bioinformatics/btz598>`__ by Vieira and Rocha (2019):
-
-- CoBAMP: a Python framework for metabolic pathway analysis in constraint-based models, *Bioinformatics*, btz598
-
-Released under the GNU Public License (version 3.0).
-
-
-.. |License| image:: https://img.shields.io/badge/license-GPL%20v3.0-blue.svg
-   :target: https://opensource.org/licenses/GPL-3.0
-.. |PyPI version| image:: https://badge.fury.io/py/cobamp.svg
-   :target: https://badge.fury.io/py/cobamp
-.. |RTD version| image:: https://readthedocs.org/projects/cobamp/badge/?version=latest&style=plastic
-   :target: https://cobamp.readthedocs.io/
```

### Comparing `cobamp-0.2.1/src/cobamp.egg-info/SOURCES.txt` & `cobamp-0.2.2/src/cobamp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

