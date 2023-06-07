# Comparing `tmp/BDPotentiometer-0.0.1.tar.gz` & `tmp/BDPotentiometer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDPotentiometer-0.0.1.tar", last modified: Thu Apr 27 06:30:38 2023, max compression
+gzip compressed data, was "BDPotentiometer-0.0.2.tar", last modified: Wed Jun  7 21:48:36 2023, max compression
```

## Comparing `BDPotentiometer-0.0.1.tar` & `BDPotentiometer-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-04-27 06:30:38.901796 BDPotentiometer-0.0.1/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-04-27 06:30:38.899231 BDPotentiometer-0.0.1/BDPotentiometer/
--rw-r--r--   0 anton      (501) staff       (20)    10198 2023-04-27 06:18:49.000000 BDPotentiometer-0.0.1/BDPotentiometer/DigitalPotentiometer.py
--rw-r--r--   0 anton      (501) staff       (20)     6236 2023-04-27 06:20:25.000000 BDPotentiometer-0.0.1/BDPotentiometer/MCP4xx1.py
--rw-r--r--   0 anton      (501) staff       (20)     1690 2023-04-27 06:20:25.000000 BDPotentiometer-0.0.1/BDPotentiometer/MCP4xx2.py
--rw-r--r--   0 anton      (501) staff       (20)     3616 2023-04-26 15:34:59.000000 BDPotentiometer-0.0.1/BDPotentiometer/MCP4xxx.py
--rw-r--r--   0 anton      (501) staff       (20)     1046 2023-04-26 16:50:04.000000 BDPotentiometer-0.0.1/BDPotentiometer/__gpiozero_helpers.py
--rw-r--r--   0 anton      (501) staff       (20)     3116 2023-04-26 15:23:37.000000 BDPotentiometer-0.0.1/BDPotentiometer/__helpers.py
--rw-r--r--   0 anton      (501) staff       (20)      365 2023-04-26 16:50:04.000000 BDPotentiometer-0.0.1/BDPotentiometer/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)       22 2023-04-21 08:30:19.000000 BDPotentiometer-0.0.1/BDPotentiometer/_version.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-04-27 06:30:38.901373 BDPotentiometer-0.0.1/BDPotentiometer.egg-info/
--rw-r--r--   0 anton      (501) staff       (20)     1425 2023-04-27 06:30:38.000000 BDPotentiometer-0.0.1/BDPotentiometer.egg-info/PKG-INFO
--rw-r--r--   0 anton      (501) staff       (20)      478 2023-04-27 06:30:38.000000 BDPotentiometer-0.0.1/BDPotentiometer.egg-info/SOURCES.txt
--rw-r--r--   0 anton      (501) staff       (20)        1 2023-04-27 06:30:38.000000 BDPotentiometer-0.0.1/BDPotentiometer.egg-info/dependency_links.txt
--rw-r--r--   0 anton      (501) staff       (20)       16 2023-04-27 06:30:38.000000 BDPotentiometer-0.0.1/BDPotentiometer.egg-info/top_level.txt
--rw-r--r--   0 anton      (501) staff       (20)    11358 2023-04-21 08:16:42.000000 BDPotentiometer-0.0.1/LICENSE.txt
--rw-r--r--   0 anton      (501) staff       (20)      272 2023-04-21 08:30:19.000000 BDPotentiometer-0.0.1/MANIFEST.in
--rw-r--r--   0 anton      (501) staff       (20)       78 2023-04-21 08:30:19.000000 BDPotentiometer-0.0.1/NOTICE.txt
--rw-r--r--   0 anton      (501) staff       (20)     1425 2023-04-27 06:30:38.901929 BDPotentiometer-0.0.1/PKG-INFO
--rw-r--r--   0 anton      (501) staff       (20)      556 2023-04-26 15:00:24.000000 BDPotentiometer-0.0.1/README.md
--rw-r--r--   0 anton      (501) staff       (20)      118 2023-04-26 08:32:51.000000 BDPotentiometer-0.0.1/pyproject.toml
--rw-r--r--   0 anton      (501) staff       (20)       79 2023-04-27 06:30:38.902423 BDPotentiometer-0.0.1/setup.cfg
--rw-r--r--   0 anton      (501) staff       (20)     1651 2023-04-26 08:56:59.000000 BDPotentiometer-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:48:36.110678 BDPotentiometer-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-07 21:48:36.110678 BDPotentiometer-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:48:36.110678 BDPotentiometer-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:48:36.106677 BDPotentiometer-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:48:36.106677 BDPotentiometer-0.0.2/src/BDPotentiometer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/src/BDPotentiometer/__gpiozero_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/src/BDPotentiometer/__helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/src/BDPotentiometer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/src/BDPotentiometer/digital_potentiometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/src/BDPotentiometer/digital_wiper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:48:36.106677 BDPotentiometer-0.0.2/src/BDPotentiometer/mcp4xxx/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/src/BDPotentiometer/mcp4xxx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/src/BDPotentiometer/mcp4xxx/mcp4xx1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/src/BDPotentiometer/mcp4xxx/mcp4xx2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/src/BDPotentiometer/mcp4xxx/mcp4xxx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/src/BDPotentiometer/potentiometer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:48:36.106677 BDPotentiometer-0.0.2/src/BDPotentiometer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-07 21:48:36.000000 BDPotentiometer-0.0.2/src/BDPotentiometer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-07 21:48:36.000000 BDPotentiometer-0.0.2/src/BDPotentiometer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:48:36.000000 BDPotentiometer-0.0.2/src/BDPotentiometer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 21:48:36.000000 BDPotentiometer-0.0.2/src/BDPotentiometer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 21:48:36.000000 BDPotentiometer-0.0.2/src/BDPotentiometer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:48:36.110678 BDPotentiometer-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12697 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/tests/test_digital_potentiometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/tests/test_digital_wiper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/tests/test_potentiometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-07 21:48:24.000000 BDPotentiometer-0.0.2/tests/test_version.py
```

