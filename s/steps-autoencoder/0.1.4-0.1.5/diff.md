# Comparing `tmp/steps-autoencoder-0.1.4.tar.gz` & `tmp/steps-autoencoder-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steps-autoencoder-0.1.4.tar", last modified: Tue Jun  6 22:04:39 2023, max compression
+gzip compressed data, was "steps-autoencoder-0.1.5.tar", last modified: Tue Jun  6 22:09:49 2023, max compression
```

## Comparing `steps-autoencoder-0.1.4.tar` & `steps-autoencoder-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 22:04:39.421087 steps-autoencoder-0.1.4/
--rw-r--r--   0 ffee21     (501) staff       (20)    11324 2023-06-06 17:22:47.000000 steps-autoencoder-0.1.4/LICENSE
--rw-r--r--   0 ffee21     (501) staff       (20)      250 2023-06-06 22:04:39.420955 steps-autoencoder-0.1.4/PKG-INFO
--rw-r--r--   0 ffee21     (501) staff       (20)        0 2023-06-06 17:19:09.000000 steps-autoencoder-0.1.4/README.md
--rw-r--r--   0 ffee21     (501) staff       (20)       38 2023-06-06 22:04:39.421133 steps-autoencoder-0.1.4/setup.cfg
--rw-r--r--   0 ffee21     (501) staff       (20)     1941 2023-06-06 21:59:28.000000 steps-autoencoder-0.1.4/setup.py
-drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 22:04:39.420003 steps-autoencoder-0.1.4/steps_autoencoder/
--rw-r--r--   0 ffee21     (501) staff       (20)       31 2023-06-06 17:30:00.000000 steps-autoencoder-0.1.4/steps_autoencoder/__init__.py
--rw-r--r--   0 ffee21     (501) staff       (20)       27 2023-06-06 17:31:32.000000 steps-autoencoder-0.1.4/steps_autoencoder/models.py
-drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 22:04:39.420600 steps-autoencoder-0.1.4/steps_autoencoder.egg-info/
--rw-r--r--   0 ffee21     (501) staff       (20)      250 2023-06-06 22:04:39.000000 steps-autoencoder-0.1.4/steps_autoencoder.egg-info/PKG-INFO
--rw-r--r--   0 ffee21     (501) staff       (20)      332 2023-06-06 22:04:39.000000 steps-autoencoder-0.1.4/steps_autoencoder.egg-info/SOURCES.txt
--rw-r--r--   0 ffee21     (501) staff       (20)        1 2023-06-06 22:04:39.000000 steps-autoencoder-0.1.4/steps_autoencoder.egg-info/dependency_links.txt
--rw-r--r--   0 ffee21     (501) staff       (20)       11 2023-06-06 22:04:39.000000 steps-autoencoder-0.1.4/steps_autoencoder.egg-info/requires.txt
--rw-r--r--   0 ffee21     (501) staff       (20)       24 2023-06-06 22:04:39.000000 steps-autoencoder-0.1.4/steps_autoencoder.egg-info/top_level.txt
-drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 22:04:39.420797 steps-autoencoder-0.1.4/tests/
--rw-r--r--   0 ffee21     (501) staff       (20)        0 2023-06-06 17:19:39.000000 steps-autoencoder-0.1.4/tests/__init__.py
--rw-r--r--   0 ffee21     (501) staff       (20)      269 2023-06-06 22:04:11.000000 steps-autoencoder-0.1.4/tests/test_autoencoder.py
+drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 22:09:49.432402 steps-autoencoder-0.1.5/
+-rw-r--r--   0 ffee21     (501) staff       (20)    11324 2023-06-06 17:22:47.000000 steps-autoencoder-0.1.5/LICENSE
+-rw-r--r--   0 ffee21     (501) staff       (20)      250 2023-06-06 22:09:49.432260 steps-autoencoder-0.1.5/PKG-INFO
+-rw-r--r--   0 ffee21     (501) staff       (20)        0 2023-06-06 17:19:09.000000 steps-autoencoder-0.1.5/README.md
+-rw-r--r--   0 ffee21     (501) staff       (20)       38 2023-06-06 22:09:49.432449 steps-autoencoder-0.1.5/setup.cfg
+-rw-r--r--   0 ffee21     (501) staff       (20)     1941 2023-06-06 21:59:28.000000 steps-autoencoder-0.1.5/setup.py
+drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 22:09:49.431252 steps-autoencoder-0.1.5/steps_autoencoder/
+-rw-r--r--   0 ffee21     (501) staff       (20)       31 2023-06-06 17:30:00.000000 steps-autoencoder-0.1.5/steps_autoencoder/__init__.py
+-rw-r--r--   0 ffee21     (501) staff       (20)    30564 2023-06-06 22:09:41.000000 steps-autoencoder-0.1.5/steps_autoencoder/models.py
+drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 22:09:49.431881 steps-autoencoder-0.1.5/steps_autoencoder.egg-info/
+-rw-r--r--   0 ffee21     (501) staff       (20)      250 2023-06-06 22:09:49.000000 steps-autoencoder-0.1.5/steps_autoencoder.egg-info/PKG-INFO
+-rw-r--r--   0 ffee21     (501) staff       (20)      332 2023-06-06 22:09:49.000000 steps-autoencoder-0.1.5/steps_autoencoder.egg-info/SOURCES.txt
+-rw-r--r--   0 ffee21     (501) staff       (20)        1 2023-06-06 22:09:49.000000 steps-autoencoder-0.1.5/steps_autoencoder.egg-info/dependency_links.txt
+-rw-r--r--   0 ffee21     (501) staff       (20)       32 2023-06-06 22:09:49.000000 steps-autoencoder-0.1.5/steps_autoencoder.egg-info/requires.txt
+-rw-r--r--   0 ffee21     (501) staff       (20)       24 2023-06-06 22:09:49.000000 steps-autoencoder-0.1.5/steps_autoencoder.egg-info/top_level.txt
+drwxr-xr-x   0 ffee21     (501) staff       (20)        0 2023-06-06 22:09:49.432080 steps-autoencoder-0.1.5/tests/
+-rw-r--r--   0 ffee21     (501) staff       (20)        0 2023-06-06 17:19:39.000000 steps-autoencoder-0.1.5/tests/__init__.py
+-rw-r--r--   0 ffee21     (501) staff       (20)    14414 2023-06-06 22:05:34.000000 steps-autoencoder-0.1.5/tests/test_autoencoder.py
```

### Comparing `steps-autoencoder-0.1.4/LICENSE` & `steps-autoencoder-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `steps-autoencoder-0.1.4/setup.py` & `steps-autoencoder-0.1.5/setup.py`

 * *Files identical despite different names*

