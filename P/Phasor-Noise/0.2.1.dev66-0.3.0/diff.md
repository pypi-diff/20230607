# Comparing `tmp/Phasor Noise-0.2.1.dev66.tar.gz` & `tmp/Phasor Noise-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Phasor Noise-0.2.1.dev66.tar", last modified: Tue May 23 19:07:19 2023, max compression
+gzip compressed data, was "Phasor Noise-0.3.0.tar", last modified: Wed Jun  7 16:47:52 2023, max compression
```

## Comparing `Phasor Noise-0.2.1.dev66.tar` & `Phasor Noise-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.458249 Phasor Noise-0.2.1.dev66/
--rw-rw-rw-   0        0        0      284 2023-05-23 19:07:18.000000 Phasor Noise-0.2.1.dev66/AUTHORS
--rw-rw-rw-   0        0        0    35869 2023-05-23 18:50:34.000000 Phasor Noise-0.2.1.dev66/LICENSE
--rw-rw-rw-   0        0        0      176 2023-05-23 18:54:52.000000 Phasor Noise-0.2.1.dev66/Makefile
--rw-rw-rw-   0        0        0     1125 2023-05-23 19:07:19.462253 Phasor Noise-0.2.1.dev66/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.376803 Phasor Noise-0.2.1.dev66/docs/
--rw-rw-rw-   0        0        0      603 2023-05-23 18:53:08.000000 Phasor Noise-0.2.1.dev66/docs/Makefile
--rw-rw-rw-   0        0        0        0 2023-05-23 18:53:08.000000 Phasor Noise-0.2.1.dev66/docs/README.rst
--rwxrwxrwx   0        0        0      827 2023-05-23 18:53:08.000000 Phasor Noise-0.2.1.dev66/docs/make.bat
--rw-rw-rw-   0        0        0       24 2023-05-23 18:53:08.000000 Phasor Noise-0.2.1.dev66/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.384825 Phasor Noise-0.2.1.dev66/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.384825 Phasor Noise-0.2.1.dev66/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.393113 Phasor Noise-0.2.1.dev66/docs/source/api/GUI/
--rw-rw-rw-   0        0        0      128 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/docs/source/api/GUI/index.rst
--rw-rw-rw-   0        0        0      125 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/docs/source/api/GUI/menu.rst
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.393113 Phasor Noise-0.2.1.dev66/docs/source/api/analysis/
--rw-rw-rw-   0        0        0      174 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/docs/source/api/analysis/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.397113 Phasor Noise-0.2.1.dev66/docs/source/api/generator/
--rw-rw-rw-   0        0        0      190 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/docs/source/api/generator/index.rst
--rw-rw-rw-   0        0        0      232 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/docs/source/api/index.rst
--rw-rw-rw-   0        0        0     9197 2023-05-23 19:02:19.000000 Phasor Noise-0.2.1.dev66/docs/source/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.405114 Phasor Noise-0.2.1.dev66/docs/source/getting_started/
--rw-rw-rw-   0        0        0      196 2023-05-23 18:53:08.000000 Phasor Noise-0.2.1.dev66/docs/source/getting_started/index.rst
--rw-rw-rw-   0        0        0      193 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/docs/source/getting_started/installation.rst
--rw-rw-rw-   0        0        0      668 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.410456 Phasor Noise-0.2.1.dev66/docs/source/user_guide/
--rw-rw-rw-   0        0        0       99 2023-05-23 18:53:08.000000 Phasor Noise-0.2.1.dev66/docs/source/user_guide/index.rst
--rw-rw-rw-   0        0        0       89 2023-05-23 18:53:08.000000 Phasor Noise-0.2.1.dev66/requirements.txt
--rw-rw-rw-   0        0        0      637 2023-05-23 19:07:19.465278 Phasor Noise-0.2.1.dev66/setup.cfg
--rw-rw-rw-   0        0        0      489 2023-05-23 19:03:51.000000 Phasor Noise-0.2.1.dev66/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.344095 Phasor Noise-0.2.1.dev66/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.454252 Phasor Noise-0.2.1.dev66/src/Phasor_Noise.egg-info/
--rw-rw-rw-   0        0        0     1125 2023-05-23 19:07:18.000000 Phasor Noise-0.2.1.dev66/src/Phasor_Noise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1128 2023-05-23 19:07:19.000000 Phasor Noise-0.2.1.dev66/src/Phasor_Noise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 19:07:18.000000 Phasor Noise-0.2.1.dev66/src/Phasor_Noise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 21:01:55.000000 Phasor Noise-0.2.1.dev66/src/Phasor_Noise.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-05-23 19:07:18.000000 Phasor Noise-0.2.1.dev66/src/Phasor_Noise.egg-info/pbr.json
--rw-rw-rw-   0        0        0       86 2023-05-23 19:07:18.000000 Phasor Noise-0.2.1.dev66/src/Phasor_Noise.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-23 19:07:18.000000 Phasor Noise-0.2.1.dev66/src/Phasor_Noise.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.412826 Phasor Noise-0.2.1.dev66/src/phasor_noise/
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.420971 Phasor Noise-0.2.1.dev66/src/phasor_noise/GUI/
--rw-rw-rw-   0        0        0    22629 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/src/phasor_noise/GUI/__init__.py
--rw-rw-rw-   0        0        0      185 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/src/phasor_noise/GUI/directory.py
--rw-rw-rw-   0        0        0     1436 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/src/phasor_noise/GUI/menu.py
--rw-rw-rw-   0        0        0      234 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/src/phasor_noise/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.420971 Phasor Noise-0.2.1.dev66/src/phasor_noise/analysis/
--rw-rw-rw-   0        0        0     1139 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/src/phasor_noise/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:07:19.428024 Phasor Noise-0.2.1.dev66/src/phasor_noise/generator/
--rw-rw-rw-   0        0        0     5325 2023-05-23 18:53:09.000000 Phasor Noise-0.2.1.dev66/src/phasor_noise/generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.896189 Phasor Noise-0.3.0/
+-rw-rw-rw-   0        0        0      284 2023-06-07 16:47:52.000000 Phasor Noise-0.3.0/AUTHORS
+-rw-rw-rw-   0        0        0    35869 2023-05-23 18:50:34.000000 Phasor Noise-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-06-07 16:45:25.000000 Phasor Noise-0.3.0/Makefile
+-rw-rw-rw-   0        0        0     1832 2023-06-07 16:47:52.900197 Phasor Noise-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1342 2023-06-07 16:47:28.000000 Phasor Noise-0.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.839782 Phasor Noise-0.3.0/docs/
+-rw-rw-rw-   0        0        0      603 2023-05-23 18:53:08.000000 Phasor Noise-0.3.0/docs/Makefile
+-rw-rw-rw-   0        0        0        0 2023-05-23 18:53:08.000000 Phasor Noise-0.3.0/docs/README.rst
+-rwxrwxrwx   0        0        0      827 2023-05-23 18:53:08.000000 Phasor Noise-0.3.0/docs/make.bat
+-rw-rw-rw-   0        0        0       24 2023-05-23 18:53:08.000000 Phasor Noise-0.3.0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.847799 Phasor Noise-0.3.0/docs/source/
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.851892 Phasor Noise-0.3.0/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.855801 Phasor Noise-0.3.0/docs/source/api/GUI/
+-rw-rw-rw-   0        0        0      128 2023-05-23 18:53:09.000000 Phasor Noise-0.3.0/docs/source/api/GUI/index.rst
+-rw-rw-rw-   0        0        0      125 2023-05-23 18:53:09.000000 Phasor Noise-0.3.0/docs/source/api/GUI/menu.rst
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.859795 Phasor Noise-0.3.0/docs/source/api/analysis/
+-rw-rw-rw-   0        0        0      174 2023-05-23 18:53:09.000000 Phasor Noise-0.3.0/docs/source/api/analysis/index.rst
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.863581 Phasor Noise-0.3.0/docs/source/api/generator/
+-rw-rw-rw-   0        0        0      190 2023-05-23 18:53:09.000000 Phasor Noise-0.3.0/docs/source/api/generator/index.rst
+-rw-rw-rw-   0        0        0      232 2023-05-23 18:53:09.000000 Phasor Noise-0.3.0/docs/source/api/index.rst
+-rw-rw-rw-   0        0        0     9197 2023-05-23 19:02:19.000000 Phasor Noise-0.3.0/docs/source/conf.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.867601 Phasor Noise-0.3.0/docs/source/getting_started/
+-rw-rw-rw-   0        0        0      196 2023-05-23 18:53:08.000000 Phasor Noise-0.3.0/docs/source/getting_started/index.rst
+-rw-rw-rw-   0        0        0      193 2023-05-23 18:53:09.000000 Phasor Noise-0.3.0/docs/source/getting_started/installation.rst
+-rw-rw-rw-   0        0        0      668 2023-05-23 18:53:09.000000 Phasor Noise-0.3.0/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.867601 Phasor Noise-0.3.0/docs/source/user_guide/
+-rw-rw-rw-   0        0        0       99 2023-05-23 18:53:08.000000 Phasor Noise-0.3.0/docs/source/user_guide/index.rst
+-rw-rw-rw-   0        0        0       89 2023-05-23 18:53:08.000000 Phasor Noise-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0      728 2023-06-07 16:47:52.900197 Phasor Noise-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      183 2023-06-07 16:38:57.000000 Phasor Noise-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.814884 Phasor Noise-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.896189 Phasor Noise-0.3.0/src/Phasor_Noise.egg-info/
+-rw-rw-rw-   0        0        0     1832 2023-06-07 16:47:52.000000 Phasor Noise-0.3.0/src/Phasor_Noise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1171 2023-06-07 16:47:52.000000 Phasor Noise-0.3.0/src/Phasor_Noise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 16:47:52.000000 Phasor Noise-0.3.0/src/Phasor_Noise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-07 16:47:52.000000 Phasor Noise-0.3.0/src/Phasor_Noise.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 21:01:55.000000 Phasor Noise-0.3.0/src/Phasor_Noise.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-06-07 16:47:52.000000 Phasor Noise-0.3.0/src/Phasor_Noise.egg-info/pbr.json
+-rw-rw-rw-   0        0        0       86 2023-06-07 16:47:52.000000 Phasor Noise-0.3.0/src/Phasor_Noise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-07 16:47:52.000000 Phasor Noise-0.3.0/src/Phasor_Noise.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.871768 Phasor Noise-0.3.0/src/phasor_noise/
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.873464 Phasor Noise-0.3.0/src/phasor_noise/GUI/
+-rw-rw-rw-   0        0        0    22669 2023-06-07 16:38:57.000000 Phasor Noise-0.3.0/src/phasor_noise/GUI/__init__.py
+-rw-rw-rw-   0        0        0      385 2023-06-07 16:38:57.000000 Phasor Noise-0.3.0/src/phasor_noise/GUI/directory.py
+-rw-rw-rw-   0        0        0     1436 2023-05-23 18:53:09.000000 Phasor Noise-0.3.0/src/phasor_noise/GUI/menu.py
+-rw-rw-rw-   0        0        0      236 2023-06-07 16:38:57.000000 Phasor Noise-0.3.0/src/phasor_noise/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.873464 Phasor Noise-0.3.0/src/phasor_noise/analysis/
+-rw-rw-rw-   0        0        0     1139 2023-05-23 18:53:09.000000 Phasor Noise-0.3.0/src/phasor_noise/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:47:52.873464 Phasor Noise-0.3.0/src/phasor_noise/generator/
+-rw-rw-rw-   0        0        0     5325 2023-05-23 18:53:09.000000 Phasor Noise-0.3.0/src/phasor_noise/generator/__init__.py
```

### Comparing `Phasor Noise-0.2.1.dev66/LICENSE` & `Phasor Noise-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Phasor Noise-0.2.1.dev66/docs/Makefile` & `Phasor Noise-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Phasor Noise-0.2.1.dev66/docs/make.bat` & `Phasor Noise-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Phasor Noise-0.2.1.dev66/docs/source/conf.py` & `Phasor Noise-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `Phasor Noise-0.2.1.dev66/docs/source/index.rst` & `Phasor Noise-0.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `Phasor Noise-0.2.1.dev66/src/Phasor_Noise.egg-info/PKG-INFO` & `Phasor Noise-0.3.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,30 @@
-Metadata-Version: 2.1
-Name: Phasor-Noise
-Version: 0.2.1.dev66
-Home-page: https://github.com/etachouzin/phasor_noise
-Author: Alexis Le Meur, Etienne Tachouzin, Paul Martin, Guillaume Hisleur, Paul Bedrossian
-Author-email: phasor_noise_dev@outlook.fr
-Maintainer: Alexis Le Meur, Etienne Tachouzin, Paul Martin, Guillaume Hisleur, Paul Bedrossian
-Maintainer-email: phasor_noise_dev@outlook.fr
-License: GNU
-Keywords: phasor_noise,generator
-License-File: LICENSE
-License-File: AUTHORS
+.. _`Procedural Phasor Noise`: https://hal.science/hal-02118508/file/ProceduralPhasorNoise.pdf
+
+|GPL| |Update| |PyPI|  |HAL|
+
+.. |GPL| image:: https://img.shields.io/github/license/etachouzin/phasor_noise?color=blue
+   :alt: GPL
+
+.. |Update| image:: https://img.shields.io/github/last-commit/etachouzin/phasor_noise
+   :alt: GitHub last commit
+
+.. |PyPI| image:: https://img.shields.io/static/v1?logo=pypi&message=PyPI&label=&color=yellow
+   :target: https://pypi.org/project/Phasor-Noise/
+   :alt: PyPI
+
+.. |HAL| image:: https://hal.science/assets/img/hal-logo-header.png
+   :target: https://hal.science/
+   :alt: HAL
+   :width: 20pt
 
 About The Project
 ------------------
 We created a Phasor noise generator with a graphical interface to visualize how the different parameters affect the noise created.
