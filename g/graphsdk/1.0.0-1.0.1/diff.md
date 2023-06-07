# Comparing `tmp/graphsdk-1.0.0.tar.gz` & `tmp/graphsdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphsdk-1.0.0.tar", last modified: Wed Jun  7 09:29:08 2023, max compression
+gzip compressed data, was "graphsdk-1.0.1.tar", last modified: Wed Jun  7 11:21:55 2023, max compression
```

## Comparing `graphsdk-1.0.0.tar` & `graphsdk-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 09:29:08.163501 graphsdk-1.0.0/
--rw-rw-r--   0 codiant   (1000) codiant   (1000)     1079 2023-06-07 09:28:43.000000 graphsdk-1.0.0/LICENSE.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)     1702 2023-06-07 09:29:08.163501 graphsdk-1.0.0/PKG-INFO
--rw-rw-r--   0 codiant   (1000) codiant   (1000)       62 2023-06-07 09:23:51.000000 graphsdk-1.0.0/README.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)       85 2023-06-07 09:22:22.000000 graphsdk-1.0.0/pyproject.toml
--rw-rw-r--   0 codiant   (1000) codiant   (1000)      746 2023-06-07 09:29:08.163501 graphsdk-1.0.0/setup.cfg
-drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 09:29:08.163501 graphsdk-1.0.0/src/
-drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 09:29:08.163501 graphsdk-1.0.0/src/graphsdk.egg-info/
--rw-rw-r--   0 codiant   (1000) codiant   (1000)     1702 2023-06-07 09:29:08.000000 graphsdk-1.0.0/src/graphsdk.egg-info/PKG-INFO
--rw-rw-r--   0 codiant   (1000) codiant   (1000)      191 2023-06-07 09:29:08.000000 graphsdk-1.0.0/src/graphsdk.egg-info/SOURCES.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)        1 2023-06-07 09:29:08.000000 graphsdk-1.0.0/src/graphsdk.egg-info/dependency_links.txt
--rw-rw-r--   0 codiant   (1000) codiant   (1000)        1 2023-06-07 09:29:08.000000 graphsdk-1.0.0/src/graphsdk.egg-info/top_level.txt
+drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 11:21:55.168110 graphsdk-1.0.1/
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)     1079 2023-06-07 09:28:43.000000 graphsdk-1.0.1/LICENSE.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)     1658 2023-06-07 11:21:55.168110 graphsdk-1.0.1/PKG-INFO
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)       62 2023-06-07 09:23:51.000000 graphsdk-1.0.1/README.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)       85 2023-06-07 09:22:22.000000 graphsdk-1.0.1/pyproject.toml
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)      904 2023-06-07 11:21:55.168110 graphsdk-1.0.1/setup.cfg
+drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 11:21:55.168110 graphsdk-1.0.1/src/
+drwxrwxr-x   0 codiant   (1000) codiant   (1000)        0 2023-06-07 11:21:55.168110 graphsdk-1.0.1/src/graphsdk.egg-info/
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)     1658 2023-06-07 11:21:55.000000 graphsdk-1.0.1/src/graphsdk.egg-info/PKG-INFO
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)      226 2023-06-07 11:21:55.000000 graphsdk-1.0.1/src/graphsdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)        1 2023-06-07 11:21:55.000000 graphsdk-1.0.1/src/graphsdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)      162 2023-06-07 11:21:55.000000 graphsdk-1.0.1/src/graphsdk.egg-info/requires.txt
+-rw-rw-r--   0 codiant   (1000) codiant   (1000)        1 2023-06-07 11:21:55.000000 graphsdk-1.0.1/src/graphsdk.egg-info/top_level.txt
```

### Comparing `graphsdk-1.0.0/LICENSE.txt` & `graphsdk-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

