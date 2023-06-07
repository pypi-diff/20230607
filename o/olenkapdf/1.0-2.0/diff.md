# Comparing `tmp/olenkapdf-1.0.tar.gz` & `tmp/olenkapdf-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/olenkapdf-1.0.tar", last modified: Wed Jun  7 12:50:11 2023, max compression
+gzip compressed data, was "dist/olenkapdf-2.0.tar", last modified: Wed Jun  7 13:04:43 2023, max compression
```

## Comparing `olenkapdf-1.0.tar` & `olenkapdf-2.0.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxr-xr-x   0 olenkasalo   (501) staff       (20)        0 2023-06-07 12:50:11.904350 olenkapdf-1.0/
--rw-r--r--   0 olenkasalo   (501) staff       (20)      210 2023-06-07 12:50:11.903617 olenkapdf-1.0/PKG-INFO
--rw-r--r--   0 olenkasalo   (501) staff       (20)       36 2023-06-07 12:43:31.000000 olenkapdf-1.0/README.md
-drwxr-xr-x   0 olenkasalo   (501) staff       (20)        0 2023-06-07 12:50:11.902698 olenkapdf-1.0/olenkapdf.egg-info/
--rw-r--r--   0 olenkasalo   (501) staff       (20)      210 2023-06-07 12:50:11.000000 olenkapdf-1.0/olenkapdf.egg-info/PKG-INFO
--rw-r--r--   0 olenkasalo   (501) staff       (20)      150 2023-06-07 12:50:11.000000 olenkapdf-1.0/olenkapdf.egg-info/SOURCES.txt
--rw-r--r--   0 olenkasalo   (501) staff       (20)        1 2023-06-07 12:50:11.000000 olenkapdf-1.0/olenkapdf.egg-info/dependency_links.txt
--rw-r--r--   0 olenkasalo   (501) staff       (20)        1 2023-06-07 12:50:11.000000 olenkapdf-1.0/olenkapdf.egg-info/top_level.txt
--rw-r--r--   0 olenkasalo   (501) staff       (20)       38 2023-06-07 12:50:11.904557 olenkapdf-1.0/setup.cfg
--rw-r--r--   0 olenkasalo   (501) staff       (20)      221 2023-06-07 12:43:31.000000 olenkapdf-1.0/setup.py
+drwxr-xr-x   0 olenkasalo   (501) staff       (20)        0 2023-06-07 13:04:43.598004 olenkapdf-2.0/
+-rw-r--r--   0 olenkasalo   (501) staff       (20)      210 2023-06-07 13:04:43.597521 olenkapdf-2.0/PKG-INFO
+-rw-r--r--   0 olenkasalo   (501) staff       (20)       36 2023-06-07 12:43:31.000000 olenkapdf-2.0/README.md
+drwxr-xr-x   0 olenkasalo   (501) staff       (20)        0 2023-06-07 13:04:43.586522 olenkapdf-2.0/olenkapdf/
+-rw-r--r--   0 olenkasalo   (501) staff       (20)        0 2023-06-07 12:35:32.000000 olenkapdf-2.0/olenkapdf/__init__.py
+-rw-r--r--   0 olenkasalo   (501) staff       (20)        0 2023-06-07 12:36:41.000000 olenkapdf-2.0/olenkapdf/pdf2image.py
+-rw-r--r--   0 olenkasalo   (501) staff       (20)       36 2023-06-07 12:36:28.000000 olenkapdf-2.0/olenkapdf/pdf2text.py
+drwxr-xr-x   0 olenkasalo   (501) staff       (20)        0 2023-06-07 13:04:43.596047 olenkapdf-2.0/olenkapdf.egg-info/
+-rw-r--r--   0 olenkasalo   (501) staff       (20)      210 2023-06-07 13:04:43.000000 olenkapdf-2.0/olenkapdf.egg-info/PKG-INFO
+-rw-r--r--   0 olenkasalo   (501) staff       (20)      217 2023-06-07 13:04:43.000000 olenkapdf-2.0/olenkapdf.egg-info/SOURCES.txt
+-rw-r--r--   0 olenkasalo   (501) staff       (20)        1 2023-06-07 13:04:43.000000 olenkapdf-2.0/olenkapdf.egg-info/dependency_links.txt
+-rw-r--r--   0 olenkasalo   (501) staff       (20)       10 2023-06-07 13:04:43.000000 olenkapdf-2.0/olenkapdf.egg-info/top_level.txt
+-rw-r--r--   0 olenkasalo   (501) staff       (20)       38 2023-06-07 13:04:43.598181 olenkapdf-2.0/setup.cfg
+-rw-r--r--   0 olenkasalo   (501) staff       (20)      221 2023-06-07 13:04:14.000000 olenkapdf-2.0/setup.py
```