+We created it with this study `Procedural Phasor Noise`_
 
 Installation
 -------------
 
 1. Install from PyPI
 
 .. code:: console
@@ -43,8 +50,7 @@
 Authors
 -----------
 * Alexis Le Meur
 * Etienne Tachouzin
 * Paul Martin
 * Guillaume Hisleur
 * Paul Bedrossian
-
```

### Comparing `Phasor Noise-0.2.1.dev66/src/Phasor_Noise.egg-info/SOURCES.txt` & `Phasor Noise-0.3.0/src/Phasor_Noise.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/phasor_noise/GUI/directory.py
 src/phasor_noise/GUI/menu.py
 src/phasor_noise/analysis/__init__.py
 src/phasor_noise/generator/__init__.py
 src/Phasor_Noise.egg-info/PKG-INFO
 src/Phasor_Noise.egg-info/SOURCES.txt
 src/Phasor_Noise.egg-info/dependency_links.txt
+src/Phasor_Noise.egg-info/entry_points.txt
 src/Phasor_Noise.egg-info/not-zip-safe
 src/Phasor_Noise.egg-info/pbr.json
 src/Phasor_Noise.egg-info/requires.txt
 src/Phasor_Noise.egg-info/top_level.txt
 src/phasor_noise/__init__.py
 src/phasor_noise/GUI/__init__.py
 src/phasor_noise/GUI/directory.py
