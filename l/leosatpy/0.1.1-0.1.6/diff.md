# Comparing `tmp/leosatpy-0.1.1.tar.gz` & `tmp/leosatpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leosatpy-0.1.1.tar", last modified: Mon Jun  5 01:48:24 2023, max compression
+gzip compressed data, was "leosatpy-0.1.6.tar", last modified: Wed Jun  7 03:34:56 2023, max compression
```

## Comparing `leosatpy-0.1.1.tar` & `leosatpy-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-05 01:48:24.083762 leosatpy-0.1.1/
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    35149 2022-08-24 02:26:29.000000 leosatpy-0.1.1/LICENSE
--rw-r--r--   0 cadam     (1000) cadam     (1000)    15293 2023-06-05 01:48:24.082762 leosatpy-0.1.1/PKG-INFO
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    14434 2023-06-05 01:41:34.000000 leosatpy-0.1.1/README.rst
-drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-05 01:48:24.080762 leosatpy-0.1.1/leosatpy/
--rw-r--r--   0 cadam     (1000) cadam     (1000)        0 2023-06-02 19:27:22.000000 leosatpy-0.1.1/leosatpy/__init__.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)    99209 2023-06-04 04:25:17.000000 leosatpy-0.1.1/leosatpy/analyseSatObs.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)    64014 2023-06-04 04:25:17.000000 leosatpy-0.1.1/leosatpy/calibrateSatObs.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)     4101 2023-06-02 00:45:41.000000 leosatpy-0.1.1/leosatpy/leosatpy_config.ini
--rw-r--r--   0 cadam     (1000) cadam     (1000)    96052 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/reduceSatObs.py
-drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-05 01:48:24.082762 leosatpy-0.1.1/leosatpy/utils/
--rw-r--r--   0 cadam     (1000) cadam     (1000)        0 2023-06-02 03:30:59.000000 leosatpy-0.1.1/leosatpy/utils/__init__.py
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    20810 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/arguments.py
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    16314 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/base_conf.py
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    22529 2023-06-04 04:13:22.000000 leosatpy-0.1.1/leosatpy/utils/dataset.py
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    11394 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/photometry.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)    33834 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/satellites.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)    78259 2023-06-02 05:07:49.000000 leosatpy-0.1.1/leosatpy/utils/sources.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)    26135 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/tables.py
--rw-rw-r--   0 cadam     (1000) cadam     (1000)    24200 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/telescope_conf.py
--rw-r--r--   0 cadam     (1000) cadam     (1000)    31224 2023-06-04 05:15:44.000000 leosatpy-0.1.1/leosatpy/utils/transformations.py
--rw-rw-r--   0 cadam     (1000) cadam     (1000)       81 2023-06-05 01:42:11.000000 leosatpy-0.1.1/leosatpy/utils/version.py
-drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-05 01:48:24.081762 leosatpy-0.1.1/leosatpy.egg-info/
--rw-r--r--   0 cadam     (1000) cadam     (1000)    15293 2023-06-05 01:48:24.000000 leosatpy-0.1.1/leosatpy.egg-info/PKG-INFO
--rw-r--r--   0 cadam     (1000) cadam     (1000)      724 2023-06-05 01:48:24.000000 leosatpy-0.1.1/leosatpy.egg-info/SOURCES.txt
--rw-r--r--   0 cadam     (1000) cadam     (1000)        1 2023-06-05 01:48:24.000000 leosatpy-0.1.1/leosatpy.egg-info/dependency_links.txt
--rw-r--r--   0 cadam     (1000) cadam     (1000)      152 2023-06-05 01:48:24.000000 leosatpy-0.1.1/leosatpy.egg-info/entry_points.txt
--rw-r--r--   0 cadam     (1000) cadam     (1000)        1 2023-06-02 19:16:57.000000 leosatpy-0.1.1/leosatpy.egg-info/not-zip-safe
--rw-r--r--   0 cadam     (1000) cadam     (1000)      365 2023-06-05 01:48:24.000000 leosatpy-0.1.1/leosatpy.egg-info/requires.txt
--rw-r--r--   0 cadam     (1000) cadam     (1000)        9 2023-06-05 01:48:24.000000 leosatpy-0.1.1/leosatpy.egg-info/top_level.txt
--rw-r--r--   0 cadam     (1000) cadam     (1000)       86 2023-06-02 16:48:25.000000 leosatpy-0.1.1/pyproject.toml
--rw-r--r--   0 cadam     (1000) cadam     (1000)      364 2023-05-29 13:43:59.000000 leosatpy-0.1.1/requirements.txt
--rw-r--r--   0 cadam     (1000) cadam     (1000)       38 2023-06-05 01:48:24.083762 leosatpy-0.1.1/setup.cfg
--rw-r--r--   0 cadam     (1000) cadam     (1000)     2012 2023-06-02 20:38:58.000000 leosatpy-0.1.1/setup.py
+drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-07 03:34:56.090863 leosatpy-0.1.6/
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    35149 2022-08-24 02:26:29.000000 leosatpy-0.1.6/LICENSE
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    15884 2023-06-07 03:34:56.090863 leosatpy-0.1.6/PKG-INFO
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    15025 2023-06-07 03:26:20.000000 leosatpy-0.1.6/README.rst
+drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-07 03:34:56.087863 leosatpy-0.1.6/leosatpy/
+-rw-r--r--   0 cadam     (1000) cadam     (1000)        0 2023-06-02 19:27:22.000000 leosatpy-0.1.6/leosatpy/__init__.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    98559 2023-06-07 02:55:44.000000 leosatpy-0.1.6/leosatpy/analyseSatObs.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    63201 2023-06-06 16:17:49.000000 leosatpy-0.1.6/leosatpy/calibrateSatObs.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)     3782 2023-06-07 02:26:45.000000 leosatpy-0.1.6/leosatpy/leosatpy_config.ini
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    95030 2023-06-07 02:00:42.000000 leosatpy-0.1.6/leosatpy/reduceSatObs.py
+drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-07 03:34:56.090863 leosatpy-0.1.6/leosatpy/utils/
+-rw-r--r--   0 cadam     (1000) cadam     (1000)        0 2023-06-02 03:30:59.000000 leosatpy-0.1.6/leosatpy/utils/__init__.py
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    20810 2023-06-04 05:15:44.000000 leosatpy-0.1.6/leosatpy/utils/arguments.py
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    16336 2023-06-07 02:00:42.000000 leosatpy-0.1.6/leosatpy/utils/base_conf.py
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    22415 2023-06-06 16:17:48.000000 leosatpy-0.1.6/leosatpy/utils/dataset.py
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    11394 2023-06-04 05:15:44.000000 leosatpy-0.1.6/leosatpy/utils/photometry.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    33834 2023-06-04 05:15:44.000000 leosatpy-0.1.6/leosatpy/utils/satellites.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    78441 2023-06-07 02:13:58.000000 leosatpy-0.1.6/leosatpy/utils/sources.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    26135 2023-06-04 05:15:44.000000 leosatpy-0.1.6/leosatpy/utils/tables.py
+-rw-rw-r--   0 cadam     (1000) cadam     (1000)    24200 2023-06-04 05:15:44.000000 leosatpy-0.1.6/leosatpy/utils/telescope_conf.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    30690 2023-06-06 16:17:49.000000 leosatpy-0.1.6/leosatpy/utils/transformations.py
+-rw-r--r--   0 cadam     (1000) cadam     (1000)       81 2023-06-07 03:24:12.000000 leosatpy-0.1.6/leosatpy/utils/version.py
+drwxr-xr-x   0 cadam     (1000) cadam     (1000)        0 2023-06-07 03:34:56.088863 leosatpy-0.1.6/leosatpy.egg-info/
+-rw-r--r--   0 cadam     (1000) cadam     (1000)    15884 2023-06-07 03:34:56.000000 leosatpy-0.1.6/leosatpy.egg-info/PKG-INFO
+-rw-r--r--   0 cadam     (1000) cadam     (1000)      724 2023-06-07 03:34:56.000000 leosatpy-0.1.6/leosatpy.egg-info/SOURCES.txt
+-rw-r--r--   0 cadam     (1000) cadam     (1000)        1 2023-06-07 03:34:56.000000 leosatpy-0.1.6/leosatpy.egg-info/dependency_links.txt
+-rw-r--r--   0 cadam     (1000) cadam     (1000)      152 2023-06-07 03:34:56.000000 leosatpy-0.1.6/leosatpy.egg-info/entry_points.txt
+-rw-r--r--   0 cadam     (1000) cadam     (1000)        1 2023-06-06 18:47:22.000000 leosatpy-0.1.6/leosatpy.egg-info/not-zip-safe
+-rw-r--r--   0 cadam     (1000) cadam     (1000)      365 2023-06-07 03:34:56.000000 leosatpy-0.1.6/leosatpy.egg-info/requires.txt
+-rw-r--r--   0 cadam     (1000) cadam     (1000)        9 2023-06-07 03:34:56.000000 leosatpy-0.1.6/leosatpy.egg-info/top_level.txt
+-rw-r--r--   0 cadam     (1000) cadam     (1000)       86 2023-06-02 16:48:25.000000 leosatpy-0.1.6/pyproject.toml
+-rw-r--r--   0 cadam     (1000) cadam     (1000)      364 2023-05-29 13:43:59.000000 leosatpy-0.1.6/requirements.txt
+-rw-r--r--   0 cadam     (1000) cadam     (1000)       38 2023-06-07 03:34:56.090863 leosatpy-0.1.6/setup.cfg
+-rw-r--r--   0 cadam     (1000) cadam     (1000)     2012 2023-06-02 20:38:58.000000 leosatpy-0.1.6/setup.py
```

### Comparing `leosatpy-0.1.1/LICENSE` & `leosatpy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.1/PKG-INFO` & `leosatpy-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leosatpy
-Version: 0.1.1
+Version: 0.1.6
 Summary: LEOSatpy is a highly-automated end-to-end pipeline for the reduction, calibration, and analysis of Low Earth Orbit Satellite observations from various telescopes.
 Home-page: http://leosatpy.readthedocs.io/
 Download-URL: https://github.com/CLEOsat-group/leosatpy/archive/master.zip
 Author: Christian Adam
 Author-email: christian.adam84@gmail.com
 License: GNU General Public License v3.0
 Classifier: Development Status :: 3 - Alpha
