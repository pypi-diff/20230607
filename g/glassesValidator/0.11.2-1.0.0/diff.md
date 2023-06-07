# Comparing `tmp/glassesValidator-0.11.2.tar.gz` & `tmp/glassesValidator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glassesValidator-0.11.2.tar", last modified: Fri Feb 24 14:02:43 2023, max compression
+gzip compressed data, was "glassesValidator-1.0.0.tar", last modified: Wed Jun  7 06:50:09 2023, max compression
```

## Comparing `glassesValidator-0.11.2.tar` & `glassesValidator-1.0.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.660967 glassesValidator-0.11.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-02-24 14:02:43.660967 glassesValidator-0.11.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38318 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 14:02:43.660967 glassesValidator-0.11.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.632966 glassesValidator-0.11.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.636966 glassesValidator-0.11.2/src/glassesValidator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.636966 glassesValidator-0.11.2/src/glassesValidator/GUI/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_general_imgui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.640966 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/async_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    23666 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/filepicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)   122142 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/imagehelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/msgbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/process_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.644966 glassesValidator-0.11.2/src/glassesValidator/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/config/markerPositions.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.644966 glassesValidator-0.11.2/src/glassesValidator/config/poster/
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/config/poster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   218472 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/config/poster/poster.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/config/poster/poster.tex
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/config/targetPositions.csv
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/config/validationSetup.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.648966 glassesValidator-0.11.2/src/glassesValidator/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/preprocess/SMI_ETG.py
--rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/preprocess/SeeTrue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/preprocess/pupilLabs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/preprocess/tobii_G2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/preprocess/tobii_G3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.652967 glassesValidator-0.11.2/src/glassesValidator/process/
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/process/_image_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/process/b_codeMarkerInterval.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/process/c_detectMarkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/process/d_gazeToPoster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/process/e1_computeOffsetsToTargets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/process/e2_determineFixationIntervals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/process/f_calculateDataQuality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.652967 glassesValidator-0.11.2/src/glassesValidator/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.652967 glassesValidator-0.11.2/src/glassesValidator/resources/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/resources/fonts/Karla-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   556216 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/resources/fonts/NotoSans-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/resources/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1243500 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/resources/fonts/materialdesignicons-webfont.7.0.96.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.656967 glassesValidator-0.11.2/src/glassesValidator/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/resources/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29894 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/resources/icons/icon.icns
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/resources/icons/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/resources/icons/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.656967 glassesValidator-0.11.2/src/glassesValidator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    53486 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10589 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/utils/makeVideo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.660967 glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    56886 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/iso.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/mpeglookups.py
--rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/non_iso.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-24 14:02:32.000000 glassesValidator-0.11.2/src/glassesValidator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:02:43.636966 glassesValidator-0.11.2/src/glassesValidator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-02-24 14:02:43.000000 glassesValidator-0.11.2/src/glassesValidator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-02-24 14:02:43.000000 glassesValidator-0.11.2/src/glassesValidator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 14:02:43.000000 glassesValidator-0.11.2/src/glassesValidator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-24 14:02:43.000000 glassesValidator-0.11.2/src/glassesValidator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-24 14:02:43.000000 glassesValidator-0.11.2/src/glassesValidator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.737289 glassesValidator-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-07 06:50:09.737289 glassesValidator-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    44073 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 06:50:09.737289 glassesValidator-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.725287 glassesValidator-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.725287 glassesValidator-1.0.0/src/glassesValidator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.729288 glassesValidator-1.0.0/src/glassesValidator/GUI/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_general_imgui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.729288 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/async_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23666 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/filepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122315 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/imagehelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/msgbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/process_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.729288 glassesValidator-1.0.0/src/glassesValidator/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/markerPositions.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.733288 glassesValidator-1.0.0/src/glassesValidator/config/poster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/poster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   218472 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/poster/poster.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/poster/poster.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/targetPositions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/validationSetup.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.733288 glassesValidator-1.0.0/src/glassesValidator/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/preprocess/SMI_ETG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/preprocess/SeeTrue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26420 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/preprocess/pupilLabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/preprocess/tobii_G2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/preprocess/tobii_G3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.733288 glassesValidator-1.0.0/src/glassesValidator/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/_image_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/b_codeMarkerInterval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/c_detectMarkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/d_gazeToPoster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/e1_computeOffsetsToTargets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/e2_determineFixationIntervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/f_calculateDataQuality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.733288 glassesValidator-1.0.0/src/glassesValidator/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.733288 glassesValidator-1.0.0/src/glassesValidator/resources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/fonts/Karla-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   556216 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/fonts/NotoSans-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1243500 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/fonts/materialdesignicons-webfont.7.0.96.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.737289 glassesValidator-1.0.0/src/glassesValidator/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29894 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/icons/icon.icns
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/icons/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/icons/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.737289 glassesValidator-1.0.0/src/glassesValidator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    53577 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/makeVideo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.737289 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56886 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/iso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/mpeglookups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/non_iso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.729288 glassesValidator-1.0.0/src/glassesValidator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-07 06:50:09.000000 glassesValidator-1.0.0/src/glassesValidator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-07 06:50:09.000000 glassesValidator-1.0.0/src/glassesValidator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:50:09.000000 glassesValidator-1.0.0/src/glassesValidator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 06:50:09.000000 glassesValidator-1.0.0/src/glassesValidator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-07 06:50:09.000000 glassesValidator-1.0.0/src/glassesValidator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 06:50:09.000000 glassesValidator-1.0.0/src/glassesValidator.egg-info/top_level.txt
```

### Comparing `glassesValidator-0.11.2/LICENSE` & `glassesValidator-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/PKG-INFO` & `glassesValidator-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glassesValidator
-Version: 0.11.2
+Version: 1.0.0
 Summary: Automatic determination of accuracy of wearable eye tracker recordings.
 Home-page: https://github.com/dcnieho/glassesValidator
 Author: Diederick Niehorster
 Author-email: diederick_c.niehorster@humlab.lu.se
 License: MIT License
         
         Copyright (c) 2022-2023 Diederick Niehorster
@@ -24,13 +24,13 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Source Code, https://github.com/dcnieho/glassesValidator
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: ==3.10.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `glassesValidator-0.11.2/README.md` & `glassesValidator-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-# GlassesValidator
+[![PyPI Latest Release](https://img.shields.io/pypi/v/glassesValidator.svg)](https://pypi.org/project/glassesValidator/)
+[![image](https://img.shields.io/pypi/pyversions/glassesValidator.svg)](https://pypi.org/project/glassesValidator/)
+[![DOI](https://zenodo.org/badge/DOI/10.3758/s13428-023-02105-5.svg)](https://doi.org/10.3758/s13428-023-02105-5)
+
+# GlassesValidator v1.0.0
 Tool for automatic determination of data quality (accuracy and precision) of wearable eye tracker recordings.
 
 Please note that this software is currently in beta, and the accompanying paper is not yet published. As such,
 the software is potentially subject to change, and we urge users to carefully check the results generated by
 glassesValidator. Please provide us with feedback on *anything* you notice, *no matter how small*.
 
 A preliminary reference to the upcoming paper is:<br>
@@ -10,65 +14,106 @@
 A data quality tool for eye tracking glasses.
 
 However, as long as the paper is not accepted, please cite this work as follows:<br>
 Niehorster, D.C., Hessels, R.S., Benjamins, J.S., Nyström, M. and Hooge, I.T.C. (2022). GlassesValidator:
 A data quality tool for eye tracking glasses. Available from https://github.com/dcnieho/glassesValidator
 
 # How to acquire
-GlassesValidator is available from `https://github.com/dcnieho/glassesValidator`, and supports Windows, MacOS and Linux.
+GlassesValidator is available from `https://github.com/dcnieho/glassesValidator`, and supports Windows, MacOS and Linux. Right
+now only Python 3.10 is supported. Support for Python 3.11 is forthcoming once some blocking bugs have been resolved by me
+and upstream.
 
 For Windows users who wish to use the glassesValidator GUI, the easiest way to acquire glassesValidator is to [download
 a standalone executable](https://github.com/dcnieho/glassesValidator/releases/latest). The standalone executable is not
 available for MacOS or Linux.
 
 For users on Windows, Mac or Linux who wish to use glassesValidator in their Python code, the easiest way to acquire
 glassesValidator is to install it directly into your Python distribution using the command
 `python -m pip install glassesValidator`. Should that fail, this repository is pip-installable as well:
 `python -m pip install git+https://github.com/dcnieho/glassesValidator.git#egg=glassesValidator`. NB: on some platforms you may have
 to replace `python` with `python3` in the above command lines.
 
-Once pip-installed in your Python distribution, running the GUI on any of the supported operating systems requires only the following two lines of code:
+Once pip-installed in your Python distribution, the GUI can be run on any of the supported operating systems by typing `glassesValidator` in
+the terminal. From Python, running the GUI requires only the following two lines of code:
 ```python
 import glassesValidator
 glassesValidator.GUI.run()
 ```
 
 # Usage
-The glassesValidator validation procedure consists of two parts, 1) a poster that is used during a recording, and 2) Python software
-for offline processing of the recording to estimate data quality measures.
+The glassesValidator validation procedure consists of two parts, 1) a poster and validation procedure that is used during a recording, and 2) Python software
+for offline processing of the recording to estimate data quality measures. The glassesValidator package includes a graphical user interface (GUI)
+that can be used to perform all processing. Below we describe an example workflow using the GUI. Advanced users can however opt to call all the GUI's
+functionality directly from their own Python scripts without making use of the graphical user interface. The interested reader is referred to the glassesValidator
+manual for further details regarding how to use the glassesValidator functionality directly from their own scripts.
+
+## Workflow and example data
+Here we first present an example workflow using the GUI. More detailed information about [using the GUI](#the-gui), or [the programming API](#api), are provided
+below.
+
+1. Before recording, the researcher prints [the poster](#the-poster) included with glassesValidator on A2 paper. See the instructions in [the section about the
+   poster](#the-poster) for checking if the poster is printed correctly.
+2. Before recording, the researcher hangs the printed poster on a flat surface, such as a wall. Vertical positioning of the poster depends on the experiment
+   setting, but we think that a suitable default is to hang the poster such that the top row of fixation targets is at eye height for an average-length participant.
+3. The operator positions the participant in front of the glassesValidator poster. An easy method for positioning the participant is to ask them to stretch their
+   arm out straight forward and stand at a distance where their fist touches the poster. The operator then issues the following suggested instructions:
+   `Look at the nine fixation targets in reading order for one second each. Start with the top-left (red) target. When looking at the fixation targets, keep your
+   head as still as possible, move only your eyes.` These verbal instructions could be accompanied by pointing at the fixation targets in the desired looking order
+   to further help the participant to follow the instructions.
+4. To start calculating accuracy and precision, the researcher imports the recordings for which data quality should be determined into a glassesValidator project
+   (after any [preprocessing if required](#required-preprocessing-outside-glassesvalidator), for instance by drag-dropping a folder with recordings onto the
+   glassesValidator GUI window and selecting the import action.
+5. Once imported, the researcher indicates which episode(s) of each recording contain a validation using a graphical interface included with glassesValidator.
+6. The recordings are then further processed automatically, and data quality is determined for validation episodes in the recording.
+7. Finally, once all recordings have been processed, the researcher exports the data quality measures from the recordings in the project into a summary Excel file.
+   This summary function can optionally average the data quality values over the fixation targets for each recording.
+
+Example recordings with which steps 4-7 can be practiced is included in the [example_data subfolder](/example_data). This folder contains example recordings of a
+participant executing the validation procedure with a Pupil Invisible and a Tobii Pro Glasses 2. You can import these recordings directly into glassesValidator.
+Also included in each recordings subfolder is an example `analysisInterval.tsv` file for denoting where the validation interval is in the recording (step 5 above).
+To use these files, after importing a recording into your [glassesValidator project](#glassesvalidator-projects) (step 4 above), copy the corresponding
+`analysisInterval.tsv` to the recording's folder in the glassesValidator project before running the `Code validation intervals` action.
 
 ## glassesValidator projects
 The glassesValidator GUI organizes recordings into a project folder. Each recording to be processed is imported into this project folder
 and all further processing is done inside it. The source directories containing the original recordings remain untouched when running
 glassesValidator. The glassesValidator project folder can furthermore contain a folder specifying the configuration of the project.
 Such a configuration should be made if you used a poster different from the default (if no configuration folder is present, the default
 settings are automatically used), and can be deployed with the `Deploy config` button in the GUI, or the
 `glassesValidator.config.deploy_validation_config()` call from Python.
 
-
 ## Eye trackers
 glassesValidator supports the following eye trackers:
 - Pupil Core
 - Pupil Invisible
+- Pupil Neon
 - SeeTrue
 - SMI ETG 1 and ETG 2
 - Tobii Pro Glasses 2
 - Tobii Pro Glasses 3
 
 Pull requests or partial help implementing support for further wearable eye trackers are gladly received. To support a new eye tracker,
 device support in [`glassesValidator.preprocess`](#glassesValidatorpreprocess) should be implemented and the new eye tracker added to
 the [`glassesValidator.utils.EyeTracker` `Enum`](#glassesValidatorutils).
 
 ### Required preprocessing outside glassesValidator
 For some eye trackers, the recording delivered by the eye tracker's recording unit or software can be directly imported into
 glassesValidator. Recordings from some other eye trackers however require some steps to be performed in the manufacturer's
 software before they can be imported into glassesValidator. These are:
-- *Pupil Core* and *Pupil Invisible*: Each recording should 1) be opened in Pupil Player, and 2) an export of the recording
-  (`e` hotkey) should be run from pupil player. Make sure to disable the `World Video Exporter` in the `Plugin Manager` before
-  exporting, as the exported video is not used by glassesValidator and takes a long time to create.
+- *Pupil eye trackers*: Recordings should either be preprocessed using Pupil Player (*Pupil Core* and *Pupil Invisible*) or exported
+  from Pupil Cloud (*Pupil Invisible* and *Pupil Neon*).
+  - Using Pupil Player (*Pupil Core* and *Pupil Invisible*): Each recording should 1) be opened in Pupil Player, and 2) an export of the
+    recording (`e` hotkey) should be run from pupil player. Make sure to disable the `World Video Exporter` in the `Plugin Manager`
+    before exporting, as the exported video is not used by glassesValidator and takes a long time to create. Note that importing a Pupil
+    Player export of a Pupil Invisible export requires an internet connection, which is used to retrieve the scene camera calibration
+    from Pupil Lab's servers.
+  - Using Pupil Cloud (*Pupil Invisible* and *Pupil Neon*): Export the recordings using the `Timeseries data + Scene video` action.
+  - For the *Pupil Core*, for best results you may wish to do a scene camera calibration yourself, see https://docs.pupil-labs.com/core/software/pupil-capture/#camera-intrinsics-estimation.
+    If you do not do so, a generic calibration will be used by Pupil Capture during data recording, by Pupil Player during data
+    analysis and by glassesValidator, which may result in worse accuracy.
 - *SMI ETG*: For SMI ETG recordings, access to BeGaze is required and the following steps should be performed:
   - Export gaze data: `Export` -> `Legacy: Export Raw Data to File`.
     - In the `General` tab, make sure you select the following:
       - `Channel`: enable both eyes
       - `Points of Regard (POR)`: enable `Gaze position`, `Eye position`, `Gaze vector`
       - `Binocular`: enable `Gaze position`
       - `Misc Data`: enable `Frame counter`
@@ -104,17 +149,18 @@
 The default poster is available 1) [here](/src/glassesValidator/config/poster/poster.pdf), 2) from the GUI with the `Get poster
 pdf` button, and 3) can also be acquired from a Python script by calling
 `glassesValidator.config.poster.deploy_default_pdf()`.
 The default poster should be printed at A2 size, as defined
 in the pdf file, and is designed to cover a reasonable field of view when participants view it at armslength (i.e., 20 x 17.5 deg
 at 60 cm). In order to check that the poster was printed at the correct scale, one should measure the sides of the ArUco markers.
 We strongly recommend performing this check because printers may not be calibrated. In the case of the default glassesValidator
