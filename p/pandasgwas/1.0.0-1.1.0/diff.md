# Comparing `tmp/pandasgwas-1.0.0.tar.gz` & `tmp/pandasgwas-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasgwas-1.0.0.tar", last modified: Sat May 13 06:25:03 2023, max compression
+gzip compressed data, was "pandasgwas-1.1.0.tar", last modified: Wed Jun  7 03:35:37 2023, max compression
```

## Comparing `pandasgwas-1.0.0.tar` & `pandasgwas-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 06:25:03.575496 pandasgwas-1.0.0/
--rw-rw-rw-   0        0        0     1118 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     6564 2023-05-13 06:25:03.575496 pandasgwas-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5851 2023-05-13 06:22:54.000000 pandasgwas-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 06:25:03.513002 pandasgwas-1.0.0/pandasgwas/
--rw-rw-rw-   0        0        0     8596 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/Association.py
--rw-rw-rw-   0        0        0     1362 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/Browser.py
--rw-rw-rw-   0        0        0     8198 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/Study.py
--rw-rw-rw-   0        0        0     3795 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/Trait.py
--rw-rw-rw-   0        0        0     6284 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/Variant.py
--rw-rw-rw-   0        0        0     1862 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/__init__.py
--rw-rw-rw-   0        0        0    10818 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/client.py
--rw-rw-rw-   0        0        0    78270 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/cytogenetic_bands.csv
--rw-rw-rw-   0        0        0     4871 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/get_associations.py
--rw-rw-rw-   0        0        0     6828 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/get_studies.py
--rw-rw-rw-   0        0        0     4369 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/get_traits.py
--rw-rw-rw-   0        0        0     7700 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/get_variants.py
--rw-rw-rw-   0        0        0  2771641 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/harmonised_list.txt
--rw-rw-rw-   0        0        0     1296 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/set_operation.py
--rw-rw-rw-   0        0        0     5348 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/summary_statistics.py
--rw-rw-rw-   0        0        0      826 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pandasgwas/utility.py
-drwxrwxrwx   0        0        0        0 2023-05-13 06:25:03.575496 pandasgwas-1.0.0/pandasgwas.egg-info/
--rw-rw-rw-   0        0        0     6564 2023-05-13 06:25:02.000000 pandasgwas-1.0.0/pandasgwas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      620 2023-05-13 06:25:03.000000 pandasgwas-1.0.0/pandasgwas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 06:25:02.000000 pandasgwas-1.0.0/pandasgwas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-13 06:25:02.000000 pandasgwas-1.0.0/pandasgwas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-13 06:25:02.000000 pandasgwas-1.0.0/pandasgwas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-18 02:33:30.000000 pandasgwas-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 06:25:03.575496 pandasgwas-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-05-13 06:15:24.000000 pandasgwas-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:35:37.862442 pandasgwas-1.1.0/
+-rw-rw-rw-   0        0        0     1118 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     6567 2023-06-07 03:35:37.860441 pandasgwas-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5852 2023-06-07 02:49:12.000000 pandasgwas-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 03:35:37.802477 pandasgwas-1.1.0/pandasgwas/
+-rw-rw-rw-   0        0        0     8596 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/Association.py
+-rw-rw-rw-   0        0        0     1362 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/Browser.py
+-rw-rw-rw-   0        0        0     8198 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/Study.py
+-rw-rw-rw-   0        0        0     3795 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/Trait.py
+-rw-rw-rw-   0        0        0     6284 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/Variant.py
+-rw-rw-rw-   0        0        0     1862 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/__init__.py
+-rw-rw-rw-   0        0        0    10818 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/client.py
+-rw-rw-rw-   0        0        0    78270 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/cytogenetic_bands.csv
+-rw-rw-rw-   0        0        0     4871 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/get_associations.py
+-rw-rw-rw-   0        0        0     6828 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/get_studies.py
+-rw-rw-rw-   0        0        0     4369 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/get_traits.py
+-rw-rw-rw-   0        0        0     7700 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/get_variants.py
+-rw-rw-rw-   0        0        0  2771641 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/harmonised_list.txt
+-rw-rw-rw-   0        0        0     1296 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/set_operation.py
+-rw-rw-rw-   0        0        0     5348 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/summary_statistics.py
+-rw-rw-rw-   0        0        0      826 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pandasgwas/utility.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:35:37.857444 pandasgwas-1.1.0/pandasgwas.egg-info/
+-rw-rw-rw-   0        0        0     6567 2023-06-07 03:35:37.000000 pandasgwas-1.1.0/pandasgwas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2023-06-07 03:35:37.000000 pandasgwas-1.1.0/pandasgwas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 03:35:37.000000 pandasgwas-1.1.0/pandasgwas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-07 03:35:37.000000 pandasgwas-1.1.0/pandasgwas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 03:35:37.000000 pandasgwas-1.1.0/pandasgwas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-18 02:33:30.000000 pandasgwas-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 03:35:37.862442 pandasgwas-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2023-06-07 03:33:13.000000 pandasgwas-1.1.0/setup.py
```

### Comparing `pandasgwas-1.0.0/LICENSE` & `pandasgwas-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/PKG-INFO` & `pandasgwas-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pandasgwas
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python package for easy retrieval of GWAS Catalog data
 Home-page: https://github.com/caotianze/pandasgwas
 Author: Cao Tianze
 Author-email: hnrcao@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/caotianze/pandasgwas/issues
 Keywords: gwas,genomics,snp,bioinformatics,pandas
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pandasGWAS: a Python package for easy retrieval of GWAS Catalog data
 ## News
 On 4 May 2023, the work has been published in BMC Genomics.    
 Starting from V0.99.18, pandasGWAS can cache API requests in memory.    
