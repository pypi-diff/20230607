# Comparing `tmp/hsmm_mvpy-0.1.0b0.tar.gz` & `tmp/hsmm_mvpy-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmm_mvpy-0.1.0b0.tar", last modified: Tue Jun  6 12:33:32 2023, max compression
+gzip compressed data, was "hsmm_mvpy-0.1.0b1.tar", last modified: Wed Jun  7 12:10:05 2023, max compression
```

## Comparing `hsmm_mvpy-0.1.0b0.tar` & `hsmm_mvpy-0.1.0b1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-06 12:33:32.710551 hsmm_mvpy-0.1.0b0/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b0/LICENSE.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    23787 2023-06-06 12:33:32.710551 hsmm_mvpy-0.1.0b0/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    21421 2023-06-06 10:06:52.000000 hsmm_mvpy-0.1.0b0/README.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      844 2023-06-06 12:33:16.000000 hsmm_mvpy-0.1.0b0/pyproject.toml
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-06 12:33:32.710551 hsmm_mvpy-0.1.0b0/setup.cfg
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-06 12:33:32.710551 hsmm_mvpy-0.1.0b0/src/
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-06 12:33:32.710551 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      171 2022-09-28 08:31:43.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/__init__.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    56649 2023-06-06 12:11:24.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/models.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    10494 2023-05-30 15:57:35.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/simulations.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    40133 2023-06-06 09:51:30.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/utils.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    21011 2023-06-06 10:51:18.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/visu.py
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-06 12:33:32.710551 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    23787 2023-06-06 12:33:32.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      343 2023-06-06 12:33:32.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-06 12:33:32.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       83 2023-06-06 12:33:32.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/requires.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-06 12:33:32.000000 hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/top_level.txt
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-07 12:10:05.863505 hsmm_mvpy-0.1.0b1/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b1/LICENSE.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    23839 2023-06-07 12:10:05.863505 hsmm_mvpy-0.1.0b1/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    21473 2023-06-06 12:45:29.000000 hsmm_mvpy-0.1.0b1/README.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      845 2023-06-07 12:09:30.000000 hsmm_mvpy-0.1.0b1/pyproject.toml
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-07 12:10:05.863505 hsmm_mvpy-0.1.0b1/setup.cfg
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-07 12:10:05.863505 hsmm_mvpy-0.1.0b1/src/
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-07 12:10:05.863505 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      171 2022-09-28 08:31:43.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/__init__.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    56703 2023-06-07 12:06:48.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/models.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    10494 2023-05-30 15:57:35.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/simulations.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    40133 2023-06-06 09:51:30.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/utils.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    21011 2023-06-06 10:51:18.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/visu.py
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-07 12:10:05.863505 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    23839 2023-06-07 12:10:05.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      343 2023-06-07 12:10:05.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-07 12:10:05.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       83 2023-06-07 12:10:05.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/requires.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-07 12:10:05.000000 hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/top_level.txt
```

### Comparing `hsmm_mvpy-0.1.0b0/LICENSE.md` & `hsmm_mvpy-0.1.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b0/PKG-INFO` & `hsmm_mvpy-0.1.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm_mvpy
-Version: 0.1.0b0
+Version: 0.1.0b1
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
         
