# Comparing `tmp/autodistill-owl-vit-0.0.1.tar.gz` & `tmp/autodistill_owl_vit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-owl-vit-0.0.1.tar", last modified: Wed Jun  7 11:06:35 2023, max compression
+gzip compressed data, was "autodistill_owl_vit-0.1.0.tar", last modified: Wed Jun  7 13:42:03 2023, max compression
```

## Comparing `autodistill-owl-vit-0.0.1.tar` & `autodistill_owl_vit-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:35.301197 autodistill-owl-vit-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)      365 2023-06-07 11:06:35.301071 autodistill-owl-vit-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)       20 2023-06-07 11:06:33.000000 autodistill-owl-vit-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:35.300137 autodistill-owl-vit-0.0.1/autodistill_owl_vit/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-06-07 11:06:33.000000 autodistill-owl-vit-0.0.1/autodistill_owl_vit/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:35.300892 autodistill-owl-vit-0.0.1/autodistill_owl_vit.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      365 2023-06-07 11:06:35.000000 autodistill-owl-vit-0.0.1/autodistill_owl_vit.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      264 2023-06-07 11:06:35.000000 autodistill-owl-vit-0.0.1/autodistill_owl_vit.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 11:06:35.000000 autodistill-owl-vit-0.0.1/autodistill_owl_vit.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       53 2023-06-07 11:06:35.000000 autodistill-owl-vit-0.0.1/autodistill_owl_vit.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       20 2023-06-07 11:06:35.000000 autodistill-owl-vit-0.0.1/autodistill_owl_vit.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-07 11:06:35.301239 autodistill-owl-vit-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      983 2023-06-07 11:06:33.000000 autodistill-owl-vit-0.0.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 13:42:03.107805 autodistill_owl_vit-0.1.0/
+-rw-r--r--   0 james      (501) staff       (20)    10173 2023-06-07 13:04:07.000000 autodistill_owl_vit-0.1.0/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     2227 2023-06-07 13:42:03.107651 autodistill_owl_vit-0.1.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1748 2023-06-07 13:40:23.000000 autodistill_owl_vit-0.1.0/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 13:42:03.105847 autodistill_owl_vit-0.1.0/autodistill_owl_vit/
+-rw-r--r--   0 james      (501) staff       (20)       69 2023-06-06 08:41:04.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1447 2023-06-06 09:25:50.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit/owlvit.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 13:42:03.107119 autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2227 2023-06-07 13:42:03.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      321 2023-06-07 13:42:03.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 13:42:03.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       90 2023-06-07 13:42:03.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       20 2023-06-07 13:42:03.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-07 13:42:03.107851 autodistill_owl_vit-0.1.0/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1166 2023-06-07 13:41:09.000000 autodistill_owl_vit-0.1.0/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 13:42:03.107301 autodistill_owl_vit-0.1.0/test/
+-rw-r--r--   0 james      (501) staff       (20)       91 2023-06-06 08:40:14.000000 autodistill_owl_vit-0.1.0/test/test_hello.py
```

### Comparing `autodistill-owl-vit-0.0.1/setup.py` & `autodistill_owl_vit-0.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-
 import setuptools
 from setuptools import find_packages
 import re
 
 with open("./autodistill_owl_vit/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="autodistill-owl-vit",
+    name="autodistill_owl_vit",  
     version=version,
     author="Roboflow",
     author_email="support@roboflow.com",
-    description="",
+    description="OWL-ViT module for use with Autodistill",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=[],
+    url="https://github.com/autodistill/autodistill-owl-vit",
+    install_requires=[
+        "torch",
+        "supervision",
+        "numpy",
+        "transformers"
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