```

### Comparing `Phasor Noise-0.2.1.dev66/src/phasor_noise/GUI/__init__.py` & `Phasor Noise-0.3.0/src/phasor_noise/GUI/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,28 +44,28 @@
             "min_freq": self.img_freq_min.get(),
             "max_freq": self.img_freq_max.get(),
             "min_angle": self.img_angle_min.get(),
             "max_angle": self.img_angle_max.get(),
             "min_bandwidth": self.img_bandwidth_min.get(),
             "max_bandwidth": self.img_bandwidth_max.get()
         }
-        config_file = open(f"{config_directory}/config.json", 'w')
+        config_file = open(f"{config_directory()}/config.json", 'w')
         json.dump(new_config, config_file)
 
     def reload(self):
         """
         Reload the page
         """
         self.page.destroy()
-        path = f"{config_directory}/config.json"
+        path = f"{config_directory()}/config.json"
         if os.path.exists(path):
-            config_file = open(f"{config_directory}/config.json", "r")
+            config_file = open(f"{config_directory()}/config.json", "r")
             config = json.load(config_file)
         else:
-            config_file = open(f"{config_directory}/config.json", "w")
+            config_file = open(f"{config_directory()}/config.json", "w")
             config = {"x": "100", "y": "100", "nb_ker": "10", "min_freq": "1", "max_freq": "1", "min_angle": "-1.57",
                       "max_angle": "1.57", "min_bandwidth": "0.1", "max_bandwidth": "0.1"}
             json.dump(config, config_file)
         self.config = config
         self.load_page()
 
     def load_page(self):