@@ -59,31 +59,43 @@
     :alt: PyPI
     :target: https://pypi.org/project/leosatpy/
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/leosatpy
     :alt: PyPI - Python Version
     :target: https://pypi.org/project/leosatpy/
 
+.. |release| image:: https://img.shields.io/github/v/release/CLEOsat-Group/leosatpy?include_prereleases
+    :alt: GitHub release (latest SemVer including pre-releases)
+    :target: https://github.com/CLEOsat-group/leosatpy
+
 .. |last-commit| image:: https://img.shields.io/github/last-commit/CLEOsat-Group/leosatpy
     :alt: GitHub last commit
     :target: https://github.com/CLEOsat-group/leosatpy
 
 .. |license| image:: https://img.shields.io/github/license/CLEOsat-Group/leosatpy
     :alt: GitHub
     :target: https://github.com/CLEOsat-group/leosatpy/blob/master/LICENSE
 
+.. |rtd| image:: https://readthedocs.org/projects/leosatpy/badge/?version=latest
+    :target: https://leosatpy.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. |zenodo| image:: https://zenodo.org/badge/526672685.svg
+    :target: https://zenodo.org/badge/latestdoi/526672685
+    :alt: Zenodo
+
 ..
     |stars| |watch|
 
 LEOSatpy
 ========
 
 .. badges
 
-|pypi| |python| |last-commit| |license|
+|pypi| |python| |release| |last-commit| |license| |rtd| |zenodo|
 
 **LEOSatpy** (Low Earth Orbit satellite python) is an end-to-end pipeline to process and analyse
 satellite trail observations from various telescopes.
 
 The pipeline is written in Python 3 and provides the following functionalities:
 
 ===========================  ==========================================================================
@@ -91,15 +103,15 @@
 ===========================  ==========================================================================
 ``reduceSatObs``             Full reduction of raw-FITS images including bias, dark, and flat reduction.
 ``calibrateSatObs``          WCS calibration, i.e. plate solving, using `GAIA DR3 <https://ui.adsabs.harvard.edu/abs/2020yCat.1350....0G/abstract>`_ positions via the `Astroquery <https://astroquery.readthedocs.io/en/latest/#>`_ tool.
 ``analyseSatObs``            Satellite trail(s) detection and aperture photometry using
                              comparison stars from the `GSC v2.4.3 <https://ui.adsabs.harvard.edu/#abs/2008AJ....136..735L>`_ catalog.
 ===========================  ==========================================================================
 
-The full documentation for LEOSatpy can be found `here <https://docs.readthedocs.io/en/stable/tutorial/>`_.
+The full documentation for LEOSatpy can be found `here <http://leosatpy.readthedocs.io/>`_.
 
 LEOSatpy is distributed under the GNU General Public License v3. See the
 `LICENSE <https://github.com/CLEOsat-group/leosatpy/blob/master/LICENSE>`_ file for the precise terms and conditions.
 
 Currently supported telescopes:
     * 0.6-metre Chakana telescope at the |ckoir|_ of the Universidad de Antofagasta, Antofagasta, Chile.
     * 0.9-metre |ctio|_ (SMARTS)
@@ -266,15 +278,16 @@
         │   └── science_data (e.g., STARLINK)
         │       ├── auxiliary
         │       ├── calibrated
         │       ├── catalogs
         │       ├── figures
         │       │   └── Sat-ID (e.g., STARLINK-3568)
         │       ├── raw
-        │       └── reduced
+        │       ├── reduced
+        │       └── tle_predictions
         ├── YYYY-MM-DD
         └── YYYY-MM-DD
 
 .. attention::
 
     To prevent unexpected behaviour during the program execution, please also check and make sure that:
 
@@ -360,15 +373,15 @@
 Citing LEOSatpy
 ---------------
 
 When publishing data processed and analysed with LEOSatpy, please cite:
 
 ::
 
-    Adam, C. et al., 2023 (in preparation). "Estimating the impact to astronomy from the Oneweb satellite constellation using multicolour observations".
+    Adam et al. (2023) (in preparation). "Estimating the impact to astronomy from the Oneweb satellite constellation using multicolour observations".
     Software pipeline available at https://github.com/CLEOsat-group/leosatpy.
 
 Acknowledgements
 ----------------
 
 Alongside the packages listed in the ``requirements.txt``, this project uses workflows and code adopted from the following packages:
```

### Comparing `leosatpy-0.1.1/README.rst` & `leosatpy-0.1.6/leosatpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: leosatpy
+Version: 0.1.6
+Summary: LEOSatpy is a highly-automated end-to-end pipeline for the reduction, calibration, and analysis of Low Earth Orbit Satellite observations from various telescopes.
+Home-page: http://leosatpy.readthedocs.io/
+Download-URL: https://github.com/CLEOsat-group/leosatpy/archive/master.zip
+Author: Christian Adam
+Author-email: christian.adam84@gmail.com
+License: GNU General Public License v3.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 .. Define variables
 
 .. _ckoir: https://www.astro.uantof.cl/research/observatorios/ckoirama-observatory/
 
 .. |ckoir| replace:: Ckoirama Observatory
 
 .. _ctio: http://www.astro.yale.edu/smarts/0.9m.html
@@ -40,31 +59,43 @@
     :alt: PyPI
     :target: https://pypi.org/project/leosatpy/
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/leosatpy
     :alt: PyPI - Python Version
     :target: https://pypi.org/project/leosatpy/
 
+.. |release| image:: https://img.shields.io/github/v/release/CLEOsat-Group/leosatpy?include_prereleases
+    :alt: GitHub release (latest SemVer including pre-releases)
+    :target: https://github.com/CLEOsat-group/leosatpy
+
 .. |last-commit| image:: https://img.shields.io/github/last-commit/CLEOsat-Group/leosatpy
     :alt: GitHub last commit
     :target: https://github.com/CLEOsat-group/leosatpy
 
 .. |license| image:: https://img.shields.io/github/license/CLEOsat-Group/leosatpy
     :alt: GitHub
     :target: https://github.com/CLEOsat-group/leosatpy/blob/master/LICENSE
 
+.. |rtd| image:: https://readthedocs.org/projects/leosatpy/badge/?version=latest
+    :target: https://leosatpy.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. |zenodo| image:: https://zenodo.org/badge/526672685.svg
+    :target: https://zenodo.org/badge/latestdoi/526672685
+    :alt: Zenodo
+
 ..
     |stars| |watch|
 
 LEOSatpy
 ========
 
 .. badges
 
