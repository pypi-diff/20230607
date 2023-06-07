# Comparing `tmp/dghs-imgutils-0.1.0.tar.gz` & `tmp/dghs-imgutils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dghs-imgutils-0.1.0.tar", last modified: Thu May 18 08:52:53 2023, max compression
+gzip compressed data, was "dghs-imgutils-0.1.1.tar", last modified: Wed Jun  7 14:23:11 2023, max compression
```

## Comparing `dghs-imgutils-0.1.0.tar` & `dghs-imgutils-0.1.1.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.610600 dghs-imgutils-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-18 08:51:55.000000 dghs-imgutils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-18 08:51:55.000000 dghs-imgutils-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-18 08:51:55.000000 dghs-imgutils-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/dghs_imgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-05-18 08:52:53.000000 dghs-imgutils-0.1.0/dghs_imgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-18 08:52:53.000000 dghs-imgutils-0.1.0/dghs_imgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:52:53.000000 dghs-imgutils-0.1.0/dghs_imgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-18 08:52:53.000000 dghs-imgutils-0.1.0/dghs_imgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 08:52:53.000000 dghs-imgutils-0.1.0/dghs_imgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/data/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/data/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/data/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/data/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/data/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/detect/_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/detect/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/detect/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/detect/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/detect/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/edge/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/edge/canny.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/edge/lineart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/edge/lineart_anime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/metrics/aesthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/metrics/lpips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/metrics/psnr_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/segment/isnetis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/tagging/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/tagging/deepdanbooru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/tagging/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/tagging/mldanbooru.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/tagging/wd14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/utils/onnxruntime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/validate/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/validate/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/validate/monochrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/validate/truncate.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/requirements-zoo.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:52:53.610600 dghs-imgutils-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.735640 dghs-imgutils-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 14:22:09.000000 dghs-imgutils-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-07 14:22:09.000000 dghs-imgutils-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-06-07 14:23:11.735640 dghs-imgutils-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-06-07 14:22:09.000000 dghs-imgutils-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/dghs_imgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-06-07 14:23:11.000000 dghs-imgutils-0.1.1/dghs_imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-07 14:23:11.000000 dghs-imgutils-0.1.1/dghs_imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:23:11.000000 dghs-imgutils-0.1.1/dghs_imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-07 14:23:11.000000 dghs-imgutils-0.1.1/dghs_imgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 14:23:11.000000 dghs-imgutils-0.1.1/dghs_imgutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/data/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/data/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/data/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/data/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/detect/_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/detect/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/detect/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/detect/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/detect/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/edge/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/edge/canny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/edge/lineart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/edge/lineart_anime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/metrics/aesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/metrics/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/metrics/psnr_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/segment/isnetis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.731640 dghs-imgutils-0.1.1/imgutils/tagging/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/tagging/deepdanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/tagging/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/tagging/mldanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/tagging/wd14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.735640 dghs-imgutils-0.1.1/imgutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/utils/onnxruntime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:11.735640 dghs-imgutils-0.1.1/imgutils/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/validate/aicheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/validate/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/validate/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/validate/monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/imgutils/validate/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/requirements-zoo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:23:11.735640 dghs-imgutils-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-07 14:22:10.000000 dghs-imgutils-0.1.1/setup.py
```

### Comparing `dghs-imgutils-0.1.0/LICENSE` & `dghs-imgutils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/PKG-INFO` & `dghs-imgutils-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.1.0
+Version: 0.1.1
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: doc
 Provides-Extra: gpu
 Provides-Extra: test
