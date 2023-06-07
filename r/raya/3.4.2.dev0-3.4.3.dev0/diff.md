# Comparing `tmp/raya-3.4.2.dev0.tar.gz` & `tmp/raya-3.4.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raya-3.4.2.dev0.tar", last modified: Mon Jun  5 21:36:42 2023, max compression
+gzip compressed data, was "raya-3.4.3.dev0.tar", last modified: Wed Jun  7 02:53:20 2023, max compression
```

## Comparing `raya-3.4.2.dev0.tar` & `raya-3.4.3.dev0.tar`

### file list

```diff
@@ -1,76 +1,75 @@
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-06-05 21:36:42.656989 raya-3.4.2.dev0/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1074 2023-01-29 19:45:42.000000 raya-3.4.2.dev0/LICENSE
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      534 2023-06-05 21:36:42.656989 raya-3.4.2.dev0/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      150 2023-05-15 19:14:17.000000 raya-3.4.2.dev0/README.md
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      103 2023-01-29 19:45:42.000000 raya-3.4.2.dev0/pyproject.toml
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       38 2023-06-05 21:36:42.656989 raya-3.4.2.dev0/setup.cfg
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2752 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/setup.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-06-05 21:36:42.652989 raya-3.4.2.dev0/src/
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-06-05 21:36:42.652989 raya-3.4.2.dev0/src/raya/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       38 2023-05-15 19:14:17.000000 raya-3.4.2.dev0/src/raya/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       25 2023-06-05 16:50:03.000000 raya-3.4.2.dev0/src/raya/_version.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     3183 2023-06-05 21:36:41.000000 raya-3.4.2.dev0/src/raya/application_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      664 2023-06-05 21:36:41.000000 raya-3.4.2.dev0/src/raya/constants.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-06-05 21:36:42.652989 raya-3.4.2.dev0/src/raya/controllers/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.2.dev0/src/raya/controllers/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      260 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/analytics_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)    17485 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/arms_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      620 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/base_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       90 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/base_pseudo_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1222 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/cameras_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      425 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/communication_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2838 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/cv_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1387 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/fleet_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      523 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/grasping_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      924 2023-06-05 21:36:41.000000 raya-3.4.2.dev0/src/raya/controllers/interactions_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1298 2023-06-05 21:36:41.000000 raya-3.4.2.dev0/src/raya/controllers/leds_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1171 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/lidar_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     3127 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/manipulation_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2042 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/motion_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     7148 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/navigation_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1367 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/sensors_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      808 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/skills_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2590 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/sound_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     8614 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/controllers/ui_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       59 2023-06-05 21:36:41.000000 raya-3.4.2.dev0/src/raya/entry_point.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     4681 2023-06-05 21:36:41.000000 raya-3.4.2.dev0/src/raya/enumerations.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)    13099 2023-06-05 21:36:41.000000 raya-3.4.2.dev0/src/raya/exceptions.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6272 2023-06-05 21:36:41.000000 raya-3.4.2.dev0/src/raya/exceptions_handler.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-06-05 21:36:42.652989 raya-3.4.2.dev0/src/raya/handlers/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-06-05 16:48:28.000000 raya-3.4.2.dev0/src/raya/handlers/__init__.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-06-05 21:36:42.656989 raya-3.4.2.dev0/src/raya/handlers/cv/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-06-05 16:48:28.000000 raya-3.4.2.dev0/src/raya/handlers/cv/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      877 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/classifier_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      844 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/detector_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      743 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/estimator_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      302 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/faces_detector_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      831 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/faces_recognizer_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      305 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/hand_estimator_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      183 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/model_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      790 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/objects_classifier_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      782 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/objects_detector_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      794 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/objects_segmentator_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      783 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/planes_segmentator_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      862 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/recognizer_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      871 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/segmentator_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      703 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/cv/tags_detector_handler.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-06-05 21:36:42.656989 raya-3.4.2.dev0/src/raya/handlers/general/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-06-05 16:48:28.000000 raya-3.4.2.dev0/src/raya/handlers/general/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      330 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/handlers/general/callback_handler.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-06-05 21:36:42.656989 raya-3.4.2.dev0/src/raya/listeners/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.2.dev0/src/raya/listeners/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       77 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/listeners/lidar_listeners.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      160 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/listeners/sensors_listeners.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      352 2023-06-05 21:36:41.000000 raya-3.4.2.dev0/src/raya/logger.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2055 2023-06-05 21:36:41.000000 raya-3.4.2.dev0/src/raya/raya_interface.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      257 2023-06-05 21:36:41.000000 raya-3.4.2.dev0/src/raya/standalone_handler.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-06-05 21:36:42.656989 raya-3.4.2.dev0/src/raya/tools/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.2.dev0/src/raya/tools/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/tools/filesystem.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      984 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/tools/fsm.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      152 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya/tools/image.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-06-05 21:36:42.652989 raya-3.4.2.dev0/src/raya.egg-info/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      534 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya.egg-info/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2314 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya.egg-info/SOURCES.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya.egg-info/dependency_links.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        5 2023-06-05 21:36:42.000000 raya-3.4.2.dev0/src/raya.egg-info/top_level.txt
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/PKG-INFO
+-rw-rw-r--   0 prod      (1001) prod      (1001)      150 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/README.md
+-rw-rw-r--   0 prod      (1001) prod      (1001)      103 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/pyproject.toml
+-rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/setup.cfg
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2752 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/setup.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.682632 raya-3.4.3.dev0/src/
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.682632 raya-3.4.3.dev0/src/raya/
+-rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       25 2023-06-07 02:53:11.000000 raya-3.4.3.dev0/src/raya/_version.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3183 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/application_base.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      664 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/constants.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.682632 raya-3.4.3.dev0/src/raya/controllers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/controllers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      260 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/analytics_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)    17485 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/arms_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      620 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/base_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       90 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/base_pseudo_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1222 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/cameras_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      425 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/controllers/communication_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2838 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/controllers/cv_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1387 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/fleet_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      523 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/grasping_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      924 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/controllers/interactions_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1298 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/leds_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1171 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/lidar_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3127 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/manipulation_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2042 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/controllers/motion_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     7148 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/navigation_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1367 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/sensors_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      808 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/skills_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2590 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/controllers/sound_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     8614 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/ui_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       59 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/entry_point.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     4681 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/enumerations.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)    13099 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/exceptions.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     6272 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/exceptions_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.682632 raya-3.4.3.dev0/src/raya/handlers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/handlers/__init__.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/src/raya/handlers/cv/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/handlers/cv/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      877 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/classifier_handler_base.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      844 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/detector_handler_base.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      743 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/estimator_handler_base.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      302 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/faces_detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      831 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/faces_recognizer_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      305 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/hand_estimator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      183 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/model_base.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      790 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/objects_classifier_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      782 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/objects_detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      794 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/objects_segmentator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      783 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/planes_segmentator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      862 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/recognizer_handler_base.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      871 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/segmentator_handler_base.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      703 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/tags_detector_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/src/raya/handlers/general/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/handlers/general/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      330 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/general/callback_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/src/raya/listeners/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/listeners/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       77 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/listeners/lidar_listeners.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      160 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/listeners/sensors_listeners.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      352 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/logger.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2055 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/raya_interface.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      257 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/standalone_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/src/raya/tools/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/tools/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      399 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/tools/filesystem.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      984 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/tools/fsm.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      152 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/tools/image.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.682632 raya-3.4.3.dev0/src/raya.egg-info/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya.egg-info/PKG-INFO
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2306 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya.egg-info/SOURCES.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)        1 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya.egg-info/dependency_links.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)        5 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya.egg-info/top_level.txt
```

### Comparing `raya-3.4.2.dev0/setup.py` & `raya-3.4.3.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/application_base.py` & `raya-3.4.3.dev0/src/raya/application_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/constants.py` & `raya-3.4.3.dev0/src/raya/constants.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/arms_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/arms_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/base_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/cameras_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/cameras_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/cv_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/cv_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/fleet_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/fleet_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/grasping_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/grasping_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/interactions_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/interactions_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/leds_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/leds_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/lidar_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/lidar_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/manipulation_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/manipulation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/motion_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/motion_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/navigation_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/navigation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/sensors_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/sensors_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/skills_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/skills_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/sound_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/sound_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/controllers/ui_controller.py` & `raya-3.4.3.dev0/src/raya/controllers/ui_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/enumerations.py` & `raya-3.4.3.dev0/src/raya/enumerations.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/exceptions.py` & `raya-3.4.3.dev0/src/raya/exceptions.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/exceptions_handler.py` & `raya-3.4.3.dev0/src/raya/exceptions_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/handlers/cv/classifier_handler_base.py` & `raya-3.4.3.dev0/src/raya/handlers/cv/classifier_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/handlers/cv/detector_handler_base.py` & `raya-3.4.3.dev0/src/raya/handlers/cv/detector_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/handlers/cv/estimator_handler_base.py` & `raya-3.4.3.dev0/src/raya/handlers/cv/estimator_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/handlers/cv/faces_recognizer_handler.py` & `raya-3.4.3.dev0/src/raya/handlers/cv/faces_recognizer_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/handlers/cv/objects_classifier_handler.py` & `raya-3.4.3.dev0/src/raya/handlers/cv/objects_classifier_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/handlers/cv/objects_detector_handler.py` & `raya-3.4.3.dev0/src/raya/handlers/cv/objects_detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/handlers/cv/objects_segmentator_handler.py` & `raya-3.4.3.dev0/src/raya/handlers/cv/objects_segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/handlers/cv/planes_segmentator_handler.py` & `raya-3.4.3.dev0/src/raya/handlers/cv/planes_segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/handlers/cv/recognizer_handler_base.py` & `raya-3.4.3.dev0/src/raya/handlers/cv/recognizer_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/handlers/cv/segmentator_handler_base.py` & `raya-3.4.3.dev0/src/raya/handlers/cv/segmentator_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/handlers/cv/tags_detector_handler.py` & `raya-3.4.3.dev0/src/raya/handlers/cv/tags_detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/raya_interface.py` & `raya-3.4.3.dev0/src/raya/raya_interface.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya/tools/fsm.py` & `raya-3.4.3.dev0/src/raya/tools/fsm.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.2.dev0/src/raya.egg-info/SOURCES.txt` & `raya-3.4.3.dev0/src/raya.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 pyproject.toml
 setup.py
 src/raya/__init__.py
 src/raya/_version.py
 src/raya/application_base.py
 src/raya/constants.py
```