-|pypi| |python| |last-commit| |license|
+|pypi| |python| |release| |last-commit| |license| |rtd| |zenodo|
 
 **LEOSatpy** (Low Earth Orbit satellite python) is an end-to-end pipeline to process and analyse
 satellite trail observations from various telescopes.
 
 The pipeline is written in Python 3 and provides the following functionalities:
 
 ===========================  ==========================================================================
@@ -72,15 +103,15 @@
 ===========================  ==========================================================================
 ``reduceSatObs``             Full reduction of raw-FITS images including bias, dark, and flat reduction.
 ``calibrateSatObs``          WCS calibration, i.e. plate solving, using `GAIA DR3 <https://ui.adsabs.harvard.edu/abs/2020yCat.1350....0G/abstract>`_ positions via the `Astroquery <https://astroquery.readthedocs.io/en/latest/#>`_ tool.
 ``analyseSatObs``            Satellite trail(s) detection and aperture photometry using
                              comparison stars from the `GSC v2.4.3 <https://ui.adsabs.harvard.edu/#abs/2008AJ....136..735L>`_ catalog.
 ===========================  ==========================================================================
 
-The full documentation for LEOSatpy can be found `here <https://docs.readthedocs.io/en/stable/tutorial/>`_.
+The full documentation for LEOSatpy can be found `here <http://leosatpy.readthedocs.io/>`_.
 
 LEOSatpy is distributed under the GNU General Public License v3. See the
 `LICENSE <https://github.com/CLEOsat-group/leosatpy/blob/master/LICENSE>`_ file for the precise terms and conditions.
 
 Currently supported telescopes:
     * 0.6-metre Chakana telescope at the |ckoir|_ of the Universidad de Antofagasta, Antofagasta, Chile.
     * 0.9-metre |ctio|_ (SMARTS)
@@ -247,15 +278,16 @@
         │   └── science_data (e.g., STARLINK)
         │       ├── auxiliary
         │       ├── calibrated
         │       ├── catalogs
         │       ├── figures
         │       │   └── Sat-ID (e.g., STARLINK-3568)
         │       ├── raw
-        │       └── reduced
+        │       ├── reduced
+        │       └── tle_predictions
         ├── YYYY-MM-DD
         └── YYYY-MM-DD
 
 .. attention::
 
     To prevent unexpected behaviour during the program execution, please also check and make sure that:
 
@@ -341,15 +373,15 @@
 Citing LEOSatpy
 ---------------
 
 When publishing data processed and analysed with LEOSatpy, please cite:
 
 ::
 
-    Adam, C. et al., 2023 (in preparation). "Estimating the impact to astronomy from the Oneweb satellite constellation using multicolour observations".
+    Adam et al. (2023) (in preparation). "Estimating the impact to astronomy from the Oneweb satellite constellation using multicolour observations".
     Software pipeline available at https://github.com/CLEOsat-group/leosatpy.
 
 Acknowledgements
 ----------------
 
 Alongside the packages listed in the ``requirements.txt``, this project uses workflows and code adopted from the following packages:
```

### Comparing `leosatpy-0.1.1/leosatpy/analyseSatObs.py` & `leosatpy-0.1.6/leosatpy/analyseSatObs.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 import argparse
 import gc
 import os
 import logging
 import sys
 import warnings
 import time
-import configparser
 import collections
 from datetime import (timedelta, datetime, timezone)
 from pathlib import Path
 
 # THIRD PARTY
 import pandas as pd
 import numpy as np
@@ -129,23 +128,19 @@
 _log.setLevel(_base_conf.LOG_LEVEL)
 stream = logging.StreamHandler()
 stream.setFormatter(_base_conf.FORMATTER)
 _log.addHandler(stream)
 _log_level = _log.level
 
 
-# figure size
-figsize = (10, 6)
-
 pass_str = _base_conf.BCOLORS.PASS + "SUCCESSFUL" + _base_conf.BCOLORS.ENDC
 fail_str = _base_conf.BCOLORS.FAIL + "FAILED" + _base_conf.BCOLORS.ENDC
 
 frmt = "%Y-%m-%dT%H:%M:%S.%f"
 
-# todo: rethink the config structure!!!
 # -----------------------------------------------------------------------------
 
 
 # noinspection PyAugmentAssignment
 class AnalyseSatObs(object):
     """Perform photometric, i.e., integrated flux and differential magnitude,
      analysis on satellite trails.
@@ -195,14 +190,15 @@
 
         self._log = log
         self._log_level = log_level
         self._hdu_idx = args.hdu_idx
         self._force_extract = args.force_detection
         self._force_download = args.force_download
         self._plot_images = plot_images
+        self._figsize = (10, 6)
         self._work_dir = None
         self._plt_path = None
         self._aux_path = None
         self._cat_path = None
         self._sat_id = None
         self._silent = silent
         self._verbose = verbose
@@ -235,14 +231,15 @@
         ds = DataSet(input_args=self._input_path,
                      prog_typ='satPhotometry',
                      log=self._log, log_level=self._log_level)
 
         # load configuration
         ds.load_config()
         self._config = ds.config
+        self._figsize = self._config['FIG_SIZE']
 
         self._obsTable = ObsTables(config=self._config)
         self._obsTable.load_obs_table()
         self._obs_info = ObsTables.obs_info
         self._obj_info = ObsTables.obj_info
 
         # Load Region-of-Interest
@@ -332,35 +329,14 @@
         td = timedelta(seconds=dt)
 
         if not self._silent:
             self._log.info(f"Program execution time in hh:mm:ss: {td}")
         self._log.info('====>  Satellite analysis finished <====')
         sys.exit(0)
 
-    def _load_config(self):
-        """ Load base configuration file """
-
-        # configuration file name
-        configfile = f"{self._root_dir}/leosatpy_config.ini"
-        config = configparser.ConfigParser()
-        config.optionxform = lambda option: option
-
-        self._log.info('> Read configuration')
-        config.read(configfile)
-
-        for group in ['Satellite_analysis', 'Detection']:
-            items = dict(config.items(group))
-            self._config.update(items)
-            for key, value in items.items():
-                try:
-                    val = eval(value)
-                except NameError:
-                    val = value
-                self._config[key] = val
-
     def _analyse_sat_trails(self, files: list, sat_name: str):
         """ Run satellite trail detection and photometry.
 
         Detect which image has a trail, determine parameters,
         perform relative photometry with standard stars,
         and calculate angles and corrections from tle data.
 
@@ -1050,15 +1026,15 @@
         mask = np.array(~sigma_clip(corrections, sigma=3.,
                                     cenfunc=np.nanmedian).mask)
         corrections_cleaned = corrections[mask]
 
         aper_correction = np.nanmedian(corrections_cleaned, axis=None)
         aper_correction_err = np.nanstd(corrections_cleaned, axis=None)
 