+Provides-Extra: doc
 License-File: LICENSE
 
 # imgutils
 
 [![PyPI](https://img.shields.io/pypi/v/dghs-imgutils)](https://pypi.org/project/dghs-imgutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dghs-imgutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/loc.json)
@@ -92,32 +92,36 @@
 # [0, 0, 0, 1, 1, -1, -1, -1, -1]
 ```
 
 ### Object Detection
 
 Currently, object detection is supported for anime heads and person, as shown below
 
+* Face Detection
+
+![face detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/face_detect_demo.plot.py.svg)
+
 * Head Detection
 
-![head detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/head_detect.plot.py.svg)
+![head detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/head_detect_demo.plot.py.svg)
 
 * Person Detection
 
-![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect.plot.py.svg)
+![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect_demo.plot.py.svg)
 
 Based on practical tests, head detection currently has a very stable performance and can be used for automation tasks.
 However, person detection is still being further iterated and will focus on enhancing detection capabilities for
 artistic illustrations in the future.
 
 ### Edge Detection / Lineart Generation
 
 Anime images can be converted to line drawings using the model provided
 by [patrickvonplaten/controlnet_aux](https://github.com/patrickvonplaten/controlnet_aux), as shown below.
 
-![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge.plot.py.svg)
+![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge_demo.plot.py.svg)
 
 It is worth noting that the `lineart` model may consume more computational resources, while `canny` is the fastest but
 has average effect. Therefore, `lineart_anime` may be the most balanced choice in most cases.
 
 ### Monochrome Image Detection
 
 When filtering the crawled images, we need to remove monochrome images. However, monochrome images are often not simply
```

### Comparing `dghs-imgutils-0.1.0/README.md` & `dghs-imgutils-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,32 +67,36 @@
 # [0, 0, 0, 1, 1, -1, -1, -1, -1]
 ```
 
 ### Object Detection
 
 Currently, object detection is supported for anime heads and person, as shown below
 
+* Face Detection
+
+![face detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/face_detect_demo.plot.py.svg)
+
 * Head Detection
 
-![head detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/head_detect.plot.py.svg)
+![head detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/head_detect_demo.plot.py.svg)
 
 * Person Detection
 
-![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect.plot.py.svg)
+![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect_demo.plot.py.svg)
 
 Based on practical tests, head detection currently has a very stable performance and can be used for automation tasks.
 However, person detection is still being further iterated and will focus on enhancing detection capabilities for
 artistic illustrations in the future.
 
 ### Edge Detection / Lineart Generation
 
 Anime images can be converted to line drawings using the model provided
 by [patrickvonplaten/controlnet_aux](https://github.com/patrickvonplaten/controlnet_aux), as shown below.
 
-![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge.plot.py.svg)
+![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge_demo.plot.py.svg)
 
 It is worth noting that the `lineart` model may consume more computational resources, while `canny` is the fastest but
 has average effect. Therefore, `lineart_anime` may be the most balanced choice in most cases.
 
 ### Monochrome Image Detection
 
 When filtering the crawled images, we need to remove monochrome images. However, monochrome images are often not simply
```

### Comparing `dghs-imgutils-0.1.0/dghs_imgutils.egg-info/PKG-INFO` & `dghs-imgutils-0.1.1/dghs_imgutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.1.0
+Version: 0.1.1
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: doc
 Provides-Extra: gpu
 Provides-Extra: test
+Provides-Extra: doc
 License-File: LICENSE
 
 # imgutils
 
 [![PyPI](https://img.shields.io/pypi/v/dghs-imgutils)](https://pypi.org/project/dghs-imgutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dghs-imgutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/loc.json)
@@ -92,32 +92,36 @@
 # [0, 0, 0, 1, 1, -1, -1, -1, -1]
 ```
 
 ### Object Detection
 
 Currently, object detection is supported for anime heads and person, as shown below
 
+* Face Detection
+
+![face detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/face_detect_demo.plot.py.svg)
+
 * Head Detection
 
-![head detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/head_detect.plot.py.svg)
+![head detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/head_detect_demo.plot.py.svg)
 
 * Person Detection
 
-![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect.plot.py.svg)
+![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect_demo.plot.py.svg)
 
 Based on practical tests, head detection currently has a very stable performance and can be used for automation tasks.
 However, person detection is still being further iterated and will focus on enhancing detection capabilities for
 artistic illustrations in the future.
 
 ### Edge Detection / Lineart Generation
 
 Anime images can be converted to line drawings using the model provided
 by [patrickvonplaten/controlnet_aux](https://github.com/patrickvonplaten/controlnet_aux), as shown below.
 
-![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge.plot.py.svg)
+![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge_demo.plot.py.svg)
 
 It is worth noting that the `lineart` model may consume more computational resources, while `canny` is the fastest but
 has average effect. Therefore, `lineart_anime` may be the most balanced choice in most cases.
 
 ### Monochrome Image Detection
 
 When filtering the crawled images, we need to remove monochrome images. However, monochrome images are often not simply
```

### Comparing `dghs-imgutils-0.1.0/dghs_imgutils.egg-info/SOURCES.txt` & `dghs-imgutils-0.1.1/dghs_imgutils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -42,10 +42,12 @@
 imgutils/tagging/deepdanbooru.py
 imgutils/tagging/format.py
 imgutils/tagging/mldanbooru.py
 imgutils/tagging/wd14.py
 imgutils/utils/__init__.py
 imgutils/utils/onnxruntime.py
 imgutils/validate/__init__.py
+imgutils/validate/aicheck.py
+imgutils/validate/classify.py
 imgutils/validate/color.py
 imgutils/validate/monochrome.py
 imgutils/validate/truncate.py
```

### Comparing `dghs-imgutils-0.1.0/dghs_imgutils.egg-info/requires.txt` & `dghs-imgutils-0.1.1/dghs_imgutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/config/meta.py` & `dghs-imgutils-0.1.1/imgutils/config/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Meta information for imgutils package.
 """
 
 #: Title of this project (should be `imgutils`).
 __TITLE__ = 'imgutils'
 
 #: Version of this project.
-__VERSION__ = '0.1.0'
+__VERSION__ = '0.1.1'
 
 #: Short description of the project, will be included in ``setup.py``.
 __DESCRIPTION__ = 'A convenient and user-friendly anime-style image data processing library that integrates ' \
                   'various advanced anime-style image processing models.'
 
 #: Author of this project.
 __AUTHOR__ = 'narugo1992, 7eu7d'
```

### Comparing `dghs-imgutils-0.1.0/imgutils/data/background.py` & `dghs-imgutils-0.1.1/imgutils/data/background.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/data/decode.py` & `dghs-imgutils-0.1.1/imgutils/data/decode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/data/encode.py` & `dghs-imgutils-0.1.1/imgutils/data/encode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/data/image.py` & `dghs-imgutils-0.1.1/imgutils/data/image.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/data/layer.py` & `dghs-imgutils-0.1.1/imgutils/data/layer.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/detect/_yolo.py` & `dghs-imgutils-0.1.1/imgutils/detect/_yolo.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/detect/face.py` & `dghs-imgutils-0.1.1/imgutils/detect/face.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,54 +9,53 @@
         :align: center
 
     This is an overall benchmark of all the face detect models:
 
     .. image:: face_detect_benchmark.plot.py.svg
         :align: center
 
+    The models are hosted on
+    `huggingface - deepghs/anime_face_detection <https://huggingface.co/deepghs/anime_face_detection>`_.
+
 """
 from functools import lru_cache
 from typing import List, Tuple
 
 from huggingface_hub import hf_hub_download
 
 from ._yolo import _image_preprocess, _data_postprocess
 from ..data import ImageTyping, load_image, rgb_encode
 from ..utils import open_onnx_model
 
-_VERSIONS = {
-    'v0': '',
-    'v1': 'v1_',
-}
-
 
 @lru_cache()
-def _open_face_detect_model(level: str = 's', version: str = 'v1'):
+def _open_face_detect_model(level: str = 's', version: str = 'v1.4'):
     return open_onnx_model(hf_hub_download(
-        'deepghs/imgutils-models',
-        f'face_detect/face_detect_{_VERSIONS[version]}best_{level}.onnx'
+        f'deepghs/anime_face_detection',
+        f'face_detect_{version}_{level}/model.onnx'
     ))
 
 
-def detect_faces(image: ImageTyping, level: str = 's', version: str = 'v1', max_infer_size=640,
-                 conf_threshold: float = 0.45, iou_threshold: float = 0.7) \
+def detect_faces(image: ImageTyping, level: str = 's', version: str = 'v1.4', max_infer_size=640,
+                 conf_threshold: float = 0.25, iou_threshold: float = 0.7) \
         -> List[Tuple[Tuple[int, int, int, int], str, float]]:
     """
     Overview:
         Detect human faces in anime images.
 
     :param image: Image to detect.
     :param level: The model level being used can be either `s` or `n`.
         The `n` model runs faster with smaller system overface, while the `s` model achieves higher accuracy.
         The default value is `s`.
-    :param version: Version of model, default is ``v1``. Available versions are ``v0`` and ``v1``.
+    :param version: Version of model, default is ``v1.4``.
+        Available versions are ``v0``, ``v1``, ``v1.3`` and ``v1.4``.
     :param max_infer_size: The maximum image size used for model inference, if the image size exceeds this limit,
         the image will be resized and used for inference. The default value is `640` pixels.
     :param conf_threshold: The confidence threshold, only detection results with confidence scores above
-        this threshold will be returned. The default value is `0.45`.
+        this threshold will be returned. The default value is `0.25`.
     :param iou_threshold: The detection area coverage overlap threshold, areas with overlaps above this threshold
         will be discarded. The default value is `0.7`.
     :return: The detection results list, each item includes the detected area `(x0, y0, x1, y1)`,
         the target type (always `face`) and the target confidence score.
 
     Examples::
         >>> from imgutils.detect import detect_faces, detection_visualize
```

### Comparing `dghs-imgutils-0.1.0/imgutils/detect/head.py` & `dghs-imgutils-0.1.1/imgutils/detect/head.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/detect/person.py` & `dghs-imgutils-0.1.1/imgutils/detect/person.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/detect/visual.py` & `dghs-imgutils-0.1.1/imgutils/detect/visual.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/edge/__init__.py` & `dghs-imgutils-0.1.1/imgutils/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/edge/_base.py` & `dghs-imgutils-0.1.1/imgutils/edge/_base.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/edge/canny.py` & `dghs-imgutils-0.1.1/imgutils/edge/canny.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/edge/lineart.py` & `dghs-imgutils-0.1.1/imgutils/edge/lineart.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/edge/lineart_anime.py` & `dghs-imgutils-0.1.1/imgutils/edge/lineart_anime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/metrics/aesthetic.py` & `dghs-imgutils-0.1.1/imgutils/metrics/aesthetic.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/metrics/lpips.py` & `dghs-imgutils-0.1.1/imgutils/metrics/lpips.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/metrics/psnr_.py` & `dghs-imgutils-0.1.1/imgutils/metrics/psnr_.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/segment/isnetis.py` & `dghs-imgutils-0.1.1/imgutils/segment/isnetis.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/tagging/deepdanbooru.py` & `dghs-imgutils-0.1.1/imgutils/tagging/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/tagging/format.py` & `dghs-imgutils-0.1.1/imgutils/tagging/format.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/tagging/mldanbooru.py` & `dghs-imgutils-0.1.1/imgutils/tagging/mldanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/tagging/wd14.py` & `dghs-imgutils-0.1.1/imgutils/tagging/wd14.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/utils/onnxruntime.py` & `dghs-imgutils-0.1.1/imgutils/utils/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/validate/color.py` & `dghs-imgutils-0.1.1/imgutils/validate/color.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/imgutils/validate/monochrome.py` & `dghs-imgutils-0.1.1/imgutils/validate/monochrome.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     .. image:: monochrome.plot.py.svg
         :align: center
 
     This is an overall benchmark of all the monochrome validation models:
 
     .. image:: monochrome_benchmark.plot.py.svg
         :align: center
+
+    The models are hosted on `huggingface - deepghs/monochrome_detect <https://huggingface.co/deepghs/monochrome_detect>`_.
 """
 from functools import lru_cache
 from typing import Optional, Tuple, Mapping
 
 import numpy as np
 from PIL import Image
 from huggingface_hub import hf_hub_download
@@ -24,26 +26,29 @@
 from ..utils import open_onnx_model
 
 __all__ = [
     'get_monochrome_score',
     'is_monochrome',
 ]
 
-_MODELS: Mapping[int, str] = {
-    0: 'monochrome-caformer-110.onnx',
-    2: 'monochrome-caformer_safe2-80.onnx',
-    4: 'monochrome-caformer_safe4-70.onnx',
+_MODELS: Mapping[Tuple[str, bool], str] = {
+    ('caformer_s36', False): 'caformer_s36_plus',
+    ('caformer_s36', True): 'caformer_s36_plus_safe2',
+    ('mobilenetv3', False): 'mobilenetv3_large_100',
+    ('mobilenetv3', True): 'mobilenetv3_large_100_safe2',
+    ('mobilenetv3_dist', False): 'mobilenetv3_large_100_dist',
+    ('mobilenetv3_dist', True): 'mobilenetv3_large_100_dist_safe2',
 }
 
 
 @lru_cache()
-def _monochrome_validate_model(ckpt):
+def _monochrome_validate_model(model: str, safe: bool):
     return open_onnx_model(hf_hub_download(
-        'deepghs/imgutils-models',
-        f'monochrome/{ckpt}'
+        f'deepghs/monochrome_detect',
+        f'{_MODELS[(model, safe)]}/model.onnx',
     ))
 
 
 def _2d_encode(image: Image.Image, size: Tuple[int, int] = (384, 384),
                normalize: Optional[Tuple[float, float]] = (0.5, 0.5)):
     image = image.resize(size, Image.BILINEAR)
     data = rgb_encode(image, order_='CHW')
@@ -53,72 +58,76 @@
         mean = np.asarray([mean_]).reshape((-1, 1, 1))
         std = np.asarray([std_]).reshape((-1, 1, 1))
         data = (data - mean) / std
 
     return data
 
 
-def get_monochrome_score(image: ImageTyping, safe: int = 2) -> float:
+def get_monochrome_score(image: ImageTyping, model: str = 'mobilenetv3_dist', safe: bool = True) -> float:
     """
     Overview:
         Get monochrome score of the given image.
 
     :param image: Image to predict, can be a ``PIL.Image`` object or the path of the image file.
-    :param safe: Safe level, with optional values including ``0``, ``2``, and ``4``,
-        corresponding to different levels of the model. The default value is 2.
-        For more technical details about this model, please refer to:
-        https://huggingface.co/deepghs/imgutils-models#monochrome .
+    :param model: The model used for inference. The default value is ``mobilenetv3_dist``,
+        which offers high runtime performance. If you need better accuracy, just use ``caformer_s36``.
+    :param safe: Whether to enable the safe mode. When enabled, calculations will be performed using a model
+        with higher precision but lower recall. The default value is ``True``.
 
     Examples::
-        >>> import os
         >>> from imgutils.validate import get_monochrome_score
         >>>
         >>> get_monochrome_score('mono/1.jpg')  # monochrome images
-        0.9789709448814392
+        0.9614395499229431
         >>> get_monochrome_score('mono/2.jpg')
-        0.973383903503418
+        0.9458909034729004
         >>> get_monochrome_score('mono/3.jpg')
-        0.9789378046989441
+        0.9559807777404785
         >>> get_monochrome_score('mono/4.jpg')
-        0.9920350909233093
+        0.9651952981948853
         >>> get_monochrome_score('mono/5.jpg')
-        0.9865685701370239
+        0.9379720687866211
         >>> get_monochrome_score('mono/6.jpg')
-        0.9589458703994751
+        0.8814834356307983
+        >>>
         >>> get_monochrome_score('colored/7.jpg')  # colored images
-        0.019315600395202637
+        0.03941023349761963
         >>> get_monochrome_score('colored/8.jpg')
-        0.008630834519863129
+        0.07492382079362869
         >>> get_monochrome_score('colored/9.jpg')
-        0.08635691553354263
+        0.09546589106321335
         >>> get_monochrome_score('colored/10.jpg')
-        0.01357574388384819
+        0.016521310433745384
         >>> get_monochrome_score('colored/11.jpg')
-        0.00710612116381526
+        0.005693843588232994
         >>> get_monochrome_score('colored/12.jpg')
-        0.025258518755435944
+        0.0315730981528759
     """
-    if safe not in _MODELS:
-        raise ValueError(f'Safe level should be one of {set(sorted(_MODELS.keys()))!r}, but {safe!r} found.')
+    safe = bool(safe)
+    if (model, safe) not in _MODELS:
+        raise ValueError(f'Unknown model for monochrome detection - {model!r}, {safe!r}.')
 
     image = load_image(image, mode='RGB')
     input_data = _2d_encode(image).astype(np.float32)
     input_data = np.stack([input_data])
-    output_data, = _monochrome_validate_model(_MODELS[safe]).run(['output'], {'input': input_data})
-    return float(output_data[0][1])
+    output_data, = _monochrome_validate_model(model, safe).run(['output'], {'input': input_data})
+    return output_data[0][0].item()
 
 
-def is_monochrome(image: ImageTyping, threshold: float = 0.5, safe: int = 2) -> bool:
+def is_monochrome(image: ImageTyping, threshold: float = 0.5,
+                  model: str = 'mobilenetv3_dist', safe: bool = True) -> bool:
     """
     Overview:
         Predict if the image is monochrome.
 
     :param image: Image to predict, can be a ``PIL.Image`` object or the path of the image file.
     :param threshold: Threshold value during prediction. If the score is higher than the threshold,
         the image will be classified as monochrome.
+    :param model: The model used for inference. The default value is ``mobilenetv3_dist``,
+        which offers high runtime performance. If you need better accuracy, just use ``caformer_s36``.
     :param safe: Safe level, with optional values including ``0``, ``2``, and ``4``,
         corresponding to different levels of the model. The default value is 2.
         For more technical details about this model, please refer to:
         https://huggingface.co/deepghs/imgutils-models#monochrome .
 
     Examples:
         >>> import os
@@ -145,8 +154,8 @@
         >>> is_monochrome('colored/10.jpg')
         False
         >>> is_monochrome('colored/11.jpg')
         False
         >>> is_monochrome('colored/12.jpg')
         False
     """
-    return get_monochrome_score(image, safe) >= threshold
+    return get_monochrome_score(image, model, safe) >= threshold
```

### Comparing `dghs-imgutils-0.1.0/imgutils/validate/truncate.py` & `dghs-imgutils-0.1.1/imgutils/validate/truncate.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.1.0/setup.py` & `dghs-imgutils-0.1.1/setup.py`

 * *Files identical despite different names*

