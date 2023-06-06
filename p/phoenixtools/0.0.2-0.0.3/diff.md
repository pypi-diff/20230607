# Comparing `tmp/phoenixtools-0.0.2.tar.gz` & `tmp/phoenixtools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phoenixtools-0.0.2.tar", last modified: Tue Jun  6 23:31:14 2023, max compression
+gzip compressed data, was "phoenixtools-0.0.3.tar", last modified: Tue Jun  6 23:41:22 2023, max compression
```

## Comparing `phoenixtools-0.0.2.tar` & `phoenixtools-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-06 23:31:14.426451 phoenixtools-0.0.2/
--rw-r--r--   0 runner    (1000) runner    (1000)      453 2023-06-06 23:31:14.426451 phoenixtools-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-06 23:31:14.426451 phoenixtools-0.0.2/phoenixtools/
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-06-06 23:29:11.000000 phoenixtools-0.0.2/phoenixtools/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      145 2023-06-06 23:29:04.000000 phoenixtools-0.0.2/phoenixtools/iptools.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-06 23:31:14.426451 phoenixtools-0.0.2/phoenixtools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      453 2023-06-06 23:31:14.000000 phoenixtools-0.0.2/phoenixtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2023-06-06 23:31:14.000000 phoenixtools-0.0.2/phoenixtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-06 23:31:14.000000 phoenixtools-0.0.2/phoenixtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-06-06 23:31:14.000000 phoenixtools-0.0.2/phoenixtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-06 23:31:14.426451 phoenixtools-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      964 2023-06-06 23:29:24.000000 phoenixtools-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-06 23:41:22.817853 phoenixtools-0.0.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)      453 2023-06-06 23:41:22.817853 phoenixtools-0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-06 23:41:22.817853 phoenixtools-0.0.3/phoenixtools/
+-rw-r--r--   0 runner    (1000) runner    (1000)       28 2023-06-06 23:37:43.000000 phoenixtools-0.0.3/phoenixtools/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      172 2023-06-06 23:39:57.000000 phoenixtools-0.0.3/phoenixtools/iptools.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-06 23:41:22.817853 phoenixtools-0.0.3/phoenixtools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      453 2023-06-06 23:41:22.000000 phoenixtools-0.0.3/phoenixtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      201 2023-06-06 23:41:22.000000 phoenixtools-0.0.3/phoenixtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-06 23:41:22.000000 phoenixtools-0.0.3/phoenixtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-06-06 23:41:22.000000 phoenixtools-0.0.3/phoenixtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-06 23:41:22.817853 phoenixtools-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      964 2023-06-06 23:41:10.000000 phoenixtools-0.0.3/setup.py
```

### Comparing `phoenixtools-0.0.2/setup.py` & `phoenixtools-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'Easy hacking tools'
 LONG_DESCRIPTION = 'Easy hacking tools used for educational purposes'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="phoenixtools",
```