-        fig = plt.figure(figsize=(10, 6))
+        fig = plt.figure(figsize=self._figsize)
         gs = gridspec.GridSpec(1, 1)
         ax = fig.add_subplot(gs[0, 0])
 
         # the histogram of the data
         ax.hist(corrections_cleaned, bins='auto',
                 density=True, facecolor='b',
                 alpha=0.75,
@@ -1610,15 +1586,15 @@
         elif img_norm == 'log':
             nm = ImageNormalize(vmin=vmin, vmax=vmax, stretch=LogStretch())
         else:
             nm = ImageNormalize(vmin=vmin, vmax=vmax, stretch=SqrtStretch())
         if cmap is None:
             cmap = 'Greys'
 
-        fig = plt.figure(figsize=figsize)
+        fig = plt.figure(figsize=self._figsize)
         gs = gridspec.GridSpec(2, 2)
         ax1 = fig.add_subplot(gs[0, 0])
         ax2 = fig.add_subplot(gs[0, 1])
         ax3 = fig.add_subplot(gs[1, 0])
         ax4 = fig.add_subplot(gs[1, 1])
 
         ax1.imshow(img, origin='lower',
@@ -1695,15 +1671,15 @@
     def _plot_centroid_fit(self, fit_results: dict, fname: str, reg_data: dict):
         """"""
 
         result = fit_results['lin_fit']
         x = fit_results['lin_x']
         y = fit_results['lin_y']
 
-        fig = plt.figure(figsize=figsize)
+        fig = plt.figure(figsize=self._figsize)
 
         gs = gridspec.GridSpec(1, 1)
         ax = fig.add_subplot(gs[0, 0])
         ax.plot(x, y, 'bo')
         ax.plot(x, result.best_fit, 'r-')
 
         # format axis
@@ -1776,15 +1752,15 @@
         """
 
         result = fit_results['quad_fit']
 
         x = fit_results['quad_x']
         y = fit_results['quad_y']
 
-        fig = plt.figure(figsize=figsize)
+        fig = plt.figure(figsize=self._figsize)
         gs = gridspec.GridSpec(1, 1)
         ax = fig.add_subplot(gs[0, 0])
         ax.plot(np.rad2deg(x), y, 'bo')
         ax.plot(np.rad2deg(x), result.best_fit, 'r-')
 
         # format axis
         ax.tick_params(
@@ -1856,15 +1832,15 @@
         elif img_norm == 'log':
             nm = ImageNormalize(vmin=vmin, vmax=vmax, stretch=LogStretch())
         else:
             nm = ImageNormalize(vmin=vmin, vmax=vmax, stretch=SqrtStretch())
         if cmap is None:
             cmap = 'Greys'
 
-        fig = plt.figure(figsize=figsize)
+        fig = plt.figure(figsize=self._figsize)
         gs = gridspec.GridSpec(1, 1)
         ax = fig.add_subplot(gs[0, 0])
 
         ax.imshow(img, origin='lower',
                   extent=[cols[0], cols[-1],
                           rows[0], rows[-1]],
                   cmap=cmap,
@@ -1909,15 +1885,15 @@
 
     def _plot_photometry_snr(self, src_pos: list, fluxes: np.ndarray,
                              apers: list, optimum_aper: float,
                              file_base: str, mode: str = 'sat'):
         """Plot the Signal-to-Noise ratio results from curve-of-growth estimation"""
 
         flux_med = np.nanmedian(fluxes[:, :, 2], axis=1) / np.nanmax(np.nanmedian(fluxes[:, :, 2], axis=1))
-        fig = plt.figure(figsize=figsize)
+        fig = plt.figure(figsize=self._figsize)
 
         gs = gridspec.GridSpec(1, 2)
         ax1 = fig.add_subplot(gs[0, 0])
         ax2 = fig.add_subplot(gs[0, 1])
 
         # plot fluxes
         for r in range(len(src_pos)):
@@ -2003,22 +1979,22 @@
     def _plot_aperture_photometry(self, fluxes: np.ndarray, rapers: list,
                                   opt_aprad: float, file_base: str):
         """"""
         snr_arr = fluxes[:, :, 2]
         snr_med = np.nanmedian(snr_arr, axis=1) / np.nanmax(np.nanmedian(snr_arr, axis=1))
         snr_max = np.array([np.nanmax(snr_arr[:, r]) for r in range(fluxes.shape[1])])
 
-        fig = plt.figure(figsize=(10, 6), constrained_layout=True, layout='compressed')
+        fig = plt.figure(figsize=self._figsize, constrained_layout=True, layout='compressed')
         # plt.set_loglevel('WARNING')
         widths = [50, 1]
         gs = gridspec.GridSpec(2, 2, figure=fig, width_ratios=widths)
 
         # set up the normalization and the colormap
         normalize = mcolors.Normalize(vmin=np.min(snr_max), vmax=np.max(snr_max))
-        colormap = cm.jet
+        colormap = mpl.colormaps['jet']
 
         ax1 = fig.add_subplot(gs[0, 0])
         ax2 = fig.add_subplot(gs[1, 0], sharex=ax1)
 
         for r in range(fluxes.shape[1]):
             color = colormap(normalize(snr_max[r]))
             ax1.plot(rapers, fluxes[:, r, 2] / np.nanmax(fluxes[:, r, 2]),
@@ -2181,15 +2157,15 @@
         elif img_norm == 'log':
             nm = ImageNormalize(vmin=vmin, vmax=vmax, stretch=LogStretch())
         else:
             nm = ImageNormalize(vmin=vmin, vmax=vmax, stretch=SqrtStretch())
         if cmap is None:
             cmap = 'cividis'
 
-        fig = plt.figure(figsize=figsize)
+        fig = plt.figure(figsize=self._figsize)
 
         gs = gridspec.GridSpec(1, 1)
         ax = fig.add_subplot(gs[0, 0])
 
         # plot the image
         ax.imshow(image, origin='lower',
                   cmap=cmap,
```

### Comparing `leosatpy-0.1.1/leosatpy/calibrateSatObs.py` & `leosatpy-0.1.6/leosatpy/calibrateSatObs.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 import sys
 import logging
 import warnings
 import time
 from datetime import (
     timedelta, datetime, timezone)
 import collections
-import configparser
 from pathlib import Path
 import argparse
 
 # THIRD PARTY
 import numpy as np
 import pandas as pd
 
@@ -104,28 +103,26 @@
 __status__ = "Production"
 
 __taskname__ = 'calibrateSatObs'
 
 # -----------------------------------------------------------------------------
 
 """ Parameter used in the script """
-# -----------------------------------------------------------------------------
+
 # Logging and console output
 logging.root.handlers = []
 _log = logging.getLogger()
 _log.setLevel(_base_conf.LOG_LEVEL)
 stream = logging.StreamHandler()
 stream.setFormatter(_base_conf.FORMATTER)
 _log.addHandler(stream)
 _log_level = _log.level
 
 
 # -----------------------------------------------------------------------------
-# changelog
-# version 0.1.0 alpha version
 
 
 class CalibrateObsWCS(object):
     """Class to calibrate the image world coordinate system."""
 
     def __init__(self,
                  input_path: str, args: argparse.Namespace = None,
@@ -289,35 +286,14 @@
         """
 
         now = datetime.now(tz=timezone.utc)
         time_stamp = f"{now:%Y-%m-%d_%H_%M_%S}"
 
         return time_stamp
 
-    def _load_config(self):
-        """ Load base configuration file """
-
-        # configuration file name
-        configfile = f"{self._root_dir}/leosatpy_config.ini"
-        config = configparser.ConfigParser()
-        config.optionxform = lambda option: option
-
-        self._log.info('> Read configuration')
-        config.read(configfile)
-
-        for group in ['Calibration', 'Detection']:
-            items = dict(config.items(group))
-            self._config.update(items)
-            for key, value in items.items():
-                try:
-                    val = eval(value)
-                except NameError:
-                    val = value
-                self._config[key] = val
-
     def _run_single_calibration(self, file_src_path, file_df, catalog="GAIADR3", hdu_idx=0):
         """Run astrometric calibration on a given dataset.
 
         Create the required folder and run full calibration procedure.
 
         """
 
@@ -441,15 +417,15 @@
         ref_positions_before = init_wcsprm.s2p(ref_tbl[["RA", "DEC"]].values, 0)['pixcrd']
 
         # test with lower number of stars
         # src_tbl = src_tbl.head(170)
         max_wcs_iter = self._config['MAX_WCS_FUNC_ITER']
 
         match_radius = self._config['MATCH_RADIUS']
-        match_radius = kernel_fwhm[0] if match_radius == -1 else match_radius
+        match_radius = kernel_fwhm[0] if match_radius == 'fwhm' else match_radius
 
         best_wcsprm, converged = self.get_wcs(src_tbl, ref_tbl,
                                               init_wcsprm,
                                               match_radius,
                                               max_wcs_iter)
 
         # Move scaling to cdelt and out of the pc matrix
@@ -1395,15 +1371,15 @@
         elif norm == 'log':
             nm = ImageNormalize(vmin=vmin, vmax=vmax, stretch=LogStretch())
         else:
             nm = ImageNormalize(vmin=vmin, vmax=vmax, stretch=SqrtStretch())
         if cmap is None:
             cmap = 'Greys_r'
 
-        figsize = (10, 6)
+        figsize = self._config['FIG_SIZE']
         fig = plt.figure(figsize=figsize)
         fig.canvas.manager.set_window_title(f'Input for {file_name}')
 
         gs = gridspec.GridSpec(1, 2)
         ax1 = fig.add_subplot(gs[0, 0])
 
         im1 = ax1.imshow(imgarr, origin='lower', norm=nm, cmap=cmap)
```

### Comparing `leosatpy-0.1.1/leosatpy/leosatpy_config.ini` & `leosatpy-0.1.6/leosatpy/leosatpy_config.ini`

 * *Files 14% similar despite different names*

```diff
@@ -2,52 +2,32 @@
 
 # Result table configuration
 # !!! Change this to desired directory and name !!!
 RESULT_TABLE_PATH = '~'
 RESULT_TABLE_NAME = 'results_leosatpy.csv'
 
 # Region of interest
-# Mostly for SPM data. Does not support duplicate file name entries at the moment
-# !!! Caution: Has to be created before use !!!
+# Table with Mostly for SPM data. Does not support duplicate file name entries at the moment
 ROI_TABLE_NAME = 'leosatpy_regions_of_interest.csv'
 
-# Astrometric reference catalog name
-DEF_ASTROMETRY_CATALOG = 'GAIADR3'
-
-# Photometric reference catalog name
-DEF_PHOTOMETRY_CATALOG = 'GSC243'
-
-# Figure type. Can be 'png', 'pdf', or ''.
-# If '', plots are saved in both types
-FIG_TYPE = 'png'
-
-# Figure resolution
-FIG_DPI = 150
-
-# Scale indicator length in arcmin
-LINE_LENGTH = 5
-
-# Compass arrow length in fractions of the length
-ARROW_LENGTH = 0.15
-
 [Reduction]
 
 # Reduction type selection; set to False if True and no files are found
 BIAS_CORRECT = True
 DARK_CORRECT = True
 FLAT_CORRECT = True
 FLATDARK_CORRECT = False
 OVERSCAN_CORRECT = True
 
 # Additional options (experimental)
 CORRECT_GAIN = False
 CORRECT_COSMIC = False
 EST_UNCERTAINTY = False
 
-# Reduction method control
+# Combine method controls
 COMBINE_METHOD_BIAS = 'median'
 COMBINE_METHOD_DARK = 'average'
 COMBINE_METHOD_FLAT = 'median'
 
 [Detection]
 
 # Background estimation
@@ -55,66 +35,60 @@
 BKG_MED_WIN_SIZE = 5
 
 # Source extraction
 SOURCE_BOX_SIZE = 21
 SOURCE_MIN_NO = 5
 SOURCE_MAX_NO = 1000
 
-# FWHM control
-FWHM_INIT_GUESS = 5
+# FWHM estimation controls
+FWHM_INIT_GUESS = 5.
 FWHM_LIM_MIN = 1.
 FWHM_LIM_MAX = 30.
 
-# Threshold controls
-THRESHOLD_VALUE = 10.
+# Source detection threshold controls
+THRESHOLD_VALUE = 15.
 THRESHOLD_VALUE_LIM = 3.
 THRESHOLD_FUDGE_FACTOR = 5.
 THRESHOLD_FINE_FUDGE_FACTOR = 0.1
 
 # Sigma clipping
 SIGMACLIP_FWHM_SIGMA = 3.
 
 # Source separation controls
 ISOLATE_SOURCES_INIT_SEP = 20.
 ISOLATE_SOURCES_FWHM_SEP = 5.
 
-# Source fit control
+# Source fitting controls
 MAX_FUNC_ITER = 50
 FITTING_METHOD = 'least_square'
 DEFAULT_MOFF_BETA = 4.765
 
 [Calibration]
 
 # Reference catalog magnitude limit (default is GAIAdr3 g-band magnitude).
 # If -1, the full catalog for the FoV is downloaded
-REF_CATALOG_MAG_LIM = 19
+REF_CATALOG_MAG_LIM = 19.
 
 # Maximum number of iterations for the WCS algorithm
 MAX_WCS_FUNC_ITER = 10
 
 # Maximum number of bright sources from reference catalog to consider
 REF_SOURCES_MAX_NO = 2500
 
 # Maximum number of detected sources to use
 # If -1, all detected sources are used
 MAX_NO_OBS_SOURCES = -1
 
 # Bin size/resolution of scale (in pixel) and rotation (in deg) for 2d histogram
-DISTANCE_BIN_SIZE = 1
+DISTANCE_BIN_SIZE = 1.
 ANG_BIN_SIZE = 0.1
 
-# Frequency cut off threshold as fraction of the maximum frequency in the FFT of the source catalog.
-FREQU_THRESHOLD = 1
-
-# Width in pixel for the offset determination
-OFFSET_BINWIDTH = 1
-
 # Radius within which a source is considered matched (in pixel)
-# If -1, the FWHM of the detected sources is used
-MATCH_RADIUS = -1
+# If 'fwhm', the FWHM of the detected sources is used
+MATCH_RADIUS = 'fwhm'
 
 # Minimum number of matched sources for convergence
 MIN_SOURCE_NO_CONVERGENCE = 5
 
 # Convergence threshold as fraction of detected sources matched
 THRESHOLD_CONVERGENCE = 0.95
 
@@ -138,28 +112,45 @@
 
 # Hough space sub-window size in rho direction in multiple of FWHM
 RHO_SUB_WIN_RES_FWHM = 6.
 
 # Fitting method used in trail parameter estimation
 TRAIL_PARAMS_FITTING_METHOD = 'least_square'
 
-# Maximum number of standard stars sources to consider
-NUM_STD_MAX = 500
-
 # Minimum number of standard stars sources in a given band
 NUM_STD_MIN = 5
 
+# Maximum number of standard stars sources to consider
+NUM_STD_MAX = 500
+
 # Aperture radii control, values in multiple of fwhm
 APER_RAD = 1.7
 INF_APER_RAD = 2.5
 
 # Optimum aperture estimator control, values in multiple of fwhm
 APER_START = 0.1
-APER_STOP = 5
+APER_STOP = 5.
 APER_STEP_SIZE = 0.1
 
 # Inner and outer radius of circular aperture for sky estimation in aperture photometry, values in multiple of fwhm
-RSKYIN = 2
-RSKYOUT = 3
+RSKYIN = 2.
+RSKYOUT = 3.
 
 # Time step size for angular velocity calculation in seconds
-DT_STEP_SIZE = 0.01
+DT_STEP_SIZE = 0.01
+
+[Plotting]
+
+# Figure size
+FIG_SIZE = (10, 6)
+
+# Figure type. Can be 'png', or 'pdf'.
+FIG_TYPE = 'png'
+
+# Figure resolution
+FIG_DPI = 150
+
+# Scale indicator length in arcmin
+LINE_LENGTH = 5.
+
+# Compass arrow length in fractions of the length
+ARROW_LENGTH = 0.15
```

### Comparing `leosatpy-0.1.1/leosatpy/reduceSatObs.py` & `leosatpy-0.1.6/leosatpy/reduceSatObs.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 # -----------------------------------------------------------------------------
 
 """ Modules """
 from __future__ import annotations
 
 import argparse
 import collections
-import configparser
 import gc
 import logging
 import os
 # STDLIB
 import re
 import sys
 import time
@@ -87,22 +86,14 @@
 stream.setFormatter(_base_conf.FORMATTER)
 _log.addHandler(stream)
 _log_level = _log.level
 
 
 # -----------------------------------------------------------------------------
 
-# changelog
-# version 0.3.0 first method's
-# version 0.3.1 added an error message for missing calibration files
-# version 0.3.2 fixed a bug that caused the result file to be overwritten
-# version 0.4.0 added check for filter in flat file creation to avoid copying too much data
-# version 0.5.0 added check to take calibration files from the same date if possible
-# version 0.5.1 rename class
-
 
 class ReduceSatObs(object):
     """ Class to reduce satellite observations from different telescopes."""
 
     def __init__(self,
                  input_path: str,
                  args: argparse.Namespace = None,
@@ -215,35 +206,14 @@
         dt = endtime - starttime
         td = timedelta(seconds=dt)
 
         if not silent:
             self._log.info(f"Program execution time: {td}")
         self._log.info('====> Science image reduction finished <====')
 
-    def _load_config(self):
-        """ Load base configuration file """
-
-        # configuration file name
-        configfile = f"{self._root_dir}/leosatpy_config.ini"
-        config = configparser.ConfigParser()
-        config.optionxform = lambda option: option
-
-        self._log.info('> Read configuration')
-        config.read(configfile)
-
-        for group in ['Reduction']:
-            items = dict(config.items(group))
-            self._config.update(items)
-            for key, value in items.items():
-                try:
-                    val = eval(value)
-                except NameError:
-                    val = value
-                self._config[key] = val
-
     def _run_single_reduction(self, sci_src_path: str, fits_files_dict: dict):
         """Run reduction on a given dataset.
 
         Create the required folder, copy science and calibration files and
         run the full-reduction procedure.
 
         """
@@ -611,27 +581,30 @@
             ccd = CCDData.read(fname, unit=u.Unit("adu"))
             ccd_expt = ccd.header['exptime']
 
             # trim image and update header
             trimmed = True if trim_section is not None else False
             oscan_corrected = True if oscan_section is not None else False
             ccd = self._trim_image(img_ccd=ccd, obsparams=obsparams,
-                                   namps=namps, oscansec=oscan_section, trimsec=trim_section,
+                                   namps=namps, oscansec=oscan_section,
+                                   trimsec=trim_section,
                                    trimmed=trimmed, oscan_corrected=oscan_corrected)
+
             # create an uncertainty map
             if error:
                 ccd = ccdproc.create_deviation(ccd, gain=gain,
-                                               readnoise=readnoise)
+                                               readnoise=readnoise,
+                                               disregard_nan=True)
             # gain correct
             if gain is not None and self._config['CORRECT_GAIN']:
                 ccd = ccdproc.gain_correct(ccd, gain)
 
             # cosmic ray correction
             if cosmic and gain is not None and self._config['CORRECT_GAIN']:
-                ccd = self._clean_cosmic_ray(ccd, image_filter,
+                ccd = self._clean_cosmic_ray(ccd, ccd_mask_fname,
                                              mbox=mbox, rbox=rbox, gbox=gbox, sigclip=sigclip,
                                              cleantype=cleantype, cosmic_method=cosmic_method)
 
             # mask bad pixel
             if 'ccd_mask' in obsparams and obsparams['ccd_mask'][self._bin_str] is not None:
                 ccd_mask_list = obsparams['ccd_mask'][self._bin_str]
                 for yx in ccd_mask_list:
@@ -723,51 +696,53 @@
 
             self._obsTable.update_obs_table(fbase, hdr_dict, obsparams)
 
             del ccd
         del files_list
         gc.collect()
 
-    def _clean_cosmic_ray(self, ccd, image_filter,
+    def _clean_cosmic_ray(self, ccd, ccd_mask_fname,
                           mbox=15, rbox=15, gbox=11, sigclip=5,
                           cleantype="medmask",
                           cosmic_method='lacosmic'):
         """ Clean cosmic rays.
 
         Parameters
         ----------
         ccd: 
-        image_filter: 
+        ccd_mask_fname:
         mbox: 
         rbox: 
         gbox: 
         sigclip: 
         cleantype: 
         cosmic_method: 
 
         Returns
         -------
         ccd: astropy.nddata.CCDData
             An object of the same type as the ccd is returned.
         """
+
         ctype = cosmic_method.lower().strip()
         ctypes = ['lacosmic', 'median']
         if ctype not in ctypes:
             self._log.warning('> Cosmic ray type "%s" NOT available [%s]' % (ctype, ' | '.join(ctypes)))
             return
 
-        ccd_mask_fname = os.path.join(self._master_calib_path, 'mask_from_ccdmask_%s_%s.fits' % (image_filter,
-                                                                                                 self._bin_str))
         ccd_mask_fname = ccd_mask_fname if os.path.exists(ccd_mask_fname) else None
+
         if ccd_mask_fname is not None and isinstance(ccd_mask_fname, str):
             ccd_mask = self._convert_fits_to_ccd(ccd_mask_fname, single=True)
             ccd.mask = ccd_mask.data
 
         if ctype == 'lacosmic':
-            ccd = ccdproc.cosmicray_lacosmic(ccd, sigclip=sigclip, cleantype=cleantype)
+            ccd = ccdproc.cosmicray_lacosmic(ccd,
+                                             sigclip=sigclip,
+                                             cleantype=cleantype, gain_apply=False)
         elif ctype == 'median':
             ccd = ccdproc.cosmicray_median(ccd, mbox=mbox, rbox=rbox, gbox=gbox)
         if isinstance(ccd, CCDData):
             ccd.header['COSMIC'] = ctype.upper()
         return ccd
 
     def _create_master_flat(self, files_list, obsparams, flat_filter=None, mflat_fname=None,
@@ -1613,20 +1588,27 @@
         same_date = []
         diff_date = []
         for file_path in files:
             # load fits file
             hdul = fits.open(file_path, mode='readonly', ignore_missing_end=True)
             hdul.verify('fix')
             prim_hdr = hdul[0].header
+
             self._log.debug("  Check Obs-Date")
             if 'time-obs'.upper() in prim_hdr:
-                t = pd.to_datetime(f"{prim_hdr['date-obs'.upper()]}T{prim_hdr['time-obs'.upper()]}",
-                                   format=frmt, utc=False)
+                time_string = f"{prim_hdr['date-obs'.upper()]}T{prim_hdr['time-obs'.upper()]}"
+
             else:
-                t = pd.to_datetime(prim_hdr['date-obs'.upper()], format=frmt, utc=False)
+                time_string = prim_hdr['date-obs'.upper()]
+
+            frmt = _base_conf.has_fractional_seconds(time_string)
+
+            t = pd.to_datetime(time_string,
+                               format=frmt, utc=False)
+
             t_short = t.strftime('%Y-%m-%d')
             if t_short == obs_date.strftime('%Y-%m-%d'):
                 same_date.append(file_path)
             else:
                 diff_date.append(file_path)
 
         if not same_date:
```

### Comparing `leosatpy-0.1.1/leosatpy/utils/arguments.py` & `leosatpy-0.1.6/leosatpy/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.1/leosatpy/utils/base_conf.py` & `leosatpy-0.1.6/leosatpy/utils/base_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #
 # -----------------------------------------------------------------------------
 
 """ Modules """
 import os
 import logging
 import warnings
+from dateutil.parser import parse
 import numpy as np
 from colorlog import ColoredFormatter
 from astropy import wcs
 from astropy.io import fits
 from astropy.utils.exceptions import (AstropyUserWarning, AstropyWarning)
 
 # from .telescope_conf import *
@@ -82,23 +83,30 @@
                    'TELESCOP', 'FLI', 'FPA', 'CAM_NAME']
 
 # default timeout for selection
 DEF_TIMEOUT = 3  # in seconds
 
 # time delta in days for folder search in reduction of calibration files
 TIMEDELTA_DAYS = 7  # +-days
-FRMT = "%Y-%m-%dT%H:%M:%S.%f"
+FRMT_FS = "%Y-%m-%dT%H:%M:%S.%f"
+FRMT = "%Y-%m-%dT%H:%M:%S"
 
-ROUND_DECIMAL = 5
 
-# # keywords relevant for reduction
-# CORRECT_GAIN = False
-# EST_UNCERTAINTY = False
-# COMBINE_METHOD = 'average'  # Bias, dark and flat combine method; can be median as well
-# COMBINE_METHOD_FLAT = 'median'  # Bias, dark and flat combine method; can be median as well
+def has_fractional_seconds(time_string):
+    # Parse the time string into a datetime object
+    dt = parse(time_string)
+
+    # Check if the datetime object has fractional seconds
+    if dt.microsecond > 0:
+        return FRMT_FS
+    else:
+        return FRMT
+
+
+ROUND_DECIMAL = 5
 
 IMAGETYP_LIGHT = 'science'
 IMAGETYP_BIAS = 'bias'
 IMAGETYP_DARK = 'dark'
 IMAGETYP_FLAT = 'flat'
 
 BINNING_DKEYS = ('BINX', 'BINY')
@@ -192,15 +200,14 @@
 }
 
 # list of available catalogs for photometry
 ALLCATALOGS = ['GAIADR1', 'GAIADR2', 'GAIADR3', 'GAIAEDR3',
                '2MASS', 'PS1DR1', 'PS1DR2',
                'GSC241', 'GSC242', 'GSC243']
 
-DEF_PHOTOMETRY_CATALOG = 'GSC242'
 
 DEF_ASTROQUERY_CATALOGS = {
     'GAIADR3': 'gaiadr3.gaia_source',
     'GSC242': 'I/353/gsc242'
 }
 
 # Dictionary of supported astrometric catalogs with column name translations.
```

### Comparing `leosatpy-0.1.1/leosatpy/utils/dataset.py` & `leosatpy-0.1.6/leosatpy/utils/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,14 @@
 __credits__ = ["Eduardo Unda-Sanzana, Jeremy Tregloan-Reed, Christian Adam"]
 __license__ = "GPL-3.0 license"
 __maintainer__ = "Christian Adam"
 __email__ = "christian.adam84@gmail.com"
 __status__ = "Production"
 
 # -----------------------------------------------------------------------------
-# changelog
-# version 0.1.0 added first method's
-# version 0.1.1 cleanup and documentation update
-# version 0.1.2 spelling check and some minor fixes
 
 # Logging
 _log = logging.getLogger(__name__)
 
 
 class DataSet(object):
     """Initialize and validate given input."""
@@ -148,24 +144,24 @@
             # handle the error as appropriate for your application
             sys.exit(1)
 
         # read config file
         config.read(configfile)
 
         conf_groups = ['Reduction', 'Calibration',
-                       'Detection', 'Satellite_analysis']
+                       'Detection', 'Satellite_analysis', 'Plotting']
 
         if self._mode == 'reduceSatObs':
             conf_groups = ['Reduction']
         if self._mode == 'calibWCS':
             conf_groups = ['Calibration',
-                           'Detection']
+                           'Detection', 'Plotting']
         if self._mode == 'satPhotometry':
             conf_groups = ['Detection',
-                           'Satellite_analysis']
+                           'Satellite_analysis', 'Plotting']
 
         for group in conf_groups:
             items = dict(config.items(group))
             self._config.update(items)
             for key, value in items.items():
                 try:
                     val = eval(value)
