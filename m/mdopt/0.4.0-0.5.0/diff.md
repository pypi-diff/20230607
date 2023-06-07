# Comparing `tmp/mdopt-0.4.0.tar.gz` & `tmp/mdopt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdopt-0.4.0.tar", max compression
+gzip compressed data, was "mdopt-0.5.0.tar", max compression
```

## Comparing `mdopt-0.4.0.tar` & `mdopt-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1078 2023-02-07 16:00:32.106100 mdopt-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     1434 2023-06-04 04:29:40.989489 mdopt-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-02-07 16:00:32.119334 mdopt-0.4.0/mdopt/__init__.py
--rw-r--r--   0        0        0        0 2023-02-07 16:00:32.119407 mdopt-0.4.0/mdopt/contractor/__init__.py
--rw-r--r--   0        0        0    10640 2023-05-11 01:00:55.742426 mdopt-0.4.0/mdopt/contractor/contractor.py
--rw-r--r--   0        0        0        0 2023-03-08 10:03:23.369496 mdopt-0.4.0/mdopt/mps/__init__.py
--rw-r--r--   0        0        0    31245 2023-06-06 20:18:50.091990 mdopt-0.4.0/mdopt/mps/canonical.py
--rw-r--r--   0        0        0    26381 2023-05-08 12:52:41.868101 mdopt-0.4.0/mdopt/mps/explicit.py
--rw-r--r--   0        0        0    22933 2023-06-06 03:45:48.064434 mdopt-0.4.0/mdopt/mps/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 04:00:18.160606 mdopt-0.4.0/mdopt/optimiser/__init__.py
--rw-r--r--   0        0        0    13767 2023-03-08 10:03:23.370998 mdopt-0.4.0/mdopt/optimiser/dephasing_dmrg.py
--rw-r--r--   0        0        0    12325 2023-03-21 00:50:18.847156 mdopt-0.4.0/mdopt/optimiser/dmrg.py
--rw-r--r--   0        0        0     4336 2023-04-17 04:00:18.160933 mdopt-0.4.0/mdopt/optimiser/utils.py
--rw-r--r--   0        0        0        0 2023-02-07 16:00:32.120222 mdopt-0.4.0/mdopt/utils/__init__.py
--rw-r--r--   0        0        0    16600 2023-06-06 03:44:55.970289 mdopt-0.4.0/mdopt/utils/utils.py
--rw-r--r--   0        0        0     1259 2023-06-07 06:03:36.654466 mdopt-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2441 1970-01-01 00:00:00.000000 mdopt-0.4.0/setup.py
--rw-r--r--   0        0        0     2371 1970-01-01 00:00:00.000000 mdopt-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-02-07 16:00:32.106100 mdopt-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     1434 2023-06-04 04:29:40.989489 mdopt-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-07 16:00:32.119334 mdopt-0.5.0/mdopt/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-07 16:00:32.119407 mdopt-0.5.0/mdopt/contractor/__init__.py
+-rw-r--r--   0        0        0    10640 2023-05-11 01:00:55.742426 mdopt-0.5.0/mdopt/contractor/contractor.py
+-rw-r--r--   0        0        0        0 2023-03-08 10:03:23.369496 mdopt-0.5.0/mdopt/mps/__init__.py
+-rw-r--r--   0        0        0    31245 2023-06-07 06:11:28.233353 mdopt-0.5.0/mdopt/mps/canonical.py
+-rw-r--r--   0        0        0    26381 2023-05-08 12:52:41.868101 mdopt-0.5.0/mdopt/mps/explicit.py
+-rw-r--r--   0        0        0    22933 2023-06-07 06:11:28.233422 mdopt-0.5.0/mdopt/mps/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 04:00:18.160606 mdopt-0.5.0/mdopt/optimiser/__init__.py
+-rw-r--r--   0        0        0    13767 2023-03-08 10:03:23.370998 mdopt-0.5.0/mdopt/optimiser/dephasing_dmrg.py
+-rw-r--r--   0        0        0    12325 2023-03-21 00:50:18.847156 mdopt-0.5.0/mdopt/optimiser/dmrg.py
+-rw-r--r--   0        0        0     4336 2023-04-17 04:00:18.160933 mdopt-0.5.0/mdopt/optimiser/utils.py
+-rw-r--r--   0        0        0        0 2023-02-07 16:00:32.120222 mdopt-0.5.0/mdopt/utils/__init__.py
+-rw-r--r--   0        0        0    16600 2023-06-06 03:44:55.970289 mdopt-0.5.0/mdopt/utils/utils.py
+-rw-r--r--   0        0        0     1258 2023-06-07 06:12:17.004118 mdopt-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 mdopt-0.5.0/setup.py
+-rw-r--r--   0        0        0     2368 1970-01-01 00:00:00.000000 mdopt-0.5.0/PKG-INFO
```

### Comparing `mdopt-0.4.0/LICENSE.md` & `mdopt-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mdopt-0.4.0/README.md` & `mdopt-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mdopt-0.4.0/mdopt/contractor/contractor.py` & `mdopt-0.5.0/mdopt/contractor/contractor.py`

 * *Files identical despite different names*

### Comparing `mdopt-0.4.0/mdopt/mps/canonical.py` & `mdopt-0.5.0/mdopt/mps/canonical.py`

 * *Files identical despite different names*

### Comparing `mdopt-0.4.0/mdopt/mps/explicit.py` & `mdopt-0.5.0/mdopt/mps/explicit.py`

 * *Files identical despite different names*

### Comparing `mdopt-0.4.0/mdopt/mps/utils.py` & `mdopt-0.5.0/mdopt/mps/utils.py`

 * *Files identical despite different names*

### Comparing `mdopt-0.4.0/mdopt/optimiser/dephasing_dmrg.py` & `mdopt-0.5.0/mdopt/optimiser/dephasing_dmrg.py`

 * *Files identical despite different names*

### Comparing `mdopt-0.4.0/mdopt/optimiser/dmrg.py` & `mdopt-0.5.0/mdopt/optimiser/dmrg.py`

 * *Files identical despite different names*

### Comparing `mdopt-0.4.0/mdopt/optimiser/utils.py` & `mdopt-0.5.0/mdopt/optimiser/utils.py`

 * *Files identical despite different names*

### Comparing `mdopt-0.4.0/mdopt/utils/utils.py` & `mdopt-0.5.0/mdopt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mdopt-0.4.0/pyproject.toml` & `mdopt-0.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mdopt"
-version = "0.4.0"
+version = "0.5.0"
 description = "Discrete optimisation in the tensor-network (specifically, MPS-MPO) language."
 authors = [
     "Aleksandr Berezutskii <berezutskii.aleksandr@gmail.com>",
 ]
 maintainers = [
     "Aleksandr Berezutskii <berezutskii.aleksandr@gmail.com>"
 ]
