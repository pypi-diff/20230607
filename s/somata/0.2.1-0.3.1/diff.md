# Comparing `tmp/somata-0.2.1.tar.gz` & `tmp/somata-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somata-0.2.1.tar", last modified: Tue Nov 22 00:02:13 2022, max compression
+gzip compressed data, was "somata-0.3.1.tar", last modified: Wed Jun  7 03:54:08 2023, max compression
```

## Comparing `somata-0.2.1.tar` & `somata-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,49 @@
-drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2022-11-22 00:02:13.622081 somata-0.2.1/
--rw-r--r--   0 alexhe     (501) staff       (20)     1622 2022-11-12 21:40:21.000000 somata-0.2.1/LICENSE
--rw-r--r--   0 alexhe     (501) staff       (20)    23161 2022-11-22 00:02:13.622163 somata-0.2.1/PKG-INFO
--rw-r--r--   0 alexhe     (501) staff       (20)    22313 2022-11-22 00:01:39.000000 somata-0.2.1/README.md
--rw-r--r--   0 alexhe     (501) staff       (20)       89 2022-11-12 21:40:21.000000 somata-0.2.1/pyproject.toml
--rw-r--r--   0 alexhe     (501) staff       (20)      976 2022-11-22 00:02:13.622481 somata-0.2.1/setup.cfg
--rw-r--r--   0 alexhe     (501) staff       (20)       69 2022-11-12 21:40:21.000000 somata-0.2.1/setup.py
-drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2022-11-22 00:02:13.617818 somata-0.2.1/somata/
--rw-r--r--   0 alexhe     (501) staff       (20)       89 2022-11-12 21:40:21.000000 somata-0.2.1/somata/__init__.py
-drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2022-11-22 00:02:13.620042 somata-0.2.1/somata/basic_models/
--rw-r--r--   0 alexhe     (501) staff       (20)      424 2022-11-12 21:40:21.000000 somata-0.2.1/somata/basic_models/__init__.py
--rw-r--r--   0 alexhe     (501) staff       (20)    18600 2022-11-21 23:14:06.000000 somata-0.2.1/somata/basic_models/arn.py
--rw-r--r--   0 alexhe     (501) staff       (20)     3873 2022-11-21 23:14:06.000000 somata-0.2.1/somata/basic_models/gen.py
--rw-r--r--   0 alexhe     (501) staff       (20)    35291 2022-11-21 23:14:06.000000 somata-0.2.1/somata/basic_models/osc.py
--rw-r--r--   0 alexhe     (501) staff       (20)    52644 2022-11-21 23:14:06.000000 somata-0.2.1/somata/basic_models/ssm.py
-drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2022-11-22 00:02:13.620689 somata-0.2.1/somata/exact_inference/
--rw-r--r--   0 alexhe     (501) staff       (20)      253 2022-11-21 23:14:06.000000 somata-0.2.1/somata/exact_inference/__init__.py
--rw-r--r--   0 alexhe     (501) staff       (20)    18513 2022-11-21 23:14:06.000000 somata-0.2.1/somata/exact_inference/dp_func.py
--rw-r--r--   0 alexhe     (501) staff       (20)     3132 2022-11-12 21:40:21.000000 somata-0.2.1/somata/exact_inference/em.py
-drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2022-11-22 00:02:13.621455 somata-0.2.1/somata/iterative_oscillator/
--rw-r--r--   0 alexhe     (501) staff       (20)      118 2022-11-12 21:40:21.000000 somata-0.2.1/somata/iterative_oscillator/__init__.py
--rw-r--r--   0 alexhe     (501) staff       (20)    16589 2022-11-12 21:40:21.000000 somata-0.2.1/somata/iterative_oscillator/helper_functions.py
--rw-r--r--   0 alexhe     (501) staff       (20)     8686 2022-11-12 21:40:21.000000 somata-0.2.1/somata/iterative_oscillator/iter_osc.py
-drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2022-11-22 00:02:13.621840 somata-0.2.1/somata/multitaper/
--rw-r--r--   0 alexhe     (501) staff       (20)      210 2022-11-12 21:40:21.000000 somata-0.2.1/somata/multitaper/__init__.py
--rw-r--r--   0 alexhe     (501) staff       (20)    24106 2022-11-12 21:40:21.000000 somata-0.2.1/somata/multitaper/multitaper_spectrogram_python.py
-drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2022-11-22 00:02:13.619127 somata-0.2.1/somata.egg-info/
--rw-r--r--   0 alexhe     (501) staff       (20)    23161 2022-11-22 00:02:13.000000 somata-0.2.1/somata.egg-info/PKG-INFO
--rw-r--r--   0 alexhe     (501) staff       (20)      666 2022-11-22 00:02:13.000000 somata-0.2.1/somata.egg-info/SOURCES.txt
--rw-r--r--   0 alexhe     (501) staff       (20)        1 2022-11-22 00:02:13.000000 somata-0.2.1/somata.egg-info/dependency_links.txt
--rw-r--r--   0 alexhe     (501) staff       (20)       90 2022-11-22 00:02:13.000000 somata-0.2.1/somata.egg-info/requires.txt
--rw-r--r--   0 alexhe     (501) staff       (20)        7 2022-11-22 00:02:13.000000 somata-0.2.1/somata.egg-info/top_level.txt
+drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2023-06-07 03:54:08.487106 somata-0.3.1/
+-rw-r--r--   0 alexhe     (501) staff       (20)     1622 2022-11-12 21:40:21.000000 somata-0.3.1/LICENSE
+-rw-r--r--   0 alexhe     (501) staff       (20)    25735 2023-06-07 03:54:08.487204 somata-0.3.1/PKG-INFO
+-rw-r--r--   0 alexhe     (501) staff       (20)    24887 2023-06-07 03:47:05.000000 somata-0.3.1/README.md
+-rw-r--r--   0 alexhe     (501) staff       (20)       89 2022-11-12 21:40:21.000000 somata-0.3.1/pyproject.toml
+-rw-r--r--   0 alexhe     (501) staff       (20)     1022 2023-06-07 03:54:08.487571 somata-0.3.1/setup.cfg
+-rw-r--r--   0 alexhe     (501) staff       (20)       69 2023-06-07 03:37:59.000000 somata-0.3.1/setup.py
+drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2023-06-07 03:54:08.480927 somata-0.3.1/somata/
+-rw-r--r--   0 alexhe     (501) staff       (20)       89 2022-11-12 21:40:21.000000 somata-0.3.1/somata/__init__.py
+drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2023-06-07 03:54:08.482224 somata-0.3.1/somata/_preprocessing/
+-rw-r--r--   0 alexhe     (501) staff       (20)        0 2023-06-07 03:43:32.000000 somata-0.3.1/somata/_preprocessing/__init__.py
+-rw-r--r--   0 alexhe     (501) staff       (20)     8390 2023-06-07 03:43:32.000000 somata-0.3.1/somata/_preprocessing/_colored_noise_utils.py
+drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2023-06-07 03:54:08.483172 somata-0.3.1/somata/basic_models/
+-rw-r--r--   0 alexhe     (501) staff       (20)      424 2022-11-12 21:40:21.000000 somata-0.3.1/somata/basic_models/__init__.py
+-rw-r--r--   0 alexhe     (501) staff       (20)    18499 2023-06-07 03:47:05.000000 somata-0.3.1/somata/basic_models/arn.py
+-rw-r--r--   0 alexhe     (501) staff       (20)     4028 2023-06-07 03:47:05.000000 somata-0.3.1/somata/basic_models/gen.py
+-rw-r--r--   0 alexhe     (501) staff       (20)    35171 2023-06-07 03:47:05.000000 somata-0.3.1/somata/basic_models/osc.py
+-rw-r--r--   0 alexhe     (501) staff       (20)    53699 2023-06-07 03:47:05.000000 somata-0.3.1/somata/basic_models/ssm.py
+drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2023-06-07 03:54:08.483772 somata-0.3.1/somata/exact_inference/
+-rw-r--r--   0 alexhe     (501) staff       (20)      253 2023-06-07 03:47:05.000000 somata-0.3.1/somata/exact_inference/__init__.py
+-rw-r--r--   0 alexhe     (501) staff       (20)    18513 2023-06-07 03:47:05.000000 somata-0.3.1/somata/exact_inference/dp_func.py
+-rw-r--r--   0 alexhe     (501) staff       (20)     3231 2023-06-07 03:46:22.000000 somata-0.3.1/somata/exact_inference/em.py
+drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2023-06-07 03:54:08.484389 somata-0.3.1/somata/iterative_oscillator/
+-rw-r--r--   0 alexhe     (501) staff       (20)      118 2022-11-12 21:40:21.000000 somata-0.3.1/somata/iterative_oscillator/__init__.py
+-rw-r--r--   0 alexhe     (501) staff       (20)    13463 2023-06-07 03:46:12.000000 somata-0.3.1/somata/iterative_oscillator/helper_functions.py
+-rw-r--r--   0 alexhe     (501) staff       (20)    14018 2023-06-07 03:46:16.000000 somata-0.3.1/somata/iterative_oscillator/iter_osc.py
+drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2023-06-07 03:54:08.484854 somata-0.3.1/somata/multitaper/
+-rw-r--r--   0 alexhe     (501) staff       (20)      176 2023-06-07 03:45:41.000000 somata-0.3.1/somata/multitaper/__init__.py
+-rw-r--r--   0 alexhe     (501) staff       (20)      805 2023-06-07 03:45:41.000000 somata-0.3.1/somata/multitaper/fast_psd_multitaper.py
+-rw-r--r--   0 alexhe     (501) staff       (20)    24323 2023-06-07 03:46:12.000000 somata-0.3.1/somata/multitaper/multitaper_spectrogram_python.py
+drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2023-06-07 03:54:08.485336 somata-0.3.1/somata/switching/
+-rw-r--r--   0 alexhe     (501) staff       (20)      176 2023-06-07 03:43:32.000000 somata-0.3.1/somata/switching/__init__.py
+-rw-r--r--   0 alexhe     (501) staff       (20)    33465 2023-06-07 03:46:12.000000 somata-0.3.1/somata/switching/traditional.py
+-rw-r--r--   0 alexhe     (501) staff       (20)    23212 2023-06-07 03:46:22.000000 somata-0.3.1/somata/switching/vb.py
+drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2023-06-07 03:54:08.485702 somata-0.3.1/somata/utils/
+-rw-r--r--   0 alexhe     (501) staff       (20)      140 2023-06-07 03:46:12.000000 somata-0.3.1/somata/utils/__init__.py
+-rw-r--r--   0 alexhe     (501) staff       (20)     2180 2023-06-07 03:46:12.000000 somata-0.3.1/somata/utils/helper_functions.py
+drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2023-06-07 03:54:08.481880 somata-0.3.1/somata.egg-info/
+-rw-r--r--   0 alexhe     (501) staff       (20)    25735 2023-06-07 03:54:08.000000 somata-0.3.1/somata.egg-info/PKG-INFO
+-rw-r--r--   0 alexhe     (501) staff       (20)     1049 2023-06-07 03:54:08.000000 somata-0.3.1/somata.egg-info/SOURCES.txt
+-rw-r--r--   0 alexhe     (501) staff       (20)       40 2023-06-07 03:54:08.000000 somata-0.3.1/somata.egg-info/dependency_links.txt
+-rw-r--r--   0 alexhe     (501) staff       (20)       76 2023-06-07 03:54:08.000000 somata-0.3.1/somata.egg-info/requires.txt
+-rw-r--r--   0 alexhe     (501) staff       (20)        7 2023-06-07 03:54:08.000000 somata-0.3.1/somata.egg-info/top_level.txt
+drwxr-xr-x   0 alexhe     (501) staff       (20)        0 2023-06-07 03:54:08.486970 somata-0.3.1/tests/
+-rw-r--r--   0 alexhe     (501) staff       (20)     2565 2022-11-12 21:40:50.000000 somata-0.3.1/tests/test_basic_models.py
+-rw-r--r--   0 alexhe     (501) staff       (20)     8107 2023-06-07 03:47:05.000000 somata-0.3.1/tests/test_dp_func.py
+-rw-r--r--   0 alexhe     (501) staff       (20)     2350 2023-06-07 03:46:22.000000 somata-0.3.1/tests/test_iter_osc.py
+-rw-r--r--   0 alexhe     (501) staff       (20)     1266 2022-11-12 21:40:50.000000 somata-0.3.1/tests/test_load_data.py
+-rw-r--r--   0 alexhe     (501) staff       (20)     4646 2023-06-07 03:43:32.000000 somata-0.3.1/tests/test_switching.py
```

### Comparing `somata-0.2.1/LICENSE` & `somata-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `somata-0.2.1/PKG-INFO` & `somata-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: somata
-Version: 0.2.1
-Summary: State-space Oscillator Modeling And Time-series Analysis
-Home-page: https://github.com/mh105/somata
-Author: Mingjian He
-Author-email: mh105@mit.edu
-Keywords: state-space oscillator time-series
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Utilities
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # somata
 
 Github: https://github.com/mh105/somata
 
 **State-space Oscillator Modeling And Time-series Analysis (SOMATA)** is a Python library for state-space neural signal
 processing algorithms developed in the [Purdon Lab](https://purdonlab.mgh.harvard.edu).
 Basic state-space models are introduced as class objects for flexible manipulations.
@@ -49,69 +27,78 @@
 * [Authors](#authors)
 * [Citation](#citation)
 * [License](#license)
 
 ---
 
 ## Requirements
-somata is built on `numpy` arrays for computations. `joblib` is used for multithreading. Additional dependencies include
-`matplotlib`, `scipy`, `tqdm`, `codetiming`, and `sorcery`. Full requirements for each release version will be updated
-under `install_requires` in the `setup.cfg` file. If the `environment.yml` file is used to create a new conda
-environment, all and only the required packages will be installed.
+[`somata`](https://pypi.org/project/somata/) is built on [`numpy`](https://numpy.org) arrays for computations. [`joblib`](https://joblib.readthedocs.io/en/stable/) is used for multithreading. 
+Additional dependencies include [`scipy`](https://scipy.org), [`matplotlib`](https://matplotlib.org), and [`spectrum`](https://pyspectrum.readthedocs.io/en/latest/index.html).
+An upcoming source localization module also requires [`pytorch`](https://pytorch.org) and [`MNE-python`](https://mne.tools/stable/index.html).
+Full requirements for each release version will be updated under 
+[`install_requires`](https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#platform-specific-dependencies) in the [`setup.cfg`](setup.cfg) file. 
+If the [`environment.yml`](environment.yml) file is used to [create a new conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file), 
+all and only the required packages will be installed.
 
 ## Install
 
 ```
 pip install somata
 ```
+_If the [`pytorch`](https://pytorch.org) dependency is not resolved successfully by [`pip`](https://pip.pypa.io/en/stable/) for your [OS](https://whatsmyos.com), 
+first [install `pytorch` manually](https://pytorch.org/get-started/locally/) in a [conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) that you wish to install [`somata`](https://pypi.org/project/somata/), 
+and then [execute the above line](https://packaging.python.org/en/latest/tutorials/installing-packages/#ensure-you-can-run-pip-from-the-command-line) to install [`somata`](https://pypi.org/project/somata/)._
 
 ### (For development only)
 
 - ### Fork this repo to personal git
     [How to: GitHub fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo)    
 
 - ### Clone forked copy to local computer
-    ``` git clone <forked copy ssh url> ```
+    [How to: GitHub clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)
 
 - ### Install conda
     [Recommended conda distribution: miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
-    _Apple silicon Mac: choose conda native to the ARM64 architecture instead of Intel x86_
+    _[Apple silicon Mac](https://support.apple.com/en-us/HT211814): choose conda native to the [ARM64 architecture](https://www.anaconda.com/blog/new-release-anaconda-distribution-now-supporting-m1) instead of [Intel x86](https://en.wikipedia.org/wiki/X86)._
 
 - ### Create a new conda environment
     ``` conda install mamba -n base -c conda-forge ```\
     ``` cd <repo root directory with environment.yml> ```\
     ``` mamba env create -f environment.yml ```\
-    ``` conda activate somata ```\
-    _You may also install somata in an existing environment by skipping this step._
+    ``` conda activate somata ```
+
+    _You may also install `somata` in an [existing environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#using-pip-in-an-environment) by skipping this step._
 
-- ### Install somata as a package in editable mode
+- ### Install somata as a package in development mode
     ``` cd <repo root directory with setup.py> ```\
     ``` pip install -e . ```
 
+    _[What is: Editable Installs](https://setuptools.pypa.io/en/latest/userguide/development_mode.html)_
+
 - ### Configure IDEs to use the conda environment
-    [How to: Configure an existing conda environment](https://www.jetbrains.com/help/pycharm/conda-support-creating-conda-virtual-environment.html)
+    [How to: Configure an existing conda environment](https://www.jetbrains.com/help/pycharm/conda-support-creating-conda-virtual-environment.html#existing-conda-environment)
 
 ---
 
 ## Basic state-space models
-Somata, much like a neuron body supported by dendrites, is built on a set of basic state-space models introduced as class objects.
+`somata`, much like a neuron body supported by dendrites, is built on a set of basic state-space models introduced as class objects.
 
 The motivations are to:
 - develop a standardized format to store model parameters of state-space equations
 - override Python dunder methods so `__repr__` and `__str__` return something useful
 - define arithmetic-like operations such as `A + B` and `A * B`
 - emulate `numpy.array()` operations including `.append()`
 - implement inference algorithms like Kalman filtering and parameter update (m-step) equations as callable class methods
 
-At present, and in the near future, somata will be focused on **time-invariant Gaussian linear dynamical systems**.
-This limit on models we consider simplifies basic models to avoid embedded classes such as `transition_model` and
-`observation_model`, at the cost of restricting somata to classical algorithms with only some extensions to
+At present, and in the near future, `somata` will be focused on **time-invariant Gaussian linear dynamical systems**.
+This limit on models we consider simplifies basic models to avoid nested classes such as `transition_model` and
+`observation_model`, at the cost of restricting `somata` to classical algorithms with only some extensions to
 Bayesian inference and learning. This is a deliberate choice to allow easier, faster, and cleaner applications of
-somata on neural data analysis, instead of to provide a full-fledged statistical inference package.
+`somata` in neural data analysis, instead of to provide a full-fledged statistical inference package.
 
 ---
 
 ### _class_ StateSpaceModel
 ```python
 somata.StateSpaceModel(components=None, F=None, Q=None, mu0=None, Q0=None, G=None, R=None, y=None, Fs=None)
 ```
@@ -472,45 +459,105 @@
 
 ### For more in-depth working examples with the basic models in somata
 Look at the demo script [basic_models_demo_01102022.py](examples/basic_models_demo_01102022.py) and execute the code line by line to get familiar with class objects and methods of somata basic models.
 
 ---
 
 ## Advanced neural oscillator methods
-1. [Oscillator Model Learning](#osc)
-2. [Iterative Oscillator Algorithm](#ioa)
+1. [Oscillator Model Learning](#1-oscillator-model-learning)
+2. [Phase Amplitude Coupling Estimation](#2-phase-amplitude-coupling-estimation)
+3. [Iterative Oscillator Algorithm](#3-iterative-oscillator-algorithm)
+4. [Switching State-Space Inference](#4-switching-state-space-inference)
+5. [Multi-channel Oscillator Component Analysis](#5-multi-channel-oscillator-component-analysis)
+6. [State-Space Event Related Potential](#6-state-space-event-related-potential)
+7. [Dynamic Source Localization](#7-dynamic-source-localization)
 
 ---
-1. ### Oscillator Model Learning <a name="osc"></a> [<img src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">](#osc)
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">
+</picture>
+
+### 1. Oscillator Model Learning
+
+For fitting data with oscillator models, it boils down to three steps:
+  - Initialize an oscillator model object
+  - Perform state estimation, i.e., E-step
+  - Update model parameters, i.e., M-step
+
+Given some time series `data`, we can fit an oscillator to the data using the expectation-maximization (EM) algorithm.
+```python
+from somata.basic_models import OscillatorModel as Osc
+o1 = Osc(freq=1, Fs=100, y=data)  # create an oscillator object instance
+_ = [o1.m_estimate(**o1.kalman_filt_smooth(EM=True))for x in range(50)]  # run 50 steps of EM
+```
+
 ---
-2. ### Iterative Oscillator Algorithm <a name="ioa"></a> [<img src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">](#ioa)
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Missing-critical.svg?logo=Python">
+</picture>
 
-**N.B.:** We recommend downsampling to 120 Hz or less, depending on the oscillations present in your data. Highly oversampled data will make it more difficult to identify oscillatory components, increase the computational time, and could also introduce high frequency noise.
+### 2. Phase Amplitude Coupling Estimation
 
-One major goal of this method was to produce an algorithm that required minimal user intervention, if any. We recommend starting with the algorithm as is, but in the case of poor fitting, we suggest the following alterations:
-1. If the pole initialized from the one-step prediction is between two oscillations, causing poor fitting of this oscillation as it attempts to explain multiple oscillations, we recommend increasing the order of the AR model used to approximate the OSPE. Increase in increments of two, which will allow additional pairs of complex poles.
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">
+</picture>
 
-2. Conversely to point 1, if the order of the AR model is too high then multiple pairs of roots will be attributed to the same oscillation, diluting the strength needed for each of them and possibly leading to none of them being selected as the strongest root in the iterative process to initialize the next oscillation, even though together they describe the strongest oscillation. This can be identified using the innovations plot with all of the AR roots plotted. In this case we recommend decreasing the AR order in increments of 2, to decrease the number of pairs of complex poles.
+### 3. Iterative Oscillator Algorithm
 
-3. If the initialization of the additional oscillations describes a single oscillation well, but the fitting of this oscillation attempts to explain multiple oscillations and causes poor fitting, we recommend increasing the concentration hyperparameter in the Von Mises prior. This will increase the weight on the initial frequency and stop the oscillation from shifting to explain other oscillations.
+For a well-commented example script, see [IterOsc_example.py](examples/IterOsc_example.py).
 
-4. If the model does not choose the correct number of oscillations, we recommend looking at all fitted models and selecting the best fitting model based on other selection criteria or using your best judgement. You can also choose a subset of well-fitted oscillations and run the kalman filter to estimate oscillations using those fitted parameters.
+_**N.B.:** We recommend downsampling to 120 Hz or less, depending on the oscillations present in your data. Highly oversampled data will make it more difficult to identify oscillatory components, increase the computational time, and could also introduce high frequency noise._
 
-5. Note that this algorithm assumes a stationary signal, and therefore stationary parameters. Although the Kalman filtering allows some flexibility in this requirement, enabling the model to work on some time-varying signal, the success of the method depends on the strength and duration of the signal components. The weaker and more brief the time-varying component is, the more poorly the model will capture it, if it does at all. We recommend decreasing the length of your window until you have a more stationary signal.
+One major goal of this method was to produce an algorithm that requires minimal user intervention, if any. This algorithm is designed to fit well automatically in most situations, but there will still be some data sets where it does not fit well without intervention. We recommend starting with the algorithm as is, but in the case of poor fitting, we suggest the following modifications:
 
-This algorithm is designed to fit well automatically in most situations, but there will still be some data sets where it does not fit well without intervention.
+1. If the model does not choose the correct number of oscillations, we recommend looking at all fitted models and selecting the best fitting model based on other selection criteria or using your best judgement. You can also choose a subset of well-fitted oscillations and run `kalman_filt_smooth()` to estimate oscillations using those fitted parameters.
+
+2. This algorithm assumes stationary parameters, and therefore a stationary signal. Although the Kalman smoothing allows the model to work with some time-varying signal, the success of the method depends on the strength and duration of the signal components. The weaker and more brief the time-varying component is, the more poorly the model will capture it, if at all. We recommend decreasing the length of your window until you have a more stationary signal.
+
+When using this module, please cite the following [paper](https://www.biorxiv.org/content/10.1101/2022.10.30.514422):
+
+Beck, A. M., He, M., Gutierrez, R. G., & Purdon, P. L. (2022). An iterative search algorithm to identify oscillatory dynamics in neurophysiological time series. bioRxiv, 2022-10.
+
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">
+</picture>
 
-When using this module, please cite the following [paper](https://www.biorxiv.org/content/10.1101/2022.10.30.514422.abstract):
+### 4. Switching State-Space Inference
+
+When using this module, please cite the following [paper](https://www.biorxiv.org/content/10.1101/2022.11.18.517120):
+
+He, M., Das, P., Hotan, G., & Purdon, P. L. (2022). Switching state-space modeling of neural signal dynamics. bioRxiv, 2022-11.
+
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Missing-critical.svg?logo=Python">
+</picture>
+
+### 5. Multi-channel Oscillator Component Analysis
+
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Missing-critical.svg?logo=Python">
+</picture>
+
+### 6. State-Space Event Related Potential
+
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Missing-critical.svg?logo=Python">
+</picture>
 
-Beck, A. M., He, M., Gutierrez, R. G., & Purdon, P. L. (2022). An iterative search algorithm to identify oscillatory dynamics in neurophysiological time series. bioRxiv.
+### 7. Dynamic Source Localization
 
 ---
 
 ## Authors
 Mingjian He, Proloy Das, Amanda Beck, Patrick Purdon
 
 ## Citation
 Use different citation styles at: https://doi.org/10.5281/zenodo.7242130
 
 ## License
-SOMATA is licensed under the [BSD 3-Clause Clear license](https://spdx.org/licenses/BSD-3-Clause-Clear.html). \
-Copyright © 2022. All rights reserved.
+SOMATA is licensed under the [BSD 3-Clause Clear license](https://spdx.org/licenses/BSD-3-Clause-Clear.html).\
+Copyright © 2023. All rights reserved.
```