@@ -53,23 +53,23 @@
 - Describing experimental effects based on a particular stage duration
 - Estimating the effect of trial-wise manipuations on the identified stages (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
 - Time-lock EEG signal to the onset of a given stage and perform classical ERPs or time-frequency analysis based on the onset of a new stage
 - And many more (e.g. evidence accumulation models on decision stage, classification based on the number of transition events in the signal,...)
 
 
 # Documentation
-**Important note** The current tutorials are based on the latest (unstable) version not yet available through _pip_, installing through github is therefore recommended.
+**Important note** The current tutorials are based on the latest (unstable) version not yet default in _pip_, installing through github is therefore recommended or specify the beta version when installing through _pip_: ```pip install hsmm-mvpy==0.1.0b0```
 
-The package is available through *pip* with the command ```pip install hsmm_mvpy```. 
+The package is available through *pip*. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
     $ conda create -n hmp 
     $ conda activate hmp
     $ conda install pip #if not already installed
-    $ pip install hsmm_mvpy
+    $ pip install hsmm-mvpy==0.1.0b0
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
     import hsmm_mvpy as hmp
 ```
```

### Comparing `hsmm_mvpy-0.1.0b0/README.md` & `hsmm_mvpy-0.1.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 - Describing experimental effects based on a particular stage duration
 - Estimating the effect of trial-wise manipuations on the identified stages (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
 - Time-lock EEG signal to the onset of a given stage and perform classical ERPs or time-frequency analysis based on the onset of a new stage
 - And many more (e.g. evidence accumulation models on decision stage, classification based on the number of transition events in the signal,...)
 
 
 # Documentation
-**Important note** The current tutorials are based on the latest (unstable) version not yet available through _pip_, installing through github is therefore recommended.
+**Important note** The current tutorials are based on the latest (unstable) version not yet default in _pip_, installing through github is therefore recommended or specify the beta version when installing through _pip_: ```pip install hsmm-mvpy==0.1.0b0```
 
-The package is available through *pip* with the command ```pip install hsmm_mvpy```. 
+The package is available through *pip*. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
     $ conda create -n hmp 
     $ conda activate hmp
     $ conda install pip #if not already installed
-    $ pip install hsmm_mvpy
+    $ pip install hsmm-mvpy==0.1.0b0
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
     import hsmm_mvpy as hmp
 ```
```

### Comparing `hsmm_mvpy-0.1.0b0/pyproject.toml` & `hsmm_mvpy-0.1.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "hsmm_mvpy"
-version = "0.1.0-beta"
+version = "0.1.0-beta1"
 authors = [
   { name="Gabriel Weindel", email="gabriel.weindel@gmail.com" },
   { name="Leendert van Maanen", email="e@mail.com" },
   { name="Jelmer Borst", email="e@mail.com" },
 ]
 description = "Package for fitting Hidden Semi-Markov Models to electro-encephalographic data"
 readme = "README.md"
```

### Comparing `hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/models.py` & `hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -907,15 +907,15 @@
         pars_accepted, mags_accepted = pars.copy(), mags.copy()
         pars_prop = pars_accepted[:n_events+2].copy()#cumulative
         pars_prop[n_events,1] = step*j/self.shape
         last_stage = end/self.shape - np.sum(pars_prop[:n_events+1,1])
         pars_prop[n_events+1,1] = last_stage
         while last_stage*self.shape > self.location+step:
             prev_n_events, prev_lkh, prev_time = n_events, lkh, time
-            mags_prop = mags_accepted[:n_events+1].copy()
+            mags_prop = mags[:n_events+1].copy()
             lkh, mags[:n_events+1], pars[:n_events+2], _ = \
                 self.EM(n_events+1, mags_prop, pars_prop.copy(), 1, [], [])
             diffs = np.diff(mags[:n_events+1], axis=0)
             if np.all(np.any(np.abs(diffs) > threshold, axis=1)):
                 n_events += 1
                 pars_accepted = pars[:n_events+2].copy()
                 mags_accepted = mags[:n_events+2].copy()
@@ -926,21 +926,24 @@
             if trace:
                 all_mags_prop.append(mags_prop.copy())
                 all_pars_prop.append(pars_prop.copy())
                 all_mags.append(mags_accepted[:n_events].copy())
                 all_pars.append(pars_accepted[:n_events+1].copy())
                 all_diffs.append(diffs)
             j += 1
-            pars_prop = pars_accepted[:n_events+2].copy()#cumulative
+            pars_prop = pars[:n_events+2].copy()#cumulative
             pars_prop[n_events,1] = step*j/self.shape
             last_stage = end/self.shape - np.sum(pars_prop[:n_events+1,1])
             pars_prop[n_events+1,1] = last_stage
             time = np.sum(pars_prop[:n_events,1])*self.shape + \
                 self.location*n_events + step*j/self.shape
-            pbar.update(int(np.round(time-prev_time+1)))
+            try:
+                pbar.update(int(np.round(time-prev_time+1)))
+            except:
+                pbar.update(1)
         # pbar.update(int(np.round(end-prev_time)+self.location+step))
         mags = mags_accepted[:n_events, :]
         pars = pars_accepted[:n_events+1, :]
         if n_events > 1: 
             fit = self.fit_single(n_events, parameters=pars, magnitudes=mags, verbose=verbose)
         else:
             warn('Failed to find more than two stages, returning 2 stage model with default starting values')
```

### Comparing `hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/simulations.py` & `hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/simulations.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/utils.py` & `hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/utils.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b0/src/hsmm_mvpy/visu.py` & `hsmm_mvpy-0.1.0b1/src/hsmm_mvpy/visu.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b0/src/hsmm_mvpy.egg-info/PKG-INFO` & `hsmm_mvpy-0.1.0b1/src/hsmm_mvpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm-mvpy
-Version: 0.1.0b0
+Version: 0.1.0b1
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
         
@@ -53,23 +53,23 @@
 - Describing experimental effects based on a particular stage duration
 - Estimating the effect of trial-wise manipuations on the identified stages (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
 - Time-lock EEG signal to the onset of a given stage and perform classical ERPs or time-frequency analysis based on the onset of a new stage
 - And many more (e.g. evidence accumulation models on decision stage, classification based on the number of transition events in the signal,...)
 
 
 # Documentation
-**Important note** The current tutorials are based on the latest (unstable) version not yet available through _pip_, installing through github is therefore recommended.
+**Important note** The current tutorials are based on the latest (unstable) version not yet default in _pip_, installing through github is therefore recommended or specify the beta version when installing through _pip_: ```pip install hsmm-mvpy==0.1.0b0```
 
-The package is available through *pip* with the command ```pip install hsmm_mvpy```. 
+The package is available through *pip*. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
     $ conda create -n hmp 
     $ conda activate hmp
     $ conda install pip #if not already installed
-    $ pip install hsmm_mvpy
+    $ pip install hsmm-mvpy==0.1.0b0
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
     import hsmm_mvpy as hmp
 ```
```

