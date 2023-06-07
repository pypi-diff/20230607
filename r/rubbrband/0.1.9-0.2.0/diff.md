# Comparing `tmp/rubbrband-0.1.9.tar.gz` & `tmp/rubbrband-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubbrband-0.1.9.tar", last modified: Thu Feb 23 01:33:12 2023, max compression
+gzip compressed data, was "rubbrband-0.2.0.tar", last modified: Wed Jun  7 21:40:18 2023, max compression
```

## Comparing `rubbrband-0.1.9.tar` & `rubbrband-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,17 @@
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.395436 rubbrband-0.1.9/
--rw-r--r--   0 llewyn     (501) staff       (20)       36 2023-02-21 21:59:17.000000 rubbrband-0.1.9/MANIFEST.in
--rw-r--r--   0 llewyn     (501) staff       (20)       53 2023-02-23 01:33:12.395485 rubbrband-0.1.9/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)        6 2023-02-17 20:36:16.000000 rubbrband-0.1.9/README.md
--rw-r--r--   0 llewyn     (501) staff       (20)      126 2023-02-20 21:41:06.000000 rubbrband-0.1.9/pyproject.toml
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.393328 rubbrband-0.1.9/rubbrband/
--rw-r--r--   0 llewyn     (501) staff       (20)     6658 2023-02-23 01:20:10.000000 rubbrband-0.1.9/rubbrband/cli.py
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.392605 rubbrband-0.1.9/rubbrband/models/
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.394217 rubbrband-0.1.9/rubbrband/models/ControlNet/
--rw-r--r--   0 llewyn     (501) staff       (20)     2071 2023-02-20 19:35:42.000000 rubbrband-0.1.9/rubbrband/models/ControlNet/Dockerfile
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.394331 rubbrband-0.1.9/rubbrband/models/ControlNet/library-scripts/
--rw-r--r--   0 llewyn     (501) staff       (20)    11000 2023-02-20 19:35:42.000000 rubbrband-0.1.9/rubbrband/models/ControlNet/library-scripts/common-debian.sh
--rw-r--r--   0 llewyn     (501) staff       (20)      429 2023-02-22 18:14:48.000000 rubbrband-0.1.9/rubbrband/models/ControlNet/train.sh
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.394674 rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/
--rw-r--r--   0 llewyn     (501) staff       (20)     4750 2023-02-22 18:15:02.000000 rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/Dockerfile
--rw-r--r--   0 llewyn     (501) staff       (20)      762 2023-02-23 01:07:27.000000 rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/infer.sh
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.394783 rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/library-scripts/
--rw-r--r--   0 llewyn     (501) staff       (20)    11000 2023-02-20 19:35:42.000000 rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/library-scripts/common-debian.sh
--rw-r--r--   0 llewyn     (501) staff       (20)     2130 2023-02-23 01:07:27.000000 rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/train.sh
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.395120 rubbrband-0.1.9/rubbrband/models/LoRA/
--rw-r--r--   0 llewyn     (501) staff       (20)     1886 2023-02-22 18:14:48.000000 rubbrband-0.1.9/rubbrband/models/LoRA/Dockerfile
--rwxr-xr-x   0 llewyn     (501) staff       (20)       74 2023-02-23 01:20:39.000000 rubbrband-0.1.9/rubbrband/models/LoRA/infer.sh
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.395339 rubbrband-0.1.9/rubbrband/models/LoRA/library-scripts/
--rw-r--r--   0 llewyn     (501) staff       (20)    11000 2023-02-20 19:35:42.000000 rubbrband-0.1.9/rubbrband/models/LoRA/library-scripts/common-debian.sh
--rw-r--r--   0 llewyn     (501) staff       (20)      951 2023-02-23 01:21:11.000000 rubbrband-0.1.9/rubbrband/models/LoRA/library-scripts/infer.py
--rwxr-xr-x   0 llewyn     (501) staff       (20)      824 2023-02-20 19:35:42.000000 rubbrband-0.1.9/rubbrband/models/LoRA/train.sh
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.393992 rubbrband-0.1.9/rubbrband.egg-info/
--rw-r--r--   0 llewyn     (501) staff       (20)       53 2023-02-23 01:33:12.000000 rubbrband-0.1.9/rubbrband.egg-info/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)      848 2023-02-23 01:33:12.000000 rubbrband-0.1.9/rubbrband.egg-info/SOURCES.txt
--rw-r--r--   0 llewyn     (501) staff       (20)        1 2023-02-23 01:33:12.000000 rubbrband-0.1.9/rubbrband.egg-info/dependency_links.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       49 2023-02-23 01:33:12.000000 rubbrband-0.1.9/rubbrband.egg-info/entry_points.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       27 2023-02-23 01:33:12.000000 rubbrband-0.1.9/rubbrband.egg-info/requires.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       10 2023-02-23 01:33:12.000000 rubbrband-0.1.9/rubbrband.egg-info/top_level.txt
--rw-r--r--   0 llewyn     (501) staff       (20)      240 2023-02-23 01:33:12.395699 rubbrband-0.1.9/setup.cfg
--rw-r--r--   0 llewyn     (501) staff       (20)      182 2023-02-21 22:05:53.000000 rubbrband-0.1.9/setup.py
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-07 21:40:18.519135 rubbrband-0.2.0/
+-rw-r--r--   0 llewyn     (501) staff       (20)    11357 2023-03-07 10:22:28.000000 rubbrband-0.2.0/LICENSE
+-rw-r--r--   0 llewyn     (501) staff       (20)       48 2023-02-24 08:26:52.000000 rubbrband-0.2.0/MANIFEST.in
+-rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-07 21:40:18.519189 rubbrband-0.2.0/PKG-INFO
+-rw-r--r--   0 llewyn     (501) staff       (20)       54 2023-06-07 21:39:04.000000 rubbrband-0.2.0/README.md
+-rw-r--r--   0 llewyn     (501) staff       (20)       93 2023-06-07 21:38:14.000000 rubbrband-0.2.0/pyproject.toml
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-07 21:40:18.518301 rubbrband-0.2.0/rubbrband/
+-rw-r--r--   0 llewyn     (501) staff       (20)       47 2023-06-07 21:36:31.000000 rubbrband-0.2.0/rubbrband/__init__.py
+-rw-r--r--   0 llewyn     (501) staff       (20)      755 2023-06-07 21:36:24.000000 rubbrband-0.2.0/rubbrband/main.py
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-07 21:40:18.519015 rubbrband-0.2.0/rubbrband.egg-info/
+-rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-07 21:40:18.000000 rubbrband-0.2.0/rubbrband.egg-info/PKG-INFO
+-rw-r--r--   0 llewyn     (501) staff       (20)      267 2023-06-07 21:40:18.000000 rubbrband-0.2.0/rubbrband.egg-info/SOURCES.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)        1 2023-06-07 21:40:18.000000 rubbrband-0.2.0/rubbrband.egg-info/dependency_links.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)        9 2023-06-07 21:40:18.000000 rubbrband-0.2.0/rubbrband.egg-info/requires.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)       10 2023-06-07 21:40:18.000000 rubbrband-0.2.0/rubbrband.egg-info/top_level.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)      251 2023-06-07 21:40:18.519392 rubbrband-0.2.0/setup.cfg
+-rw-r--r--   0 llewyn     (501) staff       (20)      172 2023-06-07 21:37:58.000000 rubbrband-0.2.0/setup.py
```