@@ -71,15 +71,15 @@
 browser(search_DF)
 #Based on index results, download summary statistics data in $Home/pandasgwas_home.
 download(search_DF)
 #Based on the index results, load the data from $Home/pandasgwas_home and convert it into a DataFrame. 
 df = parse(search_DF)
 ```
 ## Dependencies
-python: 3.8  
+python: 3.10  
 pandas: 1.4.3  
 requests: 2.28.1  
 progressbar2: 4.0.0
 ## Documentation
 See [pandasGWAS Documentation](https://caotianze.github.io/pandasgwas/)
 ## Licensing information
 ### Source code
```

### Comparing `pandasgwas-1.0.0/README.md` & `pandasgwas-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 browser(search_DF)
 #Based on index results, download summary statistics data in $Home/pandasgwas_home.
 download(search_DF)
 #Based on the index results, load the data from $Home/pandasgwas_home and convert it into a DataFrame. 
 df = parse(search_DF)
 ```
 ## Dependencies
-python: 3.8  
+python: 3.10  
 pandas: 1.4.3  
 requests: 2.28.1  
 progressbar2: 4.0.0
 ## Documentation
 See [pandasGWAS Documentation](https://caotianze.github.io/pandasgwas/)
 ## Licensing information
 ### Source code
```

### Comparing `pandasgwas-1.0.0/pandasgwas/Association.py` & `pandasgwas-1.1.0/pandasgwas/Association.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/Browser.py` & `pandasgwas-1.1.0/pandasgwas/Browser.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/Study.py` & `pandasgwas-1.1.0/pandasgwas/Study.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/Trait.py` & `pandasgwas-1.1.0/pandasgwas/Trait.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/Variant.py` & `pandasgwas-1.1.0/pandasgwas/Variant.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/__init__.py` & `pandasgwas-1.1.0/pandasgwas/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/client.py` & `pandasgwas-1.1.0/pandasgwas/client.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/cytogenetic_bands.csv` & `pandasgwas-1.1.0/pandasgwas/cytogenetic_bands.csv`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/get_associations.py` & `pandasgwas-1.1.0/pandasgwas/get_associations.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/get_studies.py` & `pandasgwas-1.1.0/pandasgwas/get_studies.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/get_traits.py` & `pandasgwas-1.1.0/pandasgwas/get_traits.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/get_variants.py` & `pandasgwas-1.1.0/pandasgwas/get_variants.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/harmonised_list.txt` & `pandasgwas-1.1.0/pandasgwas/harmonised_list.txt`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/set_operation.py` & `pandasgwas-1.1.0/pandasgwas/set_operation.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/summary_statistics.py` & `pandasgwas-1.1.0/pandasgwas/summary_statistics.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas/utility.py` & `pandasgwas-1.1.0/pandasgwas/utility.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/pandasgwas.egg-info/PKG-INFO` & `pandasgwas-1.1.0/pandasgwas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pandasgwas
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python package for easy retrieval of GWAS Catalog data
 Home-page: https://github.com/caotianze/pandasgwas
 Author: Cao Tianze
 Author-email: hnrcao@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/caotianze/pandasgwas/issues
 Keywords: gwas,genomics,snp,bioinformatics,pandas
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pandasGWAS: a Python package for easy retrieval of GWAS Catalog data
 ## News
 On 4 May 2023, the work has been published in BMC Genomics.    
 Starting from V0.99.18, pandasGWAS can cache API requests in memory.    
@@ -71,15 +71,15 @@
 browser(search_DF)
 #Based on index results, download summary statistics data in $Home/pandasgwas_home.
 download(search_DF)
 #Based on the index results, load the data from $Home/pandasgwas_home and convert it into a DataFrame. 
 df = parse(search_DF)
 ```
 ## Dependencies
-python: 3.8  
+python: 3.10  
 pandas: 1.4.3  
 requests: 2.28.1  
 progressbar2: 4.0.0
 ## Documentation
 See [pandasGWAS Documentation](https://caotianze.github.io/pandasgwas/)
 ## Licensing information
 ### Source code
```

### Comparing `pandasgwas-1.0.0/pandasgwas.egg-info/SOURCES.txt` & `pandasgwas-1.1.0/pandasgwas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandasgwas-1.0.0/setup.py` & `pandasgwas-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pandasgwas",
-    version="1.0.0",
+    version="1.1.0",
     author="Cao Tianze",
     author_email="hnrcao@qq.com",
     description="A Python package for easy retrieval of GWAS Catalog data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/caotianze/pandasgwas",
     project_urls={
         "Bug Tracker": "https://github.com/caotianze/pandasgwas/issues",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     # package_dir={"": "pandasgwas"},
     packages=['pandasgwas'],
-    python_requires=">=3.8",
+    python_requires=">=3.10",
     install_requires=['pandas>=1.4.3', 'requests>=2.28.1', 'progressbar2>=4.0.0'],
     license="MIT",
     keywords=['gwas', 'genomics', 'snp', 'bioinformatics','pandas'],
     package_data={
         "": ["*.csv","*.txt"]
     }
 )
```

