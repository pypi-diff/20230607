# Comparing `tmp/autosubmitconfigparser-1.0.33.tar.gz` & `tmp/autosubmitconfigparser-1.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmitconfigparser-1.0.33.tar", last modified: Wed Jun  7 14:00:53 2023, max compression
+gzip compressed data, was "autosubmitconfigparser-1.0.34.tar", last modified: Wed Jun  7 14:22:36 2023, max compression
```

## Comparing `autosubmitconfigparser-1.0.33.tar` & `autosubmitconfigparser-1.0.34.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.33/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2123 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.33/README.md
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/autosubmitconfigparser/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:48:23.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:49:24.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/__init__.py
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/basicconfig.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   104405 2023-06-07 13:56:15.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/configcommon.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/autosubmit-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/autosubmit.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/expdef-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/expdef.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/git-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/jobs-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/jobs.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/local-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/platforms-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/platforms.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      275 2023-06-07 12:06:41.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/yamlparser.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2123 2023-06-07 14:00:52.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1029 2023-06-07 14:00:53.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-06-07 14:00:52.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      338 2023-06-07 14:00:52.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-06-07 14:00:53.000000 autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/top_level.txt
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.33/log/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.33/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.33/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-06-07 14:00:53.286402 autosubmitconfigparser-1.0.33/setup.cfg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1499 2023-06-07 14:00:30.000000 autosubmitconfigparser-1.0.33/setup.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:22:36.717386 autosubmitconfigparser-1.0.34/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.34/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2123 2023-06-07 14:22:36.717386 autosubmitconfigparser-1.0.34/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.34/README.md
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:22:36.713386 autosubmitconfigparser-1.0.34/autosubmitconfigparser/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:48:23.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:22:36.713386 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:49:24.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/__init__.py
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/basicconfig.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   104405 2023-06-07 13:56:15.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/configcommon.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:22:36.717386 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/autosubmit-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/autosubmit.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/expdef-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/expdef.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/git-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/jobs-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/jobs.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/local-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/platforms-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/platforms.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      275 2023-06-07 12:06:41.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/yamlparser.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:22:36.713386 autosubmitconfigparser-1.0.34/autosubmitconfigparser.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2123 2023-06-07 14:22:36.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1029 2023-06-07 14:22:36.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-06-07 14:22:36.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      314 2023-06-07 14:22:36.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-06-07 14:22:36.000000 autosubmitconfigparser-1.0.34/autosubmitconfigparser.egg-info/top_level.txt
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 14:22:36.717386 autosubmitconfigparser-1.0.34/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.34/log/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.34/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.34/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-06-07 14:22:36.717386 autosubmitconfigparser-1.0.34/setup.cfg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1473 2023-06-07 14:22:21.000000 autosubmitconfigparser-1.0.34/setup.py
```

### Comparing `autosubmitconfigparser-1.0.33/PKG-INFO` & `autosubmitconfigparser-1.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.33
+Version: 1.0.34
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 License: UNKNOWN
 Keywords: climate,weather,workflow,HPC
 Platform: UNKNOWN
```

### Comparing `autosubmitconfigparser-1.0.33/README.md` & `autosubmitconfigparser-1.0.34/README.md`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/basicconfig.py` & `autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/basicconfig.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/configcommon.py` & `autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/configcommon.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/expdef-dummy.yml` & `autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/expdef-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/expdef.yml` & `autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/expdef.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/jobs-dummy.yml` & `autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/jobs-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/jobs.yml` & `autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/jobs.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/platforms-dummy.yml` & `autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/platforms-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.33/autosubmitconfigparser/config/files/platforms.yml` & `autosubmitconfigparser-1.0.34/autosubmitconfigparser/config/files/platforms.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/PKG-INFO` & `autosubmitconfigparser-1.0.34/autosubmitconfigparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.33
+Version: 1.0.34
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 License: UNKNOWN
 Keywords: climate,weather,workflow,HPC
 Platform: UNKNOWN
```

### Comparing `autosubmitconfigparser-1.0.33/autosubmitconfigparser.egg-info/SOURCES.txt` & `autosubmitconfigparser-1.0.34/autosubmitconfigparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.33/log/fd_show.py` & `autosubmitconfigparser-1.0.34/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.33/log/log.py` & `autosubmitconfigparser-1.0.34/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.33/setup.py` & `autosubmitconfigparser-1.0.34/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autosubmitconfigparser",
-    version="1.0.33",
+    version="1.0.34",
     author="Daniel Beltran Mora",
     author_email="daniel.beltran@bsc.es",
     description="An utility library that allows to read an Autosubmit 4 experiment configuration.",
     keywords=['climate', 'weather', 'workflow', 'HPC'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git",
     include_package_data=True,
     package_data={'files': ['autosubmitconfigparser/conf/files/*']},
     packages=setuptools.find_packages(),
-    install_requires=['ruamel.yaml==0.17.31','ruamel.yaml.clib==0.2.7','packaging>19', 'six>=1.10.0', 'configobj>=5.0.6', 'argparse>=1.4.0', 'python-dateutil>=2.8.2',
+    install_requires=['ruamel.yaml==0.17.31','packaging>19', 'six>=1.10.0', 'configobj>=5.0.6', 'argparse>=1.4.0', 'python-dateutil>=2.8.2',
                        'pyparsing>=3.0.7',
                       'mock>=4.0.3', 'portalocker>=2.3.2', 'networkx>=2.6.3', 'requests>=2.27.1',
                       'bscearth.utils>=0.5.2', 'cryptography>=36.0.1', 'setuptools>=60.8.2',
                       'pip>=22.0.3', 'pythondialog', 'pytest', 'nose', 'coverage', 'PyNaCl>=1.4.0',
                       'Pygments'],
     classifiers=[
         "Programming Language :: Python :: 3.7",
```