```

### Comparing `leosatpy-0.1.1/leosatpy/utils/photometry.py` & `leosatpy-0.1.6/leosatpy/utils/photometry.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.1/leosatpy/utils/satellites.py` & `leosatpy-0.1.6/leosatpy/utils/satellites.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.1/leosatpy/utils/sources.py` & `leosatpy-0.1.6/leosatpy/utils/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         else:
 
             if failsafe > max_iter:
                 break
             else:
                 failsafe += 1
 
-            # check if threshold value is still good
+            # check if the threshold value is still good
             threshold_value_check = threshold_value + n - m
 
             # if <=0 reverse previous drop and fine_fudge factor
             if threshold_value_check < lim_threshold_value and not decrease_increment:
                 log.warning(
                     '    Threshold value has gone below background limit [%d sigma] - '
                     'increasing by smaller increment ' % lim_threshold_value)
@@ -267,15 +267,15 @@
 
             elif threshold_value_check < lim_threshold_value and decrease_increment:
                 log.critical('    FWHM detection failed - cannot find suitable threshold value ')
                 return None, None, False
             else:
                 threshold_value = round(threshold_value + n - m, 3)
 
-            # if threshold goes negative use smaller fudge factor
+            # if the threshold goes negative, use a smaller fudge factor
             if decrease_increment:
                 fudge_factor = fine_fudge_factor
 
             daofind = DAOStarFinder(fwhm=init_fwhm,
                                     threshold=threshold_value * img_std,
                                     exclude_border=True,
                                     peakmax=sat_lim,
@@ -1359,32 +1359,38 @@
                     "Defaulting to GSC242")
         catalog = "GSC243"
 
     if config["_photo_ref_cat_fname"] is not None:
         photo_ref_cat_fname = config["_photo_ref_cat_fname"]
 
     # get the observation date
