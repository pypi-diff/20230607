# Comparing `tmp/penquins-2.2.0.tar.gz` & `tmp/penquins-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penquins-2.2.0.tar", last modified: Sun Jul 24 12:39:16 2022, max compression
+gzip compressed data, was "penquins-2.3.1.tar", last modified: Wed Jun  7 07:31:43 2023, max compression
```

## Comparing `penquins-2.2.0.tar` & `penquins-2.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2022-07-24 12:39:16.474355 penquins-2.2.0/
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1068 2022-07-24 12:39:00.000000 penquins-2.2.0/LICENSE
--rw-r--r--   0 mcoughlin   (501) staff       (20)      257 2022-07-24 12:39:16.474180 penquins-2.2.0/PKG-INFO
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2022-07-24 12:39:16.472735 penquins-2.2.0/penquins/
--rw-r--r--   0 mcoughlin   (501) staff       (20)       24 2022-07-24 12:39:00.000000 penquins-2.2.0/penquins/__init__.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     9043 2022-07-24 12:39:00.000000 penquins-2.2.0/penquins/penquins.py
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2022-07-24 12:39:16.473940 penquins-2.2.0/penquins.egg-info/
--rw-r--r--   0 mcoughlin   (501) staff       (20)      257 2022-07-24 12:39:16.000000 penquins-2.2.0/penquins.egg-info/PKG-INFO
--rw-r--r--   0 mcoughlin   (501) staff       (20)      217 2022-07-24 12:39:16.000000 penquins-2.2.0/penquins.egg-info/SOURCES.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)        1 2022-07-24 12:39:16.000000 penquins-2.2.0/penquins.egg-info/dependency_links.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)       60 2022-07-24 12:39:16.000000 penquins-2.2.0/penquins.egg-info/requires.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)        9 2022-07-24 12:39:16.000000 penquins-2.2.0/penquins.egg-info/top_level.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)       38 2022-07-24 12:39:16.474411 penquins-2.2.0/setup.cfg
--rw-r--r--   0 mcoughlin   (501) staff       (20)     5088 2022-07-24 12:39:00.000000 penquins-2.2.0/setup.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-06-07 07:31:43.822434 penquins-2.3.1/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1068 2023-06-07 07:31:26.000000 penquins-2.3.1/LICENSE
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      229 2023-06-07 07:31:43.822250 penquins-2.3.1/PKG-INFO
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-06-07 07:31:43.821272 penquins-2.3.1/penquins/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)       24 2023-06-07 07:31:26.000000 penquins-2.3.1/penquins/__init__.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    34772 2023-06-07 07:31:26.000000 penquins-2.3.1/penquins/penquins.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-06-07 07:31:43.822034 penquins-2.3.1/penquins.egg-info/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      229 2023-06-07 07:31:43.000000 penquins-2.3.1/penquins.egg-info/PKG-INFO
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      217 2023-06-07 07:31:43.000000 penquins-2.3.1/penquins.egg-info/SOURCES.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)        1 2023-06-07 07:31:43.000000 penquins-2.3.1/penquins.egg-info/dependency_links.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      125 2023-06-07 07:31:43.000000 penquins-2.3.1/penquins.egg-info/requires.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)        9 2023-06-07 07:31:43.000000 penquins-2.3.1/penquins.egg-info/top_level.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)       38 2023-06-07 07:31:43.822482 penquins-2.3.1/setup.cfg
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     5197 2023-06-07 07:31:26.000000 penquins-2.3.1/setup.py
```

### Comparing `penquins-2.2.0/LICENSE` & `penquins-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `penquins-2.2.0/setup.py` & `penquins-2.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,29 +130,33 @@
 LONG_DESCRIPTION = ""
 AUTHOR = "Dmitry A. Duev"
 AUTHOR_EMAIL = "duev@caltech.edu"
 LICENSE = "MIT"
 URL = "https://github.com/dmitryduev/penquins"
 
 # VERSION should be PEP386 compatible (http://www.python.org/dev/peps/pep-0386)
-VERSION = "2.2.0"
+VERSION = "2.3.1"
 
 # Indicates if this version is a release version
 RELEASE = "dev" not in VERSION
 
 if not RELEASE:
     VERSION += get_git_devstr(sha=False)
 
 
 setup(
     name=PACKAGENAME,
     version=VERSION,
     description=DESCRIPTION,
     packages=["penquins"],
     install_requires=[
+        "astropy>=5.2.1",
+        "astropy-healpix>=0.7",
+        "healpy>=1.16.0",
+        "mocpy>=0.11.0",
         "pymongo>=3.10.1",
         "pytest>=5.3.1",
         "requests>=2.25.0",
         "tqdm>=4.46.0",
     ],
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
```

