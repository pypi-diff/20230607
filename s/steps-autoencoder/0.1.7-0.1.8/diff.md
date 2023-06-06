# Comparing `tmp/steps-autoencoder-0.1.7.tar.gz` & `tmp/steps-autoencoder-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steps-autoencoder-0.1.7.tar", last modified: Tue Jun  6 23:07:13 2023, max compression
+gzip compressed data, was "steps-autoencoder-0.1.8.tar", last modified: Tue Jun  6 23:16:23 2023, max compression
```

## Comparing `steps-autoencoder-0.1.7.tar` & `steps-autoencoder-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 23:07:13.565464 steps-autoencoder-0.1.7/
--rw-r--r--   0 ffee21     (501) staff       (20)    11324 2023-06-06 17:22:47.000000 steps-autoencoder-0.1.7/LICENSE
--rw-r--r--   0 ffee21     (501) staff       (20)      250 2023-06-06 23:07:13.565348 steps-autoencoder-0.1.7/PKG-INFO
--rw-r--r--   0 ffee21     (501) staff       (20)        0 2023-06-06 17:19:09.000000 steps-autoencoder-0.1.7/README.md
--rw-r--r--   0 ffee21     (501) staff       (20)       38 2023-06-06 23:07:13.565512 steps-autoencoder-0.1.7/setup.cfg
--rw-r--r--   0 ffee21     (501) staff       (20)     1941 2023-06-06 21:59:28.000000 steps-autoencoder-0.1.7/setup.py
-drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 23:07:13.564569 steps-autoencoder-0.1.7/steps_autoencoder/
--rw-r--r--   0 ffee21     (501) staff       (20)       31 2023-06-06 17:30:00.000000 steps-autoencoder-0.1.7/steps_autoencoder/__init__.py
--rw-r--r--   0 ffee21     (501) staff       (20)      624 2023-06-06 23:07:00.000000 steps-autoencoder-0.1.7/steps_autoencoder/data_generator.py
--rw-r--r--   0 ffee21     (501) staff       (20)    30564 2023-06-06 22:09:41.000000 steps-autoencoder-0.1.7/steps_autoencoder/models.py
-drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 23:07:13.565171 steps-autoencoder-0.1.7/steps_autoencoder.egg-info/
--rw-r--r--   0 ffee21     (501) staff       (20)      250 2023-06-06 23:07:13.000000 steps-autoencoder-0.1.7/steps_autoencoder.egg-info/PKG-INFO
--rw-r--r--   0 ffee21     (501) staff       (20)      324 2023-06-06 23:07:13.000000 steps-autoencoder-0.1.7/steps_autoencoder.egg-info/SOURCES.txt
--rw-r--r--   0 ffee21     (501) staff       (20)        1 2023-06-06 23:07:13.000000 steps-autoencoder-0.1.7/steps_autoencoder.egg-info/dependency_links.txt
--rw-r--r--   0 ffee21     (501) staff       (20)       32 2023-06-06 23:07:13.000000 steps-autoencoder-0.1.7/steps_autoencoder.egg-info/requires.txt
--rw-r--r--   0 ffee21     (501) staff       (20)       18 2023-06-06 23:07:13.000000 steps-autoencoder-0.1.7/steps_autoencoder.egg-info/top_level.txt
+drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 23:16:23.369571 steps-autoencoder-0.1.8/
+-rw-r--r--   0 ffee21     (501) staff       (20)    11324 2023-06-06 17:22:47.000000 steps-autoencoder-0.1.8/LICENSE
+-rw-r--r--   0 ffee21     (501) staff       (20)      250 2023-06-06 23:16:23.369421 steps-autoencoder-0.1.8/PKG-INFO
+-rw-r--r--   0 ffee21     (501) staff       (20)        0 2023-06-06 17:19:09.000000 steps-autoencoder-0.1.8/README.md
+-rw-r--r--   0 ffee21     (501) staff       (20)       38 2023-06-06 23:16:23.369623 steps-autoencoder-0.1.8/setup.cfg
+-rw-r--r--   0 ffee21     (501) staff       (20)     1941 2023-06-06 21:59:28.000000 steps-autoencoder-0.1.8/setup.py
+drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 23:16:23.368594 steps-autoencoder-0.1.8/steps_autoencoder/
+-rw-r--r--   0 ffee21     (501) staff       (20)       31 2023-06-06 17:30:00.000000 steps-autoencoder-0.1.8/steps_autoencoder/__init__.py
+-rw-r--r--   0 ffee21     (501) staff       (20)      624 2023-06-06 23:14:34.000000 steps-autoencoder-0.1.8/steps_autoencoder/data_generator.py
+-rw-r--r--   0 ffee21     (501) staff       (20)    30564 2023-06-06 22:09:41.000000 steps-autoencoder-0.1.8/steps_autoencoder/models.py
+drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 23:16:23.369232 steps-autoencoder-0.1.8/steps_autoencoder.egg-info/
+-rw-r--r--   0 ffee21     (501) staff       (20)      250 2023-06-06 23:16:23.000000 steps-autoencoder-0.1.8/steps_autoencoder.egg-info/PKG-INFO
+-rw-r--r--   0 ffee21     (501) staff       (20)      324 2023-06-06 23:16:23.000000 steps-autoencoder-0.1.8/steps_autoencoder.egg-info/SOURCES.txt
+-rw-r--r--   0 ffee21     (501) staff       (20)        1 2023-06-06 23:16:23.000000 steps-autoencoder-0.1.8/steps_autoencoder.egg-info/dependency_links.txt
+-rw-r--r--   0 ffee21     (501) staff       (20)       32 2023-06-06 23:16:23.000000 steps-autoencoder-0.1.8/steps_autoencoder.egg-info/requires.txt
+-rw-r--r--   0 ffee21     (501) staff       (20)       18 2023-06-06 23:16:23.000000 steps-autoencoder-0.1.8/steps_autoencoder.egg-info/top_level.txt
```

### Comparing `steps-autoencoder-0.1.7/LICENSE` & `steps-autoencoder-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `steps-autoencoder-0.1.7/setup.py` & `steps-autoencoder-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `steps-autoencoder-0.1.7/steps_autoencoder/data_generator.py` & `steps-autoencoder-0.1.8/steps_autoencoder/data_generator.py`

 * *Files identical despite different names*

### Comparing `steps-autoencoder-0.1.7/steps_autoencoder/models.py` & `steps-autoencoder-0.1.8/steps_autoencoder/models.py`

 * *Files identical despite different names*