-    t = pd.to_datetime(hdr['date-obs'], format=_base_conf.FRMT, utc=False)
-    if 'time-obs' in hdr:
-        t = pd.to_datetime(f"{hdr['date-obs']}T{hdr['time-obs']}",
-                           format=_base_conf.FRMT, utc=False)
+    if 'time-obs'.upper() in hdr:
+        time_string = f"{hdr['date-obs'.upper()]}T{hdr['time-obs'.upper()]}"
+    else:
+        time_string = hdr['date-obs'.upper()]
+
+    frmt = _base_conf.has_fractional_seconds(time_string)
+
+    t = pd.to_datetime(time_string,
+                       format=frmt, utc=False)
+
     epoch = Time(t)
 
     # set RA and DEC
     wcs = WCS(wcsprm.to_header())
     ra, dec = wcs.wcs_pix2world(hdr['NAXIS1'] // 2,
                                 hdr['NAXIS2'] // 2, 0)
 
     # estimate the radius of the FoV for ref. catalog creation
     fov_radius = compute_radius(wcs,
                                 naxis1=hdr['NAXIS1'],
                                 naxis2=hdr['NAXIS2'],
                                 ra=ra, dec=dec)
 
-    # check for source catalog file. If present and not force extraction use these catalogs
+    # check for source catalog file. If present and not force extraction, use these catalogs
     chk_ref_cat_photo = os.path.isfile(photo_ref_cat_fname + '.cat')
 
     read_ref_cat_photo = True
     if config["_force_download"] or not chk_ref_cat_photo:
         read_ref_cat_photo = False
 
     # get photometric reference catalog
@@ -1484,18 +1490,24 @@
         src_cat_fname = config["_src_cat_fname"]
     if config["_ref_cat_fname"] is not None:
         astro_ref_cat_fname = config["_ref_cat_fname"]
     if config["_photo_ref_cat_fname"] is not None:
         photo_ref_cat_fname = config["_photo_ref_cat_fname"]
 
     # get the observation date
-    t = pd.to_datetime(hdr['date-obs'], format=_base_conf.FRMT, utc=False)
-    if 'time-obs' in hdr:
-        t = pd.to_datetime(f"{hdr['date-obs']}T{hdr['time-obs']}",
-                           format=_base_conf.FRMT, utc=False)
+    if 'time-obs'.upper() in hdr:
+        time_string = f"{hdr['date-obs'.upper()]}T{hdr['time-obs'.upper()]}"
+    else:
+        time_string = hdr['date-obs'.upper()]
+
+    frmt = _base_conf.has_fractional_seconds(time_string)
+
+    t = pd.to_datetime(time_string,
+                       format=frmt, utc=False)
+
     epoch = Time(t)
 
     # set RA and DEC
     ra, dec = wcsprm.crval
     wcs = WCS(wcsprm.to_header())
 
     fov_radius = config["_fov_radius"]
@@ -1685,15 +1697,15 @@
                         bkgrms_estimator=bkgrms_estimator(),
                         edge_method=edge_method,
                         interpolator=interp, filter_size=filter_size)
 
 
 def rename_colname(table: Table, colname: str, newcol: str):
     """Convert column name in table to user-specified name"""
