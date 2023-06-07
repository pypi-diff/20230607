# Comparing `tmp/bapsdk-0.1.0.tar.gz` & `tmp/bapsdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bapsdk-0.1.0.tar", last modified: Tue Nov 15 07:39:29 2022, max compression
+gzip compressed data, was "bapsdk-0.1.2.tar", last modified: Wed Jun  7 19:31:57 2023, max compression
```

## Comparing `bapsdk-0.1.0.tar` & `bapsdk-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 z         (1000) z         (1000)        0 2022-11-15 07:39:28.995175 bapsdk-0.1.0/
--rw-rw-r--   0 z         (1000) z         (1000)     1053 2022-11-14 15:41:34.000000 bapsdk-0.1.0/LICENSE
--rw-rw-r--   0 z         (1000) z         (1000)      359 2022-11-15 07:39:28.995175 bapsdk-0.1.0/PKG-INFO
--rw-rw-r--   0 z         (1000) z         (1000)      132 2022-11-15 07:06:36.000000 bapsdk-0.1.0/README.md
-drwxrwxr-x   0 z         (1000) z         (1000)        0 2022-11-15 07:39:28.995175 bapsdk-0.1.0/bap/
--rw-rw-r--   0 z         (1000) z         (1000)       58 2022-11-11 13:15:26.000000 bapsdk-0.1.0/bap/__init__.py
--rw-rw-r--   0 z         (1000) z         (1000)      388 2022-11-11 16:37:48.000000 bapsdk-0.1.0/bap/_aiogram.py
--rw-rw-r--   0 z         (1000) z         (1000)      502 2022-11-11 20:52:01.000000 bapsdk-0.1.0/bap/_bap.py
-drwxrwxr-x   0 z         (1000) z         (1000)        0 2022-11-15 07:39:28.995175 bapsdk-0.1.0/bapsdk.egg-info/
--rw-rw-r--   0 z         (1000) z         (1000)      359 2022-11-15 07:39:28.000000 bapsdk-0.1.0/bapsdk.egg-info/PKG-INFO
--rw-rw-r--   0 z         (1000) z         (1000)      219 2022-11-15 07:39:28.000000 bapsdk-0.1.0/bapsdk.egg-info/SOURCES.txt
--rw-rw-r--   0 z         (1000) z         (1000)        1 2022-11-15 07:39:28.000000 bapsdk-0.1.0/bapsdk.egg-info/dependency_links.txt
--rw-rw-r--   0 z         (1000) z         (1000)       34 2022-11-15 07:39:28.000000 bapsdk-0.1.0/bapsdk.egg-info/requires.txt
--rw-rw-r--   0 z         (1000) z         (1000)        4 2022-11-15 07:39:28.000000 bapsdk-0.1.0/bapsdk.egg-info/top_level.txt
--rw-rw-r--   0 z         (1000) z         (1000)       38 2022-11-15 07:39:28.995175 bapsdk-0.1.0/setup.cfg
--rw-rw-r--   0 z         (1000) z         (1000)      498 2022-11-11 13:08:40.000000 bapsdk-0.1.0/setup.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-07 19:31:57.403482 bapsdk-0.1.2/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1053 2023-06-07 19:03:22.000000 bapsdk-0.1.2/LICENSE
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      399 2023-06-07 19:31:57.399482 bapsdk-0.1.2/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1140 2023-06-07 19:00:05.000000 bapsdk-0.1.2/README.md
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-07 19:31:57.399482 bapsdk-0.1.2/bap/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       58 2023-06-07 18:51:08.000000 bapsdk-0.1.2/bap/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      388 2023-06-07 18:51:08.000000 bapsdk-0.1.2/bap/_aiogram.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      519 2023-06-07 18:56:14.000000 bapsdk-0.1.2/bap/_bap.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-07 19:31:57.399482 bapsdk-0.1.2/bapsdk.egg-info/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      399 2023-06-07 19:31:57.000000 bapsdk-0.1.2/bapsdk.egg-info/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      219 2023-06-07 19:31:57.000000 bapsdk-0.1.2/bapsdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-06-07 19:31:57.000000 bapsdk-0.1.2/bapsdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       34 2023-06-07 19:31:57.000000 bapsdk-0.1.2/bapsdk.egg-info/requires.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        4 2023-06-07 19:31:57.000000 bapsdk-0.1.2/bapsdk.egg-info/top_level.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-06-07 19:31:57.403482 bapsdk-0.1.2/setup.cfg
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      549 2023-06-07 19:31:50.000000 bapsdk-0.1.2/setup.py
```

### Comparing `bapsdk-0.1.0/LICENSE` & `bapsdk-0.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Codd Tech
+Copyright (c) 2022 codd.tech
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

