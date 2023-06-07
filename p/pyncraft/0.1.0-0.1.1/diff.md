# Comparing `tmp/pyncraft-0.1.0.tar.gz` & `tmp/pyncraft-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyncraft-0.1.0.tar", last modified: Tue Jun  6 04:05:47 2023, max compression
+gzip compressed data, was "pyncraft-0.1.1.tar", last modified: Wed Jun  7 04:13:54 2023, max compression
```

## Comparing `pyncraft-0.1.0.tar` & `pyncraft-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 04:05:47.322206 pyncraft-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-06-06 03:05:16.000000 pyncraft-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      969 2023-06-06 04:05:47.320711 pyncraft-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-02 15:23:05.000000 pyncraft-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 04:05:47.264605 pyncraft-0.1.0/pyncraft/
--rw-rw-rw-   0        0        0        0 2023-06-02 17:29:00.000000 pyncraft-0.1.0/pyncraft/__init__.py
--rw-rw-rw-   0        0        0     2993 2023-06-02 17:29:00.000000 pyncraft-0.1.0/pyncraft/block.py
--rw-rw-rw-   0        0        0     1956 2023-06-03 02:32:24.000000 pyncraft-0.1.0/pyncraft/connection.py
--rw-rw-rw-   0        0        0     3404 2023-06-02 17:29:01.000000 pyncraft-0.1.0/pyncraft/entity.py
--rw-rw-rw-   0        0        0     1807 2023-06-02 17:29:01.000000 pyncraft-0.1.0/pyncraft/event.py
--rw-rw-rw-   0        0        0      777 2023-06-02 18:21:46.000000 pyncraft-0.1.0/pyncraft/logger.py
--rw-rw-rw-   0        0        0    14665 2023-06-05 01:37:25.000000 pyncraft-0.1.0/pyncraft/minecraft.py
--rw-rw-rw-   0        0        0      159 2023-06-02 18:22:17.000000 pyncraft-0.1.0/pyncraft/settings.py
--rw-rw-rw-   0        0        0      487 2023-06-02 17:29:00.000000 pyncraft-0.1.0/pyncraft/util.py
--rw-rw-rw-   0        0        0     2458 2023-06-02 17:29:00.000000 pyncraft-0.1.0/pyncraft/vec3.py
-drwxrwxrwx   0        0        0        0 2023-06-06 04:05:47.315362 pyncraft-0.1.0/pyncraft.egg-info/
--rw-rw-rw-   0        0        0      969 2023-06-06 04:05:46.000000 pyncraft-0.1.0/pyncraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-06-06 04:05:47.000000 pyncraft-0.1.0/pyncraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 04:05:46.000000 pyncraft-0.1.0/pyncraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 04:05:46.000000 pyncraft-0.1.0/pyncraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 04:05:47.323311 pyncraft-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     9487 2023-06-06 03:42:51.000000 pyncraft-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:13:54.760940 pyncraft-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-06-06 03:05:16.000000 pyncraft-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1334 2023-06-07 04:13:54.757962 pyncraft-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-06-07 01:53:06.000000 pyncraft-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 04:13:54.741295 pyncraft-0.1.1/pyncraft/
+-rw-rw-rw-   0        0        0        0 2023-06-02 17:29:00.000000 pyncraft-0.1.1/pyncraft/__init__.py
+-rw-rw-rw-   0        0        0     2993 2023-06-02 17:29:00.000000 pyncraft-0.1.1/pyncraft/block.py
+-rw-rw-rw-   0        0        0     1956 2023-06-03 02:32:24.000000 pyncraft-0.1.1/pyncraft/connection.py
+-rw-rw-rw-   0        0        0     3404 2023-06-02 17:29:01.000000 pyncraft-0.1.1/pyncraft/entity.py
+-rw-rw-rw-   0        0        0     1807 2023-06-02 17:29:01.000000 pyncraft-0.1.1/pyncraft/event.py
+-rw-rw-rw-   0        0        0      777 2023-06-02 18:21:46.000000 pyncraft-0.1.1/pyncraft/logger.py
+-rw-rw-rw-   0        0        0    14665 2023-06-05 01:37:25.000000 pyncraft-0.1.1/pyncraft/minecraft.py
+-rw-rw-rw-   0        0        0      159 2023-06-02 18:22:17.000000 pyncraft-0.1.1/pyncraft/settings.py
+-rw-rw-rw-   0        0        0      487 2023-06-02 17:29:00.000000 pyncraft-0.1.1/pyncraft/util.py
+-rw-rw-rw-   0        0        0     2458 2023-06-02 17:29:00.000000 pyncraft-0.1.1/pyncraft/vec3.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:13:54.755875 pyncraft-0.1.1/pyncraft.egg-info/
+-rw-rw-rw-   0        0        0     1334 2023-06-07 04:13:54.000000 pyncraft-0.1.1/pyncraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-06-07 04:13:54.000000 pyncraft-0.1.1/pyncraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 04:13:54.000000 pyncraft-0.1.1/pyncraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-07 04:13:54.000000 pyncraft-0.1.1/pyncraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 04:13:54.000000 pyncraft-0.1.1/pyncraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 04:13:54.760940 pyncraft-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     9508 2023-06-07 04:09:23.000000 pyncraft-0.1.1/setup.py
```

### Comparing `pyncraft-0.1.0/LICENSE` & `pyncraft-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.0/pyncraft/block.py` & `pyncraft-0.1.1/pyncraft/block.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.0/pyncraft/connection.py` & `pyncraft-0.1.1/pyncraft/connection.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.0/pyncraft/entity.py` & `pyncraft-0.1.1/pyncraft/entity.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.0/pyncraft/event.py` & `pyncraft-0.1.1/pyncraft/event.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.0/pyncraft/logger.py` & `pyncraft-0.1.1/pyncraft/logger.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.0/pyncraft/minecraft.py` & `pyncraft-0.1.1/pyncraft/minecraft.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.0/pyncraft/vec3.py` & `pyncraft-0.1.1/pyncraft/vec3.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.1.0/setup.py` & `pyncraft-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version='0.1.0',  # Required
+    version='0.1.1',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Python interface to minecraft + pyncraft bukkit plugin',  # Optional
 
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
@@ -137,15 +137,15 @@
 
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
-    install_requires=[],
+    install_requires=["ipdb","stl-to-voxel"],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
```

