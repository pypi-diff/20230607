# Comparing `tmp/geneCGR-1.1.tar.gz` & `tmp/geneCGR-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneCGR-1.1.tar", last modified: Wed Jun  7 09:24:25 2023, max compression
+gzip compressed data, was "geneCGR-1.2.tar", last modified: Wed Jun  7 15:01:12 2023, max compression
```

## Comparing `geneCGR-1.1.tar` & `geneCGR-1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 09:24:25.651558 geneCGR-1.1/
--rw-rw-rw-   0        0        0      136 2023-06-07 09:24:25.651558 geneCGR-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-07 09:24:25.651558 geneCGR-1.1/geneCGR/
--rw-rw-rw-   0        0        0      461 2023-06-07 09:24:12.000000 geneCGR-1.1/geneCGR/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:24:25.651558 geneCGR-1.1/geneCGR.egg-info/
--rw-rw-rw-   0        0        0      136 2023-06-07 09:24:25.000000 geneCGR-1.1/geneCGR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-06-07 09:24:25.000000 geneCGR-1.1/geneCGR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 09:24:25.000000 geneCGR-1.1/geneCGR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 09:24:25.000000 geneCGR-1.1/geneCGR.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 09:24:25.651558 geneCGR-1.1/setup.cfg
--rw-rw-rw-   0        0        0      217 2023-06-07 09:24:18.000000 geneCGR-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:01:12.763994 geneCGR-1.2/
+-rw-rw-rw-   0        0        0      136 2023-06-07 15:01:12.763994 geneCGR-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-07 15:01:12.763994 geneCGR-1.2/geneCGR/
+-rw-rw-rw-   0        0        0      463 2023-06-07 15:01:06.000000 geneCGR-1.2/geneCGR/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 15:01:12.763994 geneCGR-1.2/geneCGR.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-06-07 15:01:12.000000 geneCGR-1.2/geneCGR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-06-07 15:01:12.000000 geneCGR-1.2/geneCGR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 15:01:12.000000 geneCGR-1.2/geneCGR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-07 15:01:12.000000 geneCGR-1.2/geneCGR.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 15:01:12.763994 geneCGR-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      217 2023-06-07 15:01:03.000000 geneCGR-1.2/setup.py
```