-    # If table is missing a column, add a column with values of None
+    # If the table is missing a column, add a column with values of None
     if colname != '':
         table.rename_column(colname, newcol)
     else:
         empty_column = Column(data=[None] * len(table), name=newcol, dtype=np.float64)
         table.add_column(empty_column)
 
 
@@ -1887,15 +1899,15 @@
         has_data = np.any(np.array([x1, x2, x3]), axis=1).all()
         if not has_data:
             log.critical("Insufficient data for magnitude conversion.")
             del ref_cat, cat_srt, df, alt_cat
             gc.collect()
             return None, filter_keys, has_mag_conv, False
 
-        # convert band from catalog to observation
+        # convert the band from catalog to observation
         alt_mags, alt_mags_err = phot.convert_ssds_to_bvri(f=filter_keys[0],
                                                            x1=x1, x2=x2, x3=x3)
 
         new_df = pd.DataFrame({filter_keys[0]: alt_mags,
                                filter_keys[1]: alt_mags_err}, index=alt_cat.index)
 
         cat_srt.update(new_df)
```

### Comparing `leosatpy-0.1.1/leosatpy/utils/tables.py` & `leosatpy-0.1.6/leosatpy/utils/tables.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.1/leosatpy/utils/telescope_conf.py` & `leosatpy-0.1.6/leosatpy/utils/telescope_conf.py`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.1/leosatpy/utils/transformations.py` & `leosatpy-0.1.6/leosatpy/utils/transformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 import inspect
 import logging
 
 import numpy as np
 from astropy.wcs import WCS, utils
 from fast_histogram import histogram2d
 
-# pipeline-specific modules
-from . import base_conf as _base_conf
 
 # -----------------------------------------------------------------------------
 
 """ Meta-info """
 __author__ = "Christian Adam"
 __copyright__ = 'Copyright 2021-2023, CLEOSat group'
 __credits__ = ["Eduardo Unda-Sanzana, Jeremy Tregloan-Reed, Christian Adam"]
@@ -53,16 +51,14 @@
 
 log = logging.getLogger(__name__)
 
 MODULE_PATH = os.path.dirname(inspect.getfile(inspect.currentframe()))
 
 
 # -----------------------------------------------------------------------------
-# changelog
-# version 0.1.0 alpha version
 
 
 def get_scale_and_rotation(observation, catalog, wcsprm, scale_guessed,
                            dist_bin_size, ang_bin_size):
     """Calculate the scale and rotation compared to the catalog based on the method of Kaiser et al. (1999).
 
     This should be quite similar to the approach by SCAMP.
@@ -161,50 +157,40 @@
         scaling_reflected, rotation_reflected, signal_reflected, \
         corr_, corr_reflected
     gc.collect()
 
     return wcsprm_new, (scaling, rotation, signal, confidence)
 
 
-def get_offset_with_orientation(observation, catalog, wcsprm, fast=False,
+def get_offset_with_orientation(observation, catalog, wcsprm,
                                 report_global=""):
     """Use offset from cross-correlation but with trying 0,90,180,270 rotation.
 
     Parameters
     ----------
     observation: ~pandas.Dataframe
         pandas dataframe with sources on the observation
     catalog: pd.Dataframe
         pandas dataframe with nearby sources from online catalogs with accurate astrometric information
     wcsprm: astropy.wcs.wcsprm
         World coordinate system object describing translation between image and skycoord
-    fast: bool, optional
-        If true, will run with a subset of the sources to increase speed.
     report_global: str, optional
 
     Returns
     -------
     wcs, signal, report
     """
 
     # Initialize logging for this user-callable function
     log.setLevel(logging.getLevelName(log.getEffectiveLevel()))
 
     observation = copy(observation)
     N_SOURCES = observation.shape[0]
-    if fast:
-        if N_SOURCES > _base_conf.USE_N_SOURCES:
-            N_SOURCES = _base_conf.USE_N_SOURCES
-        observation = observation.nlargest(N_SOURCES, 'flux')
-        N_CATALOG = N_SOURCES * 4
-        catalog = catalog.nsmallest(N_CATALOG, 'mag')
 
     log.debug("> offset_with_orientation, searching for offset while considering 0,90,180,270 rotations")
-    if fast:
-        log.debug("> running in fast mode")
 
     # Already checking for reflections with the scaling and general rotations,
     # but in case rot_scale is of it is nice to have
     rotations = np.array([[[1, 0], [0, 1]], [[-1, 0], [0, -1]],
                           [[-1, 0], [0, 1]], [[1, 0], [0, -1]],
                           [[0, 1], [1, 0]], [[0, -1], [-1, 0]],
                           [[0, -1], [1, 0]], [[0, 1], [-1, 0]]])
@@ -783,15 +769,15 @@
 def shift_translation(src_image, target_image):
     """
     Translation registration by cross-correlation (like FFT up-sampled cross-correlation)
     Parameters
     ----------
      src_image: ndarray of the reference image.
      target_image: ndarray of the image to register.
-     Must be the same dimensionality as src_image.
+        Must be the same dimensionality as src_image.
 
     Returns
     -------
       - shift : ndarray of the shift pixels vector required to register the target_image the with src_image.
     """
     # The two images need to have the same size
     if src_image.shape != target_image.shape:
```

