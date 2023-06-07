# Comparing `tmp/pydna-6.0.0a1.tar.gz` & `tmp/pydna-6.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydna-6.0.0a1.tar", max compression
+gzip compressed data, was "pydna-6.0.0a2.tar", max compression
```

## Comparing `pydna-6.0.0a1.tar` & `pydna-6.0.0a2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rwxr-xr-x   0        0        0     6255 2023-06-05 10:13:56.394878 pydna-6.0.0a1/LICENSE.txt
--rwxr-xr-x   0        0        0    13820 2023-06-05 10:13:56.394878 pydna-6.0.0a1/README.md
--rw-r--r--   0        0        0     2937 2023-06-05 10:14:33.755828 pydna-6.0.0a1/pyproject.toml
--rw-r--r--   0        0        0    12827 2023-06-05 10:14:33.755828 pydna-6.0.0a1/src/pydna/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/_pretty.py
--rw-r--r--   0        0        0    10903 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/_thermodynamic_data.py
--rw-r--r--   0        0        0     2099 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/all.py
--rwxr-xr-x   0        0        0     5732 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/amplicon.py
--rw-r--r--   0        0        0    18635 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/amplify.py
--rw-r--r--   0        0        0    19159 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/assembly.py
--rw-r--r--   0        0        0     2053 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/biosubclasses.py
--rw-r--r--   0        0        0     2408 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/codon.py
--rw-r--r--   0        0        0    11157 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/common_sub_strings.py
--rwxr-xr-x   0        0        0      975 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/conftest.py
--rw-r--r--   0        0        0     7967 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/contig.py
--rwxr-xr-x   0        0        0    26230 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/design.py
--rw-r--r--   0        0        0     1315 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/download.py
--rw-r--r--   0        0        0    42601 2023-06-05 10:13:56.538881 pydna-6.0.0a1/src/pydna/dseq.py
--rw-r--r--   0        0        0    45167 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/dseqrecord.py
--rw-r--r--   0        0        0     3471 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/editor.py
--rwxr-xr-x   0        0        0     1343 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/fakeseq.py
--rw-r--r--   0        0        0     8425 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/gateway.py
--rwxr-xr-x   0        0        0     3537 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/gel.py
--rw-r--r--   0        0        0     8809 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/genbank.py
--rw-r--r--   0        0        0     1704 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/genbankfile.py
--rw-r--r--   0        0        0    20690 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/genbankfixer.py
--rw-r--r--   0        0        0     5714 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/genbankrecord.py
--rw-r--r--   0        0        0     1747 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/goldengate.py
--rw-r--r--   0        0        0     2958 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/gui.py
--rwxr-xr-x   0        0        0     3574 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/ladders.py
--rw-r--r--   0        0        0     1802 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/myenzymes.py
--rw-r--r--   0        0        0     7164 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/myprimers.py
--rw-r--r--   0        0        0     7997 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/parsers.py
--rw-r--r--   0        0        0     2533 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/primer.py
--rw-r--r--   0        0        0     1710 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/readers.py
--rw-r--r--   0        0        0     4123 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/seq.py
--rwxr-xr-x   0        0        0    21956 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/seqrecord.py
--rw-r--r--   0        0        0     1642 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/sequence_picker.py
--rw-r--r--   0        0        0     2629 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/threading_timer_decorator_exit.py
--rw-r--r--   0        0        0     9753 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/tm.py
--rw-r--r--   0        0        0    23408 2023-06-05 10:13:56.542882 pydna-6.0.0a1/src/pydna/utils.py
--rw-r--r--   0        0        0    15140 1970-01-01 00:00:00.000000 pydna-6.0.0a1/PKG-INFO
+-rwxr-xr-x   0        0        0     6255 2023-06-07 06:38:43.866768 pydna-6.0.0a2/LICENSE.txt
+-rwxr-xr-x   0        0        0    13807 2023-06-07 06:38:43.866768 pydna-6.0.0a2/README.md
+-rw-r--r--   0        0        0     2937 2023-06-07 06:39:29.363227 pydna-6.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0    12835 2023-06-07 06:39:29.367227 pydna-6.0.0a2/src/pydna/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/_pretty.py
+-rw-r--r--   0        0        0    10903 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/_thermodynamic_data.py
+-rw-r--r--   0        0        0     2099 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/all.py
+-rwxr-xr-x   0        0        0     5732 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/amplicon.py
+-rw-r--r--   0        0        0    18635 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/amplify.py
+-rw-r--r--   0        0        0    19159 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/assembly.py
+-rw-r--r--   0        0        0     2053 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/biosubclasses.py
+-rw-r--r--   0        0        0     2408 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/codon.py
+-rw-r--r--   0        0        0    11157 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/common_sub_strings.py
+-rwxr-xr-x   0        0        0      975 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/conftest.py
+-rw-r--r--   0        0        0     7967 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/contig.py
+-rwxr-xr-x   0        0        0    26230 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/design.py
+-rw-r--r--   0        0        0     1315 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/download.py
+-rw-r--r--   0        0        0    42601 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/dseq.py
+-rw-r--r--   0        0        0    45177 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/dseqrecord.py
+-rw-r--r--   0        0        0     3471 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/editor.py
+-rwxr-xr-x   0        0        0     1343 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/fakeseq.py
+-rw-r--r--   0        0        0     8425 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/gateway.py
+-rwxr-xr-x   0        0        0     3537 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/gel.py
+-rw-r--r--   0        0        0     8809 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/genbank.py
+-rw-r--r--   0        0        0     1704 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/genbankfile.py
+-rw-r--r--   0        0        0    20690 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/genbankfixer.py
+-rw-r--r--   0        0        0     5714 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/genbankrecord.py
+-rw-r--r--   0        0        0     1747 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/goldengate.py
+-rw-r--r--   0        0        0     2958 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/gui.py
+-rwxr-xr-x   0        0        0     3574 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/ladders.py
+-rw-r--r--   0        0        0     1802 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/myenzymes.py
+-rw-r--r--   0        0        0     7164 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/myprimers.py
+-rw-r--r--   0        0        0     7997 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/parsers.py
+-rw-r--r--   0        0        0     2533 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/primer.py
+-rw-r--r--   0        0        0     1710 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/readers.py
+-rw-r--r--   0        0        0     4123 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/seq.py
+-rwxr-xr-x   0        0        0    21956 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/seqrecord.py
+-rw-r--r--   0        0        0     1642 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/sequence_picker.py
+-rw-r--r--   0        0        0     2629 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/threading_timer_decorator_exit.py
+-rw-r--r--   0        0        0     9753 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/tm.py
+-rw-r--r--   0        0        0    23408 2023-06-07 06:38:44.038769 pydna-6.0.0a2/src/pydna/utils.py
+-rw-r--r--   0        0        0    15127 1970-01-01 00:00:00.000000 pydna-6.0.0a2/PKG-INFO
```

### Comparing `pydna-6.0.0a1/LICENSE.txt` & `pydna-6.0.0a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/README.md` & `pydna-6.0.0a2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1
+Name: pydna
+Version: 6.0.0a2
+Summary: Representing double stranded DNA and functions for simulating cloning and homologous recombination between DNA molecules.
+License: BSD
+Author: BjornFJohansson
+Author-email: bjornjobb@gmail.com
+Requires-Python: >=3.8
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: download
+Provides-Extra: express
+Provides-Extra: gel
+Provides-Extra: gui
+Requires-Dist: appdirs (>=1.4.4)
+Requires-Dist: biopython (>=1.80)
+Requires-Dist: cai2 (>=1.0.5) ; extra == "express"
+Requires-Dist: matplotlib (>=3.4.3) ; extra == "gel"
+Requires-Dist: networkx (>=2.8.8)
+Requires-Dist: pillow (>=8.4.0) ; extra == "gel"
+Requires-Dist: prettytable (>=3.5.0)
+Requires-Dist: pydivsufsort (>=0.0.11)
+Requires-Dist: pyfiglet (>=0.8.post1)
+Requires-Dist: pyparsing (>=2.4.7) ; extra == "download"
+Requires-Dist: pyperclip (>=1.8.2)
+Requires-Dist: pyqt5 (>=5.15.0) ; extra == "gui"
+Requires-Dist: requests (>=2.26.0) ; extra == "download"
+Requires-Dist: scipy (>=1.8.0) ; extra == "gel"
+Description-Content-Type: text/markdown
+
 # ![icon](https://raw.githubusercontent.com/bjornFJohansson/pydna/master/docs/pics/pydna.resized.png) pydna
 
 | [![Tests & Coverage](https://github.com/BjornFJohansson/pydna/actions/workflows/pydna_test_and_coverage_workflow.yml/badge.svg?branch=dev_bjorn)](https://github.com/BjornFJohansson/pydna/actions/workflows/pydna_test_and_coverage_workflow.yml) | [![codecov](https://codecov.io/gh/BjornFJohansson/pydna/branch/master/graph/badge.svg)](https://codecov.io/gh/BjornFJohansson/pydna/branch/master) | [![PyPI version](https://badge.fury.io/py/pydna.svg)](https://badge.fury.io/py/pydna)    | [![Google group : pydna](https://img.shields.io/badge/Google%20Group-pydna-blue.svg)](https://groups.google.com/g/pydna)              |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
 | [![Documentation Status](https://readthedocs.org/projects/pydna/badge/?version=latest)](http://pydna.readthedocs.io/?badge=latest)                                                                   | [![GitHub issues](https://img.shields.io/github/issues/BjornFJohansson/pydna.svg)](https://github.com/BjornFJohansson/pydna/issues)                | [![Anaconda-Server Badge2](https://anaconda.org/bjornfjohansson/pydna/badges/license.svg)](https://anaconda.org/bjornfjohansson/pydna) | [![GitHub stars](https://img.shields.io/github/stars/BjornFJohansson/pydna.svg)](https://github.com/BjornFJohansson/pydna/stargazers) |
 
 
@@ -41,15 +75,15 @@
 To get started, I have compiled some [simple examples](https://github.com/MetabolicEngineeringGroupCBMA/pydna-examples#pydna-examples).
 For more elaborate use, look at some assembly strategies of D-xylose metabolic pathways [MetabolicEngineeringGroupCBMA/ypk-xylose-pathways](https://github.com/MetabolicEngineeringGroupCBMA/ypk-xylose-pathways#pereira-et-al-2016).
 
 
 
 
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 
 
 ## Usage
 
 Most pydna functionality is implemented as methods for the double stranded DNA sequence record
 classes Dseq and Dseqrecord, which are subclasses of the [Biopython](http://biopython.org/wiki/Main_Page) [Seq](http://biopython.org/wiki/Seq) and [SeqRecord](http://biopython.org/wiki/SeqRecord) classes.
@@ -84,15 +118,15 @@
 python. This is helpful to generate examples for teaching purposes.
 
 Read the documentation (below) or the [cookbook](https://github.com/BjornFJohansson/pydna/blob/master/docs/cookbook/cookbook.ipynb) with example files
 for further information.
 
 Feedback & suggestions are very welcome! Please post a message in the [google group](https://groups.google.com/d/forum/pydna) for pydna if you need help or have problems, questions or comments :sos:.
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 
 ## Who is using pydna?
 
 Taylor, L. J., & Strebel, K. (2017).
 Pyviko: an automated Python tool to design gene knockouts in complex viruses with overlapping genes.
 BMC Microbiology, 17(1), 12.
@@ -106,38 +140,38 @@
 
 
 [An Automated Protein Synthesis Pipeline with Transcriptic and Snakemake](http://blog.booleanbiotech.com/transcriptic_protein_synthesis_pipeline.html)
 
 
 and other projects on [github](https://github.com/BjornFJohansson/pydna/network/dependents?package_id=UGFja2FnZS01MjQ2MjYzNQ%3D%3D)
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 There is an open access paper in BMC Bioinformatics describing pydna:
 
 [![abstr](https://raw.githubusercontent.com/bjornFJohansson/pydna/master/docs/pics/BMC_resized.png)](http://www.biomedcentral.com/1471-2105/16/142/abstract)
 
 Please reference the above paper:
 
 
 Pereira, F., Azevedo, F., Carvalho, Â., Ribeiro, G. F., Budde, M. W., & Johansson, B. (2015). Pydna: a simulation and documentation tool for DNA assembly strategies using python. BMC Bioinformatics, 16(142), 142.
 
 
 When using pydna.
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## Documentation
 
 Documentation is built using [Sphinx](http://www.sphinx-doc.org/) from [docstrings](https://www.python.org/dev/peps/pep-0257/)
 in the code and displayed at readthedocs [![Documentation Status](https://readthedocs.org/projects/pydna/badge/?version=latest)](http://pydna.readthedocs.io/?badge=latest)
 
 The [numpy](www.numpy.org) [docstring format](https://github.com/numpy/numpy/blob/release/doc/HOWTO_DOCUMENT.rst.txt) is used.
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## Installation using pip
 
 Pip is included in recent Python versions and is the
 officially [recommended](http://python-packaging-user-guide.readthedocs.org/en/latest) tool.
 
 Pip installs the minimal installation requirements automatically, but not the optional requirements (see below).
@@ -160,69 +194,89 @@
 
     C:\> pip install pydna
 
 By default python and pip are not on the PATH. You can re-install Python and select this option during installation, or give the full path for pip. Try something like this, depending on where your copy of Python is installed:
 
     C:\Python37\Scripts\pip install pydna
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## Source Code
 
 Pydna is developed on [Github](https://github.com/BjornFJohansson/pydna) :octocat:.
+I am happy to collaborate on new features or bugfixes.
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## Minimal installation dependencies
 
-Pydna versions before 1.0.0 were compatible with python 2.7 only.
 The list below is the minimal requirements for installing pydna.
-Biopython has c-extensions, but the other modules are pure python.
+Biopython and pydivsufsort has c-extensions, but the other modules are pure python.
 
 - [Python 3.8, 3.9, 3.10 or 3.11](http://www.python.org)
-- [appdirs >=1.4.4](https://pypi.python.org/pypi/appdirs)
-- [biopython >= 1.80](http://pypi.python.org/pypi/biopython)
-- [networkx >=2.8.8](http://pypi.python.org/pypi/networkx)
-- [prettytable >=3.5.0](https://pypi.python.org/pypi/PrettyTable)
-- [pyperclip >=1.8.2](https://pypi.python.org/pypi/PrettyTable)
-- [pyfiglet >=0.8.post1](https://pypi.python.org/pypi/PrettyTable)
+- [appdirs](https://pypi.python.org/pypi/appdirs)
+- [biopython](http://pypi.python.org/pypi/biopython)
+- [networkx](http://pypi.python.org/pypi/networkx)
+- [prettytable](https://pypi.python.org/pypi/PrettyTable)
+- [pydivsufsort](https://pypi.python.org/pypi/pydivsufsort)
 
+The above modules are installed as well as pyperclip and pyfiglet.
+Pydna is importable even without these two modules.
 
 ## Optional dependencies
 
 If the modules listed below in the first column are installed, they will provide the functionality listed in the second column.
 
-| Dependency                                                  | Function in pydna                                      |
-|-------------------------------------------------------------|--------------------------------------------------------|
-| [scipy >=1.8.0](https://www.scipy.org)                      | gel simulation with pydna.gel                          |
-| [matplotlib >=3.4.3](http://matplotlib.org)                 | “                                                      |
-| [pillow >=8.4.0](https://github.com/python-pillow/Pillow)   | “                                                      |
-| [numpy](http://www.numpy.org)                               | "                                                      |
-| [pyparsing >=2.4.7](https://pypi.python.org/pypi/pyparsing) | fix corrupt Genbank files with pydna.genbankfixer      |
-| [requests >=2.26.0](https://pypi.org/project/requests)      | download sequences with pydna.download                 |
-| [cai2 >=1.0.5](https://pypi.python.org/pypi/cai2)           | codon adaptation index calculations in several modules |
-| [pyqt5 >=5.15.0](https://pypi.python.org/pypi/pyqt5)        | codon adaptation index calculations in several modules |
-
+| Dependency                                          | Function in pydna                                      |
+|-----------------------------------------------------|--------------------------------------------------------|
+| [scipy](https://www.scipy.org)                      | gel simulation with pydna.gel                          |
+| [matplotlib](http://matplotlib.org)                 | “                                                      |
+| [pillow](https://github.com/python-pillow/Pillow)   | “                                                      |
+| [numpy](http://www.numpy.org)                       | "                                                      |
+| [pyparsing](https://pypi.python.org/pypi/pyparsing) | fix corrupt Genbank files with pydna.genbankfixer      |
+| [requests](https://pypi.org/project/requests)       | download sequences with pydna.download                 |
+| [cai2](https://pypi.python.org/pypi/cai2)           | codon adaptation index calculations in several modules |
+| [pyqt5](https://pypi.python.org/pypi/pyqt5)         | future plan for gui                                    |
+| [pyperclip](https://pypi.python.org/pypi/pyperclip) | copy sequence to clipboard                             |
+| [pyfiglet](https://pypi.python.org/pypi/pyfiglet)   | print nice logotype (pydna.logo()                      |
 
-## Requirements for running tests and analyzing code coverage
+## Requirements for running tests, coverage and profiling
 
 - [pytest](https://pypi.org/project/pytest)
 - [pytest-cov](https://pypi.org/project/pytest-cov)
 - [pytest-doctestplus](https://pypi.org/project/pytest-doctestplus)
+- [pytest-profiling](https://pypi.org/project/pytest-profiling)
 - [coverage](https://pypi.org/project/coverage)
 - [nbval](https://pypi.org/project/nbval)
 - [requests-mock](https://pypi.org/project/requests-mock)
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+for instance by `pip install pytest pytest-cov pytest-doctestplus pytest-profiling coverage nbval requests-mock`
+
+Running the antire test suite also require:
+
+- scipy
+- matplotlib
+- pillow
+- pyparsing
+- requests
+- cai2
+- pyqt5
+
+That can be installed by `pip install pydna[gel,gui,download,express]`
+
+or by `pip install scipy matplotlib pillow pyparsing requests cai2 pyqt5`
+
+
+![----]( http://bit.ly/coloredline)
 
 ## Releases
 
 See the [releases](https://github.com/BjornFJohansson/pydna/releases) for changes and releases.
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## Automatic testing & Release process
 
 There are two github actions for this package:
 
 - `pydna_test_and_coverage_workflow.yml`
 - `pydna_pypi_build_workflow.yml`
@@ -231,15 +285,15 @@
 This workflow run tests, doctests and a series of Jupyter notebooks using pytest on Linux, Windows and macOS and all
 supported python versions.
 
 The other workflow builds a PyPI packages using poetry on
 
 These are triggered by publishing a github release manually from the github interface.
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## Building a PyPI package with [Poetry](https://pypi.org/project/poetry)
 
 1. Commit changes to git
 2. Tag the commit according to the [Semantic Versioning](https://semver.org) format, for example "v2.0.1a3". Do not forget the "v" or poetry will not recognize the tag.
 
         git tag v2.0.1a3
@@ -258,18 +312,19 @@
 
 6. Verify the filename of the files in the dist/ folder, they should match
 
 7. Publish to pypi
 
         poetry publish
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## History
 
 Pydna was made public in 2012 on [Google code](https://code.google.com/archive/p/pydna).
 
 
 :microbe:
 
 
 :portugal:
+
```

### Comparing `pydna-6.0.0a1/pyproject.toml` & `pydna-6.0.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 [project.urls]
 homepage = "https://github.com/BjornFJohansson/pydna#-pydna"
 documentation = "https://pydna.readthedocs.io/?badge=latest"
 repository = "https://github.com/BjornFJohansson/pydna/tree/dev_bjorn"
 changelog = "https://github.com/BjornFJohansson/pydna/blob/master/docs/CHANGELOG.md#changelog"
 [tool.poetry]
 name = "pydna"
-version = "6.0.0-a.1"
+version = "6.0.0-a.2"
 description = "Representing double stranded DNA and functions for simulating cloning and homologous recombination between DNA molecules."
 authors = ["BjornFJohansson <bjornjobb@gmail.com>"]
 license = "BSD"
 readme = "README.md"
 [tool.poetry.dependencies]
 python = ">=3.8"
 appdirs = ">=1.4.4"
```

### Comparing `pydna-6.0.0a1/src/pydna/__init__.py` & `pydna-6.0.0a2/src/pydna/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 __author__ = "Björn Johansson"
 __copyright__ = "Copyright 2013 - 2021 Björn Johansson"
 __credits__ = ["Björn Johansson", "Mark Budde"]
 __license__ = "BSD"
 __maintainer__ = "Björn Johansson"
 __email__ = "bjorn_johansson@bio.uminho.pt"
 __status__ = "Development"  # "Production" #"Prototype"
-__version__ = "6.0.0-a.1"
+__version__ = "6.0.0-a.2"
 
 # create config directory
 _os.environ["pydna_config_dir"] = _os.getenv("pydna_config_dir", _appdirs.user_config_dir("pydna"))
 config_dir = _Path(_os.environ["pydna_config_dir"])
 config_dir.mkdir(parents=True, exist_ok=True)
 
 # set path for the pydna.ini file
@@ -362,15 +362,15 @@
     """
     _table = _PrettyTable(["Variable", "Value"])
     # _table.set_style(_prettytable.DEFAULT)
     _table.align["Variable"] = "l"  # Left align
     _table.align["Value"] = "l"  # Left align
     _table.padding_width = 1  # One space between column edges and contents
     for k, v in sorted(_os.environ.items()):
-        if k.startswith("pydna"):
+        if k.lower().startswith("pydna"):
             _table.add_row([k, v])
     return _table
 
 
 def logo():
     """Ascii-art logotype of pydna."""
     from pydna._pretty import pretty_str as _pretty_str
```

### Comparing `pydna-6.0.0a1/src/pydna/_pretty.py` & `pydna-6.0.0a2/src/pydna/_pretty.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/_thermodynamic_data.py` & `pydna-6.0.0a2/src/pydna/_thermodynamic_data.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/all.py` & `pydna-6.0.0a2/src/pydna/all.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/amplicon.py` & `pydna-6.0.0a2/src/pydna/amplicon.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/amplify.py` & `pydna-6.0.0a2/src/pydna/amplify.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/assembly.py` & `pydna-6.0.0a2/src/pydna/assembly.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/biosubclasses.py` & `pydna-6.0.0a2/src/pydna/biosubclasses.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/codon.py` & `pydna-6.0.0a2/src/pydna/codon.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/common_sub_strings.py` & `pydna-6.0.0a2/src/pydna/common_sub_strings.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/conftest.py` & `pydna-6.0.0a2/src/pydna/conftest.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/contig.py` & `pydna-6.0.0a2/src/pydna/contig.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/design.py` & `pydna-6.0.0a2/src/pydna/design.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/download.py` & `pydna-6.0.0a2/src/pydna/download.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/dseq.py` & `pydna-6.0.0a2/src/pydna/dseq.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/dseqrecord.py` & `pydna-6.0.0a2/src/pydna/dseqrecord.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from pydna.utils import identifier_from_string as _identifier_from_string
 import copy as _copy
 import operator as _operator
 import os as _os
 import re as _re
 import time as _time
 import datetime as _datetime
-import pyperclip
+
 
 import logging as _logging
 
 _module_logger = _logging.getLogger("pydna." + __name__)
 
 
 try:
@@ -1163,15 +1163,17 @@
 
     def orfs(self, minsize=30):
         """docstring."""
         return tuple(Dseqrecord(s) for s in self.seq.orfs(minsize=minsize))
 
     def _copy_to_clipboard(self, sequence_format):
         """docstring."""
-        pyperclip.copy(self.format(sequence_format))
+        from pyperclip import copy
+
+        copy(self.format(sequence_format))
         return None
 
     def copy_gb_to_clipboard(self):
         """docstring."""
         self._copy_to_clipboard("gb")
         return None
```

### Comparing `pydna-6.0.0a1/src/pydna/editor.py` & `pydna-6.0.0a2/src/pydna/editor.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/fakeseq.py` & `pydna-6.0.0a2/src/pydna/fakeseq.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/gateway.py` & `pydna-6.0.0a2/src/pydna/gateway.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/gel.py` & `pydna-6.0.0a2/src/pydna/gel.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/genbank.py` & `pydna-6.0.0a2/src/pydna/genbank.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/genbankfile.py` & `pydna-6.0.0a2/src/pydna/genbankfile.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/genbankfixer.py` & `pydna-6.0.0a2/src/pydna/genbankfixer.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/genbankrecord.py` & `pydna-6.0.0a2/src/pydna/genbankrecord.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/goldengate.py` & `pydna-6.0.0a2/src/pydna/goldengate.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/gui.py` & `pydna-6.0.0a2/src/pydna/gui.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/ladders.py` & `pydna-6.0.0a2/src/pydna/ladders.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/myenzymes.py` & `pydna-6.0.0a2/src/pydna/myenzymes.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/myprimers.py` & `pydna-6.0.0a2/src/pydna/myprimers.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/parsers.py` & `pydna-6.0.0a2/src/pydna/parsers.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/primer.py` & `pydna-6.0.0a2/src/pydna/primer.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/readers.py` & `pydna-6.0.0a2/src/pydna/readers.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/seq.py` & `pydna-6.0.0a2/src/pydna/seq.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/seqrecord.py` & `pydna-6.0.0a2/src/pydna/seqrecord.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/sequence_picker.py` & `pydna-6.0.0a2/src/pydna/sequence_picker.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/threading_timer_decorator_exit.py` & `pydna-6.0.0a2/src/pydna/threading_timer_decorator_exit.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/tm.py` & `pydna-6.0.0a2/src/pydna/tm.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/src/pydna/utils.py` & `pydna-6.0.0a2/src/pydna/utils.py`

 * *Files identical despite different names*

### Comparing `pydna-6.0.0a1/PKG-INFO` & `pydna-6.0.0a2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,7 @@
-Metadata-Version: 2.1
-Name: pydna
-Version: 6.0.0a1
-Summary: Representing double stranded DNA and functions for simulating cloning and homologous recombination between DNA molecules.
-License: BSD
-Author: BjornFJohansson
-Author-email: bjornjobb@gmail.com
-Requires-Python: >=3.8
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: download
-Provides-Extra: express
-Provides-Extra: gel
-Provides-Extra: gui
-Requires-Dist: appdirs (>=1.4.4)
-Requires-Dist: biopython (>=1.80)
-Requires-Dist: cai2 (>=1.0.5) ; extra == "express"
-Requires-Dist: matplotlib (>=3.4.3) ; extra == "gel"
-Requires-Dist: networkx (>=2.8.8)
-Requires-Dist: pillow (>=8.4.0) ; extra == "gel"
-Requires-Dist: prettytable (>=3.5.0)
-Requires-Dist: pydivsufsort (>=0.0.11)
-Requires-Dist: pyfiglet (>=0.8.post1)
-Requires-Dist: pyparsing (>=2.4.7) ; extra == "download"
-Requires-Dist: pyperclip (>=1.8.2)
-Requires-Dist: pyqt5 (>=5.15.0) ; extra == "gui"
-Requires-Dist: requests (>=2.26.0) ; extra == "download"
-Requires-Dist: scipy (>=1.8.0) ; extra == "gel"
-Description-Content-Type: text/markdown
-
 # ![icon](https://raw.githubusercontent.com/bjornFJohansson/pydna/master/docs/pics/pydna.resized.png) pydna
 
 | [![Tests & Coverage](https://github.com/BjornFJohansson/pydna/actions/workflows/pydna_test_and_coverage_workflow.yml/badge.svg?branch=dev_bjorn)](https://github.com/BjornFJohansson/pydna/actions/workflows/pydna_test_and_coverage_workflow.yml) | [![codecov](https://codecov.io/gh/BjornFJohansson/pydna/branch/master/graph/badge.svg)](https://codecov.io/gh/BjornFJohansson/pydna/branch/master) | [![PyPI version](https://badge.fury.io/py/pydna.svg)](https://badge.fury.io/py/pydna)    | [![Google group : pydna](https://img.shields.io/badge/Google%20Group-pydna-blue.svg)](https://groups.google.com/g/pydna)              |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
 | [![Documentation Status](https://readthedocs.org/projects/pydna/badge/?version=latest)](http://pydna.readthedocs.io/?badge=latest)                                                                   | [![GitHub issues](https://img.shields.io/github/issues/BjornFJohansson/pydna.svg)](https://github.com/BjornFJohansson/pydna/issues)                | [![Anaconda-Server Badge2](https://anaconda.org/bjornfjohansson/pydna/badges/license.svg)](https://anaconda.org/bjornfjohansson/pydna) | [![GitHub stars](https://img.shields.io/github/stars/BjornFJohansson/pydna.svg)](https://github.com/BjornFJohansson/pydna/stargazers) |
 
 
@@ -75,15 +41,15 @@
 To get started, I have compiled some [simple examples](https://github.com/MetabolicEngineeringGroupCBMA/pydna-examples#pydna-examples).
 For more elaborate use, look at some assembly strategies of D-xylose metabolic pathways [MetabolicEngineeringGroupCBMA/ypk-xylose-pathways](https://github.com/MetabolicEngineeringGroupCBMA/ypk-xylose-pathways#pereira-et-al-2016).
 
 
 
 
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 
 
 ## Usage
 
 Most pydna functionality is implemented as methods for the double stranded DNA sequence record
 classes Dseq and Dseqrecord, which are subclasses of the [Biopython](http://biopython.org/wiki/Main_Page) [Seq](http://biopython.org/wiki/Seq) and [SeqRecord](http://biopython.org/wiki/SeqRecord) classes.
@@ -118,15 +84,15 @@
 python. This is helpful to generate examples for teaching purposes.
 
 Read the documentation (below) or the [cookbook](https://github.com/BjornFJohansson/pydna/blob/master/docs/cookbook/cookbook.ipynb) with example files
 for further information.
 
 Feedback & suggestions are very welcome! Please post a message in the [google group](https://groups.google.com/d/forum/pydna) for pydna if you need help or have problems, questions or comments :sos:.
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 
 ## Who is using pydna?
 
 Taylor, L. J., & Strebel, K. (2017).
 Pyviko: an automated Python tool to design gene knockouts in complex viruses with overlapping genes.
 BMC Microbiology, 17(1), 12.
@@ -140,38 +106,38 @@
 
 
 [An Automated Protein Synthesis Pipeline with Transcriptic and Snakemake](http://blog.booleanbiotech.com/transcriptic_protein_synthesis_pipeline.html)
 
 
 and other projects on [github](https://github.com/BjornFJohansson/pydna/network/dependents?package_id=UGFja2FnZS01MjQ2MjYzNQ%3D%3D)
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 There is an open access paper in BMC Bioinformatics describing pydna:
 
 [![abstr](https://raw.githubusercontent.com/bjornFJohansson/pydna/master/docs/pics/BMC_resized.png)](http://www.biomedcentral.com/1471-2105/16/142/abstract)
 
 Please reference the above paper:
 
 
 Pereira, F., Azevedo, F., Carvalho, Â., Ribeiro, G. F., Budde, M. W., & Johansson, B. (2015). Pydna: a simulation and documentation tool for DNA assembly strategies using python. BMC Bioinformatics, 16(142), 142.
 
 
 When using pydna.
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## Documentation
 
 Documentation is built using [Sphinx](http://www.sphinx-doc.org/) from [docstrings](https://www.python.org/dev/peps/pep-0257/)
 in the code and displayed at readthedocs [![Documentation Status](https://readthedocs.org/projects/pydna/badge/?version=latest)](http://pydna.readthedocs.io/?badge=latest)
 
 The [numpy](www.numpy.org) [docstring format](https://github.com/numpy/numpy/blob/release/doc/HOWTO_DOCUMENT.rst.txt) is used.
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## Installation using pip
 
 Pip is included in recent Python versions and is the
 officially [recommended](http://python-packaging-user-guide.readthedocs.org/en/latest) tool.
 
 Pip installs the minimal installation requirements automatically, but not the optional requirements (see below).
@@ -194,69 +160,89 @@
 
     C:\> pip install pydna
 
 By default python and pip are not on the PATH. You can re-install Python and select this option during installation, or give the full path for pip. Try something like this, depending on where your copy of Python is installed:
 
     C:\Python37\Scripts\pip install pydna
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## Source Code
 
 Pydna is developed on [Github](https://github.com/BjornFJohansson/pydna) :octocat:.
+I am happy to collaborate on new features or bugfixes.
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## Minimal installation dependencies
 
-Pydna versions before 1.0.0 were compatible with python 2.7 only.
 The list below is the minimal requirements for installing pydna.
-Biopython has c-extensions, but the other modules are pure python.
+Biopython and pydivsufsort has c-extensions, but the other modules are pure python.
 
 - [Python 3.8, 3.9, 3.10 or 3.11](http://www.python.org)
-- [appdirs >=1.4.4](https://pypi.python.org/pypi/appdirs)
-- [biopython >= 1.80](http://pypi.python.org/pypi/biopython)
-- [networkx >=2.8.8](http://pypi.python.org/pypi/networkx)
-- [prettytable >=3.5.0](https://pypi.python.org/pypi/PrettyTable)
-- [pyperclip >=1.8.2](https://pypi.python.org/pypi/PrettyTable)
-- [pyfiglet >=0.8.post1](https://pypi.python.org/pypi/PrettyTable)
+- [appdirs](https://pypi.python.org/pypi/appdirs)
+- [biopython](http://pypi.python.org/pypi/biopython)
+- [networkx](http://pypi.python.org/pypi/networkx)
+- [prettytable](https://pypi.python.org/pypi/PrettyTable)
+- [pydivsufsort](https://pypi.python.org/pypi/pydivsufsort)
 
+The above modules are installed as well as pyperclip and pyfiglet.
+Pydna is importable even without these two modules.
 
 ## Optional dependencies
 
 If the modules listed below in the first column are installed, they will provide the functionality listed in the second column.
 
-| Dependency                                                  | Function in pydna                                      |
-|-------------------------------------------------------------|--------------------------------------------------------|
-| [scipy >=1.8.0](https://www.scipy.org)                      | gel simulation with pydna.gel                          |
-| [matplotlib >=3.4.3](http://matplotlib.org)                 | “                                                      |
-| [pillow >=8.4.0](https://github.com/python-pillow/Pillow)   | “                                                      |
-| [numpy](http://www.numpy.org)                               | "                                                      |
-| [pyparsing >=2.4.7](https://pypi.python.org/pypi/pyparsing) | fix corrupt Genbank files with pydna.genbankfixer      |
-| [requests >=2.26.0](https://pypi.org/project/requests)      | download sequences with pydna.download                 |
-| [cai2 >=1.0.5](https://pypi.python.org/pypi/cai2)           | codon adaptation index calculations in several modules |
-| [pyqt5 >=5.15.0](https://pypi.python.org/pypi/pyqt5)        | codon adaptation index calculations in several modules |
-
+| Dependency                                          | Function in pydna                                      |
+|-----------------------------------------------------|--------------------------------------------------------|
+| [scipy](https://www.scipy.org)                      | gel simulation with pydna.gel                          |
+| [matplotlib](http://matplotlib.org)                 | “                                                      |
+| [pillow](https://github.com/python-pillow/Pillow)   | “                                                      |
+| [numpy](http://www.numpy.org)                       | "                                                      |
+| [pyparsing](https://pypi.python.org/pypi/pyparsing) | fix corrupt Genbank files with pydna.genbankfixer      |
+| [requests](https://pypi.org/project/requests)       | download sequences with pydna.download                 |
+| [cai2](https://pypi.python.org/pypi/cai2)           | codon adaptation index calculations in several modules |
+| [pyqt5](https://pypi.python.org/pypi/pyqt5)         | future plan for gui                                    |
+| [pyperclip](https://pypi.python.org/pypi/pyperclip) | copy sequence to clipboard                             |
+| [pyfiglet](https://pypi.python.org/pypi/pyfiglet)   | print nice logotype (pydna.logo()                      |
 
-## Requirements for running tests and analyzing code coverage
+## Requirements for running tests, coverage and profiling
 
 - [pytest](https://pypi.org/project/pytest)
 - [pytest-cov](https://pypi.org/project/pytest-cov)
 - [pytest-doctestplus](https://pypi.org/project/pytest-doctestplus)
+- [pytest-profiling](https://pypi.org/project/pytest-profiling)
 - [coverage](https://pypi.org/project/coverage)
 - [nbval](https://pypi.org/project/nbval)
 - [requests-mock](https://pypi.org/project/requests-mock)
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+for instance by `pip install pytest pytest-cov pytest-doctestplus pytest-profiling coverage nbval requests-mock`
+
+Running the antire test suite also require:
+
+- scipy
+- matplotlib
+- pillow
+- pyparsing
+- requests
+- cai2
+- pyqt5
+
+That can be installed by `pip install pydna[gel,gui,download,express]`
+
+or by `pip install scipy matplotlib pillow pyparsing requests cai2 pyqt5`
+
+
+![----]( http://bit.ly/coloredline)
 
 ## Releases
 
 See the [releases](https://github.com/BjornFJohansson/pydna/releases) for changes and releases.
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## Automatic testing & Release process
 
 There are two github actions for this package:
 
 - `pydna_test_and_coverage_workflow.yml`
 - `pydna_pypi_build_workflow.yml`
@@ -265,15 +251,15 @@
 This workflow run tests, doctests and a series of Jupyter notebooks using pytest on Linux, Windows and macOS and all
 supported python versions.
 
 The other workflow builds a PyPI packages using poetry on
 
 These are triggered by publishing a github release manually from the github interface.
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## Building a PyPI package with [Poetry](https://pypi.org/project/poetry)
 
 1. Commit changes to git
 2. Tag the commit according to the [Semantic Versioning](https://semver.org) format, for example "v2.0.1a3". Do not forget the "v" or poetry will not recognize the tag.
 
         git tag v2.0.1a3
@@ -292,19 +278,18 @@
 
 6. Verify the filename of the files in the dist/ folder, they should match
 
 7. Publish to pypi
 
         poetry publish
 
-![----](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)
+![----]( http://bit.ly/coloredline)
 
 ## History
 
 Pydna was made public in 2012 on [Google code](https://code.google.com/archive/p/pydna).
 
 
 :microbe:
 
 
 :portugal:
-
```

