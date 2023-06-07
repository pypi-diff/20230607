# Comparing `tmp/autodistill-detr-0.0.1.tar.gz` & `tmp/autodistill_detr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-detr-0.0.1.tar", last modified: Wed Jun  7 11:06:59 2023, max compression
+gzip compressed data, was "autodistill_detr-0.1.0.tar", last modified: Wed Jun  7 14:19:42 2023, max compression
```

## Comparing `autodistill-detr-0.0.1.tar` & `autodistill_detr-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:59.472711 autodistill-detr-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)      359 2023-06-07 11:06:59.472558 autodistill-detr-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)       17 2023-06-07 11:06:57.000000 autodistill-detr-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:59.471358 autodistill-detr-0.0.1/autodistill_detr/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-06-07 11:06:57.000000 autodistill-detr-0.0.1/autodistill_detr/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:59.472334 autodistill-detr-0.0.1/autodistill_detr.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      359 2023-06-07 11:06:59.000000 autodistill-detr-0.0.1/autodistill_detr.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      246 2023-06-07 11:06:59.000000 autodistill-detr-0.0.1/autodistill_detr.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 11:06:59.000000 autodistill-detr-0.0.1/autodistill_detr.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       53 2023-06-07 11:06:59.000000 autodistill-detr-0.0.1/autodistill_detr.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       17 2023-06-07 11:06:59.000000 autodistill-detr-0.0.1/autodistill_detr.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-07 11:06:59.472758 autodistill-detr-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      977 2023-06-07 11:06:57.000000 autodistill-detr-0.0.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 14:19:42.357855 autodistill_detr-0.1.0/
+-rw-r--r--   0 james      (501) staff       (20)     2219 2023-06-07 14:19:42.357688 autodistill_detr-0.1.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1771 2023-06-06 14:21:21.000000 autodistill_detr-0.1.0/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 14:19:42.355439 autodistill_detr-0.1.0/autodistill_detr/
+-rw-r--r--   0 james      (501) staff       (20)       68 2023-06-06 14:14:17.000000 autodistill_detr-0.1.0/autodistill_detr/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1451 2023-06-06 14:18:57.000000 autodistill_detr-0.1.0/autodistill_detr/detr_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 14:19:42.357395 autodistill_detr-0.1.0/autodistill_detr.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2219 2023-06-07 14:19:42.000000 autodistill_detr-0.1.0/autodistill_detr.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      277 2023-06-07 14:19:42.000000 autodistill_detr-0.1.0/autodistill_detr.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 14:19:42.000000 autodistill_detr-0.1.0/autodistill_detr.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      104 2023-06-07 14:19:42.000000 autodistill_detr-0.1.0/autodistill_detr.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       17 2023-06-07 14:19:42.000000 autodistill_detr-0.1.0/autodistill_detr.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-07 14:19:42.357902 autodistill_detr-0.1.0/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1177 2023-06-07 14:19:35.000000 autodistill_detr-0.1.0/setup.py
```

### Comparing `autodistill-detr-0.0.1/setup.py` & `autodistill_detr-0.1.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-
 import setuptools
 from setuptools import find_packages
 import re
 
 with open("./autodistill_detr/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="autodistill-detr",
+    name="autodistill_detr",
     version=version,
     author="Roboflow",
     author_email="support@roboflow.com",
-    description="",
+    description="DETR module for use with Autodistill",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=[],
+    url="https://github.com/autodistill/autodistill-detr",
+    install_requires=[
+        "supervision==0.9.0",
+        "transformers",
+        "torch",
+        "numpy",
+        "Pillow"
+    ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
-
```