### Comparing `somata-0.2.1/README.md` & `somata-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: somata
+Version: 0.3.1
+Summary: State-space Oscillator Modeling And Time-series Analysis
+Home-page: https://github.com/mh105/somata
+Author: Mingjian He
+Author-email: mh105@mit.edu
+Keywords: state-space oscillator time-series
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Utilities
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # somata
 
 Github: https://github.com/mh105/somata
 
 **State-space Oscillator Modeling And Time-series Analysis (SOMATA)** is a Python library for state-space neural signal
 processing algorithms developed in the [Purdon Lab](https://purdonlab.mgh.harvard.edu).
 Basic state-space models are introduced as class objects for flexible manipulations.
@@ -27,69 +49,78 @@
 * [Authors](#authors)
 * [Citation](#citation)
 * [License](#license)
 
 ---
 
 ## Requirements
-somata is built on `numpy` arrays for computations. `joblib` is used for multithreading. Additional dependencies include
-`matplotlib`, `scipy`, `tqdm`, `codetiming`, and `sorcery`. Full requirements for each release version will be updated
-under `install_requires` in the `setup.cfg` file. If the `environment.yml` file is used to create a new conda
-environment, all and only the required packages will be installed.
+[`somata`](https://pypi.org/project/somata/) is built on [`numpy`](https://numpy.org) arrays for computations. [`joblib`](https://joblib.readthedocs.io/en/stable/) is used for multithreading. 
+Additional dependencies include [`scipy`](https://scipy.org), [`matplotlib`](https://matplotlib.org), and [`spectrum`](https://pyspectrum.readthedocs.io/en/latest/index.html).
+An upcoming source localization module also requires [`pytorch`](https://pytorch.org) and [`MNE-python`](https://mne.tools/stable/index.html).
+Full requirements for each release version will be updated under 
+[`install_requires`](https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#platform-specific-dependencies) in the [`setup.cfg`](setup.cfg) file. 
+If the [`environment.yml`](environment.yml) file is used to [create a new conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file), 
+all and only the required packages will be installed.
 
 ## Install
 
 ```
 pip install somata
 ```
+_If the [`pytorch`](https://pytorch.org) dependency is not resolved successfully by [`pip`](https://pip.pypa.io/en/stable/) for your [OS](https://whatsmyos.com), 
+first [install `pytorch` manually](https://pytorch.org/get-started/locally/) in a [conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) that you wish to install [`somata`](https://pypi.org/project/somata/), 
+and then [execute the above line](https://packaging.python.org/en/latest/tutorials/installing-packages/#ensure-you-can-run-pip-from-the-command-line) to install [`somata`](https://pypi.org/project/somata/)._
 
 ### (For development only)
 
 - ### Fork this repo to personal git
     [How to: GitHub fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo)    
 
 - ### Clone forked copy to local computer
-    ``` git clone <forked copy ssh url> ```
+    [How to: GitHub clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)
 
 - ### Install conda
     [Recommended conda distribution: miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
-    _Apple silicon Mac: choose conda native to the ARM64 architecture instead of Intel x86_
+    _[Apple silicon Mac](https://support.apple.com/en-us/HT211814): choose conda native to the [ARM64 architecture](https://www.anaconda.com/blog/new-release-anaconda-distribution-now-supporting-m1) instead of [Intel x86](https://en.wikipedia.org/wiki/X86)._
 
 - ### Create a new conda environment
     ``` conda install mamba -n base -c conda-forge ```\
     ``` cd <repo root directory with environment.yml> ```\
     ``` mamba env create -f environment.yml ```\
-    ``` conda activate somata ```\
-    _You may also install somata in an existing environment by skipping this step._
+    ``` conda activate somata ```
+
+    _You may also install `somata` in an [existing environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#using-pip-in-an-environment) by skipping this step._
 
-- ### Install somata as a package in editable mode
+- ### Install somata as a package in development mode
     ``` cd <repo root directory with setup.py> ```\
     ``` pip install -e . ```
 
+    _[What is: Editable Installs](https://setuptools.pypa.io/en/latest/userguide/development_mode.html)_
+
 - ### Configure IDEs to use the conda environment
-    [How to: Configure an existing conda environment](https://www.jetbrains.com/help/pycharm/conda-support-creating-conda-virtual-environment.html)
+    [How to: Configure an existing conda environment](https://www.jetbrains.com/help/pycharm/conda-support-creating-conda-virtual-environment.html#existing-conda-environment)
 
 ---
 
 ## Basic state-space models
-Somata, much like a neuron body supported by dendrites, is built on a set of basic state-space models introduced as class objects.
+`somata`, much like a neuron body supported by dendrites, is built on a set of basic state-space models introduced as class objects.
 
 The motivations are to:
 - develop a standardized format to store model parameters of state-space equations
 - override Python dunder methods so `__repr__` and `__str__` return something useful
 - define arithmetic-like operations such as `A + B` and `A * B`
 - emulate `numpy.array()` operations including `.append()`
 - implement inference algorithms like Kalman filtering and parameter update (m-step) equations as callable class methods
 
-At present, and in the near future, somata will be focused on **time-invariant Gaussian linear dynamical systems**.
-This limit on models we consider simplifies basic models to avoid embedded classes such as `transition_model` and
-`observation_model`, at the cost of restricting somata to classical algorithms with only some extensions to
+At present, and in the near future, `somata` will be focused on **time-invariant Gaussian linear dynamical systems**.
+This limit on models we consider simplifies basic models to avoid nested classes such as `transition_model` and
+`observation_model`, at the cost of restricting `somata` to classical algorithms with only some extensions to
 Bayesian inference and learning. This is a deliberate choice to allow easier, faster, and cleaner applications of
-somata on neural data analysis, instead of to provide a full-fledged statistical inference package.
+`somata` in neural data analysis, instead of to provide a full-fledged statistical inference package.
 
 ---
 
 ### _class_ StateSpaceModel
 ```python
 somata.StateSpaceModel(components=None, F=None, Q=None, mu0=None, Q0=None, G=None, R=None, y=None, Fs=None)
 ```
@@ -450,45 +481,105 @@
 
 ### For more in-depth working examples with the basic models in somata
 Look at the demo script [basic_models_demo_01102022.py](examples/basic_models_demo_01102022.py) and execute the code line by line to get familiar with class objects and methods of somata basic models.
 
 ---
 
 ## Advanced neural oscillator methods
-1. [Oscillator Model Learning](#osc)
-2. [Iterative Oscillator Algorithm](#ioa)
+1. [Oscillator Model Learning](#1-oscillator-model-learning)
+2. [Phase Amplitude Coupling Estimation](#2-phase-amplitude-coupling-estimation)
+3. [Iterative Oscillator Algorithm](#3-iterative-oscillator-algorithm)
+4. [Switching State-Space Inference](#4-switching-state-space-inference)
+5. [Multi-channel Oscillator Component Analysis](#5-multi-channel-oscillator-component-analysis)
+6. [State-Space Event Related Potential](#6-state-space-event-related-potential)
+7. [Dynamic Source Localization](#7-dynamic-source-localization)
 
 ---
-1. ### Oscillator Model Learning <a name="osc"></a> [<img src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">](#osc)
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">
+</picture>
+
+### 1. Oscillator Model Learning
+
+For fitting data with oscillator models, it boils down to three steps:
+  - Initialize an oscillator model object
+  - Perform state estimation, i.e., E-step
+  - Update model parameters, i.e., M-step
+
+Given some time series `data`, we can fit an oscillator to the data using the expectation-maximization (EM) algorithm.
+```python
+from somata.basic_models import OscillatorModel as Osc
+o1 = Osc(freq=1, Fs=100, y=data)  # create an oscillator object instance
+_ = [o1.m_estimate(**o1.kalman_filt_smooth(EM=True))for x in range(50)]  # run 50 steps of EM
+```
+
 ---
-2. ### Iterative Oscillator Algorithm <a name="ioa"></a> [<img src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">](#ioa)
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Missing-critical.svg?logo=Python">
+</picture>
 
-**N.B.:** We recommend downsampling to 120 Hz or less, depending on the oscillations present in your data. Highly oversampled data will make it more difficult to identify oscillatory components, increase the computational time, and could also introduce high frequency noise.
+### 2. Phase Amplitude Coupling Estimation
 
-One major goal of this method was to produce an algorithm that required minimal user intervention, if any. We recommend starting with the algorithm as is, but in the case of poor fitting, we suggest the following alterations:
-1. If the pole initialized from the one-step prediction is between two oscillations, causing poor fitting of this oscillation as it attempts to explain multiple oscillations, we recommend increasing the order of the AR model used to approximate the OSPE. Increase in increments of two, which will allow additional pairs of complex poles.
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">
+</picture>
 
-2. Conversely to point 1, if the order of the AR model is too high then multiple pairs of roots will be attributed to the same oscillation, diluting the strength needed for each of them and possibly leading to none of them being selected as the strongest root in the iterative process to initialize the next oscillation, even though together they describe the strongest oscillation. This can be identified using the innovations plot with all of the AR roots plotted. In this case we recommend decreasing the AR order in increments of 2, to decrease the number of pairs of complex poles.
+### 3. Iterative Oscillator Algorithm
 
-3. If the initialization of the additional oscillations describes a single oscillation well, but the fitting of this oscillation attempts to explain multiple oscillations and causes poor fitting, we recommend increasing the concentration hyperparameter in the Von Mises prior. This will increase the weight on the initial frequency and stop the oscillation from shifting to explain other oscillations.
+For a well-commented example script, see [IterOsc_example.py](examples/IterOsc_example.py).
 
-4. If the model does not choose the correct number of oscillations, we recommend looking at all fitted models and selecting the best fitting model based on other selection criteria or using your best judgement. You can also choose a subset of well-fitted oscillations and run the kalman filter to estimate oscillations using those fitted parameters.
+_**N.B.:** We recommend downsampling to 120 Hz or less, depending on the oscillations present in your data. Highly oversampled data will make it more difficult to identify oscillatory components, increase the computational time, and could also introduce high frequency noise._
 
-5. Note that this algorithm assumes a stationary signal, and therefore stationary parameters. Although the Kalman filtering allows some flexibility in this requirement, enabling the model to work on some time-varying signal, the success of the method depends on the strength and duration of the signal components. The weaker and more brief the time-varying component is, the more poorly the model will capture it, if it does at all. We recommend decreasing the length of your window until you have a more stationary signal.
+One major goal of this method was to produce an algorithm that requires minimal user intervention, if any. This algorithm is designed to fit well automatically in most situations, but there will still be some data sets where it does not fit well without intervention. We recommend starting with the algorithm as is, but in the case of poor fitting, we suggest the following modifications:
 
-This algorithm is designed to fit well automatically in most situations, but there will still be some data sets where it does not fit well without intervention.
+1. If the model does not choose the correct number of oscillations, we recommend looking at all fitted models and selecting the best fitting model based on other selection criteria or using your best judgement. You can also choose a subset of well-fitted oscillations and run `kalman_filt_smooth()` to estimate oscillations using those fitted parameters.
+
+2. This algorithm assumes stationary parameters, and therefore a stationary signal. Although the Kalman smoothing allows the model to work with some time-varying signal, the success of the method depends on the strength and duration of the signal components. The weaker and more brief the time-varying component is, the more poorly the model will capture it, if at all. We recommend decreasing the length of your window until you have a more stationary signal.
+
+When using this module, please cite the following [paper](https://www.biorxiv.org/content/10.1101/2022.10.30.514422):
+
+Beck, A. M., He, M., Gutierrez, R. G., & Purdon, P. L. (2022). An iterative search algorithm to identify oscillatory dynamics in neurophysiological time series. bioRxiv, 2022-10.
+
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">
+</picture>
 
-When using this module, please cite the following [paper](https://www.biorxiv.org/content/10.1101/2022.10.30.514422.abstract):
+### 4. Switching State-Space Inference
+
+When using this module, please cite the following [paper](https://www.biorxiv.org/content/10.1101/2022.11.18.517120):
+
+He, M., Das, P., Hotan, G., & Purdon, P. L. (2022). Switching state-space modeling of neural signal dynamics. bioRxiv, 2022-11.
+
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Missing-critical.svg?logo=Python">
+</picture>
+
+### 5. Multi-channel Oscillator Component Analysis
+
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Missing-critical.svg?logo=Python">
+</picture>
+
+### 6. State-Space Event Related Potential
+
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Missing-critical.svg?logo=Python">
+</picture>
 
-Beck, A. M., He, M., Gutierrez, R. G., & Purdon, P. L. (2022). An iterative search algorithm to identify oscillatory dynamics in neurophysiological time series. bioRxiv.
+### 7. Dynamic Source Localization
 
 ---
 
 ## Authors
 Mingjian He, Proloy Das, Amanda Beck, Patrick Purdon
 
 ## Citation
 Use different citation styles at: https://doi.org/10.5281/zenodo.7242130
 
 ## License
-SOMATA is licensed under the [BSD 3-Clause Clear license](https://spdx.org/licenses/BSD-3-Clause-Clear.html). \
-Copyright © 2022. All rights reserved.
+SOMATA is licensed under the [BSD 3-Clause Clear license](https://spdx.org/licenses/BSD-3-Clause-Clear.html).\
+Copyright © 2023. All rights reserved.
```

### Comparing `somata-0.2.1/setup.cfg` & `somata-0.3.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = somata
-version = 0.2.1
+version = 0.3.1
 description = State-space Oscillator Modeling And Time-series Analysis
 author = Mingjian He
 author_email = mh105@mit.edu
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_file = LICENSE
 keywords = state-space oscillator time-series
@@ -21,22 +21,23 @@
 	Topic :: Scientific/Engineering :: Mathematics
 	Topic :: Scientific/Engineering :: Information Analysis
 
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
+	numpy>=1.22
+	colorcet
 	joblib
 	kneed
-	librosa
 	matplotlib
-	numpy>=1.22
 	scipy
 	tqdm
 	spectrum
 	codetiming
-	sorcery>=0.2.2
+dependency_links = 
+	https://conda.anaconda.org/conda-forge/
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `somata-0.2.1/somata/basic_models/arn.py` & `somata-0.3.1/somata/basic_models/arn.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 arn module contains autoregressive model of order n methods used in SOMATA
 """
 
 from somata.basic_models import StateSpaceModel as Ssm
 from somata.exact_inference import inverse
 import numpy as np
 import numbers
-from sorcery import dict_of
 from scipy.linalg import block_diag
 
 
 class AutoRegModel(Ssm):
     """
     AutoRegModel is a subclass of StateSpaceModel class dedicated
     to autoregressive models of order n
@@ -86,34 +85,38 @@
             else:
                 components = []
                 for ii in range(len(self.order)):
                     component = AutoRegModel()
                     component.default_G = np.hstack([np.array([[1.]], dtype=np.float64),
                                                      np.zeros((1, self.order[ii]-1), dtype=np.float64)])
                     components.append(component)
-                self.default_G = components[0].default_G if len(components) == 1 else self.default_G
         else:
             for ii in range(len(components)):
                 current_component: AutoRegModel = components[ii]  # type: ignore
                 assert current_component.type == 'arn', 'Encountered non-arn type component.'
                 assert current_component.default_G.shape[1] == self.order[ii], 'Components mismatch AR order.'
-            self.default_G = components[0].default_G if len(components) == 1 else self.default_G  # type: ignore
+
+        # Update default_G attribute if only a single component
+        if components is not None and len(components) == 1:
+            self.default_G = components[0].default_G
 
         # Call parent class constructor
         super().__init__(components=components, F=F, Q=Q, mu0=mu0, Q0=Q0, G=G, R=R, y=y, Fs=Fs)
 
     # Dunder methods - magic methods
     def __repr__(self):
-        """ Dynamic display depending on whether a single AR model """
+        """ Unambiguous and concise representation when calling AutoRegModel() """
+        # Dynamic display depending on whether a single AR component
         if self.default_G is None:
             return super().__repr__().replace('Ssm', 'Arn')
         else:
             return 'Arn=' + str(self.default_G.shape[1]) + '<' + hex(id(self))[-4:] + '>'
 
     def __str__(self):
+        """ Helpful information when calling print(AutoRegModel()) """
         print_str = super().__str__().replace('<Ssm object at', '<Arn object at')
         # Append additional information about autoregressive parameters
         np.set_printoptions(precision=3)
         print_str += "{0:9} = {1}\n ".format("AR order", str(self.order))
 
         # create the string for displaying coeff
         if self.coeff is None:
@@ -222,16 +225,16 @@
         assert F is not None, 'Cannot guess AR orders with None F matrix.'
         pointer = 0
         order = []
         while pointer < F.shape[0]:
             next_pointer = np.argmax(F[pointer, pointer:] == 0)
             current_order = F.shape[0] - pointer if next_pointer == 0 else next_pointer - pointer
             if current_order > 1:
-                assert (F[pointer+1:pointer+current_order, pointer:pointer+current_order-1] ==
-                        np.eye(current_order-1, dtype=np.float64)).all(), \
+                assert np.all(F[pointer+1:pointer+current_order, pointer:pointer+current_order-1] ==
+                              np.eye(current_order-1, dtype=np.float64)), \
                     'Failed to guess the autoregressive model orders. Consider input order explicitly.'
             order.append(current_order)
             pointer += current_order
         return np.array(order, dtype=np.int_)
 
     def _ssm_to_arn_param(self, F=None, Q=None, order=None):
         """ Convert from matrices F and Q to autoregressive parameters """
@@ -326,15 +329,16 @@
             if R_sigma2 is None:
                 if self.R.shape[0] > 1:
                     raise NotImplementedError('Only uni-variate observation data is supported with prior for now.')
                 else:
                     R_sigma2 = self.R[0, 0]
                     R_hyperparameter = 0.1 if R_hyperparameter is None else R_hyperparameter
 
-            return dict_of(Q_sigma2, Q_hyperparameter, R_sigma2, R_hyperparameter)
+            return {'Q_sigma2': Q_sigma2, 'Q_hyperparameter': Q_hyperparameter,
+                    'R_sigma2': R_sigma2, 'R_hyperparameter': R_hyperparameter}
 
         # recursive case
         else:
             assert self.components is not None, 'Cannot initialize priors outside base case when components is None.'
             components_prefill = self.fill_components(empty_comp=AutoRegModel(), deep_copy=True)
 
             # expand the specified prior values to the length of components
@@ -379,39 +383,29 @@
             # MAP with inverse gamma prior
             Q_init = priors['Q_sigma2']
             Q_hp = priors['Q_hyperparameter'] if 'Q_hyperparameter' in priors else 0.1
             alpha = T * Q_hp / 2  # scales with data length T according to the hyperparameter
             beta = Q_init * (alpha + 1)  # setting the mode of inverse gamma prior to be Q_init
             sigma2_Q_new = (beta + Q_ss / 2) / (alpha + T / 2 + 1)  # mode of inverse gamma posterior
 
-        Q = np.zeros_like(F, dtype=np.float64)
+        Q = np.zeros_like(F, dtype=sigma2_Q_new.dtype)
         Q[0, 0] = sigma2_Q_new
         return Q
 
     @staticmethod
     def _m_update_mu0(x_0_n=None):
         """ Update initial state mean -- mu0 """
-        mu0 = np.zeros((x_0_n.shape[0], 1), dtype=np.float64)
+        mu0 = np.zeros((x_0_n.shape[0], 1), dtype=x_0_n.dtype)
         mu0[0, 0] = x_0_n[0]
         return mu0
 
     @staticmethod
-    def _m_update_mu0_src(x_0_n=None, nstate=None):
-        """
-        Update initial state mean mu0 in dynamic
-        source localization
-        """
-        mu0 = np.zeros((x_0_n.shape[0], 1), dtype=np.float64)
-        mu0[0::nstate, 0] = x_0_n[0::nstate]
-        return mu0
-
-    @staticmethod
     def _m_update_q0(x_0_n=None, P_0_n=None, mu0=None):
         """ Update initial state covariance -- Q0 """
-        Q0 = np.zeros(P_0_n.shape, dtype=np.float64)
+        Q0 = np.zeros(P_0_n.shape, dtype=P_0_n.dtype)
         Q0[0, 0] = P_0_n[0, 0] + x_0_n[0]**2 - 2 * x_0_n[0] * mu0[0, 0] + mu0[0, 0]**2
         return Q0
 
     @staticmethod
-    def _m_update_g(y=None, x_t_n=None, P_t_n=None, h_t=None):
+    def _m_update_g(y=None, x_t_n=None, P_t_n=None, h_t=None, C=None, D=None):
         """ Update observation matrix -- G (AutoRegModel has fixed G) """
         return None
```

### Comparing `somata-0.2.1/somata/basic_models/gen.py` & `somata-0.3.1/somata/basic_models/gen.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 gen module contains general Gaussian state-space model methods used in SOMATA
 """
 
 from somata.basic_models import StateSpaceModel as Ssm
 from somata.exact_inference import inverse
 import numpy as np
-from sorcery import dict_of
 from scipy.linalg import block_diag
 
 
 class GeneralSSModel(Ssm):
     """
     GeneralSSModel is a subclass of StateSpaceModel class dedicated
     to a general single component structure of linear Gaussian
@@ -42,17 +41,19 @@
             component = GeneralSSModel(components=None)  # type: ignore
             component.default_G = np.ones((1, self.nstate), dtype=np.float64)
             self.components = [component]
             self.ncomp = 1
             self.comp_nstates = [self.nstate]
 
     def __repr__(self):
+        """ Unambiguous and concise representation when calling GeneralSSModel() """
         return super().__repr__().replace('Ssm', 'Gen')
 
     def __str__(self):
+        """ Helpful information when calling print(GeneralSSModel()) """
         print_str = super().__str__().replace('<Ssm object at', '<Gen object at')
         return print_str
 
     def get_default_q(self, components=None, E=None):
         """
         Get the default structure of state noise covariance
         matrix Q in the Q_basis block diagonal form
@@ -77,15 +78,15 @@
         if R_sigma2 is None:
             if self.R.shape[0] > 1:
                 raise NotImplementedError('Only uni-variate observation data is supported with prior for now.')
             else:
                 R_sigma2 = self.R[0, 0]
                 R_hyperparameter = 0.1 if R_hyperparameter is None else R_hyperparameter
 
-        return dict_of(R_sigma2, R_hyperparameter)
+        return {'R_sigma2': R_sigma2, 'R_hyperparameter': R_hyperparameter}
 
     @staticmethod
     def _m_update_f(A=None, B=None, C=None, q_old=None, priors=None):
         """ Update transition matrix -- F """
         approach = 'svd' if A.shape[0] >= 5 else 'gaussian'
         F = B @ inverse(A, approach=approach)
         return F
```

### Comparing `somata-0.2.1/somata/basic_models/osc.py` & `somata-0.3.1/somata/basic_models/osc.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 osc module contains Matsuda oscillator specific methods used in SOMATA
 """
 
 from somata.basic_models import StateSpaceModel as Ssm
 import numpy as np
 import numbers
-from sorcery import dict_of
 from math import atan2, sin, cos, sqrt
 from scipy.linalg import block_diag
 
 
 class OscillatorModel(Ssm):
     """
     OscillatorModel is a subclass of StateSpaceModel class
@@ -121,17 +120,19 @@
             else:
                 self.add_dc()
         else:
             self.dc_idx = None
 
     # Dunder methods - magic methods
     def __repr__(self):
+        """ Unambiguous and concise representation when calling OscillatorModel() """
         return super().__repr__().replace('Ssm', 'Osc')
 
     def __str__(self):
+        """ Helpful information when calling print(OscillatorModel()) """
         print_str = super().__str__().replace('<Ssm object at', '<Osc object at')
         # Append additional information about oscillator parameters
         np.set_printoptions(precision=3)
         print_str += "{0:9} = {1}\n ".format("damping a", str(self.a))
         if self.Fs is None:
             print_str += "{0:9} = {1}\n ".format("freq w", str(self.w))
         else:
@@ -383,15 +384,14 @@
             whitener, colorer = _setup_filters(sos1, sos2)
             # noinspection PyAttributeOutsideInit
             self.y_whiten = whitener(self.y)
 
     def visualize_freq(self, version, bw=1, y=None, sim_osc=None, sim_x=None, xlim=None, ylim=None, ax=None):
         """ Visualize the frequency spectrum of real data or the theoretical PSD of the oscillation components """
         import matplotlib.pyplot as plt
-        # noinspection PyProtectedMember
         from ..multitaper import fast_psd_multitaper
 
         # using '%matplotlib notebook' allows zooming in some contexts
         # Create an axes handle for the plot if needed
         if ax is None:
             _, ax = plt.subplots(1, 1)
         colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
@@ -409,65 +409,57 @@
                     label='scaled_data')
             psd_mt, fy_hz = fast_psd_multitaper(self.y_whiten.squeeze(), self.Fs, 0, self.Fs / 2, bw)
             ax.plot(fy_hz, 10 * np.log10(psd_mt.squeeze()), label='whitened_data')
 
         # Plot oscillator spectra
         if version == 'actual':
             kalman_out = self.dejong_filt_smooth(y, return_dict=True)
-            f_hz, h_i = self._oscillator_spectra(version, kalman_out['x_t_n'], bw)
+            h_i, f_hz = self._oscillator_spectra(version, kalman_out['x_t_n'], bw)
         else:
-            f_hz, h_i = self._oscillator_spectra(version)
+            h_i, f_hz = self._oscillator_spectra(version)
+        return_vals = (h_i, f_hz)
+
         h_sum = np.zeros((1, h_i[0].size))
         for ii in range(len(h_i)):
-            if version == 'actual':
-                ax.plot(f_hz, 10 * np.log10(h_i[ii]), label='osc %d, %0.2f Hz' % (ii + 1, self.freq[ii]))
-            elif version == 'theoretical':
-                ax.plot(f_hz, 10 * np.log10(2*h_i[ii]),
-                        label='osc %d, %0.2f Hz' % (ii + 1, self.freq[ii]))  # make spectrum one-sided
+            ax.plot(f_hz, 10 * np.log10(h_i[ii]), label='osc %d, %0.2f Hz' % (ii + 1, self.freq[ii]))
             h_sum += np.sqrt(h_i[ii])
+
         if version == 'theoretical':
             ax.axhline(10 * np.log10(2 * self.R), color='black', linestyle='dashed', label='obs noise')  # one-sided
-
         else:
             ax.plot(f_hz, 20 * np.log10(h_sum.squeeze()), color='gray', label='sum of components')
 
         # Handle simulated oscillator spectra plotting
         if sim_osc is not None and (sim_x is not None or version == 'theoretical'):
             # noinspection PyProtectedMember
-            f_sim, h_sim = sim_osc._oscillator_spectra(version, sim_x, bw)
+            h_sim, f_sim = sim_osc._oscillator_spectra(version, sim_x, bw)
+            return_vals += (h_sim, f_sim)
 
             for ii in range(len(h_sim)):
-                if version == 'actual':
-                    ax.plot(f_sim, 10 * np.log10(h_sim[ii]), linestyle='dashed', color=colors[ii],
-                            label='sim osc %d' % (ii + 1))
-                elif version == 'theoretical':
-                    ax.plot(f_sim, 10 * np.log10(2*h_sim[ii]), linestyle='dashed', color=colors[ii],
-                            label='sim osc %d' % (ii + 1))  # make spectrum one-sided
+                ax.plot(f_sim, 10 * np.log10(h_sim[ii]), linestyle='dashed', color=colors[ii],
+                        label='sim osc %d' % (ii + 1))
+
         elif sim_osc is None and sim_x is not None:
             raise RuntimeError('Do you want to plot empirical spectra of simulated data? If yes,'
                                'input sim_osc object in addition to latent states sim_x.')
         elif sim_osc is not None and sim_x is None:
             raise RuntimeError('Do you want to plot empirical spectra of simulated data? If yes,'
                                'input latent states as sim_x.')
 
         # Final axes adjustment
         ax.legend()
         ax.set_xlabel('Frequency (Hz)')
-        ax.set_ylabel('Power (dB)')
+        ax.set_ylabel('PSD (dB)')
 
         if xlim is not None:
             ax.set_xlim(xlim)
         if ylim is not None:
             ax.set_ylim(ylim)
 
-        if sim_x is not None:
-            # noinspection PyUnboundLocalVariable
-            return f_hz, h_i, f_sim, h_sim
-        else:
-            return f_hz, h_i
+        return return_vals
 
     def visualize_time(self, y=None, plot_ospe=False, ospe_ylim=None, sim_x=None, xlim=None, fig_size=(8, 8)):
         """
         Visualize time series from fitted oscillations.
         sim_x is a 2 dim array (2*ncomp, T) containing the simulated latent states
         """
         import matplotlib.pyplot as plt
@@ -532,45 +524,48 @@
 
         plt.tight_layout()
         plt.show()
         # plt.linkaxes('x')
 
         return fig, axs, x_est
 
-    def _oscillator_spectra(self, version, x_matrix=None, bw=None):
-        """ Compute theoretical or empirical/actual oscillator spectra """
-        # noinspection PyProtectedMember
+    def _oscillator_spectra(self, version='theoretical', x_matrix=None, bw=1):
+        """
+        Compute theoretical or empirical/actual oscillator spectra
+        - Note: these spectra are one-sided from 0 Hz to Nyquist frequency,
+        and these spectra correspond to PSD estimates normalized by the
+        number of time points but not normalized by sampling frequency.
+        """
         from ..multitaper import fast_psd_multitaper
 
         if version == 'theoretical':
             h_i, f_hz = self._theoretical_spectrum()
         elif version == 'actual':
             h_i = []
             for ii in range(self.ncomp):
                 # note that this is not set up for dc components
                 psd_mt, f_hz = fast_psd_multitaper(x_matrix[ii * 2, :], self.Fs, 0, self.Fs / 2, bw)
                 h_i.append(psd_mt)
         else:
             raise ValueError('Chosen version is not supported. Please select theoretical or actual')
 
         # noinspection PyUnboundLocalVariable
-        return f_hz, h_i
+        return h_i, f_hz
 
     def _theoretical_spectrum(self):
         """ Compute spectrum based on theoretical equation (Matsuda 2017) """
-        f_hz = np.linspace(0, self.Fs / 2, 1000)
+        f_hz = np.linspace(0, self.Fs / 2, 2**12)  # one-sided frequency 0 to Nyquist
         rads = f_hz * 2 * np.pi / self.Fs
         z = np.exp(1j * rads)
         a_i = (1 - 2 * self.a ** 2 * np.cos(self.w) ** 2 + self.a ** 4 * np.cos(2 * self.w)) / (
                 self.a * (self.a ** 2 - 1) * np.cos(self.w))
         b_i = 0.5 * (a_i - 2 * self.a * np.cos(self.w) + np.sqrt((a_i - 2 * self.a * np.cos(self.w)) ** 2 - 4))
         v_i = -self.sigma2 * self.a * np.cos(self.w) / b_i
-        h_i = [v_ii * np.abs(
-            1 + b_ii * z) ** 2 / np.abs(1 - 2 * a_ii * np.cos(w_ii) * z + a_ii ** 2 * z ** 2) ** 2 for
-               v_ii, b_ii, a_ii, w_ii in zip(v_i, b_i, self.a, self.w)]
+        h_i = [2 * v_ii * np.abs(1 + b_ii * z) ** 2 / np.abs(1 - 2 * a_ii * np.cos(w_ii) * z + a_ii ** 2 * z ** 2) ** 2
+               for v_ii, b_ii, a_ii, w_ii in zip(v_i, b_i, self.a, self.w)]  # one-sided spectrum
         return h_i, f_hz
 
     def _theoretical_phase(self):
         """ Compute phase response based on the complex spectrum """
         rads = np.linspace(-np.pi, np.pi, 1000)
         z = np.exp(-1j * rads)
         a_i = (1 - 2 * self.a ** 2 * np.cos(self.w) ** 2 + self.a ** 4 * np.cos(2 * self.w)) / (
@@ -625,27 +620,28 @@
             else:
                 w_prior = OscillatorModel.hz_to_rad(f_prior, self.Fs)
             kappa = 10000. if kappa is None else kappa
             vmp_param = {'kappa': kappa, 'f_prior': f_prior, 'w_prior': w_prior}
 
             # [Inverse gamma prior] on state noise covariance Q diagonal entries
             if Q_sigma2 is None:
-                assert self.Q[0, 0] == self.Q[1, 1], 'State noise sigma2 differs between real and imaginary parts'
+                assert self.Q[0, 0] == self.Q[1, 1], 'State noise sigma2 differs between real and imaginary parts.'
                 Q_sigma2 = self.Q[0, 0]
                 Q_hyperparameter = 0.1 if Q_hyperparameter is None else Q_hyperparameter
 
             # [Inverse gamma prior] on observation noise variance R <--- TODO: update to Wishart
             if R_sigma2 is None:
                 if self.R.shape[0] > 1:
                     raise NotImplementedError('Only uni-variate observation data is supported with prior for now.')
                 else:
                     R_sigma2 = self.R[0, 0]
                     R_hyperparameter = 0.1 if R_hyperparameter is None else R_hyperparameter
 
-            return dict_of(vmp_param, Q_sigma2, Q_hyperparameter, R_sigma2, R_hyperparameter)
+            return {'vmp_param': vmp_param, 'Q_sigma2': Q_sigma2, 'Q_hyperparameter': Q_hyperparameter,
+                    'R_sigma2': R_sigma2, 'R_hyperparameter': R_hyperparameter}
 
         # recursive case
         else:
             assert self.components is not None, 'Cannot initialize priors outside base case when components is None.'
             components_prefill = self.fill_components(empty_comp=OscillatorModel(), deep_copy=True)
 
             # expand the specified prior values to the length of components
@@ -726,22 +722,22 @@
             # MAP with inverse gamma prior
             Q_init = priors['Q_sigma2']
             Q_hp = priors['Q_hyperparameter'] if 'Q_hyperparameter' in priors else 0.1
             alpha = T * Q_hp / 2  # scales with data length T according to the hyperparameter
             beta = Q_init * (alpha + 1)  # setting the mode of inverse gamma prior to be Q_init
             sigma2_Q_new = (beta + Q_ss / 2) / (alpha + T / 2 + 1)  # mode of inverse gamma posterior
 
-        Q = sigma2_Q_new * np.eye(2, dtype=np.float64)
+        Q = sigma2_Q_new * np.eye(2, dtype=sigma2_Q_new.dtype)
         return Q
 
     @staticmethod
     def _m_update_q0(x_0_n=None, P_0_n=None, mu0=None):
         """ Update initial state covariance -- Q0 """
         sigma2_Q0 = OscillatorModel.tr(P_0_n + x_0_n[:, None] @ x_0_n[:, None].T
                                        - x_0_n[:, None] @ mu0.T - mu0 @ x_0_n[:, None].T + mu0 @ mu0.T) / 2
-        Q0 = sigma2_Q0 * np.eye(2, dtype=np.float64)
+        Q0 = sigma2_Q0 * np.eye(2, dtype=sigma2_Q0.dtype)
         return Q0
 
     @staticmethod
-    def _m_update_g(y=None, x_t_n=None, P_t_n=None, h_t=None):
+    def _m_update_g(y=None, x_t_n=None, P_t_n=None, h_t=None, C=None, D=None):
         """ Update observation matrix -- G (OscillatorModel has fixed G) """
         return None
```

### Comparing `somata-0.2.1/somata/basic_models/ssm.py` & `somata-0.3.1/somata/basic_models/ssm.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from somata.exact_inference import kalman, djkalman, inverse
 import numpy as np
 import numbers
 from collections.abc import Iterable
 from copy import deepcopy
 from joblib import Parallel, delayed, cpu_count
-from sorcery import dict_of
 from scipy.linalg import block_diag
 
 
 class StateSpaceModel(object):
     """ StateSpaceModel is a general object class for state-space modeling in SOMATA """
     # Class attributes (should not be manually changed or be mutable)
     # only listed here as a reference list for all attributes under Ssm
@@ -639,14 +638,15 @@
         for ii in range(self.ncomp):
             current_component: StateSpaceModel = self.components[ii]  # typehint to superclass to be flexible
             start_idx = sum(self.comp_nstates[:ii])
             end_idx = sum(self.comp_nstates[:ii+1])
 
             # Provide an empty component in the components attribute
             setattr(current_component, 'components', [deepcopy(empty_comp)])
+            current_component.components[0].default_G = current_component.default_G
 
             if getattr(self, 'F') is not None:
                 if deep_copy:
                     F = deepcopy(getattr(self, 'F')[start_idx:end_idx, start_idx:end_idx])
                 else:
                     F = getattr(self, 'F')[start_idx:end_idx, start_idx:end_idx]
                 setattr(current_component, 'F', F)
@@ -743,33 +743,38 @@
         """ Return the first not-None value """
         if a is None:
             return b
         else:
             return a
 
     @staticmethod
-    def setup_array(ssm_array, y=None):
+    def setup_array(ssm_array, y=None, skip_check_observed=False):
         """ Prepare an array of Ssm objects for other signal processing methods """
         # Convert to an array if the input is a single Ssm instance
         if hasattr(ssm_array, 'nmodel'):  # suggests that this is a single somata class object
             ssm_array = ssm_array.stack_to_array()
 
         # Fill the models with the same observed data if provided
         if y is not None:
             for m in range(len(ssm_array)):
                 ssm_array[m].y = y
 
         # Verify that observed data are identical across the array
         first_ssm: StateSpaceModel = ssm_array[0]
-        for ii in range(1, len(ssm_array)):
-            first_ssm._check_observed_data(ssm_array[ii])
+        if not skip_check_observed:
+            for ii in range(1, len(ssm_array)):
+                first_ssm._check_observed_data(ssm_array[ii])
 
         # Array dimensions
         K = len(ssm_array)  # number of models
-        T = first_ssm.ntime  # number of time points
+        Ts = [x.ntime for x in ssm_array]  # number of time points
+        if len(np.unique(Ts)) == 1:
+            T = Ts[0]
+        else:
+            T = Ts  # allow variable lengths of data in different objects
 
         return ssm_array, K, T
 
     # Kalman filtering and smoothing methods (E step)
     def kalman_filt_smooth(self, y=None, R_weights=None, return_dict=False, EM=False, skip_interp=True, seterr=None):
         """ Wrapper method for classical kalman filtering and smoothing """
         if seterr is not None:  # apply np.seterr() for parallel processes
@@ -781,18 +786,20 @@
             skip_interp=skip_interp)
 
         if seterr is not None:
             # noinspection PyUnboundLocalVariable
             np.seterr(**old_settings)
 
         if EM:  # return minimally necessary variables for EM algorithm
-            return dict_of(x_t_n, P_t_n, P_t_tmin1_n, logL)
+            return {'x_t_n': x_t_n, 'P_t_n': P_t_n, 'P_t_tmin1_n': P_t_tmin1_n, 'logL': logL}
         else:
             if return_dict:
-                return dict_of(x_t_n, P_t_n, P_t_tmin1_n, logL, x_t_t, P_t_t, K_t, x_t_tmin1, P_t_tmin1, fy_t_interp)
+                return {'x_t_n': x_t_n, 'P_t_n': P_t_n, 'P_t_tmin1_n': P_t_tmin1_n, 'logL': logL,
+                        'x_t_t': x_t_t, 'P_t_t': P_t_t, 'K_t': K_t,
+                        'x_t_tmin1': x_t_tmin1, 'P_t_tmin1': P_t_tmin1, 'fy_t_interp': fy_t_interp}
             else:
                 return x_t_n, P_t_n, P_t_tmin1_n, logL, x_t_t, P_t_t, K_t, x_t_tmin1, P_t_tmin1, fy_t_interp
 
     def dejong_filt_smooth(self, y=None, R_weights=None, return_dict=False, EM=False, skip_interp=True, seterr=None):
         """ Wrapper method for De Jong version kalman filtering and smoothing """
         if seterr is not None:  # apply np.seterr() for parallel processes
             old_settings = np.seterr(**seterr)
@@ -803,28 +810,31 @@
             skip_interp=skip_interp)
 
         if seterr is not None:
             # noinspection PyUnboundLocalVariable
             np.seterr(**old_settings)
 
         if EM:  # return minimally necessary variables for EM algorithm
-            return dict_of(x_t_n, P_t_n, P_t_tmin1_n, logL)
+            return {'x_t_n': x_t_n, 'P_t_n': P_t_n, 'P_t_tmin1_n': P_t_tmin1_n, 'logL': logL}
         else:
             if return_dict:
-                return dict_of(x_t_n, P_t_n, P_t_tmin1_n, logL, x_t_t, P_t_t, K_t, x_t_tmin1, P_t_tmin1, fy_t_interp)
+                return {'x_t_n': x_t_n, 'P_t_n': P_t_n, 'P_t_tmin1_n': P_t_tmin1_n, 'logL': logL,
+                        'x_t_t': x_t_t, 'P_t_t': P_t_t, 'K_t': K_t,
+                        'x_t_tmin1': x_t_tmin1, 'P_t_tmin1': P_t_tmin1, 'fy_t_interp': fy_t_interp}
             else:
                 return x_t_n, P_t_n, P_t_tmin1_n, logL, x_t_t, P_t_t, K_t, x_t_tmin1, P_t_tmin1, fy_t_interp
 
     @staticmethod
-    def par_kalman(ssm_array, y=None, method='kalman', R_weights=None, skip_interp=True, return_dict=False):
+    def par_kalman(ssm_array, y=None, method='kalman', skip_check_observed=False,
+                   R_weights=None, skip_interp=True, return_dict=False):
         """
         Parallel run kalman filtering and smoothing on
         an array of StateSpaceModel objects
         """
-        ssm_array, K, T = StateSpaceModel.setup_array(ssm_array, y=y)
+        ssm_array, K, _ = StateSpaceModel.setup_array(ssm_array, y=y, skip_check_observed=skip_check_observed)
 
         if method == 'kalman':
             kalman_func = getattr(StateSpaceModel, 'kalman_filt_smooth')
         elif method == 'dejong':
             kalman_func = getattr(StateSpaceModel, 'dejong_filt_smooth')
         else:
             raise ValueError('Specified method is invalid for parallel kalman calls.')
@@ -838,25 +848,25 @@
         n_jobs = max(cpu_count()-1, 1)
         results = Parallel(n_jobs=n_jobs)(delayed(kalman_func)(model, y, weights, False, False,
                                                                skip_interp, np.geterr())
                                           for model, weights in zip(ssm_array, R_weights))
 
         # Unpack results into separate variables to return
         (x_t_n_all, P_t_n_all, P_t_tmin1_n_all,
-         x_t_t_all, P_t_t_all, K_t_all, x_t_tmin1_all, P_t_tmin1_all) = tuple([[None]*K for _ in range(8)])
-        logL_all = np.zeros((K, T), dtype=np.float64)
-        fy_t_interp_all = np.zeros((K, T), dtype=np.float64)
+         x_t_t_all, P_t_t_all, K_t_all, x_t_tmin1_all, P_t_tmin1_all,
+         logL_all, fy_t_interp_all) = tuple([[None]*K for _ in range(10)])
         for m in range(K):
             (x_t_n_all[m], P_t_n_all[m], P_t_tmin1_n_all[m],
-             logL_all[m, :], x_t_t_all[m], P_t_t_all[m], K_t_all[m],
-             x_t_tmin1_all[m], P_t_tmin1_all[m], fy_t_interp_all[m, :]) = results[m]
+             logL_all[m], x_t_t_all[m], P_t_t_all[m], K_t_all[m],
+             x_t_tmin1_all[m], P_t_tmin1_all[m], fy_t_interp_all[m]) = results[m]
 
         if return_dict:
-            return dict_of(x_t_n_all, P_t_n_all, P_t_tmin1_n_all, logL_all,
-                           x_t_t_all, P_t_t_all, K_t_all, x_t_tmin1_all, P_t_tmin1_all, fy_t_interp_all)
+            return {'x_t_n_all': x_t_n_all, 'P_t_n_all': P_t_n_all, 'P_t_tmin1_n_all': P_t_tmin1_n_all,
+                    'logL_all': logL_all, 'x_t_t_all': x_t_t_all, 'P_t_t_all': P_t_t_all, 'K_t_all': K_t_all,
+                    'x_t_tmin1_all': x_t_tmin1_all, 'P_t_tmin1_all': P_t_tmin1_all, 'fy_t_interp_all': fy_t_interp_all}
         else:
             return x_t_n_all, P_t_n_all, P_t_tmin1_n_all, logL_all, \
                 x_t_t_all, P_t_t_all, K_t_all, x_t_tmin1_all, P_t_tmin1_all, fy_t_interp_all
 
     # Parameter estimation methods (M step)
     # noinspection PyUnusedLocal
     def m_estimate(self, y=None, x_t_n=None, P_t_n=None, P_t_tmin1_n=None, h_t=None, logL=None,
@@ -954,27 +964,27 @@
                                                        P_0_n=P_t_n[start_idx:end_idx, start_idx:end_idx, 0],
                                                        mu0=self.mu0[start_idx:end_idx, 0][:, None])
 
                 if 'G' in update_param and 'G' not in keep_param:
                     comp_G = current_component._m_update_g(y=y, x_t_n=x_t_n[start_idx:end_idx, :],
                                                            P_t_n=P_t_n[start_idx:end_idx, start_idx:end_idx, :],
                                                            h_t=h_t)
-                    self.G[start_idx:end_idx, start_idx:end_idx] = \
-                        comp_G if comp_G is not None else self.G[start_idx:end_idx, start_idx:end_idx]
+                    self.G[:, start_idx:end_idx] = comp_G if comp_G is not None else self.G[:, start_idx:end_idx]
 
         # Update observation noise covariance -- R
         if 'R' in update_param and 'R' not in keep_param:
             R_ss = self._m_update_r(y=y, x_t_n=x_t_n, P_t_n=P_t_n, h_t=h_t, G=self.G, priors=priors[0])
         else:
             R_ss = self._m_update_r(y=y, x_t_n=x_t_n, P_t_n=P_t_n, h_t=h_t, G=self.G, keep_R=True)
 
         if return_dict is None:
             pass
         elif return_dict:
-            return dict_of(self.F, self.Q, self.mu0, self.Q0, self.G, self.R, R_ss, A, B, C)
+            return {'F': self.F, 'Q': self.Q, 'mu0': self.mu0, 'Q0': self.Q0, 'G': self.G, 'R': self.R,
+                    'R_ss': R_ss, 'A': A, 'B': B, 'C': C}
         else:
             return self.F, self.Q, self.mu0, self.Q0, self.G, self.R, R_ss, A, B, C
 
     def update_comp_param(self):
         """ Update component specific parameters, override in subclasses """
         return
 
@@ -1070,24 +1080,30 @@
     def _m_update_q0(x_0_n=None, P_0_n=None, mu0=None):
         """ Update initial state covariance -- Q0 """
         Q0 = P_0_n + x_0_n[:, None] @ x_0_n[:, None].T \
             - x_0_n[:, None] @ mu0.T - mu0 @ x_0_n[:, None].T + mu0 @ mu0.T
         return Q0
 
     @staticmethod
-    def _m_update_g(y=None, x_t_n=None, P_t_n=None, h_t=None):
+    def _m_update_g(y=None, x_t_n=None, P_t_n=None, h_t=None, C=None, D=None):
         """ Update observation matrix -- G """
-        assert len(h_t) == y.shape[1], 'Different lengths of h_t and y. Cannot proceed with _m_update_g().'
-        P = (h_t * P_t_n[:, :, 1:]).sum(axis=2) + (h_t * x_t_n[:, 1:]) @ x_t_n[:, 1:].T
-        approach = 'svd' if P.shape[0] >= 5 else 'gaussian'
-        G = (h_t * y) @ x_t_n[:, 1:].T @ inverse(P, approach=approach)
+        if C is None:
+            assert len(h_t) == y.shape[1], 'Different lengths of h_t and y. Cannot proceed with _m_update_g().'
+            C = (h_t * P_t_n[:, :, 1:]).sum(axis=2) + (h_t * x_t_n[:, 1:]) @ x_t_n[:, 1:].T
+
+        if D is None:
+            assert len(h_t) == y.shape[1], 'Different lengths of h_t and y. Cannot proceed with _m_update_g().'
+            D = (h_t * y) @ x_t_n[:, 1:].T
+
+        approach = 'svd' if C.shape[0] >= 5 else 'gaussian'
+        G = D @ inverse(C, approach=approach)
         return G
 
     @staticmethod
-    def _m_estimate_scope(update_param, keep_param):
+    def _m_estimate_scope(update_param=('F', 'Q', 'mu0', 'Q0', 'G', 'R'), keep_param=()):
         """ Sort out the scopes of updates in m_estimate() """
         if 'F' not in update_param and 'Q' not in update_param:
             update_FQ = False
         elif 'F' in keep_param and 'Q' in keep_param:
             update_FQ = False
         else:
             update_FQ = True
```

### Comparing `somata-0.2.1/somata/exact_inference/dp_func.py` & `somata-0.3.1/somata/exact_inference/dp_func.py`

 * *Files identical despite different names*

### Comparing `somata-0.2.1/somata/exact_inference/em.py` & `somata-0.3.1/somata/exact_inference/em.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Author: Mingjian He <mh105@mit.edu>
 
 em module contains a general run_em() function that works across SOMATA
 """
 
 import numpy as np
 from tqdm import tqdm
-from sorcery import dict_of
 
 
 def run_em(obj: object, y=None, init_from_data=False, e_kwargs=None, m_kwargs=None,
            max_iter=10, stop_thresh=np.finfo(float).eps, ignore_numerr=False, return_dict=False, show_pbar=False):
     """
     run_em() is a general purpose function to organize EM algorithms used
     throughout SOMATA. The class object that is input as the first argument
@@ -32,14 +31,17 @@
     :param max_iter: maximal number of EM iterations to run
     :param stop_thresh: a stopping criterion threshold, flexible depending on the
                         stopping variable used by the e/m_step() methods of obj
     :param ignore_numerr: whether to ignore warning messages of numerical errors
     :param return_dict: None -> no return, True -> return dict, False -> return tuple of variables
     :param show_pbar: show progress bar during EM iterations
     """
+    e_kwargs = {} if e_kwargs is None else e_kwargs
+    m_kwargs = {} if m_kwargs is None else m_kwargs
+
     # Initialize from data
     if init_from_data:
         obj.initialize_from_data(y=y)
 
     # Initialize EM iterations
     em_iter = 0
     stop_var = float('inf')
@@ -68,10 +70,10 @@
     if ignore_numerr:
         # noinspection PyUnboundLocalVariable
         np.seterr(**old_settings)
 
     if return_dict is None:
         pass
     elif return_dict:
-        return dict_of(em_iter, stop_var_tally)
+        return {'em_iter': em_iter, 'stop_var_tally': stop_var_tally}
     else:
         return em_iter, stop_var_tally
```

### Comparing `somata-0.2.1/somata/iterative_oscillator/helper_functions.py` & `somata-0.3.1/somata/iterative_oscillator/helper_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,86 @@
-""" Author: Amanda Beck <ambeck@mit.edu> """
+"""
+Author: Amanda Beck <ambeck@mit.edu>
+        Mingjian He <mh105@mit.edu>
+"""
 
 import numpy as np
 from numpy import random
-from numpy.linalg import eig, inv
-from scipy.linalg import toeplitz
-from spectrum import aryule, arma_estimate, arma2psd, arburg
+from spectrum import aryule, arma2psd, arburg
 import matplotlib.pyplot as plt
 from kneed import KneeLocator
 from ..multitaper import fast_psd_multitaper
 from ..basic_models import OscillatorModel as Osc
 
 
-def innovations_wrapper(iter_osc, osc_num, fig_size=(8, 6), plot_all_poles=False, horizontal=False, ax_limit=None):
-    """ Plots the innovations for models in the original scale, used for Beck et al. 2022 """
-    osc = iter_osc.fitted_osc[osc_num]  # we're using the scaled version like in the iterations
-    innovations, ll = find_innovations(osc, y=iter_osc.added_osc[0].y)
-
-    add_freq, add_radius, all_freq, all_radii, a, b = initialize_newosc(osc.Fs, innovations, existing_freqs=None,
-                                                                        ar_order=iter_osc.ar_order,
-                                                                        burg_flag=iter_osc.burg_flag)
-
-    axlim, fig = innovations_plot(osc, iter_osc.added_osc[0].y, innovations, a, b, add_freq,
-                                  plot_all_poles=plot_all_poles,
-                                  ax_limit=ax_limit, fig_size=fig_size, horizontal=horizontal)
+def innovations_wrapper(iter_osc, iter_num, plot_all_poles=True, ax_limit=None, fig_size=(8, 6), horizontal=False):
+    """ Plots the innovations for fitted models, used for Beck et al. 2022 """
+    y = iter_osc.added_osc[0].y
+    osc = iter_osc.fitted_osc[iter_num]
+    innovations, ll = find_innovations(osc, y=y)
+
+    add_freq = iter_osc.added_osc[iter_num + 1].freq[0] if iter_num + 1 < len(iter_osc.added_osc) else None
+    add_radius = iter_osc.added_osc[iter_num + 1].a[0] if iter_num + 1 < len(iter_osc.added_osc) else None
+
+    a, b, _ = fit_ar(np.squeeze(innovations), iter_osc.osc_range * 2 - 1, iter_osc.burg_flag)
+    axlim, fig = innovations_plot(osc, y, innovations, a, b, add_freq, add_radius, plot_all_poles=plot_all_poles,
+                                  ax_limit=ax_limit, fig_size=fig_size, horizontal=horizontal, counter=iter_num)
 
     return axlim, fig
 
 
-def initial_param(y, fs, noise_start, ar_order=13, burg_flag=False):
-    """ Scale y data and prepare initialization of OscillatorModel object """
-    R_est = initialize_r(y, fs, noise_start)
-    power = np.ceil(200 / fs)
-    y_scaled = y / np.sqrt(R_est)
-    # TODO: test remove scaling all together and set R here to be R_est directly
-    add_freq, _, _, _, _, b = initialize_newosc(fs, y_scaled, ar_order=ar_order, burg_flag=burg_flag)
-    osc_init = {'y': y_scaled, 'a': 0.98 ** power, 'freq': add_freq, 'sigma2': b,
-                'Fs': fs, 'R': b}
-    return osc_init, R_est
-
-
-def initialize_r(y, fs, noise_start, noise_end=None, variance=False):
-    """ Find mean power above a certain frequency (noise_start) """
-    fft_data = np.fft.fftshift(np.fft.fft(np.squeeze(y)))
-    psd_data = np.abs(fft_data) ** 2 / y.size
-    freq = np.linspace(-fs / 2, fs / 2, psd_data.size)
-
-    min_idx = np.argmin(np.abs(freq - noise_start))
-    max_idx = np.argmin(np.abs(freq - noise_end)) if noise_end is not None else None
-    noise_spectrum = psd_data[min_idx:max_idx]
-    R_estimated = np.mean(noise_spectrum)
-
-    if variance:  # also return the variance across the specified noise frequencies
-        return R_estimated, np.var(noise_spectrum)
-    else:
-        return R_estimated
-
-
 def find_innovations(osc, y=None):
     """ Calculate innovations / one step prediction error """
     y = osc.y if y is None else y
     kalman_out = osc.dejong_filt_smooth(y=y, return_dict=True)
     x_pred = kalman_out['x_t_tmin1'][:, 1:]
     y_pred = osc.G @ x_pred
     return (y - y_pred).squeeze(), kalman_out['logL'].sum()
 
 
-def initialize_newosc(fs, innovations, existing_freqs=None, ar_order=13, burg_flag=False):
-    """ Fit AR model to innovations """
+def fit_ar(y, ar_order, burg_flag=False):
+    """ Fit AR model to a time series """
     if burg_flag:  # use Burg algorithm
-        a, p, k = arburg(np.squeeze(innovations), ar_order)
+        a, p, k = arburg(y, ar_order)
     else:  # default is Yule Walker algorithm
-        a, p, k = aryule(np.squeeze(innovations), ar_order)
+        a, p, k = aryule(y, ar_order)
+    return a, p, k
+
+
+def get_ar_psd(fs, a, p, ar_hz=None, df=0.01):
+    """ Get the PSD spectrum of a fitted AR model """
+    if ar_hz is None:
+        nfft = int(2 ** np.ceil(np.log2(fs / df)))  # nfft to achieve a [< df] sampling resolution of frequencies
+        ar_hz = np.arange(0, fs / 2, fs / nfft)  # one-sided frequency 0 to Nyquist
+        assert ar_hz.size == nfft // 2, 'Incorrect nfft in the AR theoretical spectrum.'
+    ar_psd = arma2psd(A=a, rho=p, NFFT=2 * ar_hz.size, sides='centerdc')[ar_hz.size:] * 2  # make spectrum one-sided
+    return ar_psd, ar_hz
+
+
+def initialize_newosc(fs, innovations, existing_freqs=None, freq_res=1, ar_order=13, burg_flag=False):
+    """ Initialize the new oscillator to be added """
+    a, p, k = fit_ar(np.squeeze(innovations), ar_order, burg_flag)
     r = np.roots(np.concatenate(([1], a)))
     sampling_constant = fs / 2 / np.pi
     root_freqs = np.abs(np.arctan2(np.imag(r), np.real(r)) * sampling_constant)  # force to positive frequencies
-    root_radii = np.abs(r)
-    root_radii_copy = root_radii.copy()
-    if existing_freqs is not None:
-        root_radii_copy[np.isin(root_freqs, existing_freqs)] = -1  # ignore frequencies with existing oscillators
-    largest_root_idx = np.argmax(root_radii_copy)
-    add_freq = root_freqs[largest_root_idx]
-    add_radius = root_radii[largest_root_idx]
-    return add_freq, add_radius, root_freqs, root_radii, a, p
+    root_radii = np.abs(r)  # compute the magnitude of complex roots
 
+    # within [freq_res] Hz of existing frequencies is considered as duplicated
+    root_freqs_idx = [min(abs(x - existing_freqs)) >= freq_res
+                      if existing_freqs is not None else True for x in root_freqs]
+
+    # look for the root with the largest AR theoretical PSD scaled by radius
+    ar_psd, ar_hz = get_ar_psd(fs, a, p)
+    root_psd = np.array(
+        [ar_psd[np.argmin(abs(freq - ar_hz))] * radius for freq, radius in zip(root_freqs, root_radii)])
+    sel_idx = np.argmax(root_psd[root_freqs_idx])
+    add_freq = max([root_freqs[root_freqs_idx][sel_idx], 0.1])  # lower bound added frequency to 0.1 Hz
+    add_radius = root_radii[root_freqs_idx][sel_idx]
 
-def initialize_arma(fs, innovations, ar_order=7):
-    """ Fit ARMA model to innovations """
-    a, b, rho = arma_estimate(innovations, ar_order, 1, ar_order + 5)
-    r = np.roots(np.concatenate(([1], a)))
-    sampling_constant = fs / 2 / np.pi
-    root_freqs = np.abs(np.arctan2(np.imag(r), np.real(r)) * sampling_constant)
-    root_radii = np.abs(r)
-    largest_root = np.argmax(root_radii)
-    return root_freqs[largest_root], root_radii[largest_root], root_freqs, root_radii, a, b, rho
+    return add_freq, add_radius, root_freqs, root_radii, a, p
 
 
 def aic_calc(osc, ll):
     """ Calculate AIC """
     if osc.dc_idx is None:
         param_num = osc.ncomp * 3 + 1  # each oscillator has 3 parameters + obs noise variance
     else:
@@ -114,15 +98,15 @@
     return np.exp(-deltas) / np.sum(np.exp(-deltas))
 
 
 def get_knee(ll_vec):
     """ Use 'kneed' python package to find knee/elbow """
     kneedle = KneeLocator(range(len(ll_vec)), ll_vec, S=1.0, curve="concave",
                           direction="increasing")
-    return kneedle.knee  # Returns int,  index of model at knee
+    return kneedle.knee  # Returns int, index of model at knee
 
 
 def simulate_matsuda(param_list, R=1, Fs=100, T=10):
     """
     Simulate time series from matsuda oscillators (Matsuda and Komaki 2017)
         param_list = array of dictionaries, one for each oscillation with the following entries:
             a = scalar damping factor
@@ -234,156 +218,99 @@
 
     iterosc.all_params is a list of lists. The inner lists are one list per oscillator,
     with the Osc objects over the EM iterations. The inner list is em_params
     """
     plt.figure()
     Fs = em_params[0].Fs
     psd_mt, f_hz = fast_psd_multitaper(y, Fs, 0, Fs / 2, bw)
-    plt.plot(f_hz.squeeze(), 10 * np.log10(psd_mt.squeeze()), color='black', label='observed data')
+    plt.plot(f_hz, 10 * np.log10(psd_mt), color='black', label='observed data')
     cm = plt.get_cmap('coolwarm')
     for ii in range(len(em_params)):
         # noinspection PyProtectedMember
-        h_i = em_params[ii]._theoretical_spectrum()
+        h_i, f_th = em_params[ii]._theoretical_spectrum()
         for jj in range(len(h_i)):
             cl = int(ii / len(em_params) * 256)  # y further 0~Convert to 255
-            plt.plot(f_hz, 10 * np.log10(h_i[jj]), c=cm(cl))
+            plt.plot(f_th, 10 * np.log10(h_i[jj]), c=cm(cl))
     plt.legend()
     plt.xlabel('Frequency (Hz)')
-    plt.ylabel('Power (dB)')
+    plt.ylabel('PSD (dB)')
 
 
-def innovations_plot(osc, y, innovations, a, b, add_freq, plot_all_poles=False, ax_limit=None, fig_size=(8, 6),
-                     horizontal=False, bw=2):
+def innovations_plot(osc, y, innovations, a, b, add_freq=None, add_radius=None, plot_all_poles=False, ax_limit=None,
+                     fig_size=(8, 6), horizontal=False, bw=1, counter=0):
     """ Plot fitted OscillatorModel and the innovations / one-step prediction error for that model """
     psd_mt, fy_hz = fast_psd_multitaper(innovations, osc.Fs, 0, osc.Fs / 2, bw)
-    ar_psd = arma2psd(A=a, rho=b, NFFT=2 * fy_hz.size, T=osc.Fs, sides='centerdc')
-    psd_y, freq_y = fast_psd_multitaper(y.squeeze(), osc.Fs, 0, osc.Fs / 2, bw)
+    psd_ar, _ = get_ar_psd(osc.Fs, a, b, ar_hz=fy_hz)
+    psd_y, _ = fast_psd_multitaper(y.squeeze(), osc.Fs, 0, osc.Fs / 2, bw)
 
     if horizontal:
         fig, [ax0, ax1] = plt.subplots(1, 2, figsize=fig_size)
     else:
         fig, [ax0, ax1] = plt.subplots(2, 1, sharex='all', figsize=fig_size)
-    ax0.plot(freq_y, 10 * np.log10(psd_y), color='black', label='observed data')
+    ax0.plot(fy_hz, 10 * np.log10(psd_y), color='black', label='observed data')
 
     kalman_out = osc.dejong_filt_smooth(y, return_dict=True)
 
     # noinspection PyProtectedMember
-    f_th, h_th = osc._oscillator_spectra('theoretical', kalman_out['x_t_n'], bw)
-    h_sum = np.zeros((1, h_th[0].size))
+    h_th, f_th = osc._oscillator_spectra('theoretical', kalman_out['x_t_n'], bw)
     for ii in range(len(h_th)):
-        ax0.plot(f_th, 10 * np.log10(2*h_th[ii]),
-                 label='osc %d fit, %0.2f Hz' % (ii + 1, osc.freq[ii]))  # make spectrum one-sided
-        h_sum += np.sqrt(h_th[ii])
-    h_sum += np.sqrt(osc.R)
+        ax0.plot(f_th, 10 * np.log10(h_th[ii]), label='osc %d fit, %0.2f Hz' % (ii + 1, osc.freq[ii]))
     ax0.legend(loc='upper right')
-    ax0.set_ylabel('Power (dB)')
-    ax0.set_title('Iteration %d' % len(h_th))
+    ax0.set_ylabel('PSD (dB)')
+    ax0.set_title('Iteration %d' % counter)
 
     ax1.plot(fy_hz, 10 * np.log10(psd_mt), label='OSPE', color='tab:blue')
-    ax1.plot(fy_hz, 10 * np.log10(ar_psd[fy_hz.size:] * osc.Fs * 2), linestyle='dashed', color='tab:blue',
-             label='AR fit')
+    ax1.plot(fy_hz, 10 * np.log10(psd_ar), label='AR fit', linestyle='dashed', color='tab:blue')
     if ax_limit is not None:
         ax1.set_ylim(ax_limit)
 
     ax1.set_xlabel('Frequency (Hz)')
-    ax1.set_ylabel('Power (dB)', color='tab:blue')
+    ax1.set_ylabel('PSD (dB)', color='tab:blue')
     ax1.tick_params(axis='y', labelcolor='tab:blue')
 
-    ax1.set_title('One-Step Prediction Error (OSPE) - Iteration %d' % len(h_th))
-    ax1.axvline(add_freq, color='black', linestyle='dashed', label='frequency of new oscillation, %0.2f Hz' % add_freq)
+    ax1.set_title('One-Step Prediction Error (OSPE) - Iteration %d' % counter)
+    if add_freq is not None:
+        ax1.axvline(add_freq, color='black', linestyle='dashed',
+                    label='frequency of new oscillator: %0.2f Hz' % add_freq)
     # ax1.axhline(20 * np.log10(b), color='black', label='observation noise estimate')
-    ax1.legend(loc='upper right')
-
-    r = np.roots(np.concatenate(([1], a)))
-    sampling_constant = osc.Fs / 2 / np.pi
-    root_freqs = np.abs(np.arctan2(np.imag(r), np.real(r)) * sampling_constant)
-    for rf in range(len(root_freqs)):
-        if root_freqs[rf] == osc.Fs / 2:
-            root_freqs[rf] = 0
 
     ax2 = ax1.twinx()
     if plot_all_poles:
+        r = np.roots(np.concatenate(([1], a)))
+        sampling_constant = osc.Fs / 2 / np.pi
+        root_freqs = np.abs(np.arctan2(np.imag(r), np.real(r)) * sampling_constant)  # force to positive frequencies
         ax2.scatter(root_freqs, np.abs(r), color='tab:orange')
-    ax2.scatter(add_freq, np.max(abs(r)), facecolor='tab:green', linewidth=2, label='pole for initialization')
+    if add_freq is not None and add_radius is not None:
+        ax2.scatter(add_freq, add_radius, facecolor='tab:green', linewidth=2, label='pole for initialization')
 
     ax2.set_ylim([0, 1])
     ax2.set_xlabel('Frequency (Hz)')
     ax2.set_ylabel('Root (magnitude)', color='tab:green')
     ax2.tick_params(axis='y', labelcolor='tab:green')
     ax2.spines['left'].set_color('tab:blue')
     ax2.spines['right'].set_color('tab:green')
     ax2.spines['left'].set(lw=3)
     ax2.spines['right'].set(lw=3)
 
     lines, labels = ax1.get_legend_handles_labels()
     lines2, labels2 = ax2.get_legend_handles_labels()
-    ax2.legend(lines + lines2, labels + labels2, loc='upper right')
+    ax2.legend(lines + lines2, labels + labels2, loc='lower center')
 
     fig.tight_layout()  # otherwise, the right y-label is slightly clipped
     plt.show()
 
     return ax1.get_ylim(), fig
 
 
-def compare_arma(fs, innovations, a, b, add_freq):
-    """ Plot AR and ARMA models to compare """
-    add_freq1, add_radius1, root_freqs1, root_radii1, a1, b1, rho1 = initialize_arma(fs, innovations)
-    psd_mt, fy_hz = fast_psd_multitaper(innovations, fs, 0, fs / 2, 1)
-    ar_psd = arma2psd(A=a, rho=b, NFFT=2 * fy_hz.size, T=fs, sides='centerdc')
-    arma_psd = arma2psd(A=a1, B=b1, rho=rho1, NFFT=2 * fy_hz.size, T=fs, sides='centerdc')
-
-    fig, ax = plt.subplots(2, 1, sharex='all', figsize=(8, 8))
-    ax[0].plot(fy_hz, 10 * np.log10(psd_mt), label='observed data')
-    ax[0].plot(fy_hz, 10 * np.log10(arma_psd[fy_hz.size:] * fs * 2), linestyle='dashed',
-               label='arma')  # sqrt(2) factor may be off
-    ax[0].plot(fy_hz, 10 * np.log10(ar_psd[fy_hz.size:] * fs * 2), label='ar')
-    ax[0].set_ylabel('Power (dB)')
-    ax[0].set_title('Innovations')
-    ax[0].axvline(add_freq, color='black', label='AR fit')
-    ax[0].axvline(add_freq1, color='black', linestyle='dashed', label='ARMA fit')
-    ax[0].axhline(10 * np.log10(b), color='black', label='_nolegend_')
-    ax[0].axhline(10 * np.log10(rho1), color='black', linestyle='dashed', label='_nolegend_')
-    ax[0].legend()
+def plot_fit_line(fig, slope, intercept):
+    """ Add a linear fit line to an existing innovation plot figure """
+    ax = fig.axes[1]
+    x_limits = ax.get_xlim()
+    ax.plot(x_limits, [x * slope + intercept for x in x_limits], label='linear fit', color='black')
+    ax.set_xlim(x_limits)
+
+    lines, labels = ax.get_legend_handles_labels()
+    lines2, labels2 = fig.axes[2].get_legend_handles_labels()
+    fig.axes[2].legend(lines + lines2, labels + labels2, loc='lower center')
 
-    r = np.roots(np.concatenate(([1], a)))
-    sampling_constant = fs / 2 / np.pi
-    root_freqs = np.abs(np.arctan2(np.imag(r), np.real(r)) * sampling_constant)
-    z = np.roots(np.concatenate(([1], b1)))
-    for rf in range(len(root_freqs)):
-        if root_freqs[rf] == fs / 2:
-            root_freqs[rf] = 0
-        if root_freqs1[rf] == fs / 2:
-            root_freqs1[rf] = 0
-
-    ax[1].scatter(root_freqs, np.abs(r), color='tab:green', label='ar poles')
-    ax[1].scatter(root_freqs1, root_radii1, color='tab:orange', label='arma poles')
-    ax[1].scatter(0, np.abs(z), marker='^', color='tab:orange', label='arma zeroes')
-    ax[1].set_xlabel('Frequency (Hz)')
-    ax[1].set_ylabel('Root (magnitude)')
-
-    print('ARMA: add freq: %0.2f Hz, add radius: %0.3f, add q: %0.3f' % (add_freq1, add_radius1, rho1))
-
-
-def find_a(y, p, Ri=None):
-    """ Fit AR parameters based on R (Matsuda and Komaki 2017) """
-    Ck = np.asarray([cov_k(y, ii) for ii in range(p + 1)])
-    C = toeplitz(Ck)
-
-    if Ri is None:
-        w, v = eig(C)
-        Ri = np.min(np.abs(w))
-    C_new = C - Ri * np.eye(p + 1)
-
-    a_vec = np.squeeze(inv(C_new[:-1, :-1]) @ Ck[1:, None])
-    Q = Ck[0] - np.sum(a_vec * Ck[1:])
-
-    return a_vec, Q, Ri, Ck
-
-
-def cov_k(y, k):
-    """ Calculate covariance at lag k """
-    N = y.size
-    y = y.squeeze()
-    if k > 0:
-        return np.sum(y[:(-k)] * y[k:]) / N
-    else:
-        return np.sum(y ** 2) / N
+    fig.show()
+    return fig
```

### Comparing `somata-0.2.1/somata/iterative_oscillator/iter_osc.py` & `somata-0.3.1/somata/iterative_oscillator/iter_osc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,175 +1,294 @@
-""" Author: Amanda Beck <ambeck@mit.edu> """
+"""
+Author: Amanda Beck <ambeck@mit.edu>
+        Mingjian He <mh105@mit.edu>
+"""
 
 from .helper_functions import *
 from ..basic_models import OscillatorModel as Osc
+from ..utils import estimate_r
 
 
 class IterativeOscillatorModel(object):
     """
     IterativeOscillatorModel is an object class containing fitted OscillatorModel objects
     from the iterative oscillator algorithm
     """
-    def __init__(self, y, fs, noise_start=None, ar_order=13, burg_flag=False, verbose=False):
+    def __init__(self, y, fs, estimate_R=False, noise_start=None, burg_flag=False, verbose=False):
         """
         Inputs:
             :param y: observed data
             :param fs: sampling frequency (Hz)
-            :param noise_start: frequency (Hz) above which there should be only white noise, no oscillation
-            :param ar_order: Order of autoregressive model used to model innovations / one-step prediction error
+            :param estimate_R: True will estimate empirical observation noise R
+            :param noise_start: frequency (Hz) above which white noise is assumed to estimate R
             :param burg_flag: True will use Burg algorithm to fit AR parameters instead of the default Yule-Walker
             :param verbose: print initial parameters
         """
         if noise_start is None:
             noise_start = fs / 2 - 20
             if noise_start <= 0:
                 noise_start = fs / 2 - 5
         assert noise_start > 0, 'Please redefine noise_start. Entered or calculated frequency is less than zero.'
 
         # initialize the first oscillator
-        init_params, scale_factor = initial_param(y, fs, noise_start, ar_order, burg_flag)
+        add_freq, add_radius, _, _, _, b = initialize_newosc(fs, y, ar_order=13, burg_flag=burg_flag)
+        R = estimate_r(y, fs, freq_cutoff=noise_start) if estimate_R else b
+        init_params = {'y': y, 'a': add_radius, 'freq': add_freq, 'sigma2': b, 'Fs': fs, 'R': R}
+
         if verbose:
             print('Noise starting frequency is %0.1f Hz' % noise_start)
             print('Initial oscillator parameters:')
             print(init_params)
 
         # populate instance attributes
-        # noinspection PyProtectedMember
-        self.y_original = Osc._must_be_row(Osc._process_constructor_input(y))  # make sure y is a 2D row vector
-        self.scale = scale_factor
-        self.ar_order = ar_order
         self.burg_flag = burg_flag
+        self.osc_range = None
+        self.freq_res = None
+        self.keep_param = ()
+
         self.added_osc = [Osc(**init_params)]
         self.fitted_osc = []
-        self.scaled_osc = []
-        self.AIC = []
-        self.ll = []
-        self.log_prior = []
-        self.all_params = []  # a list of lists containing Osc objects with only parameters (y dropped)
         self.priors = []
-        self.knee_index = []
-        self.Q_innov = []
+        self.all_params = []  # a list of lists containing Osc objects with only parameters (y dropped)
+        self.ll = []
+        self.ll_xre = []
+        self.AIC = []
+        self.knee_index = None
+        self.reiterated = False
 
-    def iterate(self, osc_range=7, freq_hp=3, R_hp=0.1, Q_hp=None, keep_param=(), R_sigma2='b', Q_sigma2='MLE',
-                no_priors=False, track_params=False, plot_innov=False, verbose=False):
+    def iterate(self, osc_range=7, freq_res=1, keep_param=(), reiterate=True, freq_hp=3, R_hp=0.1, Q_hp=None,
+                R_sigma2='b', Q_sigma2='MLE', no_priors=False, track_params=False, plot_innov=False, verbose=False):
         """
-        Apply Iterative Oscillator Algorithm
+        Iterative Oscillator Algorithm
 
         Reference:
             Beck, A. M., He, M., Gutierrez, R. G. & Purdon, P. L. (in prep)
 
             Matsuda & Komaki (2017). Time Series Decomposition into Oscillation
             Components and Phase Estimation. Journal of Neural Computation, 29, 332-367.
 
             Shumway, R. H., & Stoffer, D. S. (1982). An approach to time series
             smoothing and forecasting using the EM algorithm. Journal of time series
             analysis, 3(4), 253-264.
 
         Inputs:
         :param self: IterativeOscillatorModel class instance
         :param osc_range: maximum number of oscillators
+        :param freq_res: minimal oscillator frequency spacing/resolution when adding a new oscillator
+        :param keep_param: a tuple of strings for parameters to keep and not update
+        :param reiterate: whether to perform reiterations by sorting log-likelihood increases in descending order
         :param freq_hp: concentration hyperparameter in Von Mises Prior (freq_hp * data length)
         :param R_hp: hyperparameter in Inverse Gamma Prior determining weight on prior mode compared to MLE
         :param Q_hp: hyperparameter in Inverse Gamma Prior determining weight on prior mode compared to MLE
-        :param keep_param: a tuple of strings for parameters to keep and not update
         :param R_sigma2: determine prior mode for R, if None it will be noise variance from AR model
         :param Q_sigma2: determine prior mode for Q, if None it will be noise variance from AR model
         :param no_priors: override all other prior hyperparameters and proceed with no priors
         :param track_params: save parameters from EM iterations
         :param plot_innov: plot the innovations at each iteration
         :param verbose: print oscillator information during iterative search iterations
         """
-        # Copy the last oscillator so that updated parameters during iterations do not override it
-        o1 = self.added_osc[-1].copy()
+        # Store iteration settings as instance attributes
+        self.osc_range = osc_range
+        self.freq_res = freq_res
+        self.keep_param = keep_param
+
+        # Copy the first added oscillator to preserve its parameters
+        o1 = self.added_osc[0].copy()
 
         # Set up iteration variables
         start_add_osc = False
         innov_limit = None
-        self.Q_innov = [o1.R.copy()[0, 0]]
+        counter = 0
 
         # Begin iterations to search for more oscillators in the observed data
         while o1.ncomp < osc_range:
             if not start_add_osc:  # do EM learning on the initial oscillator first, don't add oscillators yet
-                b = o1.R.copy()[0, 0]
+                b = o1.R[0, 0]
                 start_add_osc = True
                 if verbose:
                     print('EM learning on the initial oscillator')
 
             else:  # add an oscillator
+                # find existing frequency
+                if abs(o1.freq[-1] - self.added_osc[-1].freq) >= self.freq_res:
+                    existing_freqs = list(o1.freq) + [x.freq[0] for x in self.added_osc[:-1]]
+                else:
+                    existing_freqs = list(o1.freq) + [x.freq[0] for x in self.added_osc]
+
                 # noinspection PyUnboundLocalVariable
-                add_freq, add_radius, all_freq, all_radii, a, b = initialize_newosc(o1.Fs, innovations,
-                                                                                    existing_freqs=None,
-                                                                                    ar_order=self.ar_order,
-                                                                                    burg_flag=self.burg_flag)
-                self.Q_innov.append(b)
+                add_freq, add_radius, _, _, a, b = initialize_newosc(
+                    o1.Fs, innovations, existing_freqs=existing_freqs, freq_res=self.freq_res,
+                    ar_order=self.osc_range * 2 - 1, burg_flag=self.burg_flag)
 
                 if verbose:
-                    print('AR: add freq: %0.2f Hz, add radius: %0.3f, add q: %0.3f' % (add_freq, add_radius, b))
+                    print('AR: add freq = %0.2f Hz, add radius = %0.3f, add sigma2 = %0.3f' % (add_freq, add_radius, b))
 
                 # plot the fitted oscillator from previous iteration and the innovation
                 if plot_innov:
-                    innov_limit, _ = innovations_plot(o1, o1.y, innovations, a, b, add_freq, ax_limit=innov_limit)
+                    innov_limit, _ = innovations_plot(o1, o1.y, innovations, a, b, add_freq, add_radius,
+                                                      plot_all_poles=True, ax_limit=innov_limit, counter=counter)
 
                 # construct an additional oscillator
                 o2 = Osc(a=add_radius, freq=add_freq, sigma2=b, Fs=o1.Fs)
-                self.added_osc.append(o2.copy(drop_y=True))
+                self.added_osc.append(o2)
                 o1.append(o2)  # add the additional oscillator to the existing oscillator instance
+                counter += 1  # accumulate iteration counter
 
             # Initialize priors for EM learning
-            input_params = {}
-            if R_hp is not None:
-                input_params.update({'R_hyperparameter': R_hp})
-            if Q_hp is not None:
-                input_params.update({'Q_hyperparameter': Q_hp})
-            if R_sigma2 is not None:
-                input_params.update({'R_sigma2': b if R_sigma2 == 'b' else R_sigma2})
-            if Q_sigma2 is not None:
-                # TODO: add the case to handle multiple Q_sigma2
-                input_params.update({'Q_sigma2': b if Q_sigma2 == 'b' else Q_sigma2})
-            if verbose:
-                print('Prior input parameters:')
-                print(input_params)
-
-            priors = None if no_priors else o1.initialize_priors(kappa=o1.ntime * freq_hp, **input_params)
+            if no_priors:
+                priors = None
+            else:
+                prior_params = {}
+                if R_hp is not None and R_sigma2 != 'MLE' and 'R' not in keep_param:
+                    prior_params.update({'R_hyperparameter': R_hp})
+                if Q_hp is not None and Q_sigma2 != 'MLE' and 'Q' not in keep_param:
+                    prior_params.update({'Q_hyperparameter': Q_hp})
+                if R_sigma2 is not None and 'R' not in keep_param:
+                    prior_params.update({'R_sigma2': b if R_sigma2 == 'b' else R_sigma2})
+                if Q_sigma2 is not None and 'Q' not in keep_param:
+                    # TODO: add the case to handle multiple Q_sigma2
+                    prior_params.update({'Q_sigma2': b if Q_sigma2 == 'b' else Q_sigma2})
+                if verbose:
+                    print('Prior input parameters:', prior_params)
+                priors = o1.initialize_priors(kappa=o1.ntime * freq_hp, **prior_params)
             self.priors.append(priors)
 
             # Run EM iterations
             em_params = []  # store the oscillator parameters throughout EM iterations
             for x in range(50):
-                _ = o1.m_estimate(**o1.dejong_filt_smooth(EM=True), priors=priors, keep_param=keep_param)
+                _ = o1.m_estimate(**o1.dejong_filt_smooth(EM=True), priors=priors, keep_param=self.keep_param)
                 if track_params:
                     em_params.append(o1.copy(drop_y=True))
             if track_params:
                 self.all_params.append(em_params)
 
             self.fitted_osc.append(o1.copy(drop_y=True))
 
             if verbose:
-                print('Oscillator %d completed' % o1.ncomp)
+                print('Iteration %d completed:' % counter)
                 print(o1)
 
-            # if plot_innov:
-            #     _ = o1.visualize_freq('theoretical')
-
             # Find the innovation spectrum
             innovations, ll = find_innovations(o1)
             self.ll.append(ll)
             self.AIC.append(aic_calc(o1, ll))  # compute AIC
 
-            # Store the parameters after scaling variance back to original y
-            scaled_o1 = o1.copy(drop_y=True)
-            scaled_o1.R *= self.scale
-            scaled_o1.sigma2 *= self.scale
-            scaled_o1.Q *= self.scale
-            scaled_o1.Q0 *= self.scale
-            self.scaled_osc.append(scaled_o1)
-
         # Find the knee_index for the selected model of fitted oscillators
         self.knee_index = get_knee(self.ll)
 
+        # Perform reiterations
+        if reiterate:
+            self.reiterate(track_params=track_params, plot_innov=plot_innov, verbose=verbose)
+
+    def reiterate(self, track_params=False, plot_innov=False, verbose=False):
+        """ Sort and re-add the oscillators in descending order of log-likelihood increase """
+        # Fast-forward to after fitting the first oscillator
+        o1 = self.fitted_osc[0].copy()
+        o1.y = self.added_osc[0].y.copy()  # add the observed data back in
+
+        # Fill in the instance attributes for the first fitted oscillator
+        added_osc_re = self.added_osc[:1]
+        fitted_osc_re = self.fitted_osc[:1]
+        priors_re = self.priors[:1]
+        all_params_re = [self.all_params[0]] if track_params else self.all_params[:1]
+        innovations, ll = find_innovations(o1)
+        ll_re = [ll]
+        AIC_re = [aic_calc(o1, ll)]
+
+        # Set up iteration variables
+        add_indices = np.diff(self.ll).argsort()[::-1] + 1
+        innov_limit = None
+        counter = 0
+
+        # Reiterate through all added oscillators
+        for add_idx in add_indices:
+            # look up the oscillator to be added next
+            o2 = self.added_osc[add_idx]
+
+            if verbose:
+                print('Re-iteration AR: add freq = %0.2f Hz, add radius = %0.3f, add sigma2 = %0.3f'
+                      % (o2.freq[0], o2.a[0], o2.sigma2[0]))
+
+            # plot the fitted oscillator from previous iteration and the innovation
+            if plot_innov:
+                a, b, _ = fit_ar(np.squeeze(innovations), self.osc_range * 2 - 1, self.burg_flag)
+                innov_limit, _ = innovations_plot(o1, o1.y, innovations, a, b, o2.freq[0], o2.a[0],
+                                                  plot_all_poles=True, ax_limit=innov_limit, counter=counter)
+
+            added_osc_re.append(o2)
+            o1.append(o2)  # add the additional oscillator to the existing oscillator instance
+            counter += 1  # accumulate iteration counter
+
+            # Initialize priors for EM learning
+            if self.priors[add_idx] is None:  # then no_priors was True during iterate()
+                priors = None
+            else:
+                prior_params = self.priors[add_idx][0].copy()
+                kappa = prior_params['vmp_param']['kappa']
+                del prior_params['vmp_param']
+                if verbose:
+                    print('Prior input parameters:', prior_params)
+                priors = o1.initialize_priors(kappa=kappa, **prior_params)
+            priors_re.append(priors)
+
+            # Run EM iterations
+            em_params = []  # store the oscillator parameters throughout EM iterations
+            for x in range(50):
+                _ = o1.m_estimate(**o1.dejong_filt_smooth(EM=True), priors=priors, keep_param=self.keep_param)
+                if track_params:
+                    em_params.append(o1.copy(drop_y=True))
+            if track_params:
+                all_params_re.append(em_params)
+
+            fitted_osc_re.append(o1.copy(drop_y=True))
+
+            if verbose:
+                print('Re-iteration %d completed:' % counter)
+                print(o1)
+
+            # Find the innovation spectrum
+            innovations, ll = find_innovations(o1)
+            ll_re.append(ll)
+            AIC_re.append(aic_calc(o1, ll))  # compute AIC
+
+        # Overwrite the instance attributes from iterate()
+        self.added_osc = added_osc_re
+        self.fitted_osc = fitted_osc_re
+        self.priors = priors_re
+        self.all_params = all_params_re
+        self.ll_xre = self.ll  # save the log likelihoods from before reiterate()
+        self.ll = ll_re  # overwrite the log likelihoods after reiterate()
+        self.AIC = AIC_re
+
+        # Find the new knee_index for the selected model of re-fitted oscillators
+        self.knee_index = get_knee(self.ll)  # knee replacement
+
+        # Update the reiterated flag
+        self.reiterated = True
+
+    def get_aperiodic(self, plot_innov=False):
+        """ Find the aperiodic component defined as prediction residual from the best model """
+        y = self.added_osc[0].y
+        osc = self.fitted_osc[self.knee_index]
+        innovations, _ = find_innovations(osc, y=y)
+
+        # Obtain the theoretical spectrum of a fitted AR model
+        a, b, _ = fit_ar(np.squeeze(innovations), self.osc_range * 2 - 1, self.burg_flag)
+        ar_psd, ar_hz = get_ar_psd(osc.Fs, a, b)
+
+        # Fit a straight line in semi-log space, i.e., log(PSD) against linear frequency (Hz)
+        from scipy import stats
+        slope, intercept, *_ = stats.linregress(ar_hz, 10 * np.log10(ar_psd))
+
+        if plot_innov:
+            _, fig = innovations_plot(osc, y, innovations, a, b, counter=self.knee_index)
+            plot_fit_line(fig, slope, intercept)
+
+        return innovations, (slope, intercept)
+
     def __repr__(self):
         """ Unambiguous and concise representation when calling IterativeOscillatorModel() """
         return 'IterOsc(' + str(len(self)) + ')<' + hex(id(self))[-4:] + '>'
 
     def __str__(self):
         """ Helpful information when calling print(IterativeOscillatorModel()) """
         print_str = "number of oscillators = %d\n " % len(self)
```

### Comparing `somata-0.2.1/somata/multitaper/multitaper_spectrogram_python.py` & `somata-0.3.1/somata/multitaper/multitaper_spectrogram_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from scipy.signal.windows import dpss
 from scipy.signal import detrend
 # Logistical Imports
 import warnings
 import timeit
 from joblib import Parallel, delayed, cpu_count
 # Visualization imports
+import colorcet  # this import is necessary to add rainbow colormap to matplotlib
 import matplotlib.pyplot as plt
-import librosa.display
 
 
 # MULTITAPER SPECTROGRAM #
 def multitaper_spectrogram(data, fs, frequency_range=None, time_bandwidth=5, num_tapers=None, window_params=None,
-                           min_nfft=0, detrend_opt='linear', multiprocess=True, n_jobs=None, weighting='unity',
-                           plot_on=False, clim_scale=True, verbose=False, xyflip=False):
+                           min_nfft=0, detrend_opt='linear', multiprocess=False, n_jobs=None, weighting='unity',
+                           plot_on=True, return_fig=False, clim_scale=True, verbose=True, xyflip=False):
     """ Compute multitaper spectrogram of timeseries data
     Usage:
     mt_spectrogram, stimes, sfreqs = multitaper_spectrogram(data, fs, frequency_range=None, time_bandwidth=5,
-                                                                   num_tapers=None, window_params=None, min_nfft=0,
-                                                                   detrend_opt='linear', multiprocess=False, cpus=False,
-                                                                    weighting='unity', plot_on=True, verbose=True,
-                                                                    xyflip=False):
+                                                            num_tapers=None, window_params=None, min_nfft=0,
+                                                            detrend_opt='linear', multiprocess=False, cpus=False,
+                                                            weighting='unity', plot_on=True, return_fig=False,
+                                                            clim_scale=True, verbose=True, xyflip=False):
         Arguments:
                 data (1d np.array): time series data -- required
                 fs (float): sampling frequency in Hz  -- required
                 frequency_range (list): 1x2 list - [<min frequency>, <max frequency>] (default: [0 nyquist])
                 time_bandwidth (float): time-half bandwidth product (window duration*half bandwidth of main lobe)
                                         (default: 5 Hz*s)
                 num_tapers (int): number of DPSS tapers to use (default: [will be computed
@@ -38,17 +38,18 @@
                                 (default: 0)
                 multiprocess (bool): Use multiprocessing to compute multitaper spectrogram (default: False)
                 n_jobs (int): Number of cpus to use if multiprocess = True (default: False). Note: if default is left
                             as None and multiprocess = True, the number of cpus used for multiprocessing will be
                             all available - 1.
                 weighting (str): weighting of tapers ('unity' (default), 'eigen', 'adapt');
                 plot_on (bool): plot results (default: True)
-                clim_scale (bool): automatically scale the colormap on the plotted spectrogram (default: true)
-                verbose (bool): display spectrogram properties (default: true)
-                xyflip (bool): transpose the mt_spectrogram output (default: false)
+                return_fig (bool): return plotted spectrogram (default: False)
+                clim_scale (bool): automatically scale the colormap on the plotted spectrogram (default: True)
+                verbose (bool): display spectrogram properties (default: True)
+                xyflip (bool): transpose the mt_spectrogram output (default: False)
         Returns:
                 mt_spectrogram (TxF np array): spectral power matrix
                 stimes (1xT np array): timepoints (s) in mt_spectrogram
                 sfreqs (1xF np array)L frequency values (Hz) in mt_spectrogram
 
         Example:
         In this example we create some chirp data and run the multitaper spectrogram on it.
@@ -62,35 +63,38 @@
             window_params = [4, 1]  # Window size is 4s with step size of 1s
             min_nfft = 0  # No minimum nfft
             detrend_opt = 'constant'  # detrend each window by subtracting the average
             multiprocess = True  # use multiprocessing
             cpus = 3  # use 3 cores in multiprocessing
             weighting = 'unity'  # weight each taper at 1
             plot_on = True  # plot spectrogram
+            return_fig = False  # do not return plotted spectrogram
             clim_scale = False # don't auto-scale the colormap
             verbose = True  # print extra info
             xyflip = False  # do not transpose spect output matrix
+
             # Generate sample chirp data
             t = np.arange(1/fs, 600, 1/fs)  # Create 10 min time array from 1/fs to 600 stepping by 1/fs
             f_start = 1  # Set chirp freq range min (Hz)
             f_end = 20  # Set chirp freq range max (Hz)
             data = chirp(t, f_start, t[-1], f_end, 'logarithmic')
             # Compute the multitaper spectrogram
             spect, stimes, sfreqs = multitaper_spectrogram(data, fs, frequency_range, time_bandwidth, num_tapers,
                                                            window_params, min_nfft, detrend_opt, multiprocess,
-                                                           cpus, weighting, plot_on, verbose, xyflip):
+                                                           cpus, weighting, plot_on, return_fig, clim_scale,
+                                                           verbose, xyflip):
 
         This code is companion to the paper:
         "Sleep Neurophysiological Dynamics Through the Lens of Multitaper Spectral Analysis"
            Michael J. Prerau, Ritchie E. Brown, Matt T. Bianchi, Jeffrey M. Ellenbogen, Patrick L. Purdon
            December 7, 2016 : 60-92
            DOI: 10.1152/physiol.00062.2015
          which should be cited for academic use of this code.
 
-         A full tutorial on the multitaper spectrogram can be found at:  #   https://www.sleepEEG.org/multitaper
+         A full tutorial on the multitaper spectrogram can be found at: # https://www.sleepEEG.org/multitaper
 
         Copyright 2021 Michael J. Prerau Laboratory. - https://www.sleepEEG.org
         Authors: Michael J. Prerau, Ph.D., Thomas Possidente, Mingjian He
 
   __________________________________________________________________________________________________________________
     """
 
@@ -103,15 +107,15 @@
 
     # Set up spectrogram parameters
     [window_idxs, stimes, sfreqs, freq_inds] = process_spectrogram_params(fs, nfft, frequency_range, window_start,
                                                                           winsize_samples)
     # Display spectrogram parameters
     if verbose:
         display_spectrogram_props(fs, time_bandwidth, num_tapers, [winsize_samples, winstep_samples], frequency_range,
-                                  detrend_opt)
+                                  nfft, detrend_opt)
 
     # Split data into segments and preallocate
     data_segments = data[window_idxs]
 
     # COMPUTE THE MULTITAPER SPECTROGRAM
     #     STEP 1: Compute DPSS tapers based on desired spectral properties
     #     STEP 2: Multiply the data segment by the DPSS Tapers
@@ -158,33 +162,44 @@
         mt_spectrogram = mt_spectrogram.T
 
     # End timer and get elapsed compute time
     toc = timeit.default_timer()
     if verbose:
         print("\n Multitaper compute time: " + "%.2f" % (toc - tic) + " seconds")
 
+    if all(mt_spectrogram.flatten() == 0):
+        print("\n Data was all zeros, no output")
+
     # Plot multitaper spectrogram
     if plot_on:
+        # convert from power to dB
+        spect_data = nanpow2db(mt_spectrogram)
 
-        # Eliminate bad data from colormap scaling
-        spect_data = mt_spectrogram
-        clim = np.percentile(spect_data, [5, 95])  # Scale colormap from 5th percentile to 95th
-
-        plt.figure(1, figsize=(10, 5))
-        librosa.display.specshow(nanpow2db(mt_spectrogram), x_axis='time', y_axis='linear',
-                                 x_coords=stimes, y_coords=sfreqs, shading='auto', cmap="jet")
-        plt.colorbar(label='Power (dB)')
-        plt.xlabel("Time (HH:MM:SS)")
-        plt.ylabel("Frequency (Hz)")
+        # Set x and y axes
+        dx = stimes[1] - stimes[0]
+        dy = sfreqs[1] - sfreqs[0]
+        extent = [stimes[0]-dx, stimes[-1]+dx, sfreqs[-1]+dy, sfreqs[0]-dy]
+
+        # Plot spectrogram
+        fig, ax = plt.subplots()
+        im = ax.imshow(spect_data, extent=extent, aspect='auto')
+        fig.colorbar(im, ax=ax, label='PSD (dB)', shrink=0.8)
+        ax.set_xlabel("Time (HH:MM:SS)")
+        ax.set_ylabel("Frequency (Hz)")
+        im.set_cmap(plt.cm.get_cmap('cet_rainbow4'))
+        ax.invert_yaxis()
+
+        # Scale colormap
         if clim_scale:
-            plt.clim(clim)  # actually change colorbar scale
-        plt.show()
+            clim = np.percentile(spect_data, [5, 98])  # from 5th percentile to 98th
+            im.set_clim(clim)  # actually change colorbar scale
 
-    if all(mt_spectrogram.flatten() == 0):
-        print("\n Data was all zeros, no output")
+        fig.show()
+        if return_fig:
+            return mt_spectrogram, stimes, sfreqs, (fig, ax)
 
     return mt_spectrogram, stimes, sfreqs
 
 
 # Helper Functions #
 
 # Process User Inputs #
@@ -340,37 +355,39 @@
     window_idxs = np.atleast_2d(window_start).T + np.arange(0, datawin_size, 1)
     window_idxs = window_idxs.astype(int)
 
     return [window_idxs, stimes, sfreqs, freq_inds]
 
 
 # DISPLAY SPECTROGRAM PROPERTIES
-def display_spectrogram_props(fs, time_bandwidth, num_tapers, data_window_params, frequency_range, detrend_opt):
+def display_spectrogram_props(fs, time_bandwidth, num_tapers, data_window_params, frequency_range, nfft, detrend_opt):
     """ Prints spectrogram properties
         Arguments:
             fs (float): sampling frequency in Hz  -- required
             time_bandwidth (float): time-half bandwidth product (window duration*1/2*frequency_resolution) -- required
             num_tapers (int): number of DPSS tapers to use -- required
             data_window_params (list): 1x2 list - [window length(s), window step size(s)] -- required
             frequency_range (list): 1x2 list - [<min frequency>, <max frequency>] -- required
-            detrend_opt (str): detrend data window ('linear' (default), 'constant', 'off')
+            nfft(float): number of fast fourier transform samples -- required
+            detrend_opt (str): detrend data window ('linear' (default), 'constant', 'off') -- required
         Returns:
             This function does not return anything
     """
 
     data_window_params = np.asarray(data_window_params) / fs
 
     # Print spectrogram properties
     print("Multitaper Spectrogram Properties: ")
     print('     Spectral Resolution: ' + str(2 * time_bandwidth / data_window_params[0]) + 'Hz')
     print('     Window Length: ' + str(data_window_params[0]) + 's')
     print('     Window Step: ' + str(data_window_params[1]) + 's')
     print('     Time Half-Bandwidth Product: ' + str(time_bandwidth))
     print('     Number of Tapers: ' + str(num_tapers))
     print('     Frequency Range: ' + str(frequency_range[0]) + "-" + str(frequency_range[1]) + 'Hz')
+    print('     NFFT: ' + str(nfft))
     print('     Detrend: ' + detrend_opt + '\n')
 
 
 # NANPOW2DB
 def nanpow2db(y):
     """ Power to dB conversion, setting bad values to nans
         Arguments:
@@ -423,14 +440,19 @@
 
     # If segment has all zeros, return vector of zeros
     if all(data_segment == 0):
         ret = np.empty(sum(freq_inds))
         ret.fill(0)
         return ret
 
+    if any(np.isnan(data_segment)):
+        ret = np.empty(sum(freq_inds))
+        ret.fill(np.nan)
+        return ret
+
     # Option to detrend data to remove low frequency DC component
     if detrend_opt != 'off':
         data_segment = detrend(data_segment, type=detrend_opt)
 
     # Multiply data by dpss tapers (STEP 2)
     tapered_data = np.multiply(np.mat(data_segment).T, np.mat(dpss_tapers.T))
 
@@ -458,18 +480,7 @@
 
     else:
         # eigenvalue or uniform weights
         mt_spectrum = np.dot(spower, wt)
         mt_spectrum = np.reshape(mt_spectrum, nfft)  # reshape to 1D
 
     return mt_spectrum[freq_inds]
-
-
-def fast_psd_multitaper(x, sfreq, freq_min, freq_max, bandwidth):
-    """ Fast multitaper PSD estimate with windowing """
-    window_length = min(x.size / sfreq, 10)  # max to 10s windows
-    time_bandwidth = bandwidth / 2 * window_length
-    spect, _, freq = multitaper_spectrogram(data=x, fs=sfreq, frequency_range=[freq_min, freq_max],
-                                            time_bandwidth=time_bandwidth,
-                                            window_params=[window_length, 1], detrend_opt='linear')
-    psd = np.mean(spect, 1) * sfreq  # scale back the normalization by sampling frequency
-    return psd, freq
```

### Comparing `somata-0.2.1/somata.egg-info/PKG-INFO` & `somata-0.3.1/somata.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somata
-Version: 0.2.1
+Version: 0.3.1
 Summary: State-space Oscillator Modeling And Time-series Analysis
 Home-page: https://github.com/mh105/somata
 Author: Mingjian He
 Author-email: mh105@mit.edu
 Keywords: state-space oscillator time-series
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -49,69 +49,78 @@
 * [Authors](#authors)
 * [Citation](#citation)
 * [License](#license)
 
 ---
 
 ## Requirements
-somata is built on `numpy` arrays for computations. `joblib` is used for multithreading. Additional dependencies include
-`matplotlib`, `scipy`, `tqdm`, `codetiming`, and `sorcery`. Full requirements for each release version will be updated
-under `install_requires` in the `setup.cfg` file. If the `environment.yml` file is used to create a new conda
-environment, all and only the required packages will be installed.
+[`somata`](https://pypi.org/project/somata/) is built on [`numpy`](https://numpy.org) arrays for computations. [`joblib`](https://joblib.readthedocs.io/en/stable/) is used for multithreading. 
+Additional dependencies include [`scipy`](https://scipy.org), [`matplotlib`](https://matplotlib.org), and [`spectrum`](https://pyspectrum.readthedocs.io/en/latest/index.html).
+An upcoming source localization module also requires [`pytorch`](https://pytorch.org) and [`MNE-python`](https://mne.tools/stable/index.html).
+Full requirements for each release version will be updated under 
+[`install_requires`](https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#platform-specific-dependencies) in the [`setup.cfg`](setup.cfg) file. 
+If the [`environment.yml`](environment.yml) file is used to [create a new conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file), 
+all and only the required packages will be installed.
 
 ## Install
 
 ```
 pip install somata
 ```
+_If the [`pytorch`](https://pytorch.org) dependency is not resolved successfully by [`pip`](https://pip.pypa.io/en/stable/) for your [OS](https://whatsmyos.com), 
+first [install `pytorch` manually](https://pytorch.org/get-started/locally/) in a [conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) that you wish to install [`somata`](https://pypi.org/project/somata/), 
+and then [execute the above line](https://packaging.python.org/en/latest/tutorials/installing-packages/#ensure-you-can-run-pip-from-the-command-line) to install [`somata`](https://pypi.org/project/somata/)._
 
 ### (For development only)
 
 - ### Fork this repo to personal git
     [How to: GitHub fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo)    
 
 - ### Clone forked copy to local computer
-    ``` git clone <forked copy ssh url> ```
+    [How to: GitHub clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)
 
 - ### Install conda
     [Recommended conda distribution: miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
-    _Apple silicon Mac: choose conda native to the ARM64 architecture instead of Intel x86_
+    _[Apple silicon Mac](https://support.apple.com/en-us/HT211814): choose conda native to the [ARM64 architecture](https://www.anaconda.com/blog/new-release-anaconda-distribution-now-supporting-m1) instead of [Intel x86](https://en.wikipedia.org/wiki/X86)._
 
 - ### Create a new conda environment
     ``` conda install mamba -n base -c conda-forge ```\
     ``` cd <repo root directory with environment.yml> ```\
     ``` mamba env create -f environment.yml ```\
-    ``` conda activate somata ```\
-    _You may also install somata in an existing environment by skipping this step._
+    ``` conda activate somata ```
 
-- ### Install somata as a package in editable mode
+    _You may also install `somata` in an [existing environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#using-pip-in-an-environment) by skipping this step._
+
+- ### Install somata as a package in development mode
     ``` cd <repo root directory with setup.py> ```\
     ``` pip install -e . ```
 
+    _[What is: Editable Installs](https://setuptools.pypa.io/en/latest/userguide/development_mode.html)_
+
 - ### Configure IDEs to use the conda environment
-    [How to: Configure an existing conda environment](https://www.jetbrains.com/help/pycharm/conda-support-creating-conda-virtual-environment.html)
+    [How to: Configure an existing conda environment](https://www.jetbrains.com/help/pycharm/conda-support-creating-conda-virtual-environment.html#existing-conda-environment)
 
 ---
 
 ## Basic state-space models
-Somata, much like a neuron body supported by dendrites, is built on a set of basic state-space models introduced as class objects.
+`somata`, much like a neuron body supported by dendrites, is built on a set of basic state-space models introduced as class objects.
 
 The motivations are to:
 - develop a standardized format to store model parameters of state-space equations
 - override Python dunder methods so `__repr__` and `__str__` return something useful
 - define arithmetic-like operations such as `A + B` and `A * B`
 - emulate `numpy.array()` operations including `.append()`
 - implement inference algorithms like Kalman filtering and parameter update (m-step) equations as callable class methods
 
-At present, and in the near future, somata will be focused on **time-invariant Gaussian linear dynamical systems**.
-This limit on models we consider simplifies basic models to avoid embedded classes such as `transition_model` and
-`observation_model`, at the cost of restricting somata to classical algorithms with only some extensions to
+At present, and in the near future, `somata` will be focused on **time-invariant Gaussian linear dynamical systems**.
+This limit on models we consider simplifies basic models to avoid nested classes such as `transition_model` and
+`observation_model`, at the cost of restricting `somata` to classical algorithms with only some extensions to
 Bayesian inference and learning. This is a deliberate choice to allow easier, faster, and cleaner applications of
-somata on neural data analysis, instead of to provide a full-fledged statistical inference package.
+`somata` in neural data analysis, instead of to provide a full-fledged statistical inference package.
 
 ---
 
 ### _class_ StateSpaceModel
 ```python
 somata.StateSpaceModel(components=None, F=None, Q=None, mu0=None, Q0=None, G=None, R=None, y=None, Fs=None)
 ```
@@ -472,45 +481,105 @@
 
 ### For more in-depth working examples with the basic models in somata
 Look at the demo script [basic_models_demo_01102022.py](examples/basic_models_demo_01102022.py) and execute the code line by line to get familiar with class objects and methods of somata basic models.
 
 ---
 
 ## Advanced neural oscillator methods
-1. [Oscillator Model Learning](#osc)
-2. [Iterative Oscillator Algorithm](#ioa)
+1. [Oscillator Model Learning](#1-oscillator-model-learning)
+2. [Phase Amplitude Coupling Estimation](#2-phase-amplitude-coupling-estimation)
+3. [Iterative Oscillator Algorithm](#3-iterative-oscillator-algorithm)
+4. [Switching State-Space Inference](#4-switching-state-space-inference)
+5. [Multi-channel Oscillator Component Analysis](#5-multi-channel-oscillator-component-analysis)
+6. [State-Space Event Related Potential](#6-state-space-event-related-potential)
+7. [Dynamic Source Localization](#7-dynamic-source-localization)
+
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">
+</picture>
+
+### 1. Oscillator Model Learning
+
+For fitting data with oscillator models, it boils down to three steps:
+  - Initialize an oscillator model object
+  - Perform state estimation, i.e., E-step
+  - Update model parameters, i.e., M-step
+
+Given some time series `data`, we can fit an oscillator to the data using the expectation-maximization (EM) algorithm.
+```python
+from somata.basic_models import OscillatorModel as Osc
+o1 = Osc(freq=1, Fs=100, y=data)  # create an oscillator object instance
+_ = [o1.m_estimate(**o1.kalman_filt_smooth(EM=True))for x in range(50)]  # run 50 steps of EM
+```
 
 ---
-1. ### Oscillator Model Learning <a name="osc"></a> [<img src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">](#osc)
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Missing-critical.svg?logo=Python">
+</picture>
+
+### 2. Phase Amplitude Coupling Estimation
+
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">
+</picture>
+
+### 3. Iterative Oscillator Algorithm
+
+For a well-commented example script, see [IterOsc_example.py](examples/IterOsc_example.py).
+
+_**N.B.:** We recommend downsampling to 120 Hz or less, depending on the oscillations present in your data. Highly oversampled data will make it more difficult to identify oscillatory components, increase the computational time, and could also introduce high frequency noise._
+
+One major goal of this method was to produce an algorithm that requires minimal user intervention, if any. This algorithm is designed to fit well automatically in most situations, but there will still be some data sets where it does not fit well without intervention. We recommend starting with the algorithm as is, but in the case of poor fitting, we suggest the following modifications:
+
+1. If the model does not choose the correct number of oscillations, we recommend looking at all fitted models and selecting the best fitting model based on other selection criteria or using your best judgement. You can also choose a subset of well-fitted oscillations and run `kalman_filt_smooth()` to estimate oscillations using those fitted parameters.
+
+2. This algorithm assumes stationary parameters, and therefore a stationary signal. Although the Kalman smoothing allows the model to work with some time-varying signal, the success of the method depends on the strength and duration of the signal components. The weaker and more brief the time-varying component is, the more poorly the model will capture it, if at all. We recommend decreasing the length of your window until you have a more stationary signal.
+
+When using this module, please cite the following [paper](https://www.biorxiv.org/content/10.1101/2022.10.30.514422):
+
+Beck, A. M., He, M., Gutierrez, R. G., & Purdon, P. L. (2022). An iterative search algorithm to identify oscillatory dynamics in neurophysiological time series. bioRxiv, 2022-10.
+
 ---
-2. ### Iterative Oscillator Algorithm <a name="ioa"></a> [<img src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">](#ioa)
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Functional-success.svg?logo=Python">
+</picture>
 
-**N.B.:** We recommend downsampling to 120 Hz or less, depending on the oscillations present in your data. Highly oversampled data will make it more difficult to identify oscillatory components, increase the computational time, and could also introduce high frequency noise.
+### 4. Switching State-Space Inference
 
-One major goal of this method was to produce an algorithm that required minimal user intervention, if any. We recommend starting with the algorithm as is, but in the case of poor fitting, we suggest the following alterations:
-1. If the pole initialized from the one-step prediction is between two oscillations, causing poor fitting of this oscillation as it attempts to explain multiple oscillations, we recommend increasing the order of the AR model used to approximate the OSPE. Increase in increments of two, which will allow additional pairs of complex poles.
+When using this module, please cite the following [paper](https://www.biorxiv.org/content/10.1101/2022.11.18.517120):
 
-2. Conversely to point 1, if the order of the AR model is too high then multiple pairs of roots will be attributed to the same oscillation, diluting the strength needed for each of them and possibly leading to none of them being selected as the strongest root in the iterative process to initialize the next oscillation, even though together they describe the strongest oscillation. This can be identified using the innovations plot with all of the AR roots plotted. In this case we recommend decreasing the AR order in increments of 2, to decrease the number of pairs of complex poles.
+He, M., Das, P., Hotan, G., & Purdon, P. L. (2022). Switching state-space modeling of neural signal dynamics. bioRxiv, 2022-11.
 
-3. If the initialization of the additional oscillations describes a single oscillation well, but the fitting of this oscillation attempts to explain multiple oscillations and causes poor fitting, we recommend increasing the concentration hyperparameter in the Von Mises prior. This will increase the weight on the initial frequency and stop the oscillation from shifting to explain other oscillations.
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Missing-critical.svg?logo=Python">
+</picture>
 
-4. If the model does not choose the correct number of oscillations, we recommend looking at all fitted models and selecting the best fitting model based on other selection criteria or using your best judgement. You can also choose a subset of well-fitted oscillations and run the kalman filter to estimate oscillations using those fitted parameters.
+### 5. Multi-channel Oscillator Component Analysis
 
-5. Note that this algorithm assumes a stationary signal, and therefore stationary parameters. Although the Kalman filtering allows some flexibility in this requirement, enabling the model to work on some time-varying signal, the success of the method depends on the strength and duration of the signal components. The weaker and more brief the time-varying component is, the more poorly the model will capture it, if it does at all. We recommend decreasing the length of your window until you have a more stationary signal.
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Missing-critical.svg?logo=Python">
+</picture>
 
-This algorithm is designed to fit well automatically in most situations, but there will still be some data sets where it does not fit well without intervention.
+### 6. State-Space Event Related Potential
 
-When using this module, please cite the following [paper](https://www.biorxiv.org/content/10.1101/2022.10.30.514422.abstract):
+---
+<picture>
+   <img align="right" src="https://img.shields.io/badge/Status-Missing-critical.svg?logo=Python">
+</picture>
 
-Beck, A. M., He, M., Gutierrez, R. G., & Purdon, P. L. (2022). An iterative search algorithm to identify oscillatory dynamics in neurophysiological time series. bioRxiv.
+### 7. Dynamic Source Localization
 
 ---
 
 ## Authors
 Mingjian He, Proloy Das, Amanda Beck, Patrick Purdon
 
 ## Citation
 Use different citation styles at: https://doi.org/10.5281/zenodo.7242130
 
 ## License
-SOMATA is licensed under the [BSD 3-Clause Clear license](https://spdx.org/licenses/BSD-3-Clause-Clear.html). \
-Copyright © 2022. All rights reserved.
+SOMATA is licensed under the [BSD 3-Clause Clear license](https://spdx.org/licenses/BSD-3-Clause-Clear.html).\
+Copyright © 2023. All rights reserved.
```

