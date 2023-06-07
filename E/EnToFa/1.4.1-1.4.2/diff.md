# Comparing `tmp/EnToFa-1.4.1.tar.gz` & `tmp/EnToFa-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnToFa-1.4.1.tar", last modified: Wed Jun  7 04:54:02 2023, max compression
+gzip compressed data, was "EnToFa-1.4.2.tar", last modified: Wed Jun  7 05:10:12 2023, max compression
```

## Comparing `EnToFa-1.4.1.tar` & `EnToFa-1.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:54:02.904998 EnToFa-1.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:54:02.904998 EnToFa-1.4.1/EnToFa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-07 04:54:02.000000 EnToFa-1.4.1/EnToFa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-07 04:54:02.000000 EnToFa-1.4.1/EnToFa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 04:54:02.000000 EnToFa-1.4.1/EnToFa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 04:54:02.000000 EnToFa-1.4.1/EnToFa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 04:54:02.000000 EnToFa-1.4.1/EnToFa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 04:54:02.000000 EnToFa-1.4.1/EnToFa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-07 04:53:52.000000 EnToFa-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-07 04:54:02.904998 EnToFa-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-07 04:53:52.000000 EnToFa-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 04:54:02.904998 EnToFa-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-07 04:53:52.000000 EnToFa-1.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-07 04:53:52.000000 EnToFa-1.4.1/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:12.877929 EnToFa-1.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:12.877929 EnToFa-1.4.2/EnToFa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-07 05:10:12.000000 EnToFa-1.4.2/EnToFa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-07 05:10:12.000000 EnToFa-1.4.2/EnToFa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 05:10:12.000000 EnToFa-1.4.2/EnToFa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 05:10:12.000000 EnToFa-1.4.2/EnToFa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 05:10:12.000000 EnToFa-1.4.2/EnToFa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 05:10:12.000000 EnToFa-1.4.2/EnToFa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-07 05:09:58.000000 EnToFa-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-07 05:10:12.877929 EnToFa-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-07 05:09:58.000000 EnToFa-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 05:10:12.877929 EnToFa-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-07 05:09:58.000000 EnToFa-1.4.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-07 05:09:58.000000 EnToFa-1.4.2/translator.py
```

### Comparing `EnToFa-1.4.1/EnToFa.egg-info/PKG-INFO` & `EnToFa-1.4.2/EnToFa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnToFa
-Version: 1.4.1
+Version: 1.4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <br>
 
 <h1 align="center">
   Potplayer English To Persian Translator
@@ -12,15 +12,15 @@
 
 <p align="center"><img src="https://raw.githubusercontent.com/jepbura/potplayer-english-to-persian-translator/master/assets/images/07.png" alt="E2F" /></p>
 
 - [What is EnToFa?](#what-is-bura-cli)
 - [Installation Windows](#installation-windows)
 - [Potplayer Settings](#potplayer-settings)
 
-## What is EnToFa?
+## What is [EnToFa](https://pypi.org/project/EnToFa)?
 
 In the normal mode, **Potplayer** can simultaneously translate all the subtitles and, for individual words, if you click on the word, it will open the word's translation in your browser, which may take a considerable amount of time. However, with **EnToFa**, which is a Python code, it translates words from English to Persian instantly. This version is only available for Windows.
 
 ## Installation Windows
 
 After installing `Python` and `pip`, you only need to install `EnToFa` by running the following command:
```

### Comparing `EnToFa-1.4.1/LICENSE` & `EnToFa-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EnToFa-1.4.1/PKG-INFO` & `EnToFa-1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnToFa
-Version: 1.4.1
+Version: 1.4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <br>
 
 <h1 align="center">
   Potplayer English To Persian Translator
@@ -12,15 +12,15 @@
 
 <p align="center"><img src="https://raw.githubusercontent.com/jepbura/potplayer-english-to-persian-translator/master/assets/images/07.png" alt="E2F" /></p>
 
 - [What is EnToFa?](#what-is-bura-cli)
 - [Installation Windows](#installation-windows)
 - [Potplayer Settings](#potplayer-settings)
 
-## What is EnToFa?
+## What is [EnToFa](https://pypi.org/project/EnToFa)?
 
 In the normal mode, **Potplayer** can simultaneously translate all the subtitles and, for individual words, if you click on the word, it will open the word's translation in your browser, which may take a considerable amount of time. However, with **EnToFa**, which is a Python code, it translates words from English to Persian instantly. This version is only available for Windows.
 
 ## Installation Windows
 
 After installing `Python` and `pip`, you only need to install `EnToFa` by running the following command:
```

### Comparing `EnToFa-1.4.1/README.md` & `EnToFa-1.4.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 <p align="center"><img src="https://raw.githubusercontent.com/jepbura/potplayer-english-to-persian-translator/master/assets/images/07.png" alt="E2F" /></p>
 
 - [What is EnToFa?](#what-is-bura-cli)
 - [Installation Windows](#installation-windows)
 - [Potplayer Settings](#potplayer-settings)
 
-## What is EnToFa?
+## What is [EnToFa](https://pypi.org/project/EnToFa)?
 
 In the normal mode, **Potplayer** can simultaneously translate all the subtitles and, for individual words, if you click on the word, it will open the word's translation in your browser, which may take a considerable amount of time. However, with **EnToFa**, which is a Python code, it translates words from English to Persian instantly. This version is only available for Windows.
 
 ## Installation Windows
 
 After installing `Python` and `pip`, you only need to install `EnToFa` by running the following command:
```

### Comparing `EnToFa-1.4.1/translator.py` & `EnToFa-1.4.2/translator.py`

 * *Files identical despite different names*