-poster, each ArUco marker should have sides that are 4.19 cm long. If the poster was printed at the wrong scale, one must adapt
-the glassesValidator configuration to match the size and position of the ArUco markers and fixation targets on your poster ([see
-"Customizing the poster" below](#customizing-the-poster)).
+poster, the distance between the left side of the left-most column of ArUco markers and the right side of the right-most column of
+ArUco markers should be 35.6 cm (each ArUco marker should have sides that are 4.19 cm long). If the poster was printed at the wrong
+scale, one must adapt the glassesValidator configuration to match the size and position of the ArUco markers and fixation targets
+on your poster ([see "Customizing the poster" below](#customizing-the-poster)).
 
 ### Customizing the poster
 The poster pdf file is generated by the [LaTeX file in the same folder as the pdf](/src/glassesValidator/config/poster/poster.tex).
 Its looks are defined in the files in the [config folder](/src/glassesValidator/config). As described above, this configuration can be
 deployed and then edited. The edited configuration can both be used to generate a new poster with LaTeX and for performing the
 data quality calculations.
 Specifically, the files [`markerPositions.csv`](/src/glassesValidator/config/markerPositions.csv) and
@@ -168,15 +214,15 @@
 ## The GUI
 ![Glasses viewer screenshot](/.github/images/screenshot.png?raw=true)
 Click the screenshot to see a full-size version.
 
 The simplest way to use glassesValidator is by means of its GUI, see above. The full workflow can be performed in the GUI.
 Specifically, it supports:
 
-- GlassesValidator project management, such as making new projects or opening them
+- GlassesValidator project management, such as making new projects or opening them.
 - Importing recordings into a glassesValidator project. Recordings can be found by glassesValidator by drag-dropping one or multiple
   directories onto the GUI or by clicking the `Add recordings` button (not shown) and selecting one or multiple directories. The
   selected directories and all their subdirectories are then searched for recordings, and the user can select which of the found
   recordings should be added to the glassesValidator import. Once listed in the GUI, the import action can then be started, which
   copies over data from the selected recording to the glassesValidator project folder, and transforms it to a common format.
 - Showing a listing of the recordings in the project and several properties about them, where available. these properties currently
   are:
@@ -325,14 +371,15 @@
 |function|inputs|description|
 | --- | --- | --- |
 |`get_recording_info()`|<ol><li>[`source_dir`](#common-input-arguments)</li><li>`device`: `glassesValidator.utils.EyeTracker`</li></ol>|Determine if provided path contains a recording/recordings made with the specified eye tracker (`device`) and if so, get info about these recordings.|
 |`do_import()`|<ol><li>[`output_dir`](#common-input-arguments)</li><li>[`source_dir`](#common-input-arguments)</li><li>`device`: `glassesValidator.utils.EyeTracker`</li><li>[`rec_info`](#common-input-arguments)</li></ol>|Import the specified recording to a subdirectory of `output_dir`. Either `device` or `rec_info` must be specified. Does nothing if directory does not contain a recording made with the specified eye tracker.|
 |  |  |  |
 |`pupil_core()`|<ol><li>[`output_dir`](#common-input-arguments)</li><li>[`source_dir`](#common-input-arguments)</li><li>[`rec_info`](#common-input-arguments)</li></ol>|Import a Pupil Core recording to a subdirectory of `output_dir`. Does nothing if directory does not contain a Pupil Core recording. `rec_info` is optional.|
 |`pupil_invisible()`|<ol><li>[`output_dir`](#common-input-arguments)</li><li>[`source_dir`](#common-input-arguments)</li><li>[`rec_info`](#common-input-arguments)</li></ol>|Import a Pupil Invisible recording to a subdirectory of `output_dir`. Does nothing if directory does not contain a Pupil Invisible recording. `rec_info` is optional.|
+|`pupil_neon()`|<ol><li>[`output_dir`](#common-input-arguments)</li><li>[`source_dir`](#common-input-arguments)</li><li>[`rec_info`](#common-input-arguments)</li></ol>|Import a Pupil Neon recording to a subdirectory of `output_dir`. Does nothing if directory does not contain a Pupil Neon recording. `rec_info` is optional.|
 |`SeeTrue()`|<ol><li>[`output_dir`](#common-input-arguments)</li><li>[`source_dir`](#common-input-arguments)</li><li>[`rec_info`](#common-input-arguments)</li><li>`cam_cal_file`: OpenCV XML file containing a camera calibration to be used when processing this recording. Optional.</li></ol>|Import a SeeTrue recording to a subdirectory of `output_dir`. Does nothing if directory does not contain a SeeTrue recording. `rec_info` is optional.|
 |`SMI_ETG()`|<ol><li>[`output_dir`](#common-input-arguments)</li><li>[`source_dir`](#common-input-arguments)</li><li>[`rec_info`](#common-input-arguments)</li></ol>|Import a SMI ETG recording to a subdirectory of `output_dir`. Does nothing if directory does not contain a SMI ETG 1 or 2 recording. `rec_info` is optional.|
 |`tobii_G2()`|<ol><li>[`output_dir`](#common-input-arguments)</li><li>[`source_dir`](#common-input-arguments)</li><li>[`rec_info`](#common-input-arguments)</li></ol>|Import a Tobii Pro Glasses 2 recording to a subdirectory of `output_dir`. Does nothing if directory does not contain a Tobii Pro Glasses 2 recording. `rec_info` is optional.|
 |`tobii_G3()`|<ol><li>[`output_dir`](#common-input-arguments)</li><li>[`source_dir`](#common-input-arguments)</li><li>[`rec_info`](#common-input-arguments)</li></ol>|Import a Tobii Pro Glasses 3 recording to a subdirectory of `output_dir`. Does nothing if directory does not contain a Tobii Pro Glasses 3 recording. `rec_info` is optional.|
 
 ### glassesValidator.process
 |function|inputs/members|description|
@@ -351,15 +398,15 @@
 |`DataQualityType`|`enum.Enum`<ul><li>`DataQualityType.viewpos_vidpos_homography`</li><li>`DataQualityType.pose_vidpos_homography`</li><li>`DataQualityType.pose_vidpos_ray`</li><li>`DataQualityType.pose_left_eye`</li><li>`DataQualityType.pose_right_eye`</li><li>`DataQualityType.pose_left_right_avg`</li></ul>|See [Advanced settings section in The GUI section](#advanced-settings) above.|
 
 ### glassesValidator.utils
 |function|inputs/members|description|
 | --- | --- | --- |
 |`make_video()`|<ol><li>[`working_dir`](#common-input-arguments)</li><li>[`config_dir`](#common-input-arguments)</li><li>`show_rejected_markers`: if `True`, rejected ArUco marker candidates are also drawn on the video.</li><li>`add_audio_to_poster_video`: if `True`, audio is added to poster video, not only to the scene video.</li><li>`show_visualization`: if `True`, the generated video is shown as it is created in a viewer.</li></ol>|Export annotated scene video showing gaze, detected ArUco markers and detected poster. Also exports a video showing gaze on the poster.|
 |  |  |  |
-|`EyeTracker`|`enum.Enum`<ul><li>`EyeTracker.Pupil_Core`</li><li>`EyeTracker.Pupil_Invisible`</li><li>`EyeTracker.SMI_ETG`</li><li>`EyeTracker.SeeTrue`</li><li>`EyeTracker.Tobii_Glasses_2`</li><li>`EyeTracker.Tobii_Glasses_3`</li></ul>||
+|`EyeTracker`|`enum.Enum`<ul><li>`EyeTracker.Pupil_Core`</li><li>`EyeTracker.Pupil_Invisible`</li><li>`EyeTracker.Pupil_Neon`</li><li>`EyeTracker.SMI_ETG`</li><li>`EyeTracker.SeeTrue`</li><li>`EyeTracker.Tobii_Glasses_2`</li><li>`EyeTracker.Tobii_Glasses_3`</li></ul>||
 |`Recording`|`dataclasses.dataclass`<ul><li>`Recording.name`</li><li>`Recording.source_directory`</li><li>`Recording.proc_directory_name`</li><li>`Recording.start_time`</li><li>`Recording.duration`</li><li>`Recording.eye_tracker`: `glassesValidator.utils.EyeTracker`</li><li>`Recording.project`</li><li>`Recording.participant`</li><li>`Recording.firmware_version`</li><li>`Recording.glasses_serial`</li><li>`Recording.recording_unit_serial`</li><li>`Recording.recording_software_version`</li><li>`Recording.scene_camera_serial`</li><li>`Recording.id` (internal to GUI)</li><li>`Recording.task` (internal to GUI)</li></ul>|Information about a recording|
 
 ### Common input arguments
 |argument|module(s)|description|
 | --- | --- | --- |
 |`config_dir`|`glassesValidator.config`<br>`glassesValidator.process`<br>`glassesValidator.utils`|Path to directory containing a glassesValidator setup. If `None`, the default setup is used.|
 |`source_dir`|`glassesValidator.preprocess`|Path to directory containing one (or for some eye trackers potentially multiple) eye tracker recording(s) as stored by the eye tracker's recording hardware or software.|
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/__init__.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/_general_imgui.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/_general_imgui.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/async_thread.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/async_thread.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/callbacks.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/callbacks.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/db.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/db.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/filepicker.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/filepicker.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/globals.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/globals.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 import sys
 
 from ... import __version__
 version           = __version__
 pypi_page         = "https://pypi.org/project/glassesValidator/"
 github_page       = "https://github.com/dcnieho/glassesValidator"
 developer_page    = "https://scholar.google.se/citations?user=uRUYoVgAAAAJ&hl=en"
-reference         = r"Niehorster, D.C., Hessels, R.S., Benjamins, J.S., Nyström, M. & Hooge, I.T.C. (submitted). GlassesValidator: Data quality tool for eye tracking glasses."
+paper_page        = "https://doi.org/10.3758/s13428-023-02105-5"
+reference         = r"Niehorster, D.C., Hessels, R.S., Benjamins, J.S., Nyström, M. & Hooge, I.T.C. (2023). GlassesValidator: Data quality tool for eye tracking glasses. Behavior Research Methods. doi: 10.3758/s13428-023-02105-5"
 reference_bibtex  = r"""@article{niehorster2023glassesValidator,
     Author = {Niehorster, Diederick C. and Hessels, Roy S. and Benjamins, Jeroen S. and Nystr{\"o}m, Marcus and Hooge, Ignace T. C.},
-    Journal = {},
+    Journal = {Behavior Research Methods},
     Number = {},
     Pages = {},
     Title = {GlassesValidator: A data quality tool for eye tracking glasses},
-    Year = {submitted}
+    Year = {2023},
+    doi = {10.3758/s13428-023-02105-5}
 }
 """
 
 
 from .structs import CounterContext, JobDescription, Os, Settings
 from .gui import MainGUI
 from ...utils import Recording
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/gui.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1547,22 +1547,25 @@
                 imgui.text(f"{platform.system()} {platform.release()}")
             imgui.end_group()
             imgui.same_line()
             imgui.dummy((_60, _230))
             imgui.end_group()
             imgui.spacing()
             width = imgui.get_content_region_avail().x
-            btn_width = (width - 2 * imgui.style.item_spacing.x) / 3
-            if imgui.button("󰌠 PyPI", size=(btn_width, 0)):
+            btn_tot_width = (width - 2 * imgui.style.item_spacing.x)
+            if imgui.button("󰌠 PyPI", size=(btn_tot_width/6, 0)):
                 callbacks.open_url(globals.pypi_page)
             imgui.same_line()
-            if imgui.button("󰊤 GitHub repo", size=(btn_width, 0)):
+            if imgui.button("󱓷 Paper", size=(btn_tot_width/6, 0)):
+                callbacks.open_url(globals.paper_page)
+            imgui.same_line()
+            if imgui.button("󰊤 GitHub repo", size=(btn_tot_width/3, 0)):
                 callbacks.open_url(globals.github_page)
             imgui.same_line()
-            if imgui.button("󰖟 Researcher homepage", size=(btn_width, 0)):
+            if imgui.button("󰖟 Researcher homepage", size=(btn_tot_width/3, 0)):
                 callbacks.open_url(globals.developer_page)
 
             imgui.spacing()
             imgui.spacing()
             imgui.push_text_wrap_pos(width)
             imgui.text("This software is licensed under the 3rd revision of the GNU General Public License (GPLv3) and is provided to you for free. "
                        "Furthermore, due to its license, it is also free as in freedom: you are free to use, study, modify and share this software "
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/imagehelper.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/imagehelper.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/msgbox.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/msgbox.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/process_pool.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/process_pool.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/structs.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/structs.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/GUI/_impl/utils.py` & `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/utils.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/config/__init__.py` & `glassesValidator-1.0.0/src/glassesValidator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/config/markerPositions.csv` & `glassesValidator-1.0.0/src/glassesValidator/config/markerPositions.csv`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/config/poster/__init__.py` & `glassesValidator-1.0.0/src/glassesValidator/config/poster/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/config/poster/poster.pdf` & `glassesValidator-1.0.0/src/glassesValidator/config/poster/poster.pdf`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/config/poster/poster.tex` & `glassesValidator-1.0.0/src/glassesValidator/config/poster/poster.tex`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/config/validationSetup.txt` & `glassesValidator-1.0.0/src/glassesValidator/config/validationSetup.txt`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/preprocess/SMI_ETG.py` & `glassesValidator-1.0.0/src/glassesValidator/preprocess/SMI_ETG.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,51 +21,51 @@
 import configparser
 from io import StringIO
 from scipy.spatial.transform import Rotation
 
 from .. import utils
 
 
-def preprocessData(output_dir, input_dir=None, rec_info=None):
+def preprocessData(output_dir, source_dir=None, rec_info=None):
     """
     Run all preprocessing steps on SMI data
     """
     output_dir = pathlib.Path(output_dir)
-    if input_dir is not None:
-        input_dir  = pathlib.Path(input_dir)
-        if rec_info is not None and pathlib.Path(rec_info.source_directory) != input_dir:
-            raise ValueError(f"The provided source_dir ({input_dir}) does not equal the source directory set in rec_info ({rec_info.source_directory}).")
+    if source_dir is not None:
+        source_dir  = pathlib.Path(source_dir)
+        if rec_info is not None and pathlib.Path(rec_info.source_directory) != source_dir:
+            raise ValueError(f"The provided source_dir ({source_dir}) does not equal the source directory set in rec_info ({rec_info.source_directory}).")
     elif rec_info is None:
         raise RuntimeError('Either the "input_dir" or the "rec_info" input argument should be set.')
     else:
-        input_dir  = pathlib.Path(rec_info.source_directory)
+        source_dir  = pathlib.Path(rec_info.source_directory)
 
     if rec_info is not None:
         if rec_info.eye_tracker!=utils.EyeTracker.SMI_ETG:
             raise ValueError(f'Provided rec_info is for a device ({rec_info.eye_tracker.value}) that is not an {utils.EyeTracker.SMI_ETG.value}. Cannot use.')
         if not rec_info.proc_directory_name:
             rec_info.proc_directory_name = utils.make_fs_dirname(rec_info, output_dir)
         newDir = output_dir / rec_info.proc_directory_name
         if newDir.is_dir():
             raise RuntimeError(f'Output directory specified in rec_info ({rec_info.proc_directory_name}) already exists in the outputDir ({output_dir}). Cannot use.')
 
 
-    print(f'processing: {input_dir.name}')
+    print(f'processing: {source_dir.name}')
 
 
     ### check and copy needed files to the output directory
     print('Check and copy raw data...')
     if rec_info is not None:
-        if not checkRecording(input_dir, rec_info, use_return=True):
-            raise ValueError(f"A recording with the name \"{rec_info.name}\" was not found in the folder {input_dir}. Check that the name is correct and make sure that you export the scene video and gaze data using BeGaze as described in the glassesValidator manual.")
+        if not checkRecording(source_dir, rec_info, use_return=True):
+            raise ValueError(f"A recording with the name \"{rec_info.name}\" was not found in the folder {source_dir}. Check that the name is correct and make sure that you export the scene video and gaze data using BeGaze as described in the glassesValidator manual.")
         recInfos = [rec_info]
     else:
-        recInfos = getRecordingInfo(input_dir)
+        recInfos = getRecordingInfo(source_dir)
         if recInfos is None:
-            raise RuntimeError(f"The folder {input_dir} does not contain SMI ETG recordings prepared for glassesValidator. If this is an SMI recording folder, you may not have run the required gaze data and scene video exports yet. See the glassesValidator manual for which exports you should perform with BeGaze first as well as the file naming scheme.")
+            raise RuntimeError(f"The folder {source_dir} does not contain SMI ETG recordings prepared for glassesValidator. If this is an SMI recording folder, you may not have run the required gaze data and scene video exports yet. See the glassesValidator manual for which exports you should perform with BeGaze first as well as the file naming scheme.")
 
     # make output dirs
     for i in range(len(recInfos)):
         if recInfos[i].proc_directory_name is None or not recInfos[i].proc_directory_name:
             recInfos[i].proc_directory_name = utils.make_fs_dirname(recInfos[i], output_dir)
         newDataDir = output_dir / recInfos[i].proc_directory_name
         if not newDataDir.is_dir():
@@ -78,26 +78,26 @@
         utils.get_recording_status(newDataDir, create_if_missing=True)
         utils.update_recording_status(newDataDir, utils.Task.Imported, utils.Status.Running)
 
 
     ### copy the raw data to the output directory
     for rec_info in recInfos:
         newDataDir = output_dir / rec_info.proc_directory_name
-        checkRecording(input_dir, rec_info)
-        copySMIRecordings(input_dir, newDataDir, rec_info)
+        checkRecording(source_dir, rec_info)
+        copySMIRecordings(source_dir, newDataDir, rec_info)
         print(f'Input data copied to: {newDataDir}')
 
     #### prep the data
     for rec_info in recInfos:
         newDataDir = output_dir / rec_info.proc_directory_name
         print(f'{newDataDir.name}...')
         print('  Getting camera calibration...')
-        sceneVideoDimensions = getCameraFromFile(input_dir, newDataDir)
+        sceneVideoDimensions = getCameraFromFile(source_dir, newDataDir)
         print('  Prepping gaze data...')
-        gazeDf, frameTimestamps = formatGazeData(input_dir, newDataDir, rec_info, sceneVideoDimensions)
+        gazeDf, frameTimestamps = formatGazeData(source_dir, newDataDir, rec_info, sceneVideoDimensions)
 
         # write the gaze data to a csv file
         gazeDf.to_csv(str(newDataDir / 'gazeData.tsv'), sep='\t', na_rep='nan', float_format="%.8f")
 
         # also store frame timestamps
         frameTimestamps.to_csv(str(newDataDir / 'frameTimestamps.tsv'), sep='\t')
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator/preprocess/SeeTrue.py` & `glassesValidator-1.0.0/src/glassesValidator/preprocess/SeeTrue.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,55 +13,55 @@
 import cv2
 import pandas as pd
 import numpy as np
 
 from .. import utils
 
 
-def preprocessData(output_dir, input_dir=None, rec_info=None, cam_cal_file=None):
+def preprocessData(output_dir, source_dir=None, rec_info=None, cam_cal_file=None):
 
     if shutil.which('ffmpeg') is None:
         RuntimeError('ffmpeg must be on path to prep SeeTrue recording for processing with GlassesValidator')
 
     """
     Run all preprocessing steps on SeeTrue data
     """
     output_dir = pathlib.Path(output_dir)
-    if input_dir is not None:
-        input_dir  = pathlib.Path(input_dir)
-        if rec_info is not None and pathlib.Path(rec_info.source_directory) != input_dir:
-            raise ValueError(f"The provided source_dir ({input_dir}) does not equal the source directory set in rec_info ({rec_info.source_directory}).")
+    if source_dir is not None:
+        source_dir  = pathlib.Path(source_dir)
+        if rec_info is not None and pathlib.Path(rec_info.source_directory) != source_dir:
+            raise ValueError(f"The provided source_dir ({source_dir}) does not equal the source directory set in rec_info ({rec_info.source_directory}).")
     elif rec_info is None:
         raise RuntimeError('Either the "input_dir" or the "rec_info" input argument should be set.')
     else:
-        input_dir  = pathlib.Path(rec_info.source_directory)
+        source_dir  = pathlib.Path(rec_info.source_directory)
 
     if rec_info is not None:
         if rec_info.eye_tracker!=utils.EyeTracker.SeeTrue:
             raise ValueError(f'Provided rec_info is for a device ({rec_info.eye_tracker.value}) that is not an {utils.EyeTracker.SeeTrue.value}. Cannot use.')
         if not rec_info.proc_directory_name:
             rec_info.proc_directory_name = utils.make_fs_dirname(rec_info, output_dir)
         newDir = output_dir / rec_info.proc_directory_name
         if newDir.is_dir():
             raise RuntimeError(f'Output directory specified in rec_info ({rec_info.proc_directory_name}) already exists in the outputDir ({output_dir}). Cannot use.')
 
 
-    print(f'processing: {input_dir.name}')
+    print(f'processing: {source_dir.name}')
 
 
     ### check and copy needed files to the output directory
     print('Check and copy raw data...')
     if rec_info is not None:
-        if not checkRecording(input_dir, rec_info):
-            raise ValueError(f"A recording with the name \"{rec_info.name}\" was not found in the folder {input_dir}.")
+        if not checkRecording(source_dir, rec_info):
+            raise ValueError(f"A recording with the name \"{rec_info.name}\" was not found in the folder {source_dir}.")
         recInfos = [rec_info]
     else:
-        recInfos = getRecordingInfo(input_dir)
+        recInfos = getRecordingInfo(source_dir)
         if recInfos is None:
-            raise RuntimeError(f"The folder {input_dir} does not contain SeeTrue recordings.")
+            raise RuntimeError(f"The folder {source_dir} does not contain SeeTrue recordings.")
 
     # make output dirs
     for i in range(len(recInfos)):
         if recInfos[i].proc_directory_name is None or not recInfos[i].proc_directory_name:
             recInfos[i].proc_directory_name = utils.make_fs_dirname(recInfos[i], output_dir)
         newDataDir = output_dir / recInfos[i].proc_directory_name
         if not newDataDir.is_dir():
@@ -82,15 +82,15 @@
         print('  Getting camera calibration...')
         if cam_cal_file is not None:
             shutil.copyfile(str(cam_cal_file), str(newDataDir / 'calibration.xml'))
         else:
             print('    !! No camera calibration provided!')
 
         # NB: gaze data and scene video prep are intertwined, status messages are output inside this function
-        gazeDf, frameTimestamps = copySeeTrueRecording(input_dir, newDataDir, rec_info)
+        gazeDf, frameTimestamps = copySeeTrueRecording(source_dir, newDataDir, rec_info)
 
         # write the gaze data to a csv file
         gazeDf.to_csv(str(newDataDir / 'gazeData.tsv'), sep='\t', na_rep='nan', float_format="%.8f")
 
         # also store frame timestamps
         frameTimestamps.to_csv(str(newDataDir / 'frameTimestamps.tsv'), sep='\t')
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator/preprocess/__init__.py` & `glassesValidator-1.0.0/src/glassesValidator/preprocess/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,32 +8,38 @@
 from .tobii_G2 import preprocessData as tobii_G2
 from .tobii_G3 import preprocessData as tobii_G3
 
 def pupil_core(output_dir: str | pathlib.Path, source_dir: str | pathlib.Path = None, rec_info: _utils.Recording = None):
     from .pupilLabs import preprocessData
     preprocessData(output_dir, 'Pupil Core', source_dir, rec_info)
 
-
 def pupil_invisible(output_dir: str | pathlib.Path, source_dir: str | pathlib.Path = None, rec_info: _utils.Recording = None):
     from .pupilLabs import preprocessData
     preprocessData(output_dir, 'Pupil Invisible', source_dir, rec_info)
 
+def pupil_neon(output_dir: str | pathlib.Path, source_dir: str | pathlib.Path = None, rec_info: _utils.Recording = None):
+    from .pupilLabs import preprocessData
+    preprocessData(output_dir, 'Pupil Neon', source_dir, rec_info)
+
 
 def get_recording_info(source_dir: str | pathlib.Path, device: str | _utils.EyeTracker):
     source_dir  = pathlib.Path(source_dir)
     device = _utils.type_string_to_enum(device)
 
     rec_info = None
     match device:
         case _utils.EyeTracker.Pupil_Core:
             from .pupilLabs import getRecordingInfo
             rec_info = getRecordingInfo(source_dir, device)
         case _utils.EyeTracker.Pupil_Invisible:
             from .pupilLabs import getRecordingInfo
             rec_info = getRecordingInfo(source_dir, device)
+        case _utils.EyeTracker.Pupil_Neon:
+            from .pupilLabs import getRecordingInfo
+            rec_info = getRecordingInfo(source_dir, device)
         case _utils.EyeTracker.SeeTrue:
             from .SeeTrue import getRecordingInfo
             rec_info = getRecordingInfo(source_dir)
         case _utils.EyeTracker.SMI_ETG:
             from .SMI_ETG import getRecordingInfo
             rec_info = getRecordingInfo(source_dir)
         case _utils.EyeTracker.Tobii_Glasses_2:
@@ -88,23 +94,25 @@
 
     # do the actual import/pre-process
     match device:
         case _utils.EyeTracker.Pupil_Core:
             rec_info = pupil_core(output_dir, source_dir, rec_info)
         case _utils.EyeTracker.Pupil_Invisible:
             rec_info = pupil_invisible(output_dir, source_dir, rec_info)
+        case _utils.EyeTracker.Pupil_Neon:
+            rec_info = pupil_neon(output_dir, source_dir, rec_info)
         case _utils.EyeTracker.SeeTrue:
             rec_info = SeeTrue(output_dir, source_dir, rec_info)
         case _utils.EyeTracker.SMI_ETG:
             rec_info = SMI_ETG(output_dir, source_dir, rec_info)
         case _utils.EyeTracker.Tobii_Glasses_2:
             rec_info = tobii_G2(output_dir, source_dir, rec_info)
         case _utils.EyeTracker.Tobii_Glasses_3:
             rec_info = tobii_G3(output_dir, source_dir, rec_info)
 
     if rec_info is not None and not isinstance(rec_info,list):
         rec_info = [rec_info]
     return rec_info
 
 
-__all__ = ['pupil_core','pupil_invisible','SeeTrue','SMI_ETG','tobii_G2','tobii_G3',
+__all__ = ['pupil_core','pupil_invisible','pupil_neon','SeeTrue','SMI_ETG','tobii_G2','tobii_G3',
            'get_recording_info','do_import']
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator/preprocess/pupilLabs.py` & `glassesValidator-1.0.0/src/glassesValidator/preprocess/pupilLabs.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,63 +24,63 @@
 import re
 from urllib.request import urlopen
 
 
 from .. import utils
 
 
-def preprocessData(output_dir, device=None, input_dir=None, rec_info=None):
+def preprocessData(output_dir, device=None, source_dir=None, rec_info=None):
     """
     Run all preprocessing steps on pupil data
     """
     output_dir = pathlib.Path(output_dir)
-    if input_dir is not None:
-        input_dir  = pathlib.Path(input_dir)
-        if rec_info is not None and pathlib.Path(rec_info.source_directory) != input_dir:
-            raise ValueError(f"The provided source_dir ({input_dir}) does not equal the source directory set in rec_info ({rec_info.source_directory}).")
+    if source_dir is not None:
+        source_dir  = pathlib.Path(source_dir)
+        if rec_info is not None and pathlib.Path(rec_info.source_directory) != source_dir:
+            raise ValueError(f"The provided source_dir ({source_dir}) does not equal the source directory set in rec_info ({rec_info.source_directory}).")
     elif rec_info is None:
         raise RuntimeError('Either the "input_dir" or the "rec_info" input argument should be set.')
     else:
-        input_dir  = pathlib.Path(rec_info.source_directory)
+        source_dir  = pathlib.Path(rec_info.source_directory)
 
     if rec_info is not None:
-        if not rec_info.eye_tracker in [utils.EyeTracker.Pupil_Core, utils.EyeTracker.Pupil_Invisible]:
-            raise ValueError(f'Provided rec_info is for a device ({rec_info.eye_tracker.value}) that is not a {utils.EyeTracker.Pupil_Core.value} or a {utils.EyeTracker.Pupil_Invisible.value}. Cannot use.')
+        if not rec_info.eye_tracker in [utils.EyeTracker.Pupil_Core, utils.EyeTracker.Pupil_Invisible, utils.EyeTracker.Pupil_Neon]:
+            raise ValueError(f'Provided rec_info is for a device ({rec_info.eye_tracker.value}) that is not a {utils.EyeTracker.Pupil_Core.value}, a {utils.EyeTracker.Pupil_Invisible.value} or a {utils.EyeTracker.Pupil_Neon.value}. Cannot use.')
         if not rec_info.proc_directory_name:
             rec_info.proc_directory_name = utils.make_fs_dirname(rec_info, output_dir)
         newDir = output_dir / rec_info.proc_directory_name
         if newDir.is_dir():
             raise RuntimeError(f'Output directory specified in rec_info ({rec_info.proc_directory_name}) already exists in the outputDir ({output_dir}). Cannot use.')
 
     if device is None and rec_info is None:
         raise RuntimeError('Either the "device" or the "rec_info" input argument should be set.')
     if device is not None:
         device = utils.type_string_to_enum(device)
-        if not device in [utils.EyeTracker.Pupil_Core, utils.EyeTracker.Pupil_Invisible]:
-            raise ValueError(f'Provided device ({rec_info.eye_tracker.value}) is not a {utils.EyeTracker.Pupil_Core.value} or a {utils.EyeTracker.Pupil_Invisible.value}.')
+        if not device in [utils.EyeTracker.Pupil_Core, utils.EyeTracker.Pupil_Invisible, utils.EyeTracker.Pupil_Neon]:
+            raise ValueError(f'Provided device ({rec_info.eye_tracker.value}) is not a {utils.EyeTracker.Pupil_Core.value}, a {utils.EyeTracker.Pupil_Invisible.value} or a {utils.EyeTracker.Pupil_Neon.value}.')
     if rec_info is not None:
         if device is not None:
             if rec_info.eye_tracker != device:
                 raise ValueError(f'Provided device ({device.value}) did not match device specific in rec_info ({rec_info.eye_tracker.value}). Provide matching values or do not provide the device input argument.')
         else:
             device = rec_info.eye_tracker
 
-    print(f'processing: {input_dir.name}')
+    print(f'processing: {source_dir.name}')
 
 
     ### check and copy needed files to the output directory
     print('Check and copy raw data...')
     ### check pupil recording and get export directory
-    exportFile = checkPupilRecording(input_dir)
+    exportFile, is_cloud_export = checkPupilRecording(source_dir)
     if rec_info is not None:
-        checkRecording(input_dir, rec_info)
+        checkRecording(source_dir, rec_info)
     else:
-        rec_info = getRecordingInfo(input_dir, device)
+        rec_info = getRecordingInfo(source_dir, device)
         if rec_info is None:
-            raise RuntimeError(f"The folder {input_dir} is not recognized as a {device.value} recording.")
+            raise RuntimeError(f"The folder {source_dir} is not recognized as a {device.value} recording.")
 
     # make output dir
     if rec_info.proc_directory_name is None or not rec_info.proc_directory_name:
         rec_info.proc_directory_name = utils.make_fs_dirname(rec_info, output_dir)
     newDataDir = output_dir / rec_info.proc_directory_name
     if not newDataDir.is_dir():
         newDataDir.mkdir()
@@ -90,119 +90,184 @@
 
     # make sure there is a processing status file, and update it
     utils.get_recording_status(newDataDir, create_if_missing=True)
     utils.update_recording_status(newDataDir, utils.Task.Imported, utils.Status.Running)
 
 
     # copy world video
-    shutil.copyfile(str(input_dir / 'world.mp4'), str(newDataDir / 'worldCamera.mp4'))
+    if is_cloud_export:
+        scene_vid = list(source_dir.glob('*.mp4'))
+        if len(scene_vid)!=1:
+            raise RuntimeError(f'Scene video missing or more than one found for Pupil Cloud export in folder {source_dir}')
+        shutil.copyfile(str(scene_vid[0]), str(newDataDir / 'worldCamera.mp4'))
+    else:
+        shutil.copyfile(str(source_dir / 'world.mp4'), str(newDataDir / 'worldCamera.mp4'))
     print(f'Input data copied to: {newDataDir}')
 
 
     ### get camera cal
     print('Getting camera calibration...')
-    match rec_info.eye_tracker:
-        case utils.EyeTracker.Pupil_Core:
-            sceneVideoDimensions = getCameraFromMsgPack(input_dir, newDataDir)
-        case utils.EyeTracker.Pupil_Invisible:
-            sceneVideoDimensions = getCameraCalFromOnline(input_dir, newDataDir, rec_info)
+    if is_cloud_export:
+        sceneVideoDimensions = getCameraCalFromCloudExport(source_dir, newDataDir, rec_info)
+    else:
+        match rec_info.eye_tracker:
+            case utils.EyeTracker.Pupil_Core:
+                sceneVideoDimensions = getCameraFromMsgPack(source_dir, newDataDir)
+            case utils.EyeTracker.Pupil_Invisible:
+                if (source_dir/'calibration.bin').is_file():
+                    sceneVideoDimensions = getCameraCalFromBinFile(source_dir, newDataDir)
+                else:
+                    sceneVideoDimensions = getCameraCalFromOnline(source_dir, newDataDir, rec_info)
 
 
     ### get gaze data and video frame timestamps
     print('Prepping gaze data...')
-    gazeDf, frameTimestamps = formatGazeData(input_dir, exportFile, sceneVideoDimensions, rec_info)
+    if is_cloud_export:
+        gazeDf, frameTimestamps = formatGazeDataCloudExport(source_dir, exportFile, sceneVideoDimensions, rec_info)
+    else:
+        gazeDf, frameTimestamps = formatGazeDataPupilPlayer(source_dir, exportFile, sceneVideoDimensions, rec_info)
 
     # write the gaze data to a csv file
     gazeDf.to_csv(str(newDataDir / 'gazeData.tsv'), sep='\t', na_rep='nan', float_format="%.8f")
 
     # also store frame timestamps
     frameTimestamps.to_csv(str(newDataDir / 'frameTimestamps.tsv'), sep='\t')
 
     # indicate import finished
     utils.update_recording_status(newDataDir, utils.Task.Imported, utils.Status.Finished)
 
 
 def checkPupilRecording(inputDir):
     """
-    This checks that the folder is properly prepared
-    (i.e. opened in pupil player and an export was run)
+    This checks that the folder is properly prepared,
+    i.e., either:
+    - opened in pupil player and an export was run (currently Pupil Core or Pupil Invisible)
+    - exported from Pupil Cloud (currently Pupil Invisible or Pupil Neon)
     """
     # check we have an info.player.json file
     if not (inputDir / 'info.player.json').is_file():
-        raise RuntimeError(f'info.player.json file not found for {inputDir}. Open the recording in Pupil Player before importing into glassesValidator.')
+        # possibly a pupil cloud export
+        if not (inputDir / 'info.json').is_file() or not (inputDir / 'gaze.csv').is_file():
+            raise RuntimeError(f'Neither the info.player.json file nor the info.json and gaze.csv files are found for {inputDir}. Either export from Pupil Cloud or, if the folder contains raw sensor data, open the recording in Pupil Player and run an export before importing into glassesValidator.')
+        return inputDir / 'gaze.csv', True
 
-    # check we have an export in the input dir
-    inputExpDir = inputDir / 'exports'
-    if not inputExpDir.is_dir():
-        raise RuntimeError(f'no exports folder for {inputDir}. Perform a recording export in Pupil Player before importing into glassesValidator.')
-
-    # get latest export in that folder that contain a gaze position file
-    gpFiles = sorted(list(inputExpDir.rglob('*gaze_positions*.csv')))
-    if not gpFiles:
-        raise RuntimeError(f'There are no exports in the folder {inputExpDir}. Perform a recording export in Pupil Player before importing into glassesValidator.')
+    else:
+        # check we have an export in the input dir
+        inputExpDir = inputDir / 'exports'
+        if not inputExpDir.is_dir():
+            raise RuntimeError(f'no exports folder for {inputDir}. Perform a recording export in Pupil Player before importing into glassesValidator.')
+
+        # get latest export in that folder that contain a gaze position file
+        gpFiles = sorted(list(inputExpDir.rglob('*gaze_positions*.csv')))
+        if not gpFiles:
+            raise RuntimeError(f'There are no exports in the folder {inputExpDir}. Perform a recording export in Pupil Player before importing into glassesValidator.')
 
-    return gpFiles[-1]
+        return gpFiles[-1], False
 
 
 def getRecordingInfo(inputDir, device):
     # returns None if not a recording directory
     recInfo = utils.Recording(source_directory=inputDir, eye_tracker=device)
 
-    match device:
-        case utils.EyeTracker.Pupil_Core:
-            # check this is not an invisible recording
-            file = inputDir / 'info.invisible.json'
-            if file.is_file():
-                return None
-
-            file = inputDir / 'info.player.json'
-            if not file.is_file():
-                return None
-            with open(file, 'r') as j:
-                iInfo = json.load(j)
-            recInfo.name = iInfo['recording_name']
-            recInfo.start_time = utils.Timestamp(int(iInfo['start_time_system_s'])) # UTC in seconds, keep second part
-            recInfo.duration   = int(iInfo['duration_s']*1000)                      # in seconds, convert to ms
-            recInfo.recording_software_version = iInfo['recording_software_version']
-
-            # get user name, if any
-            user_info_file = inputDir / 'user_info.csv'
-            if user_info_file.is_file():
-                df = pd.read_csv(user_info_file)
-                nameRow = df['key'].str.contains('name')
-                if any(nameRow):
-                    if not pd.isnull(df[nameRow].value).to_numpy()[0]:
-                        recInfo.participant = df.loc[nameRow,'value'].to_numpy()[0]
-
-        case utils.EyeTracker.Pupil_Invisible:
-            file = inputDir / 'info.invisible.json'
-            if not file.is_file():
-                return None
-            with open(file, 'r') as j:
-                iInfo = json.load(j)
-            recInfo.name = iInfo['template_data']['recording_name']
-            recInfo.recording_software_version = iInfo['app_version']
-            recInfo.start_time = utils.Timestamp(int(iInfo['start_time']//1000000000))  # UTC in nanoseconds, keep second part
-            recInfo.duration   = int(iInfo['duration']//1000000)                        # in nanoseconds, convert to ms
-            recInfo.glasses_serial = iInfo['glasses_serial_number']
-            recInfo.recording_unit_serial = iInfo['android_device_id']
-            recInfo.scene_camera_serial = iInfo['scene_camera_serial_number']
-            # get participant name
-            file = inputDir / 'wearer.json'
-            if file.is_file():
-                wearer_id = iInfo['wearer_id']
+    if (inputDir / 'info.player.json').is_file():
+        # Pupil player export
+        match device:
+            case utils.EyeTracker.Pupil_Core:
+                # check this is not an invisible recording
+                file = inputDir / 'info.invisible.json'
+                if file.is_file():
+                    return None
+
+                file = inputDir / 'info.player.json'
+                if not file.is_file():
+                    return None
                 with open(file, 'r') as j:
                     iInfo = json.load(j)
-                if wearer_id==iInfo['uuid']:
-                    recInfo.participant = iInfo['name']
+                recInfo.name = iInfo['recording_name']
+                recInfo.start_time = utils.Timestamp(int(iInfo['start_time_system_s'])) # UTC in seconds, keep second part
+                recInfo.duration   = int(iInfo['duration_s']*1000)                      # in seconds, convert to ms
+                recInfo.recording_software_version = iInfo['recording_software_version']
+
+                # get user name, if any
+                user_info_file = inputDir / 'user_info.csv'
+                if user_info_file.is_file():
+                    df = pd.read_csv(user_info_file)
+                    nameRow = df['key'].str.contains('name')
+                    if any(nameRow):
+                        if not pd.isnull(df[nameRow].value).to_numpy()[0]:
+                            recInfo.participant = df.loc[nameRow,'value'].to_numpy()[0]
+
+            case utils.EyeTracker.Pupil_Invisible:
+                file = inputDir / 'info.invisible.json'
+                if not file.is_file():
+                    return None
+                with open(file, 'r') as j:
+                    iInfo = json.load(j)
+                recInfo.name = iInfo['template_data']['recording_name']
+                recInfo.recording_software_version = iInfo['app_version']
+                recInfo.start_time = utils.Timestamp(int(iInfo['start_time']//1000000000))  # UTC in nanoseconds, keep second part
+                recInfo.duration   = int(iInfo['duration']//1000000)                        # in nanoseconds, convert to ms
+                recInfo.glasses_serial = iInfo['glasses_serial_number']
+                recInfo.recording_unit_serial = iInfo['android_device_id']
+                recInfo.scene_camera_serial = iInfo['scene_camera_serial_number']
+                # get participant name
+                file = inputDir / 'wearer.json'
+                if file.is_file():
+                    wearer_id = iInfo['wearer_id']
+                    with open(file, 'r') as j:
+                        iInfo = json.load(j)
+                    if wearer_id==iInfo['uuid']:
+                        recInfo.participant = iInfo['name']
+
+            case utils.EyeTracker.Pupil_Neon:
+                return None # there are no pupil player exports for the Neon eye tracker
+
+            case _:
+                print(f"Device {device} unknown")
+                return None
+    else:
+        # pupil cloud export, for either Pupil Invisible or Pupil Neon
+        if device==utils.EyeTracker.Pupil_Core:
+            return None
+
+        # raw sensor data also contain an info.json (checked below), so checking
+        # that file is not enough to see if this is a Cloud Export. Check gaze.csv
+        # presence
+        if not (inputDir / 'gaze.csv').is_file():
+            return None
+
+        file = inputDir / 'info.json'
+        if not file.is_file():
+            return None
+        with open(file, 'r') as j:
+            iInfo = json.load(j)
 
-        case _:
-            print(f"Device {device} unknown")
+        # check this is for the expected device
+        is_neon = 'Neon' in iInfo['android_device_name'] or 'frame_name' in iInfo
+        if device==utils.EyeTracker.Pupil_Invisible and is_neon:
+            return None
+        elif device==utils.EyeTracker.Pupil_Neon and not is_neon:
             return None
 
+        recInfo.name = iInfo['template_data']['recording_name']
+        recInfo.recording_software_version = iInfo['app_version']
+        recInfo.start_time = utils.Timestamp(int(iInfo['start_time']//1000000000))  # UTC in nanoseconds, keep second part
+        recInfo.duration   = int(iInfo['duration']//1000000)                        # in nanoseconds, convert to ms
+        if is_neon:
+            recInfo.glasses_serial = iInfo['module_serial_number']
+        else:
+            recInfo.glasses_serial = iInfo['glasses_serial_number']
+            recInfo.scene_camera_serial = iInfo['scene_camera_serial_number']
+        recInfo.recording_unit_serial = iInfo['android_device_id']
+        if is_neon:
+            recInfo.firmware_version = f"{iInfo['pipeline_version']} ({iInfo['firmware_version'][0]}.{iInfo['firmware_version'][1]})"
+        else:
+            recInfo.firmware_version = iInfo['pipeline_version']
+        recInfo.participant = iInfo['wearer_name']
+
     # we got a valid recording and at least some info if we got here
     # return what we've got
     return recInfo
 
 
 def checkRecording(inputDir, recInfo):
     actualRecInfo = getRecordingInfo(inputDir, recInfo.eye_tracker)
@@ -213,44 +278,68 @@
     if recInfo.duration!=actualRecInfo.duration:
         raise ValueError(f"A recording with the duration \"{recInfo.duration}\" was not found in the folder {inputDir}.")
     if recInfo.start_time.value!=actualRecInfo.start_time.value:
         raise ValueError(f"A recording with the start_time \"{recInfo.start_time.display}\" was not found in the folder {inputDir}.")
     if recInfo.recording_software_version!=actualRecInfo.recording_software_version:
         raise ValueError(f"A recording with the duration \"{recInfo.duration}\" was not found in the folder {inputDir}.")
 
-    if recInfo.eye_tracker==utils.EyeTracker.Pupil_Invisible:
-        # for invisible recordings we have a bit more info
+    # for invisible and neon recordings we have a bit more info
+    if recInfo.eye_tracker in [utils.EyeTracker.Pupil_Invisible, utils.EyeTracker.Pupil_Neon]:
         if recInfo.glasses_serial!=actualRecInfo.glasses_serial:
             raise ValueError(f"A recording with the glasses_serial \"{recInfo.glasses_serial}\" was not found in the folder {inputDir}.")
         if recInfo.recording_unit_serial!=actualRecInfo.recording_unit_serial:
             raise ValueError(f"A recording with the recording_unit_serial \"{recInfo.recording_unit_serial}\" was not found in the folder {inputDir}.")
-        if recInfo.scene_camera_serial!=actualRecInfo.scene_camera_serial:
+        if recInfo.eye_tracker==utils.EyeTracker.Pupil_Invisible and recInfo.scene_camera_serial!=actualRecInfo.scene_camera_serial:
             raise ValueError(f"A recording with the scene_camera_serial \"{recInfo.scene_camera_serial}\" was not found in the folder {inputDir}.")
         if (recInfo.participant is not None or actualRecInfo.participant is not None) and recInfo.participant!=actualRecInfo.participant:
             raise ValueError(f"A recording with the participant \"{recInfo.participant}\" was not found in the folder {inputDir}.")
 
 
 def getCameraFromMsgPack(inputDir, outputDir):
     """
     Read camera calibration from recording information file
     """
-    camera = getCamInfo(inputDir / 'world.intrinsics')
+    camInfo = getCamInfo(inputDir / 'world.intrinsics')
 
     # rename some fields, ensure they are numpy arrays
-    camera['cameraMatrix'] = np.array(camera.pop('camera_matrix'))
-    camera['distCoeff']    = np.array(camera.pop('dist_coefs')).flatten()
-    camera['resolution']   = np.array(camera['resolution'])
+    camInfo['cameraMatrix'] = np.array(camInfo.pop('camera_matrix'))
+    camInfo['distCoeff']    = np.array(camInfo.pop('dist_coefs')).flatten()
+    camInfo['resolution']   = np.array(camInfo['resolution'])
 
     # store to file
-    fs = cv2.FileStorage(str(outputDir / 'calibration.xml'), cv2.FILE_STORAGE_WRITE)
-    for key,value in camera.items():
-        fs.write(name=key,val=value)
-    fs.release()
+    storeCameraCalibration(camInfo, outputDir)
+
+    return camInfo['resolution']
+
+def getCameraCalFromBinFile(inputDir, outputDir):
+    # provided by pupil-labs
+    cal = np.fromfile(
+        inputDir / 'calibration.bin',
+        np.dtype(
+            [
+                ("serial", "5a"),
+                ("scene_camera_matrix", "(3,3)d"),
+                ("scene_distortion_coefficients", "8d"),
+                ("scene_extrinsics_affine_matrix", "(3,3)d"),
+            ]
+        ),
+    )
+    camInfo = {}
+    camInfo['serial_number']= str(cal["serial"])
+    camInfo['cameraMatrix'] = cal["scene_camera_matrix"].reshape((3,3))
+    camInfo['distCoeff']    = cal["scene_distortion_coefficients"].reshape((8,1))
+    camInfo['extrinsic']    = cal["scene_extrinsics_affine_matrix"].reshape((3,3))
 
-    return camera['resolution']
+    # get resolution from the local intrinsics file or scene video
+    camInfo['resolution']   = getSceneCameraResolution(inputDir, outputDir)
+
+    # store to xml file
+    storeCameraCalibration(camInfo, outputDir)
+
+    return camInfo['resolution']
 
 
 def getCameraCalFromOnline(inputDir, outputDir, recInfo):
     """
     Get camera calibration from pupil labs
     """
     url = f'https://api.cloud.pupil-labs.com/v2/hardware/{recInfo.scene_camera_serial}/calibration.v1?json'
@@ -262,51 +351,86 @@
     camInfo = camInfo['result']
 
     # rename some fields, ensure they are numpy arrays
     camInfo['cameraMatrix'] = np.array(camInfo.pop('camera_matrix'))
     camInfo['distCoeff']    = np.array(camInfo.pop('dist_coefs')).flatten()
     camInfo['rotation']     = np.reshape(np.array(camInfo.pop('rotation_matrix')),(3,3))
 
-    # get resolution from the local intrinsics file
-    camInfo['resolution']   = np.array(getCamInfo(inputDir / 'world.intrinsics')['resolution'])
+    # get resolution from the local intrinsics file or scene video
+    camInfo['resolution']   = getSceneCameraResolution(inputDir, outputDir)
+
+    # store to xml file
+    storeCameraCalibration(camInfo, outputDir)
+
+    return camInfo['resolution']
+
+def getCameraCalFromCloudExport(inputDir, outputDir, recInfo):
+    file = inputDir / 'scene_camera.json'
+    if not file.is_file():
+        return None
+    with open(file, 'r') as j:
+        camInfo = json.load(j)
+
+    camInfo['cameraMatrix'] = np.array(camInfo.pop('camera_matrix'))
+    if 'dist_coefs' in camInfo:
+        camInfo['distCoeff']    = np.array(camInfo.pop('dist_coefs')).flatten()
+    else:
+        camInfo['distCoeff']    = np.array(camInfo.pop('distortion_coefficients')).flatten()
+
+    # get resolution from the scene video
+    camInfo['resolution']   = getSceneCameraResolution(inputDir, outputDir)
 
     # store to xml file
+    storeCameraCalibration(camInfo, outputDir)
+
+    return camInfo['resolution']
+
+def storeCameraCalibration(camInfo, outputDir):
     fs = cv2.FileStorage(str(outputDir / 'calibration.xml'), cv2.FILE_STORAGE_WRITE)
     for key,value in camInfo.items():
         fs.write(name=key,val=value)
     fs.release()
 
-    return camInfo['resolution']
-
-
 def getCamInfo(camInfoFile):
     with open(camInfoFile, 'rb') as f:
         camInfo = msgpack.unpack(f)
 
     # get keys which denote a camera resolution
     rex = re.compile('^\(\d+, \d+\)$')
 
     keys = [k for k in camInfo if rex.match(k)]
     if len(keys)!=1:
         raise RuntimeError('No camera intrinsics or intrinsics for more than one camera found')
     return camInfo[keys[0]]
 
+def getSceneCameraResolution(inputDir, outputDir):
+    if (inputDir / 'world.intrinsics').is_file():
+        return np.array(getCamInfo(inputDir / 'world.intrinsics')['resolution'])
+    else:
+        import cv2
+        cap = cv2.VideoCapture(str(outputDir / 'worldCamera.mp4'))
+        if cap.isOpened():
+            width  = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+            height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+            cap.release()
+        return np.array([width, height])
+
 
-def formatGazeData(inputDir, exportFile, sceneVideoDimensions, recInfo):
+def formatGazeDataPupilPlayer(inputDir, exportFile, sceneVideoDimensions, recInfo):
     """
     load gazedata json file
     format to get the gaze coordinates w/r/t world camera, and timestamps for every frame of video
 
     Returns:
         - formatted dataframe with cols for timestamp, frame_idx, and gaze data
         - np array of frame timestamps
     """
 
     # convert the json file to pandas dataframe
-    df = readGazeData(exportFile, sceneVideoDimensions, recInfo)
+    df = readGazeDataPupilPlayer(exportFile, sceneVideoDimensions, recInfo)
 
     # read video file, create array of frame timestamps
     if (inputDir / 'world_lookup.npy').is_file():
         frameTimestamps = pd.DataFrame(np.load(str(inputDir / 'world_lookup.npy')))
         frameTimestamps['timestamp'] *= 1000.0
         frameTimestamps['frame_idx'] = frameTimestamps.index
         frameTimestamps.loc[frameTimestamps['container_idx']==-1,'container_frame_idx'] = -1
@@ -340,19 +464,18 @@
     t0 = frameTimestamps.iloc[0].to_numpy()
     df.loc[:,'timestamp'] -= t0
     frameTimestamps.loc[:,'timestamp'] -= t0
 
     # set timestamps as index for gaze
     df = df.set_index('timestamp')
 
-    # return the gaze data df and frame time stamps array
     return df, frameTimestamps
 
 
-def readGazeData(file,sceneVideoDimensions, recInfo):
+def readGazeDataPupilPlayer(file, sceneVideoDimensions, recInfo):
     """
     convert the gaze_positions.csv file to a pandas dataframe
     """
     isCore = recInfo.eye_tracker is utils.EyeTracker.Pupil_Core
 
     df = pd.read_csv(file)
 
@@ -400,8 +523,54 @@
     df.loc[:,'timestamp'] *= 1000.0
 
     # turn gaze locations into pixel data with origin in top-left
     df.loc[:,'vid_gaze_pos_x'] *= sceneVideoDimensions[0]
     df.loc[:,'vid_gaze_pos_y'] = (1-df.loc[:,'vid_gaze_pos_y'])*sceneVideoDimensions[1] # turn origin from bottom-left to top-left
 
     # return the dataframe
+    return df
+
+def formatGazeDataCloudExport(inputDir, exportFile, sceneVideoDimensions, recInfo):
+    df = readGazeDataCloudExport(exportFile, sceneVideoDimensions, recInfo)
+
+    frameTimestamps = pd.read_csv(inputDir/'world_timestamps.csv')
+    frameTimestamps = frameTimestamps.rename(columns={'timestamp [ns]': 'timestamp'})
+    frameTimestamps = frameTimestamps.drop(columns=[x for x in frameTimestamps.columns if x not in ['timestamp']])
+    frameTimestamps['frame_idx'] = frameTimestamps.index
+    frameTimestamps = frameTimestamps.set_index('frame_idx')
+    frameTimestamps.loc[:,'timestamp'] /= 1000000.0     # convert timestamps from ns to ms
+
+    # set t=0 to video start time
+    t0 = frameTimestamps.iloc[0].to_numpy()
+    df.loc[:,'timestamp'] -= t0
+    frameTimestamps.loc[:,'timestamp'] -= t0
+
+    # set timestamps as index for gaze
+    df = df.set_index('timestamp')
+
+    # use the frame timestamps to assign a frame number to each data point
+    frameIdx = utils.tssToFrameNumber(df.index,frameTimestamps['timestamp'].to_numpy())
+    df.insert(0,'frame_idx',frameIdx['frame_idx'])
+
+    return df, frameTimestamps
+
+
+def readGazeDataCloudExport(file, sceneVideoDimensions, recInfo):
+    df = pd.read_csv(file)
+
+    # rename and reorder columns
+    lookup = {'timestamp [ns]': 'timestamp',
+              'gaze x [px]': 'vid_gaze_pos_x',
+              'gaze y [px]': 'vid_gaze_pos_y'}
+    df=df.rename(columns=lookup)
+    df=df.drop(columns=[x for x in df.columns if x not in ['timestamp','vid_gaze_pos_x','vid_gaze_pos_y','worn']])
+
+    # mark data where eye tracker is not worn as missing
+    todo = [lookup[k] for k in lookup if lookup[k] in df.columns]
+    toRemove = df.worn == 0
+    for c in todo[2:]:
+        df.loc[toRemove,c] = np.nan
+
+    # convert timestamps from ns to ms
+    df.loc[:,'timestamp'] /= 1000000.0
+
     return df
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator/preprocess/tobii_G2.py` & `glassesValidator-1.0.0/src/glassesValidator/preprocess/tobii_G2.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,50 +21,50 @@
 import struct
 import math
 import datetime
 
 from .. import utils
 
 
-def preprocessData(output_dir, input_dir=None, rec_info=None):
+def preprocessData(output_dir, source_dir=None, rec_info=None):
     """
     Run all preprocessing steps on tobii data
     """
     output_dir = pathlib.Path(output_dir)
-    if input_dir is not None:
-        input_dir  = pathlib.Path(input_dir)
-        if rec_info is not None and pathlib.Path(rec_info.source_directory) != input_dir:
-            raise ValueError(f"The provided source_dir ({input_dir}) does not equal the source directory set in rec_info ({rec_info.source_directory}).")
+    if source_dir is not None:
+        source_dir  = pathlib.Path(source_dir)
+        if rec_info is not None and pathlib.Path(rec_info.source_directory) != source_dir:
+            raise ValueError(f"The provided source_dir ({source_dir}) does not equal the source directory set in rec_info ({rec_info.source_directory}).")
     elif rec_info is None:
         raise RuntimeError('Either the "input_dir" or the "rec_info" input argument should be set.')
     else:
-        input_dir  = pathlib.Path(rec_info.source_directory)
+        source_dir  = pathlib.Path(rec_info.source_directory)
 
     if rec_info is not None:
         if rec_info.eye_tracker!=utils.EyeTracker.Tobii_Glasses_2:
             raise ValueError(f'Provided rec_info is for a device ({rec_info.eye_tracker.value}) that is not an {utils.EyeTracker.Tobii_Glasses_2.value}. Cannot use.')
         if not rec_info.proc_directory_name:
             rec_info.proc_directory_name = utils.make_fs_dirname(rec_info, output_dir)
         newDir = output_dir / rec_info.proc_directory_name
         if newDir.is_dir():
             raise RuntimeError(f'Output directory specified in rec_info ({rec_info.proc_directory_name}) already exists in the outputDir ({output_dir}). Cannot use.')
 
 
-    print(f'processing: {input_dir.name}')
+    print(f'processing: {source_dir.name}')
 
 
     ### check and copy needed files to the output directory
     print('Check and copy raw data...')
     ### check tobii recording and get export directory
     if rec_info is not None:
-        checkRecording(input_dir, rec_info)
+        checkRecording(source_dir, rec_info)
     else:
-        rec_info = getRecordingInfo(input_dir)
+        rec_info = getRecordingInfo(source_dir)
         if rec_info is None:
-            raise RuntimeError(f"The folder {input_dir} is not recognized as a Tobii Glasses 2 recording.")
+            raise RuntimeError(f"The folder {source_dir} is not recognized as a Tobii Glasses 2 recording.")
 
     # make output dir
     if rec_info.proc_directory_name is None or not rec_info.proc_directory_name:
         rec_info.proc_directory_name = utils.make_fs_dirname(rec_info, output_dir)
     newDataDir = output_dir / rec_info.proc_directory_name
     if not newDataDir.is_dir():
         newDataDir.mkdir()
@@ -74,15 +74,15 @@
 
     # make sure there is a processing status file, and update it
     utils.get_recording_status(newDataDir, create_if_missing=True)
     utils.update_recording_status(newDataDir, utils.Task.Imported, utils.Status.Running)
 
 
     ### copy the raw data to the output directory
-    copyTobiiRecording(input_dir, newDataDir)
+    copyTobiiRecording(source_dir, newDataDir)
     print(f'Input data copied to: {newDataDir}')
 
     #### prep the copied data...
     print('Getting camera calibration...')
     sceneVideoDimensions = getCameraFromTSLV(newDataDir)
     print('Prepping gaze data...')
     gazeDf, frameTimestamps = formatGazeData(newDataDir, sceneVideoDimensions)
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator/preprocess/tobii_G3.py` & `glassesValidator-1.0.0/src/glassesValidator/preprocess/tobii_G3.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,50 +20,50 @@
 import numpy as np
 import math
 import datetime
 
 from .. import utils
 
 
-def preprocessData(output_dir, input_dir=None, rec_info=None):
+def preprocessData(output_dir, source_dir=None, rec_info=None):
     """
     Run all preprocessing steps on tobii data
     """
     output_dir = pathlib.Path(output_dir)
-    if input_dir is not None:
-        input_dir  = pathlib.Path(input_dir)
-        if rec_info is not None and pathlib.Path(rec_info.source_directory) != input_dir:
-            raise ValueError(f"The provided source_dir ({input_dir}) does not equal the source directory set in rec_info ({rec_info.source_directory}).")
+    if source_dir is not None:
+        source_dir  = pathlib.Path(source_dir)
+        if rec_info is not None and pathlib.Path(rec_info.source_directory) != source_dir:
+            raise ValueError(f"The provided source_dir ({source_dir}) does not equal the source directory set in rec_info ({rec_info.source_directory}).")
     elif rec_info is None:
         raise RuntimeError('Either the "input_dir" or the "rec_info" input argument should be set.')
     else:
-        input_dir  = pathlib.Path(rec_info.source_directory)
+        source_dir  = pathlib.Path(rec_info.source_directory)
 
     if rec_info is not None:
         if rec_info.eye_tracker!=utils.EyeTracker.Tobii_Glasses_3:
             raise ValueError(f'Provided rec_info is for a device ({rec_info.eye_tracker.value}) that is not an {utils.EyeTracker.Tobii_Glasses_3.value}. Cannot use.')
         if not rec_info.proc_directory_name:
             rec_info.proc_directory_name = utils.make_fs_dirname(rec_info, output_dir)
         newDir = output_dir / rec_info.proc_directory_name
         if newDir.is_dir():
             raise RuntimeError(f'Output directory specified in rec_info ({rec_info.proc_directory_name}) already exists in the outputDir ({output_dir}). Cannot use.')
 
 
-    print(f'processing: {input_dir.name}')
+    print(f'processing: {source_dir.name}')
 
 
     ### check and copy needed files to the output directory
     print('Check and copy raw data...')
     ### check tobii recording and get export directory
     if rec_info is not None:
-        checkRecording(input_dir, rec_info)
+        checkRecording(source_dir, rec_info)
     else:
-        rec_info = getRecordingInfo(input_dir)
+        rec_info = getRecordingInfo(source_dir)
         if rec_info is None:
-            raise RuntimeError(f"The folder {input_dir} is not recognized as a Tobii Glasses 3 recording.")
+            raise RuntimeError(f"The folder {source_dir} is not recognized as a Tobii Glasses 3 recording.")
 
     # make output dir
     if rec_info.proc_directory_name is None or not rec_info.proc_directory_name:
         rec_info.proc_directory_name = utils.make_fs_dirname(rec_info, output_dir)
     newDataDir = output_dir / rec_info.proc_directory_name
     if not newDataDir.is_dir():
         newDataDir.mkdir()
@@ -73,20 +73,20 @@
 
     # make sure there is a processing status file, and update it
     utils.get_recording_status(newDataDir, create_if_missing=True)
     utils.update_recording_status(newDataDir, utils.Task.Imported, utils.Status.Running)
 
 
     ### copy the raw data to the output directory
-    copyTobiiRecording(input_dir, newDataDir)
+    copyTobiiRecording(source_dir, newDataDir)
     print(f'Input data copied to: {newDataDir}')
 
     #### prep the copied data...
     print('Getting camera calibration...')
-    sceneVideoDimensions = getCameraFromJson(input_dir, newDataDir)
+    sceneVideoDimensions = getCameraFromJson(source_dir, newDataDir)
     print('Prepping gaze data...')
     gazeDf, frameTimestamps = formatGazeData(newDataDir, sceneVideoDimensions)
 
     # write the gaze data to a csv file
     gazeDf.to_csv(str(newDataDir / 'gazeData.tsv'), sep='\t', na_rep='nan', float_format="%.8f")
 
     # also store frame timestamps
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator/process/__init__.py` & `glassesValidator-1.0.0/src/glassesValidator/process/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/process/_image_gui.py` & `glassesValidator-1.0.0/src/glassesValidator/process/_image_gui.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/process/b_codeMarkerInterval.py` & `glassesValidator-1.0.0/src/glassesValidator/process/b_codeMarkerInterval.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/process/c_detectMarkers.py` & `glassesValidator-1.0.0/src/glassesValidator/process/c_detectMarkers.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/process/d_gazeToPoster.py` & `glassesValidator-1.0.0/src/glassesValidator/process/d_gazeToPoster.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/process/e1_computeOffsetsToTargets.py` & `glassesValidator-1.0.0/src/glassesValidator/process/e1_computeOffsetsToTargets.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/process/e2_determineFixationIntervals.py` & `glassesValidator-1.0.0/src/glassesValidator/process/e2_determineFixationIntervals.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,32 +112,34 @@
             iFix        = np.argmin(dist)
             selected[i] = iFix
             used[iFix]  = True
 
         # make plot of data overlaid on poster, and show for each target which fixation
         # was selected
         f       = plt.figure(dpi=300)
-        imgplot = plt.imshow(poster.getImgCopy(asRGB=True),extent=(np.array(poster.bbox)[[0,2,1,3]]),alpha=.5)
+        imgplot = plt.imshow(poster.getImgCopy(asRGB=True),extent=(np.array(poster.bbox)[[0,2,3,1]]),alpha=.5)
         plt.plot(fix['xpos'],fix['ypos'],'b-')
         plt.plot(fix['xpos'],fix['ypos'],'go')
         plt.xlim([poster.bbox[0]-markerHalfSizeMm, poster.bbox[2]+markerHalfSizeMm])
         plt.ylim([poster.bbox[1]-markerHalfSizeMm, poster.bbox[3]+markerHalfSizeMm])
+        plt.gca().invert_yaxis()
         for i,t in zip(range(len(targets)),targets):
             if selected[i]==-999:
                 continue
             plt.plot([fix['xpos'][selected[i]], targets[t][0]], [fix['ypos'][selected[i]], targets[t][1]],'r-')
 
         plt.xlabel('mm')
         plt.ylabel('mm')
 
         f.savefig(str(working_dir / 'targetSelection_I2MC_interval_{}.png'.format(ival)))
         plt.close(f)
 
         # also make timseries plot of gaze data with fixations
         f = I2MC.plot.data_and_fixations(data, fix, fix_as_line=True, unit='mm', res=[[poster.bbox[0]-2*markerHalfSizeMm, poster.bbox[2]+2*markerHalfSizeMm], [poster.bbox[1]-2*markerHalfSizeMm, poster.bbox[3]+2*markerHalfSizeMm]])
+        plt.gca().invert_yaxis()
         f.savefig(str(working_dir / 'targetSelection_I2MC_interval_{}_fixations.png'.format(ival)))
         plt.close(f)
 
         # store selected intervals
         df = pd.DataFrame()
         df.index.name = 'target'
         for i,t in zip(range(len(targets)),targets):
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator/process/f_calculateDataQuality.py` & `glassesValidator-1.0.0/src/glassesValidator/process/f_calculateDataQuality.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/resources/fonts/Karla-Regular.ttf` & `glassesValidator-1.0.0/src/glassesValidator/resources/fonts/Karla-Regular.ttf`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/resources/fonts/NotoSans-Regular.ttf` & `glassesValidator-1.0.0/src/glassesValidator/resources/fonts/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/resources/fonts/materialdesignicons-webfont.7.0.96.ttf` & `glassesValidator-1.0.0/src/glassesValidator/resources/fonts/materialdesignicons-webfont.7.0.96.ttf`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/resources/icons/icon.icns` & `glassesValidator-1.0.0/src/glassesValidator/resources/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/resources/icons/icon.ico` & `glassesValidator-1.0.0/src/glassesValidator/resources/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/resources/icons/icon.png` & `glassesValidator-1.0.0/src/glassesValidator/resources/icons/icon.png`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/utils/__init__.py` & `glassesValidator-1.0.0/src/glassesValidator/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,23 +63,25 @@
     def _generate_next_value_(name, start, count, last_values):
         return name.strip("_").replace("__", "-").replace("_", " ")
 
 
 class EyeTracker(AutoName):
     Pupil_Core      = auto()
     Pupil_Invisible = auto()
+    Pupil_Neon      = auto()
     SMI_ETG         = auto()
     SeeTrue         = auto()
     Tobii_Glasses_2 = auto()
     Tobii_Glasses_3 = auto()
     Unknown         = auto()
 eye_tracker_names = [x.value for x in EyeTracker if x!=EyeTracker.Unknown]
 
 EyeTracker.Pupil_Core     .color = hex_to_rgba_0_1("#E6194B")
 EyeTracker.Pupil_Invisible.color = hex_to_rgba_0_1("#3CB44B")
+EyeTracker.Pupil_Neon     .color = hex_to_rgba_0_1("#C6B41E")
 EyeTracker.SMI_ETG        .color = hex_to_rgba_0_1("#4363D8")
 EyeTracker.SeeTrue        .color = hex_to_rgba_0_1("#911EB4")
 EyeTracker.Tobii_Glasses_2.color = hex_to_rgba_0_1("#F58231")
 EyeTracker.Tobii_Glasses_3.color = hex_to_rgba_0_1("#F032E6")
 EyeTracker.Unknown        .color = hex_to_rgba_0_1("#393939")
 
 def type_string_to_enum(device: str):
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator/utils/makeVideo.py` & `glassesValidator-1.0.0/src/glassesValidator/utils/makeVideo.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     # prep output video files
     # get which pixel format
     codec    = ffpyplayer.tools.get_format_codec(fmt='mp4')
     pix_fmt  = ffpyplayer.tools.get_best_pix_fmt('bgr24',ffpyplayer.tools.get_supported_pixfmts(codec))
     fpsFrac  = Fraction(fps).limit_denominator(10000).as_integer_ratio()
     # scene video
-    out_opts = {'pix_fmt_in':'bgr24', 'pix_fmt_out':pix_fmt, 'width_in':int(      width    ), 'height_in':int(      height    ),'frame_rate':fpsFrac}
+    out_opts = {'pix_fmt_in':'bgr24', 'pix_fmt_out':pix_fmt, 'width_in':int(    width   ), 'height_in':int(    height   ),'frame_rate':fpsFrac}
     vidOutScene  = MediaWriter(str(working_dir / 'detectOutput_scene.mp4') , [out_opts], overwrite=True)
     # poster video
     out_opts = {'pix_fmt_in':'bgr24', 'pix_fmt_out':pix_fmt, 'width_in':int(poster.width), 'height_in':int(poster.height),'frame_rate':fpsFrac}
     vidOutPoster = MediaWriter(str(working_dir / 'detectOutput_poster.mp4'), [out_opts], overwrite=True)
 
     # setup aruco marker detection
     parameters = cv2.aruco.DetectorParameters_create()
@@ -201,15 +201,16 @@
             print('  frame {}'.format(frame_idx+1))
 
         frame_idx += 1
 
     vidIn.release()
     vidOutScene.close()
     vidOutPoster.close()
-    cv2.destroyAllWindows()
+    if show_visualization:
+        cv2.destroyAllWindows()
 
     # if ffmpeg is on path, add audio to scene and optionally poster video
     if shutil.which('ffmpeg') is not None:
         todo = [working_dir / 'detectOutput_scene.mp4']
         if add_audio_to_poster_video:
             todo.append(working_dir / 'detectOutput_poster.mp4')
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/core.py` & `glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/core.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/iso.py` & `glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/iso.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/mpeglookups.py` & `glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/mpeglookups.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/non_iso.py` & `glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/non_iso.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/summary.py` & `glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/summary.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator/utils/mp4analyser/util.py` & `glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/util.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-0.11.2/src/glassesValidator.egg-info/PKG-INFO` & `glassesValidator-1.0.0/src/glassesValidator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glassesValidator
-Version: 0.11.2
+Version: 1.0.0
 Summary: Automatic determination of accuracy of wearable eye tracker recordings.
 Home-page: https://github.com/dcnieho/glassesValidator
 Author: Diederick Niehorster
 Author-email: diederick_c.niehorster@humlab.lu.se
 License: MIT License
         
         Copyright (c) 2022-2023 Diederick Niehorster
@@ -24,13 +24,13 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Source Code, https://github.com/dcnieho/glassesValidator
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: ==3.10.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `glassesValidator-0.11.2/src/glassesValidator.egg-info/SOURCES.txt` & `glassesValidator-1.0.0/src/glassesValidator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 requirements.txt
 setup.py
 src/glassesValidator/__init__.py
 src/glassesValidator/version.py
 src/glassesValidator.egg-info/PKG-INFO
 src/glassesValidator.egg-info/SOURCES.txt
 src/glassesValidator.egg-info/dependency_links.txt
+src/glassesValidator.egg-info/entry_points.txt
 src/glassesValidator.egg-info/requires.txt
 src/glassesValidator.egg-info/top_level.txt
 src/glassesValidator/GUI/__init__.py
 src/glassesValidator/GUI/_general_imgui.py
 src/glassesValidator/GUI/_impl/__init__.py
 src/glassesValidator/GUI/_impl/async_thread.py
 src/glassesValidator/GUI/_impl/callbacks.py
```