### Comparing `leosatpy-0.1.1/leosatpy.egg-info/PKG-INFO` & `leosatpy-0.1.6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: leosatpy
-Version: 0.1.1
-Summary: LEOSatpy is a highly-automated end-to-end pipeline for the reduction, calibration, and analysis of Low Earth Orbit Satellite observations from various telescopes.
-Home-page: http://leosatpy.readthedocs.io/
-Download-URL: https://github.com/CLEOsat-group/leosatpy/archive/master.zip
-Author: Christian Adam
-Author-email: christian.adam84@gmail.com
-License: GNU General Public License v3.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 .. Define variables
 
 .. _ckoir: https://www.astro.uantof.cl/research/observatorios/ckoirama-observatory/
 
 .. |ckoir| replace:: Ckoirama Observatory
 
 .. _ctio: http://www.astro.yale.edu/smarts/0.9m.html
@@ -59,31 +40,43 @@
     :alt: PyPI
     :target: https://pypi.org/project/leosatpy/
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/leosatpy
     :alt: PyPI - Python Version
     :target: https://pypi.org/project/leosatpy/
 
+.. |release| image:: https://img.shields.io/github/v/release/CLEOsat-Group/leosatpy?include_prereleases
+    :alt: GitHub release (latest SemVer including pre-releases)
+    :target: https://github.com/CLEOsat-group/leosatpy
+
 .. |last-commit| image:: https://img.shields.io/github/last-commit/CLEOsat-Group/leosatpy
     :alt: GitHub last commit
     :target: https://github.com/CLEOsat-group/leosatpy
 
 .. |license| image:: https://img.shields.io/github/license/CLEOsat-Group/leosatpy
     :alt: GitHub
     :target: https://github.com/CLEOsat-group/leosatpy/blob/master/LICENSE
 
+.. |rtd| image:: https://readthedocs.org/projects/leosatpy/badge/?version=latest
+    :target: https://leosatpy.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. |zenodo| image:: https://zenodo.org/badge/526672685.svg
+    :target: https://zenodo.org/badge/latestdoi/526672685
+    :alt: Zenodo
+
 ..
     |stars| |watch|
 
 LEOSatpy
 ========
 
 .. badges
 
-|pypi| |python| |last-commit| |license|
+|pypi| |python| |release| |last-commit| |license| |rtd| |zenodo|
 
 **LEOSatpy** (Low Earth Orbit satellite python) is an end-to-end pipeline to process and analyse
 satellite trail observations from various telescopes.
 
 The pipeline is written in Python 3 and provides the following functionalities:
 
 ===========================  ==========================================================================
@@ -91,15 +84,15 @@
 ===========================  ==========================================================================
 ``reduceSatObs``             Full reduction of raw-FITS images including bias, dark, and flat reduction.
 ``calibrateSatObs``          WCS calibration, i.e. plate solving, using `GAIA DR3 <https://ui.adsabs.harvard.edu/abs/2020yCat.1350....0G/abstract>`_ positions via the `Astroquery <https://astroquery.readthedocs.io/en/latest/#>`_ tool.
 ``analyseSatObs``            Satellite trail(s) detection and aperture photometry using
                              comparison stars from the `GSC v2.4.3 <https://ui.adsabs.harvard.edu/#abs/2008AJ....136..735L>`_ catalog.
 ===========================  ==========================================================================
 
-The full documentation for LEOSatpy can be found `here <https://docs.readthedocs.io/en/stable/tutorial/>`_.
+The full documentation for LEOSatpy can be found `here <http://leosatpy.readthedocs.io/>`_.
 
 LEOSatpy is distributed under the GNU General Public License v3. See the
 `LICENSE <https://github.com/CLEOsat-group/leosatpy/blob/master/LICENSE>`_ file for the precise terms and conditions.
 
 Currently supported telescopes:
     * 0.6-metre Chakana telescope at the |ckoir|_ of the Universidad de Antofagasta, Antofagasta, Chile.
     * 0.9-metre |ctio|_ (SMARTS)
@@ -266,15 +259,16 @@
         │   └── science_data (e.g., STARLINK)
         │       ├── auxiliary
         │       ├── calibrated
         │       ├── catalogs
         │       ├── figures
         │       │   └── Sat-ID (e.g., STARLINK-3568)
         │       ├── raw
-        │       └── reduced
+        │       ├── reduced
+        │       └── tle_predictions
         ├── YYYY-MM-DD
         └── YYYY-MM-DD
 
 .. attention::
 
     To prevent unexpected behaviour during the program execution, please also check and make sure that:
 
@@ -360,15 +354,15 @@
 Citing LEOSatpy
 ---------------
 
 When publishing data processed and analysed with LEOSatpy, please cite:
 
 ::
 
-    Adam, C. et al., 2023 (in preparation). "Estimating the impact to astronomy from the Oneweb satellite constellation using multicolour observations".
+    Adam et al. (2023) (in preparation). "Estimating the impact to astronomy from the Oneweb satellite constellation using multicolour observations".
     Software pipeline available at https://github.com/CLEOsat-group/leosatpy.
 
 Acknowledgements
 ----------------
 
 Alongside the packages listed in the ``requirements.txt``, this project uses workflows and code adopted from the following packages:
```

### Comparing `leosatpy-0.1.1/leosatpy.egg-info/SOURCES.txt` & `leosatpy-0.1.6/leosatpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leosatpy-0.1.1/setup.py` & `leosatpy-0.1.6/setup.py`

 * *Files identical despite different names*