@@ -274,52 +274,52 @@
         Show image
         """
         try:
             self.visu_img.delete(self.noise)
         except:
             pass
         try:
-            img = Image.open(f"{images_directory}/noise.png")
+            img = Image.open(f"{images_directory()}/noise.png")
             img.thumbnail((500, 500), Image.ANTIALIAS)
-            img.save(f"{images_directory}/noise_reshape.png")
-            self.img = ImageTk.PhotoImage(Image.open(f"{images_directory}/noise_reshape.png"))
+            img.save(f"{images_directory()}/noise_reshape.png")
+            self.img = ImageTk.PhotoImage(Image.open(f"{images_directory()}/noise_reshape.png"))
             self.noise = self.visu_img.create_image(0, 0, image=self.img, anchor="nw", tags="IMG")
         except:
             self.console_text.set("Générer d'abord un nouveau bruit !")
 
     def visu_mode_psd(self):
         """
         Show power spectral density
         """
         try:
             self.visu_img.delete(self.noise)
         except:
             pass
         try:
-            img = Image.open(f"{images_directory}/noise_psd.png")
+            img = Image.open(f"{images_directory()}/noise_psd.png")
             img.thumbnail((500, 500), Image.ANTIALIAS)
-            img.save(f"{images_directory}/noise_psd_reshape.png")
-            self.img = ImageTk.PhotoImage(Image.open(f"{images_directory}/noise_psd_reshape.png"))
+            img.save(f"{images_directory()}/noise_psd_reshape.png")
+            self.img = ImageTk.PhotoImage(Image.open(f"{images_directory()}/noise_psd_reshape.png"))
             self.noise = self.visu_img.create_image(0, 0, image=self.img, anchor="nw", tags="IMG")
         except:
             self.console_text.set("Générer d'abord un nouveau bruit !")
 
     def visu_mode_hist(self):
         """
         Show histogram
         """
         try:
             self.visu_img.delete(self.noise)
         except:
             pass
         try:
-            img = Image.open(f"{images_directory}/noise_hist.png")
+            img = Image.open(f"{images_directory()}/noise_hist.png")
             img.thumbnail((500, 500), Image.ANTIALIAS)
-            img.save(f"{images_directory}/noise_hist_reshape.png")
-            self.img = ImageTk.PhotoImage(Image.open(f"{images_directory}/noise_hist_reshape.png"))
+            img.save(f"{images_directory()}/noise_hist_reshape.png")
+            self.img = ImageTk.PhotoImage(Image.open(f"{images_directory()}/noise_hist_reshape.png"))
             self.noise = self.visu_img.create_image(0, 0, image=self.img, anchor="nw", tags="IMG")
         except:
             self.console_text.set("Générer d'abord un nouveau bruit !")
 
     def return_menu(self):
         """
         Menu
