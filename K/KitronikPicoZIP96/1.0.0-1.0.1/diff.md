# Comparing `tmp/KitronikPicoZIP96-1.0.0.tar.gz` & `tmp/KitronikPicoZIP96-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KitronikPicoZIP96-1.0.0.tar", last modified: Wed Jun  7 07:23:58 2023, max compression
+gzip compressed data, was "KitronikPicoZIP96-1.0.1.tar", last modified: Wed Jun  7 07:27:46 2023, max compression
```

## Comparing `KitronikPicoZIP96-1.0.0.tar` & `KitronikPicoZIP96-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-06-07 07:23:58.034331 KitronikPicoZIP96-1.0.0/
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-06-07 07:23:58.034331 KitronikPicoZIP96-1.0.0/KitronikPicoZIP96.egg-info/
--rw-r--r--   0 jack      (1000) jack      (1000)     9413 2023-06-07 07:23:57.000000 KitronikPicoZIP96-1.0.0/KitronikPicoZIP96.egg-info/PKG-INFO
--rw-r--r--   0 jack      (1000) jack      (1000)      225 2023-06-07 07:23:58.000000 KitronikPicoZIP96-1.0.0/KitronikPicoZIP96.egg-info/SOURCES.txt
--rw-r--r--   0 jack      (1000) jack      (1000)        1 2023-06-07 07:23:57.000000 KitronikPicoZIP96-1.0.0/KitronikPicoZIP96.egg-info/dependency_links.txt
--rw-r--r--   0 jack      (1000) jack      (1000)       10 2023-06-07 07:23:57.000000 KitronikPicoZIP96-1.0.0/KitronikPicoZIP96.egg-info/top_level.txt
--rw-r--r--   0 jack      (1000) jack      (1000)      379 2023-06-07 07:22:25.000000 KitronikPicoZIP96-1.0.0/KitronikPicoZIP96WheelSetup.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1070 2023-06-06 13:54:06.000000 KitronikPicoZIP96-1.0.0/LICENSE
--rw-r--r--   0 jack      (1000) jack      (1000)     9413 2023-06-07 07:23:58.034331 KitronikPicoZIP96-1.0.0/PKG-INFO
--rw-r--r--   0 jack      (1000) jack      (1000)     9221 2023-06-06 13:54:06.000000 KitronikPicoZIP96-1.0.0/README.md
--rw-r--r--   0 jack      (1000) jack      (1000)     6601 2023-06-06 13:54:06.000000 KitronikPicoZIP96-1.0.0/ZIP96Pico.py
--rw-r--r--   0 jack      (1000) jack      (1000)       38 2023-06-07 07:23:58.034331 KitronikPicoZIP96-1.0.0/setup.cfg
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-06-07 07:27:46.274334 KitronikPicoZIP96-1.0.1/
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-06-07 07:27:46.274334 KitronikPicoZIP96-1.0.1/KitronikPicoZIP96.egg-info/
+-rw-r--r--   0 jack      (1000) jack      (1000)     9412 2023-06-07 07:27:46.000000 KitronikPicoZIP96-1.0.1/KitronikPicoZIP96.egg-info/PKG-INFO
+-rw-r--r--   0 jack      (1000) jack      (1000)      225 2023-06-07 07:27:46.000000 KitronikPicoZIP96-1.0.1/KitronikPicoZIP96.egg-info/SOURCES.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)        1 2023-06-07 07:27:46.000000 KitronikPicoZIP96-1.0.1/KitronikPicoZIP96.egg-info/dependency_links.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)       10 2023-06-07 07:27:46.000000 KitronikPicoZIP96-1.0.1/KitronikPicoZIP96.egg-info/top_level.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)      379 2023-06-07 07:26:33.000000 KitronikPicoZIP96-1.0.1/KitronikPicoZIP96WheelSetup.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1070 2023-06-06 13:54:06.000000 KitronikPicoZIP96-1.0.1/LICENSE
+-rw-r--r--   0 jack      (1000) jack      (1000)     9412 2023-06-07 07:27:46.274334 KitronikPicoZIP96-1.0.1/PKG-INFO
+-rw-r--r--   0 jack      (1000) jack      (1000)     9385 2023-06-07 07:25:57.000000 KitronikPicoZIP96-1.0.1/README.md
+-rw-r--r--   0 jack      (1000) jack      (1000)     6601 2023-06-06 13:54:06.000000 KitronikPicoZIP96-1.0.1/ZIP96Pico.py
+-rw-r--r--   0 jack      (1000) jack      (1000)       38 2023-06-07 07:27:46.274334 KitronikPicoZIP96-1.0.1/setup.cfg
```