@@ -15,15 +15,15 @@
 scipy = "^1.9.2"
 opt-einsum = "^3.3.0"
 more-itertools = ">=8.12,<10.0"
 threadpoolctl = "^3.1.0"
 tqdm = "^4.64.1"
 qecstruct = "^0.2.9"
 qecsim = "^1.0b9"
-numpy = "1.24.2"
+numpy = "<1.24"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.3,<24.0"
 pylint = "^2.17.4"
```

### Comparing `mdopt-0.4.0/setup.py` & `mdopt-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 ['mdopt', 'mdopt.contractor', 'mdopt.mps', 'mdopt.optimiser', 'mdopt.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['more-itertools>=8.12,<10.0',
- 'numpy==1.24.2',
+ 'numpy<1.24',
  'opt-einsum>=3.3.0,<4.0.0',
  'qecsim>=1.0b9,<2.0',
  'qecstruct>=0.2.9,<0.3.0',
  'scipy>=1.9.2,<2.0.0',
  'threadpoolctl>=3.1.0,<4.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'mdopt',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'Discrete optimisation in the tensor-network (specifically, MPS-MPO) language.',
     'long_description': '[![codecov](https://codecov.io/gh/quicophy/mdopt/branch/main/graph/badge.svg?token=4G7VWYX0S2)](https://codecov.io/gh/quicophy/mdopt)\n[![tests](https://github.com/quicophy/mdopt/actions/workflows/tests.yml/badge.svg)](https://github.com/quicophy/mdopt/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/mdopt/badge/?version=latest)](https://mdopt.readthedocs.io/en/latest/?badge=latest)\n[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/quicophy/mdopt/main.svg)](https://results.pre-commit.ci/latest/github/quicophy/mdopt/main)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# mdopt\nmdopt is a python package built on top of numpy for discrete optimisation in the tensor-network (specifically, MPS-MPO) language. The code is hosted on github, so please feel free to submit issues and pull requests.\n\n## Installation\n\nUse the package manager [pip](https://pip.pypa.io/en/stable/) to install mdopt.\n\n```bash\npip install mdopt\n```\n\n## Usage\n\nFor usage, see the examples folder.\n\n## Cite\n```\n@software{mdopt2022,\n  author = {Aleksandr Berezutskii},\n  title = {mdopt: Discrete optimization in the tensor-network (specifically, MPS-MPO) language.},\n  url = {https://github.com/quicophy/mdopt},\n  year = {2022},\n}\n```\n',
     'author': 'Aleksandr Berezutskii',
     'author_email': 'berezutskii.aleksandr@gmail.com',
     'maintainer': 'Aleksandr Berezutskii',
     'maintainer_email': 'berezutskii.aleksandr@gmail.com',
     'url': 'None',
```

### Comparing `mdopt-0.4.0/PKG-INFO` & `mdopt-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mdopt
-Version: 0.4.0
+Version: 0.5.0
 Summary: Discrete optimisation in the tensor-network (specifically, MPS-MPO) language.
 Author: Aleksandr Berezutskii
 Author-email: berezutskii.aleksandr@gmail.com
 Maintainer: Aleksandr Berezutskii
 Maintainer-email: berezutskii.aleksandr@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: more-itertools (>=8.12,<10.0)
-Requires-Dist: numpy (==1.24.2)
+Requires-Dist: numpy (<1.24)
 Requires-Dist: opt-einsum (>=3.3.0,<4.0.0)
 Requires-Dist: qecsim (>=1.0b9,<2.0)
 Requires-Dist: qecstruct (>=0.2.9,<0.3.0)
 Requires-Dist: scipy (>=1.9.2,<2.0.0)
 Requires-Dist: threadpoolctl (>=3.1.0,<4.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
```