@@ -401,31 +401,31 @@
                     plt.plot(kernel[0][0], kernel[0][1], color="green", marker="o")
                     plt.arrow(kernel[0][0], kernel[0][1], kernel[1][0] * 5, kernel[1][1] * 5, width=1, head_width=2,
                               head_length=2, color="red")
             mean = analysis.mean(self.results[0])
             std_gap = analysis.std_gap(self.results[0])
             self.console_text.set(
                 f"Le bruit à bien été créé en {self.results[1] / 10 ** 6} ms ! \n Moyenne: {mean} \n Ecart-type: {std_gap}")
-            plt.savefig(f"{images_directory}/noise.png", bbox_inches='tight')
+            plt.savefig(f"{images_directory()}/noise.png", bbox_inches='tight')
             plt.close()
 
             mag = analysis.PSD(np.array(self.results[0]))
             plt.contourf(X, Y, mag, cmap="Greys_r")
             plt.axis('off')
             plt.colorbar()
-            plt.savefig(f"{images_directory}/noise_psd.png", bbox_inches='tight')
+            plt.savefig(f"{images_directory()}/noise_psd.png", bbox_inches='tight')
             plt.close()
 
             hist = exposure.histogram(np.array(self.results[0]))
             plt.plot(hist[1], hist[0])
 
-            plt.savefig(f"{images_directory}/noise_hist.png", bbox_inches='tight')
+            plt.savefig(f"{images_directory()}/noise_hist.png", bbox_inches='tight')
             self.visu_mode_img()
 
-            plt.savefig(f"{images_directory}/noise_hist.png", bbox_inches='tight')
+            plt.savefig(f"{images_directory()}/noise_hist.png", bbox_inches='tight')
             self.visu_mode_img()
 
         elif self.gen_mode == "Numpy":
             X = np.arange(0, self.size[0])
             Y = np.arange(0, self.size[1])
             X, Y = np.meshgrid(X, Y)
             self.results = generator.apply_noise_numpy(X, Y, deepcopy(self.kernels),
@@ -438,28 +438,28 @@
                     plt.plot(kernel[0][0], kernel[0][1], color="green", marker="o")
                     plt.arrow(kernel[0][0], kernel[0][1], kernel[1][0] * 5, kernel[1][1] * 5, width=1, head_width=2,
                               head_length=2, color="red")
             mean = analysis.mean(self.results[0])
             std_gap = analysis.std_gap(self.results[0])
             self.console_text.set(
                 f"Le bruit à bien été créé en {self.results[1] / 10 ** 6} ms !\n Moyenne: {mean}\nEcart-type: {std_gap}")
-            plt.savefig(f"{images_directory}/noise.png", bbox_inches='tight')
+            plt.savefig(f"{images_directory()}/noise.png", bbox_inches='tight')
             plt.close()
 
             mag = analysis.PSD(np.array(self.results[0]))
             plt.contourf(X, Y, mag, cmap='Greys')
             plt.axis('off')
             plt.colorbar()
-            plt.savefig(f"{images_directory}/noise_psd.png", bbox_inches='tight')
+            plt.savefig(f"{images_directory()}/noise_psd.png", bbox_inches='tight')
             plt.close()
 
             hist = exposure.histogram(np.array(self.results[0]))
             plt.plot(hist[1], hist[0])
 
-            plt.savefig(f"{images_directory}/noise_hist.png", bbox_inches='tight')
+            plt.savefig(f"{images_directory()}/noise_hist.png", bbox_inches='tight')
             self.visu_mode_img()
 
         plt.close()
 
     def one_noise_mode(self):
         """
         One noise mode
```

### Comparing `Phasor Noise-0.2.1.dev66/src/phasor_noise/GUI/menu.py` & `Phasor Noise-0.3.0/src/phasor_noise/GUI/menu.py`

 * *Files identical despite different names*

### Comparing `Phasor Noise-0.2.1.dev66/src/phasor_noise/analysis/__init__.py` & `Phasor Noise-0.3.0/src/phasor_noise/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `Phasor Noise-0.2.1.dev66/src/phasor_noise/generator/__init__.py` & `Phasor Noise-0.3.0/src/phasor_noise/generator/__init__.py`

 * *Files identical despite different names*

