# Comparing `tmp/eikobot-0.4.0.tar.gz` & `tmp/eikobot-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eikobot-0.4.0.tar", last modified: Sat Mar 11 12:58:22 2023, max compression
+gzip compressed data, was "eikobot-0.5.0.tar", last modified: Wed Jun  7 14:02:39 2023, max compression
```

## Comparing `eikobot-0.4.0.tar` & `eikobot-0.5.0.tar`

### file list

```diff
@@ -1,65 +1,77 @@
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-03-11 12:58:22.831917 eikobot-0.4.0/
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1059 2023-03-11 12:53:50.000000 eikobot-0.4.0/LICENSE
--rw-r--r--   0 yaron     (1000) yaron     (1000)     3121 2023-03-11 12:58:22.831917 eikobot-0.4.0/PKG-INFO
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2731 2023-03-11 12:53:50.000000 eikobot-0.4.0/README.md
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-03-11 12:58:22.823917 eikobot-0.4.0/eikobot/
--rw-r--r--   0 yaron     (1000) yaron     (1000)       83 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     4474 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/__main__.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-03-11 12:58:22.827917 eikobot-0.4.0/eikobot/core/
--rw-r--r--   0 yaron     (1000) yaron     (1000)       39 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/core/__init__.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-03-11 12:58:22.827917 eikobot-0.4.0/eikobot/core/compiler/
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1263 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/core/compiler/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    81082 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/compiler/_parser.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1648 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/compiler/_token.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2420 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/compiler/decorator.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-03-11 12:58:22.831917 eikobot-0.4.0/eikobot/core/compiler/definitions/
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/core/compiler/definitions/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2786 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/compiler/definitions/_resource.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1480 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/compiler/definitions/base_model.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    31274 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/compiler/definitions/base_types.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    12465 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/compiler/definitions/context.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    11974 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/compiler/definitions/function.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2777 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/compiler/definitions/typedef.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     8553 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/compiler/importlib.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     9121 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/compiler/lexer.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      306 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/core/compiler/misc.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     8892 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/core/compiler/ops.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2513 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/deployer.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2452 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/errors.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     7891 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/exporter.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     3485 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/handlers.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      359 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/helpers.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-03-11 12:58:22.831917 eikobot-0.4.0/eikobot/core/lib/
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/core/lib/__init__.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-03-11 12:58:22.831917 eikobot-0.4.0/eikobot/core/lib/std/
--rw-r--r--   0 yaron     (1000) yaron     (1000)      478 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/lib/std/__init__.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)     8906 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/lib/std/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/core/lib/std/env.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1486 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/lib/std/env.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      316 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/lib/std/file.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)     7209 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/lib/std/file.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/core/lib/std/regex.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)      325 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/core/lib/std/regex.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)       50 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/core/lib/std/test.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)      519 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/core/lib/std/test.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2248 2023-03-11 12:53:50.000000 eikobot-0.4.0/eikobot/core/logger.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      803 2023-01-12 15:52:05.000000 eikobot-0.4.0/eikobot/core/plugin.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-03-11 12:58:22.823917 eikobot-0.4.0/eikobot.egg-info/
--rw-r--r--   0 yaron     (1000) yaron     (1000)     3121 2023-03-11 12:58:22.000000 eikobot-0.4.0/eikobot.egg-info/PKG-INFO
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1583 2023-03-11 12:58:22.000000 eikobot-0.4.0/eikobot.egg-info/SOURCES.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)        1 2023-03-11 12:58:22.000000 eikobot-0.4.0/eikobot.egg-info/dependency_links.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)       49 2023-03-11 12:58:22.000000 eikobot-0.4.0/eikobot.egg-info/entry_points.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)       77 2023-03-11 12:58:22.000000 eikobot-0.4.0/eikobot.egg-info/requires.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)        8 2023-03-11 12:58:22.000000 eikobot-0.4.0/eikobot.egg-info/top_level.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)     4058 2023-03-11 12:58:22.835917 eikobot-0.4.0/setup.cfg
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1150 2023-03-11 12:53:50.000000 eikobot-0.4.0/setup.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-03-11 12:58:22.831917 eikobot-0.4.0/tests/
--rw-r--r--   0 yaron     (1000) yaron     (1000)     8295 2023-03-11 12:53:50.000000 eikobot-0.4.0/tests/test_compilation.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2792 2023-01-12 15:52:05.000000 eikobot-0.4.0/tests/test_datatypes.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      750 2023-01-12 15:52:05.000000 eikobot-0.4.0/tests/test_decorator.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     5979 2023-03-11 12:53:50.000000 eikobot-0.4.0/tests/test_deployer.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1350 2023-03-11 12:53:50.000000 eikobot-0.4.0/tests/test_exporter.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2353 2023-03-11 12:53:50.000000 eikobot-0.4.0/tests/test_import.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    16877 2023-01-12 15:52:05.000000 eikobot-0.4.0/tests/test_lexer.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     9480 2023-01-12 15:52:05.000000 eikobot-0.4.0/tests/test_parser.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      409 2023-03-11 12:53:50.000000 eikobot-0.4.0/tests/test_promises.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.167419 eikobot-0.5.0/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1059 2023-06-05 11:53:10.000000 eikobot-0.5.0/LICENSE
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     3252 2023-06-07 14:02:39.167419 eikobot-0.5.0/PKG-INFO
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2644 2023-06-07 14:01:19.000000 eikobot-0.5.0/README.md
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      159 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     6055 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/__main__.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)       39 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/__init__.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/compiler/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1263 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    85130 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/_parser.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1666 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/_token.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2420 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/decorator.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/compiler/definitions/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2786 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/_resource.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1593 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/base_model.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    35673 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/base_types.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    12465 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/context.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    12376 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/function.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2777 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/typedef.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     8553 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/importlib.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     9149 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/lexer.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      306 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/misc.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     8779 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/ops.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2828 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/deployer.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2893 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/errors.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     8016 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/exporter.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     4755 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/handlers.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      395 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/helpers.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/lib/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/__init__.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/lib/docker/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      974 2023-06-04 18:43:55.000000 eikobot-0.5.0/eikobot/core/lib/docker/__init__.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     4771 2023-06-07 10:53:48.000000 eikobot-0.5.0/eikobot/core/lib/docker/__init__.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/lib/std/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      819 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/lib/std/__init__.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    14244 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/lib/std/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/std/env.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1486 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/std/env.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      316 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/std/file.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     6997 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/lib/std/file.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/std/regex.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      325 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/std/regex.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)       50 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/std/test.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      520 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/lib/std/test.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2248 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/logger.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/package_manager/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    10302 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/package_manager/__init__.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.159419 eikobot-0.5.0/eikobot/core/package_manager/lib/
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.159419 eikobot-0.5.0/eikobot/core/package_manager/lib/eikobot-docker-0.0.2/
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.167419 eikobot-0.5.0/eikobot/core/package_manager/lib/eikobot-docker-0.0.2/docker/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      974 2023-06-04 18:43:55.000000 eikobot-0.5.0/eikobot/core/package_manager/lib/eikobot-docker-0.0.2/docker/__init__.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     4771 2023-06-07 10:53:48.000000 eikobot-0.5.0/eikobot/core/package_manager/lib/eikobot-docker-0.0.2/docker/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      803 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/plugin.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/py.typed
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot.egg-info/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     3252 2023-06-07 14:02:39.000000 eikobot-0.5.0/eikobot.egg-info/PKG-INFO
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1885 2023-06-07 14:02:39.000000 eikobot-0.5.0/eikobot.egg-info/SOURCES.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        1 2023-06-07 14:02:39.000000 eikobot-0.5.0/eikobot.egg-info/dependency_links.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)       49 2023-06-07 14:02:39.000000 eikobot-0.5.0/eikobot.egg-info/entry_points.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      108 2023-06-07 14:02:39.000000 eikobot-0.5.0/eikobot.egg-info/requires.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        8 2023-06-07 14:02:39.000000 eikobot-0.5.0/eikobot.egg-info/top_level.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     4076 2023-06-07 14:02:39.167419 eikobot-0.5.0/setup.cfg
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1401 2023-06-07 14:01:19.000000 eikobot-0.5.0/setup.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.167419 eikobot-0.5.0/tests/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     8976 2023-06-07 14:01:19.000000 eikobot-0.5.0/tests/test_compilation.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2792 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_datatypes.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      750 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_decorator.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     5979 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_deployer.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1350 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_exporter.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2353 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_import.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    16877 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_lexer.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      921 2023-06-07 14:01:19.000000 eikobot-0.5.0/tests/test_package.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     9776 2023-06-07 14:01:19.000000 eikobot-0.5.0/tests/test_parser.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      409 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_promises.py
```

### Comparing `eikobot-0.4.0/LICENSE` & `eikobot-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/PKG-INFO` & `eikobot-0.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: eikobot
-Version: 0.4.0
+Version: 0.5.0
 Summary: The eikobot desired state engine.
 Author: kazaamjt
 Author-email: kazaamjt@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Utilities
+Classifier: Intended Audience :: System Administrators
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Eikobot Desired State Engine
 
 *The little Desired State Engine that made it so.*  
 
@@ -30,24 +35,23 @@
 
 Some of it's notable features are:  
 
 - Object oriented
 - sees the infrastructure as a tree of resources, rather than a flatland
 - completely stateless*
 
-The quickest way to get started is probably by doing some of the [quickstarts](https://github.com/kazaamjt/Eikobot/blob/main/docs/quickstart.md).  
+The quickest way to get started is probably by doing some of the [quickstarts](https://github.com/kazaamjt/Eikobot/blob/main/docs/quickstarts.md).  
 For a more complete idea of how the language works,
 please see the [language overview](https://github.com/kazaamjt/Eikobot/blob/main/docs/language_overview.md).  
 
 (*If the model/modules are designed well.)  
 
 ## Installation
 
-Eikobot requires python 3.10 or up and has 3 external dependencies that can be installed using pip.  
-In fact, Eikobot can be installed using pip as well.  
+Eikobot requires python 3.10 or up and can be installed using pip.  
 
 Here is an example of how to install Eikobot:  
 (This should work on most platforms, although the python command is different if you are on windows)
 
 ```bash
 python3.10 -m venv eikobot-venv
 eikobot-venv/bin/pip install eikobot
```

### Comparing `eikobot-0.4.0/README.md` & `eikobot-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,24 +16,23 @@
 
 Some of it's notable features are:  
 
 - Object oriented
 - sees the infrastructure as a tree of resources, rather than a flatland
 - completely stateless*
 
-The quickest way to get started is probably by doing some of the [quickstarts](https://github.com/kazaamjt/Eikobot/blob/main/docs/quickstart.md).  
+The quickest way to get started is probably by doing some of the [quickstarts](https://github.com/kazaamjt/Eikobot/blob/main/docs/quickstarts.md).  
 For a more complete idea of how the language works,
 please see the [language overview](https://github.com/kazaamjt/Eikobot/blob/main/docs/language_overview.md).  
 
 (*If the model/modules are designed well.)  
 
 ## Installation
 
-Eikobot requires python 3.10 or up and has 3 external dependencies that can be installed using pip.  
-In fact, Eikobot can be installed using pip as well.  
+Eikobot requires python 3.10 or up and can be installed using pip.  
 
 Here is an example of how to install Eikobot:  
 (This should work on most platforms, although the python command is different if you are on windows)
 
 ```bash
 python3.10 -m venv eikobot-venv
 eikobot-venv/bin/pip install eikobot
```

### Comparing `eikobot-0.4.0/eikobot/__main__.py` & `eikobot-0.5.0/eikobot/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 import sys
 import time
 import traceback
 from pathlib import Path
 
 import click
 
-from .core import logger
+from . import VERSION
+from .core import logger, package_manager
 from .core.compiler import Compiler
 from .core.compiler.lexer import Token
 from .core.deployer import Deployer
 from .core.errors import EikoError, EikoPluginError
 from .core.exporter import Exporter
 
 
 @click.group()
 @click.option("--debug", is_flag=True)
+@click.version_option(VERSION)
 def cli(debug: bool = False) -> None:
     """
     The Eikobot CLI allows for compilation
     and exporting of eiko files.
     """
     log_level = logger.LOG_LEVEL.INFO
     if debug:
@@ -111,39 +113,105 @@
         f"(Process time: {pc_time_taken_formatted})"
     )
 
     return compiler
 
 
 @cli.command()
-@click.option("-f", "--file", prompt="File", help="Path to entrypoint file.")
+@click.option("-f", "--file", "file", prompt="File", help="Path to entrypoint file.")
 @click.option(
     "--enable-plugin-stacktrace",
     is_flag=True,
     help="Outputs a plugins stacktrace if it raises an exception.",
 )
-def deploy(file: str, enable_plugin_stacktrace: bool = False) -> None:
+@click.option(
+    "--dry-run",
+    is_flag=True,
+    help="Does a dry run of all the tasks in a given model.",
+)
+def deploy(
+    file: str,
+    enable_plugin_stacktrace: bool = False,
+    dry_run: bool = False,
+) -> None:
     """
     Compile, export and deploy a model from a given file.
     """
     start = time.time()
     compiler = _compile(file, False, enable_plugin_stacktrace)
     logger.info("Exporting model.")
-    exporter = Exporter()
-    exporter.export_from_context(compiler.context)
-    logger.info("Deploying model.")
-    deployer = Deployer()
-    asyncio.run(deployer.deploy(exporter, log_progress=True))
-
-    if deployer.failed:
-        logger.error(
-            "Failed to deploy model. "
-            f"({deployer.progress.done} out of {deployer.progress.total} tasks done)"
-        )
+    try:
+        exporter = Exporter()
+        exporter.export_from_context(compiler.context)
+        logger.info("Deploying model.")
+        deployer = Deployer()
+        if dry_run:
+            asyncio.run(deployer.dry_run(exporter))
+        else:
+            asyncio.run(deployer.deploy(exporter, log_progress=True))
+    except EikoError as e:
+        logger.error(str(e))
+
+        if e.index is not None:
+            logger.print_error_trace(e.index)
     else:
-        time_taken = time.time() - start
-        time_taken_formatted = str(datetime.timedelta(seconds=time_taken))
-        logger.info(f"Deployed in {time_taken_formatted}")
+        if deployer.failed:
+            logger.error(
+                "Failed to deploy model. "
+                f"({deployer.progress.done} out of {deployer.progress.total} tasks done)"
+            )
+        else:
+            time_taken = time.time() - start
+            time_taken_formatted = str(datetime.timedelta(seconds=time_taken))
+            logger.info(f"Deployed in {time_taken_formatted}")
+
+
+@cli.group()
+def package() -> None:
+    pass
+
+
+@package.command(name="build")
+def build_pkg() -> None:
+    """Builds a package in the cwd, using an eiko.toml file."""
+    try:
+        package_manager.build_pkg()
+    except EikoError as e:
+        logger.error(str(e))
+
+
+@package.command(name="install")
+@click.argument("target")
+def install_pkg(target: str) -> None:
+    """
+    Install a package from different sources.
+    """
+    try:
+        package_manager.install_pkg(target)
+    except EikoError as e:
+        logger.error(str(e))
+
+
+@package.command(name="list")
+def list_pkg() -> None:
+    """
+    Lists all installed packages.
+    """
+    packages = package_manager.get_installed_pkg()
+    for pkg in packages.values():
+        print(f"{pkg.name}=={pkg.version}")
+
+
+@package.command(name="uninstall")
+@click.argument("name")
+def uninstall_pkg(name: str) -> None:
+    """
+    Performs all required steps to delete a package.
+    """
+    try:
+        package_manager.uninstall_pkg(name)
+    except EikoError as e:
+        logger.error(str(e))
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `eikobot-0.4.0/eikobot/core/compiler/__init__.py` & `eikobot-0.5.0/eikobot/core/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/eikobot/core/compiler/_parser.py` & `eikobot-0.5.0/eikobot/core/compiler/_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     EikoBaseType,
     EikoBool,
     EikoBoolType,
     EikoBuiltinFunction,
     EikoBuiltinTypes,
     EikoDict,
     EikoDictType,
+    EikoEnumDefinition,
+    EikoEnumValue,
     EikoFloat,
     EikoFloatType,
     EikoInt,
     EikoIntType,
     EikoList,
     EikoListType,
     EikoNoneType,
@@ -749,14 +751,36 @@
                         "The provided argument did not provide a valid value.",
                         token=arg_expr.token,
                     )
                 args.append(PassedArg(arg_expr.token, arg_value))
 
             return eiko_callable.execute(self.token, args)
 
+        if isinstance(eiko_callable, EikoEnumDefinition):
+            if len(self.args.elements) != 1:
+                raise EikoCompilationError(
+                    f"Enum '{eiko_callable.name}' takes exactly 1 argument.",
+                    token=self.token,
+                )
+
+            compiled_arg = self.args.elements[0].compile(context)
+            if compiled_arg is None:
+                raise EikoCompilationError(
+                    "Expected a value, but expression did not return one.",
+                    token=self.args.elements[0].token,
+                )
+
+            if not isinstance(compiled_arg, EikoStr):
+                raise EikoCompilationError(
+                    "Expected a value of type 'str'.",
+                    token=self.args.elements[0].token,
+                )
+
+            return eiko_callable.get(compiled_arg.value, self.args.elements[0].token)
+
         if eiko_callable in EikoBuiltinTypes:
             if len(self.args.elements) != 1:
                 raise EikoCompilationError(
                     f"{eiko_callable.type.name} takes exactly 1 argument.",
                     token=self.token,
                 )
 
@@ -1474,14 +1498,17 @@
                 raise EikoCompilationError(
                     f"Type '{key_type.name}' can not be used for dictionary indexes.",
                     token=self.sub_expressions[0].token,
                 )
 
             return EikoDictType(key_type, self.sub_expressions[1].compile(context))
 
+        if isinstance(primary_type, EikoEnumDefinition):
+            return primary_type.value_type
+
         raise EikoCompilationError(
             "Not a valid type expressions.",
             token=self.token,
         )
 
     @staticmethod
     def _is_valid_dict_key_type(_type: EikoType) -> bool:
@@ -1528,14 +1555,43 @@
 
         key_type = type_list_to_type(key_types)
         value_type = type_list_to_type(value_types)
 
         return EikoDict(key_type, value_type, elements)
 
 
+@dataclass
+class EnumValueExprAst(ExprAST):
+    """Represents a value tied to an enum class."""
+
+    def __post_init__(self) -> None:
+        super().__post_init__()
+        self.value = self.token.content.lower()
+
+    def compile(self, context: CompilerContext) -> Optional[StorableTypes]:
+        raise NotImplementedError(self.token)
+
+
+@dataclass
+class EnumExprAst(ExprAST):
+    """Represents an enum definition."""
+
+    values: list[EnumValueExprAst]
+
+    def compile(self, context: CompilerContext) -> EikoEnumDefinition:
+        value_type = EikoType(self.token.content)
+        values: dict[str, EikoEnumValue] = {}
+        for value in self.values:
+            values[value.value] = EikoEnumValue(value_type, value.value)
+
+        definition = EikoEnumDefinition(self.token.content, value_type, values)
+        context.set(definition.name, definition)
+        return definition
+
+
 class Parser:
     """
     Parses tokens 1 by 1, and turns them in to Expressions.
     """
 
     def __init__(self, file: Path) -> None:
         self.lexer = Lexer(file)
@@ -1612,16 +1668,16 @@
             and self._current.content == ""
             and self._next.type == TokenType.INDENT
         ):
             self._advance()
 
     def _parse_top_level(self) -> ExprAST:
         if not (
-            self._current.type in [TokenType.INDENT, TokenType.EOF]
-            or self._current.content == ""
+            (self._current.type == TokenType.INDENT and self._current.content == "")
+            or (self._current.type == TokenType.EOF and self._current.content == "EOF")
         ):
             raise EikoParserError(
                 f"Unexpected token: '{self._current.content}'.", token=self._current
             )
 
         self._advance(skip_indentation=True)
         if self._current.type == TokenType.EOF:
@@ -1701,14 +1757,17 @@
 
         if self._current.type == TokenType.LEFT_BRACE:
             return self._parse_dict()
 
         if self._current.type == TokenType.AT_SIGN:
             return self._parse_decorator([])
 
+        if self._current.type == TokenType.ENUM:
+            return self._parse_enum()
+
         raise EikoSyntaxError(
             f"Unexpected token {self._current.type.name}.", index=self._current.index
         )
 
     def _parse_unary_op(self) -> Union[UnaryNegExprAST, UnaryNotExprAST]:
         token = self._current
         self._advance()
@@ -2011,30 +2070,32 @@
     def _parse_constructor(self) -> ConstructorExprAST:
         def_token = self._current
         self._advance()
         identifier = self._parse_identifier()
 
         if self._current.type != TokenType.LEFT_PAREN:
             raise EikoSyntaxError("Expected a '('.", index=self._current.index)
-        self._advance()
+        self._advance(skip_indentation=True)
 
         self_arg = VariableExprAST(self._current)
         self._advance()
 
         args: list[ConstructorArgExprAST] = []
         while True:
             if self._current.type == TokenType.RIGHT_PAREN:
                 self._advance()
                 break
             if self._current.type != TokenType.COMMA:
                 raise EikoSyntaxError(
                     "Expected a ',' or a ')'.", index=self._current.index
                 )
-            self._advance()
+            self._advance(skip_indentation=True)
             args.append(self._parse_consructor_arg())
+            if self._current.type == TokenType.INDENT:
+                self._advance(skip_indentation=True)
 
         if self._current.type != TokenType.COLON:
             raise EikoSyntaxError("Expected a ':'.", index=self._current.index)
         self._advance()
 
         body = self._parse_body()
 
@@ -2310,7 +2371,60 @@
             self._advance(skip_indentation=True)
 
             if self._current.type == TokenType.RIGHT_BRACE:
                 self._advance()
                 break
 
         return DictExprAST(token, kv_pairs)
+
+    def _parse_enum(self) -> EnumExprAst:
+        if self._next.type != TokenType.IDENTIFIER:
+            raise EikoParserError(
+                f"Unexpected token {self._next.content}, "
+                "expected resource identifier.",
+                token=self._next,
+            )
+
+        identifier_token = self._next
+        self._advance()
+        self._advance()
+
+        if self._current.type != TokenType.COLON:
+            raise EikoParserError(
+                f"Unexpected token '{self._current.content}'.",
+                token=self._current,
+            )
+        self._advance()
+
+        if self._current.type != TokenType.INDENT:
+            raise EikoParserError(
+                f"Unexpected token '{self._current.content}'.",
+                token=self._previous,
+            )
+
+        if self._current.content == "":
+            raise EikoParserError("Expected indentation.", token=self._previous)
+
+        values: list[EnumValueExprAst] = []
+        indent = self._current.content
+        self._advance()
+        while True:
+            if self._current.type != TokenType.IDENTIFIER:
+                raise EikoParserError(
+                    f"Unexpected token '{self._current.content}', expected an enum value identifier.",
+                    token=self._current,
+                )
+
+            values.append(EnumValueExprAst(self._current))
+            self._advance()
+
+            while self._next.type == TokenType.INDENT:
+                self._advance()
+            if self._current.type != TokenType.INDENT:
+                raise EikoInternalError(
+                    "Unexpected issue, please report this on github."
+                )
+            if self._current.content != indent:
+                break
+            self._advance()
+
+        return EnumExprAst(identifier_token, values)
```

### Comparing `eikobot-0.4.0/eikobot/core/compiler/_token.py` & `eikobot-0.5.0/eikobot/core/compiler/_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     IF = auto()
     ELIF = auto()
     ELSE = auto()
     AND = auto()
     OR = auto()
     DEF = auto()
     PROMISE = auto()
+    ENUM = auto()
 
     IDENTIFIER = auto()
 
     LEFT_PAREN = auto()
     RIGHT_PAREN = auto()
     LEFT_SQ_BRACKET = auto()
     RIGHT_SQ_BRACKET = auto()
```

### Comparing `eikobot-0.4.0/eikobot/core/compiler/decorator.py` & `eikobot-0.5.0/eikobot/core/compiler/decorator.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/eikobot/core/compiler/definitions/_resource.py` & `eikobot-0.5.0/eikobot/core/compiler/definitions/_resource.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/eikobot/core/compiler/definitions/base_model.py` & `eikobot-0.5.0/eikobot/core/compiler/definitions/base_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Based on the pydantic BaseModel,
 the EikoBaseModel allows for linking of Eiko resources
 to a more easily useable python model.
 """
-from typing import TYPE_CHECKING, ClassVar
+from typing import TYPE_CHECKING, Any, ClassVar
 
 from pydantic import BaseModel
 
 from ...errors import EikoCompilationError
 from .base_types import EikoResource
 
 if TYPE_CHECKING:
@@ -19,14 +19,18 @@
     Used to handily convert eikoclasses to python classes and back.
     """
 
     raw_resource: EikoResource
     __eiko_resource__: ClassVar[str]
     __eiko_linked_definition__: ClassVar["EikoResourceDefinition"]
 
+    def __init__(self, **data: Any) -> None:
+        super().__init__(**data)
+        self.__post_init__()
+
     def __post_init__(self) -> None:
         pass
 
     class Config:
         arbitrary_types_allowed = True
 
     @classmethod
```

### Comparing `eikobot-0.4.0/eikobot/core/compiler/definitions/base_types.py` & `eikobot-0.5.0/eikobot/core/compiler/definitions/base_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,31 +5,38 @@
 """
 from dataclasses import dataclass
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    Generic,
     Iterator,
     Optional,
     Type,
+    TypeVar,
     Union,
 )
 
 from pydantic import BaseModel, ValidationError
 
-from ...errors import EikoCompilationError, EikoInternalError
+from ...errors import (
+    EikoCompilationError,
+    EikoError,
+    EikoInternalError,
+    EikoUnresolvedPromiseError,
+)
 from .._token import Token
 
 if TYPE_CHECKING:
+    from ...handlers import HandlerContext
     from ._resource import EikoResourceDefinition
     from .base_model import EikoBaseModel
     from .context import StorableTypes
     from .typedef import EikoTypeDef
-    from ...handlers import HandlerContext
 
 
 class EikoType:
     """
     The EikoType is used for typechecking.
     It is a property of every object and performs type checking functions.
     """
@@ -443,15 +450,18 @@
 
         raise ValueError
 
     def to_py(self) -> Path:
         return self.value
 
 
-class EikoPromise(EikoBaseType):
+T = TypeVar("T")
+
+
+class EikoPromise(EikoBaseType, Generic[T]):
     """
     A promise is a piece of information that
     Eikobot might not be able to retrieve at compile time.
     Instead, this information will be filled in at deploy time.
     """
 
     def __init__(
@@ -519,31 +529,137 @@
     def printable(self, _: str = "") -> str:
         return f"Promise[{self.type}]"
 
     def truthiness(self) -> bool:
         if self.value is None:
             raise EikoCompilationError(
                 "An unfulfilled Promise cannot be checked for truthiness, "
-                "as its value does not yet exist at compile time."
+                "as its value does not yet exist."
             )
 
         return self.value.truthiness()
 
     def type_check(self, expected_type: EikoType) -> bool:
         return expected_type.type_check(self.type)
 
     def index(self) -> str:
         return f"promise-{self.parent.index()}.{self.name}"
 
-    def to_py(self) -> "EikoPromise":
+    def to_py(self) -> "EikoPromise[T]":
         return self
 
+    def resolve(self, expect: Type[T]) -> T:
+        """
+        Gets the value of a promise if it exists.
+        Raises EikoError if the promise has no value.
+        The expect param allows for runtime type checking.
+        """
+        if self.value is None:
+            raise EikoUnresolvedPromiseError(
+                "Unresolved Promise was accessed.",
+                token=self.token,
+            )
+
+        value = self.value.to_py()
+        if isinstance(value, EikoPromise):
+            value = value.resolve(expect)
+
+        if not isinstance(value, expect):
+            raise EikoError(
+                f"Promise value is of type '{type(value)}', but user expected type '{expect}'."
+            )
+
+        return value
+
+
+EikoEnumDefinitionType = EikoType("EnumDefinition")
+
+
+class EikoEnumValue(EikoBaseType):
+    """Represents values and instances of enum values"""
+
+    def __init__(self, eiko_type: EikoType, value: str) -> None:
+        super().__init__(eiko_type)
+        self.value = value
+
+    def index(self) -> str:
+        return f"{self.type}-{self.value}"
+
+    def printable(self, _: str = "") -> str:
+        return f"{self.type.name} '{self.value}'"
 
-BuiltinTypes = Union[EikoBool, EikoFloat, EikoInt, EikoStr, EikoPath, EikoNone]
-EikoBuiltinTypes = (EikoBool, EikoFloat, EikoInt, EikoStr, EikoPath, EikoNone)
+    def get_value(self) -> str:
+        return self.value
+
+    def truthiness(self) -> bool:
+        return True
+
+    def to_py(self) -> str:
+        return self.value
+
+
+class EikoEnumDefinition(EikoBaseType):
+    """Internal representation of a resource definition."""
+
+    def __init__(
+        self, name: str, value_type: EikoType, values: dict[str, EikoEnumValue]
+    ) -> None:
+        super().__init__(EikoEnumDefinitionType)
+        self.name = name
+        self.value_type = value_type
+        self.values = values
+
+    def get(self, name: str, token: Optional[Token] = None) -> EikoEnumValue:
+        value = self.values.get(name)
+        if value is None:
+            raise EikoCompilationError(
+                f"Enum '{self.name}' has no value '{name}'.",
+                token=token,
+            )
+
+        return value
+
+    def printable(self, indent: str = "") -> str:
+        string = f"ENUM '{self.name}':" + " {\n"
+        n_indent = indent + "    "
+        for value in self.values.values():
+            string += n_indent + value.printable(n_indent) + ",\n"
+        string += indent + "}\n"
+
+        return string
+
+    @classmethod
+    def convert(cls, _: "BuiltinTypes") -> "EikoBaseType":
+        raise ValueError
+
+    def get_value(self) -> PyTypes:
+        raise NotImplementedError
+
+    def truthiness(self) -> bool:
+        raise NotImplementedError
+
+    def index(self) -> str:
+        raise NotImplementedError
+
+    def to_py(self) -> Union[PyTypes, "EikoPromise"]:
+        raise NotImplementedError
+
+
+BuiltinTypes = Union[
+    EikoBool, EikoFloat, EikoInt, EikoStr, EikoPath, EikoNone, EikoEnumValue
+]
+EikoBuiltinTypes = (
+    EikoBool,
+    EikoFloat,
+    EikoInt,
+    EikoStr,
+    EikoPath,
+    EikoNone,
+    EikoEnumValue,
+)
 
 
 class EikoResource(EikoBaseType):
     """Represents a custom resource in the Eiko language."""
 
     def __init__(
         self,
@@ -596,22 +712,33 @@
                 f"cannot be assigned a value of type '{value.type}'.",
                 token=token,
             )
 
         prop = self.properties.get(name)
         if isinstance(prop, EikoUnset):
             if not value.type_check(prop.type):
-                raise EikoCompilationError(
-                    f"Type error: Tried to assign value of type '{value.type}' "
-                    f"to a property of type '{prop.type}'.",
-                    token=token,
-                )
+                if prop.type.inverse_type_check(value.type):
+                    if prop.type.typedef is not None:
+                        value = prop.type.typedef.execute(value, token)
+                    else:
+                        raise EikoInternalError(
+                            "Ran in to a typedef that does not have a constructor. "
+                            "This is most likely a bug. PLease report this on Github.",
+                            token=token,
+                        )
+                else:
+                    raise EikoCompilationError(
+                        f"Type error: Tried to assign value of type '{value.type}' "
+                        f"to a property of type '{prop.type}'.",
+                        token=token,
+                    )
 
         elif isinstance(prop, EikoPromise):
             prop.assign(value, token)
+            return
 
         elif prop is not None:
             raise EikoCompilationError(
                 "Attempted to reassign a property that was already assigned.",
                 token=token,
             )
 
@@ -640,24 +767,42 @@
 
     def index(self) -> str:
         return self._index
 
     def to_py(self) -> Union[BaseModel, dict]:
         if self._py_object is not None:
             return self._py_object
+
         new_dict: dict[str, Union[PyTypes, EikoPromise]] = {}
+        pydantic_nested: dict[str, BaseModel] = {}
         for name, value in self.properties.items():
-            new_dict[name] = value.to_py()
+            if name in ["__depends_on__"]:
+                continue
+            new_value = value.to_py()
+            if isinstance(new_value, EikoPromise):
+                if new_value.name not in self.promises:
+                    new_value = new_value.resolve(object)
+
+            # Ok follow me on this:
+            # Pydantic calls __dict__ when validating nested models
+            # thereby returning new instances of objects that should not be recreated.
+            # This can cause bugs as we rely on the objects staying the same.
+            # So we keep track of all of the nested and attributes and
+            # monkey patch them back in
+            if isinstance(new_value, BaseModel) and isinstance(value, EikoResource):
+                pydantic_nested[name] = new_value
+            new_dict[name] = new_value
 
         if self.class_ref.linked_basemodel is not None:
             try:
                 self._py_object = self.class_ref.linked_basemodel(
                     raw_resource=self, **new_dict
                 )
-                self._py_object.__post_init__()
+                for name, pydantic_object in pydantic_nested.items():
+                    object.__setattr__(self._py_object, name, pydantic_object)
                 return self._py_object
             except ValidationError as e:
                 raise EikoCompilationError(
                     f"Failed to convert resource of type '{self.class_ref.name}' to "
                     "its linked basemodel.\n"
                     f"Reason: {e}"
                 ) from e
@@ -670,14 +815,15 @@
     EikoFloat,
     EikoInt,
     EikoNone,
     EikoStr,
     EikoPath,
     EikoPromise,
     EikoResource,
+    EikoEnumValue,
 )
 _builtin_function_type = EikoType("builtin_function", EikoObjectType)
 
 
 @dataclass
 class PassedArg:
     """A passed arg is a compiled expression passed as an arg."""
```

### Comparing `eikobot-0.4.0/eikobot/core/compiler/definitions/context.py` & `eikobot-0.5.0/eikobot/core/compiler/definitions/context.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/eikobot/core/compiler/definitions/function.py` & `eikobot-0.5.0/eikobot/core/compiler/definitions/function.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """
 While real functions don't exist in the eiko language,
 constructors and plugins do, and they need some kind of representation.
 """
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Optional, Type, Union
 
-from ...errors import EikoCompilationError, EikoPluginError
+from ...errors import EikoCompilationError, EikoInternalError, EikoPluginError
 from ...plugin import EikoPluginException, EikoPluginTyping
 from .._token import Token
 from .base_types import (
     INDEXABLE_TYPES,
     EikoBaseType,
     EikoProtectedStr,
     EikoResource,
     EikoType,
     EikoUnset,
     PassedArg,
     PyTypes,
     to_eiko,
     to_eiko_type,
 )
-from .typedef import EikoTypeDef
 
 if TYPE_CHECKING:
     from .._parser import ExprAST
     from ._resource import EikoResourceDefinition
     from .context import CompilerContext, StorableTypes
 
 EikoFunctionType = EikoType("function")
@@ -84,17 +83,15 @@
                 token=callee_token,
             )
 
         handled_args: dict[str, EikoBaseType] = {}
         self_arg = list(self.args.values())[0]
         resource = EikoResource(self.parent)
         handled_args[self_arg.name] = resource
-        self._handle_args(
-            handled_args, positional_args, keyword_args, self.execution_context
-        )
+        self._handle_args(handled_args, positional_args, keyword_args)
 
         for arg_name, arg in self.args.items():
             if arg_name not in handled_args:
                 if arg.default_value is None:
                     raise EikoCompilationError(
                         f"Argument '{arg_name}' for callable '{callee_token.content}' requires a value.",
                         token=callee_token,
@@ -165,36 +162,32 @@
                 token=callee_token,
             )
 
         context.global_id_list.append(resource.index())
 
         return resource
 
-    def _handle_args(
+    def _handle_args(  # pylint: disable=too-many-branches
         self,
         handled_args: dict[str, EikoBaseType],
         positional_args: list[PassedArg],
         keyword_args: dict[str, PassedArg],
-        context: "CompilerContext",
     ) -> None:
         for passed_arg, arg in zip(positional_args, list(self.args.values())[1:]):
             if not passed_arg.value.type_check(arg.type):
                 # Try to coerce the type
                 if arg.type.inverse_type_check(passed_arg.value.type):
-                    type_constr = context.get(arg.type.name)
-                    if isinstance(type_constr, EikoTypeDef):
-                        passed_arg.value = type_constr.execute(
-                            passed_arg.value, passed_arg.token
-                        )
-                    else:
-                        raise EikoCompilationError(
-                            f"Argument '{arg.name}' expected value of type '{arg.type}', "
-                            f"but got value of type '{passed_arg.value.type}'.",
+                    if arg.type.typedef is None:
+                        raise EikoInternalError(
+                            "Failed to coerce type.",
                             token=passed_arg.token,
                         )
+                    passed_arg.value = arg.type.typedef.execute(
+                        passed_arg.value, passed_arg.token
+                    )
                 else:
                     raise EikoCompilationError(
                         f"Argument '{arg.name}' expected value of type '{arg.type}', "
                         f"but got value of type '{passed_arg.value.type}'.",
                         token=passed_arg.token,
                     )
 
@@ -211,19 +204,32 @@
             if kw_arg is None:
                 raise EikoCompilationError(
                     f"'{self.parent.name}.{self.name}()' has no argument '{arg_name}'.",
                     token=passed_arg.token,
                 )
 
             if not passed_arg.value.type_check(kw_arg.type):
-                raise EikoCompilationError(
-                    f"Argument '{kw_arg.name}' expected value of type '{kw_arg.type}', "
-                    f"but got value of type '{passed_arg.value.type}'.",
-                    token=passed_arg.token,
-                )
+                if kw_arg.type.inverse_type_check(passed_arg.value.type):
+                    if kw_arg.type.typedef is not None:
+                        passed_arg.value = kw_arg.type.typedef.execute(
+                            passed_arg.value,
+                            passed_arg.token,
+                        )
+                    else:
+                        raise EikoInternalError(
+                            "Ran in to a typedef that does not have a constructor. "
+                            "This is most likely a bug. PLease report this on Github.",
+                            token=passed_arg.token,
+                        )
+                else:
+                    raise EikoCompilationError(
+                        f"Argument '{kw_arg.name}' expected value of type '{kw_arg.type}', "
+                        f"but got value of type '{passed_arg.value.type}'.",
+                        token=passed_arg.token,
+                    )
 
             handled_args[arg_name] = passed_arg.value
 
     def truthiness(self) -> bool:
         raise NotImplementedError
```

### Comparing `eikobot-0.4.0/eikobot/core/compiler/definitions/typedef.py` & `eikobot-0.5.0/eikobot/core/compiler/definitions/typedef.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/eikobot/core/compiler/importlib.py` & `eikobot-0.5.0/eikobot/core/compiler/importlib.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/eikobot/core/compiler/lexer.py` & `eikobot-0.5.0/eikobot/core/compiler/lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "elif": TokenType.ELIF,
     "else": TokenType.ELSE,
     "from": TokenType.FROM,
     "and": TokenType.AND,
     "or": TokenType.OR,
     "def": TokenType.DEF,
     "promise": TokenType.PROMISE,
+    "enum": TokenType.ENUM,
 }
 
 SPECIAL_CHARS = {
     "(": TokenType.LEFT_PAREN,
     ")": TokenType.RIGHT_PAREN,
     "[": TokenType.LEFT_SQ_BRACKET,
     "]": TokenType.RIGHT_SQ_BRACKET,
```

### Comparing `eikobot-0.4.0/eikobot/core/compiler/ops.py` & `eikobot-0.5.0/eikobot/core/compiler/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 allowing the addition, multiplication, division, etc...
 of Eikobot builtin types.
 """
 from enum import Enum, auto
 from pathlib import Path
 from typing import Callable, Union
 
-from ..errors import EikoCompilationError, EikoInternalError
+from ..errors import EikoCompilationError, EikoInternalError, EikoSyntaxError
 from .definitions.base_types import (
     EikoBaseType,
     EikoBool,
     EikoFloat,
     EikoInt,
     EikoNumber,
     EikoPath,
@@ -49,18 +49,17 @@
 
         if op == "//":
             return BinOP.INT_DIVIDE
 
         if op == "**":
             return BinOP.EXPONENTIATION
 
-        raise EikoInternalError(
-            "Issue occured trying to parse binop. "
-            "This is deffinetly a bug, please report it on github.",
-            token=token,
+        raise EikoSyntaxError(
+            "Issue occured trying to parse binop.",
+            index=token.index,
         )
 
     def __str__(self) -> str:
         if self == BinOP.ADD:
             return "+"
         if self == BinOP.SUBTRACT:
             return "-"
@@ -206,18 +205,17 @@
 
         if token.content == ">=":
             return ComparisonOP.EQ_OR_GT
 
         if token.content == "<=":
             return ComparisonOP.EQ_OR_LT
 
-        raise EikoInternalError(
-            "Issue occured trying to parse binop. "
-            "This is deffinetly a bug, please report it on github.",
-            token=token,
+        raise EikoSyntaxError(
+            "Issue occured trying to parse binop.",
+            index=token.index,
         )
 
     def __str__(self) -> str:
         if self == ComparisonOP.LESS_THEN:
             return "<"
 
         if self == ComparisonOP.GREATHER_THEN:
```

### Comparing `eikobot-0.4.0/eikobot/core/deployer.py` & `eikobot-0.5.0/eikobot/core/deployer.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,15 +43,28 @@
         for task in exporter.base_tasks:
             task.init(self._done_cb, self._failure_cb)
             self._create_task(task)
 
         while self.asyncio_tasks:
             await asyncio.gather(*self.asyncio_tasks)
 
-        await self._clean_up()
+        logger.info("Cleaning up.")
+        for task in exporter.task_index.values():
+            if task.handler is not None:
+                await task.handler.cleanup(task.ctx)
+
+    async def dry_run(self, exporter: Exporter) -> None:
+        """Executes a dry run of all tasks."""
+        for task in exporter.base_tasks:
+            task.init()
+
+        for task in exporter.task_index.values():
+            if task.handler is not None:
+                task.ctx.resource = task.ctx.raw_resource.to_py()
+                await task.handler.__dry_run__(task.ctx)
 
     async def deploy_from_file(self, eiko_file: Path) -> None:
         """Helper funcion meant mostly for testing."""
         exporter = Exporter()
         exporter.export_from_file(eiko_file)
         await self.deploy(exporter)
 
@@ -72,13 +85,7 @@
     def _done_cb(self) -> None:
         self.progress.done += 1
         if self.progress.log:
             logger.info(f"{self.progress.done} of {self.progress.total} tasks done.")
 
     def _failure_cb(self) -> None:
         self.failed = True
-
-    async def _clean_up(self) -> None:
-        # Bit of a hack.
-        # We timeout ssh connections after 1 second of idle time
-        # so this gives them time to close automatically.
-        await asyncio.sleep(1)
```

### Comparing `eikobot-0.4.0/eikobot/core/errors.py` & `eikobot-0.5.0/eikobot/core/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,18 @@
         self, reason: str, *args: object, token: Optional[Token] = None
     ) -> None:
         super().__init__(reason, *args)
         self.token = token
         self.index = None if token is None else token.index
 
 
+class EikoUnresolvedPromiseError(EikoError):
+    """A promise that wasn't resolved by the time it was accessed"""
+
+
 class EikoInternalError(EikoError):
     """
     Something went wrong inside the compiler,
     most likely caused by a bug and not the user.
     """
 
     def __init__(
@@ -87,7 +91,19 @@
     most likely caused by a bug and not the user.
     """
 
     def __init__(
         self, reason: str, *args: object, token: Optional[Token] = None
     ) -> None:
         super().__init__("ExportError: " + reason, *args, token=token)
+
+
+class EikoDeployError(EikoError):
+    """
+    Something went wrong inside the compiler,
+    most likely caused by a bug and not the user.
+    """
+
+    def __init__(
+        self, reason: str, *args: object, token: Optional[Token] = None
+    ) -> None:
+        super().__init__("DeployError: " + reason, *args, token=token)
```

### Comparing `eikobot-0.4.0/eikobot/core/exporter.py` & `eikobot-0.5.0/eikobot/core/exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Callable, Optional, Union
 
 from . import logger
 from .compiler import Compiler, CompilerContext
-from .errors import EikoExportError, EikoInternalError
+from .errors import EikoDeployError, EikoExportError, EikoInternalError
 from .handlers import Handler, HandlerContext
 from .helpers import EikoDict, EikoList, EikoResource
 
 
 @dataclass
 class Task:
     """A task is a piece of work the backend needs to do."""
@@ -38,68 +38,71 @@
         self._failure_cb = failure_cb
         self.depends_on_copy = self.depends_on.copy()
         for dependant in self.dependants:
             dependant.init(done_cb, failure_cb)
 
     async def execute(self) -> None:
         """Executes the task, than let's it's dependants know it's done."""
-        logger.info(f"starting task '{self.task_id}'")
-        self._resolve_promises()
-        if self.handler is not None:
-            await self.handler.execute(self.ctx)
-            await self.handler.resolve_promises(self.ctx)
-        else:
-            raise EikoInternalError(
-                "Deployer failed to execute a task because a handler was missing. "
-            )
+        logger.info(f"Starting task '{self.task_id}'")
+        self.ctx.resource = self.ctx.raw_resource.to_py()
+        await self._run_handler()
+
+        if self.ctx.failed or not self.ctx.deployed:
+            logger.error(f"Failed task '{self.task_id}'")
+            if self._failure_cb is not None:
+                self._failure_cb()
+            return
 
         for name, promise in self.ctx.raw_resource.promises.items():
             if promise.value is None:
                 logger.error(
                     f"Resource '{self.task_id}' was deployed, "
                     f"but promise '{name}' was not fullfilled."
                 )
                 if self._failure_cb is not None:
                     self._failure_cb()
                 return
 
-            self.ctx.raw_resource.properties[name] = promise.value
-
-        self.ctx.resource = self.ctx.raw_resource.to_py()
-
-        if self.ctx.failed or not self.ctx.deployed:
-            logger.error(f"Failed task '{self.task_id}'")
-            if self._failure_cb is not None:
-                self._failure_cb()
-            return
-
         logger.debug(f"Done executing task '{self.task_id}'")
         for sub_task in self.dependants:
             sub_task.remove_dep(self)
 
         if self._done_cb is not None:
             self._done_cb()
 
-    def _resolve_promises(self) -> None:
-        """Resolves external promises."""
-        for name, promise in self.ctx.raw_resource.get_external_promises():
-            logger.debug(
-                f"Task '{self.task_id}' is resolving extenral promise "
-                f"'{promise.parent.index()}.{promise.name}'."
-            )
-            if promise.value is None:
-                raise EikoInternalError(
-                    "An external promise was not resolved. "
-                    "This should have been caught earlier.",
-                    token=promise.token,
-                )
-
-            self.ctx.raw_resource.properties[name] = promise.value
+    async def _run_handler(self) -> None:
+        if self.handler is not None:
+            try:
+                await self.handler.__pre__(self.ctx)
+                if self.ctx.failed:
+                    raise EikoDeployError("Pre deploy failed.")
+
+                await self.handler.execute(self.ctx)
+                if self.ctx.failed or not self.ctx.deployed:
+                    raise EikoDeployError("Handler execution failed.")
+
+                await self.handler.resolve_promises(self.ctx)
+                if self.ctx.failed:
+                    raise EikoDeployError("Resolving promises failed.")
+
+            except Exception as e:  # pylint: disable=broad-exception-caught
+                self.ctx.failed = True
+                logger.error(f"Failed to deploy '{self.task_id}': {e}")
+
+            try:
+                await self.handler.__post__(self.ctx)
+            except Exception as e:
+                raise EikoDeployError(
+                    f"Failed to cleanup for task '{self.task_id}': {e}",
+                ) from e
 
-        self.ctx.resource = self.ctx.raw_resource.to_py()
+        else:
+            raise EikoInternalError(
+                "Deployer failed to execute a task because a handler was missing. "
+            )
 
     def remove_dep(self, task: "Task") -> None:
         self.depends_on_copy.remove(task)
 
     def process_sub_task(self, sub_task: "Task") -> None:
         """
         Adds a task as a dependancy for this task.
```

### Comparing `eikobot-0.4.0/eikobot/core/handlers.py` & `eikobot-0.5.0/eikobot/core/handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from dataclasses import dataclass
 from typing import Any, Union
 
 from . import logger
 from .compiler.definitions.base_model import BaseModel
 from .compiler.definitions.base_types import EikoResource
+from .errors import EikoUnresolvedPromiseError
 
 
 @dataclass
 class HandlerContext:
     """A HandlerContext keeps track of things required for a deployment."""
 
     raw_resource: EikoResource
@@ -41,20 +42,32 @@
 
 
 class Handler:
     """A handler implements methods for a resource to be managed."""
 
     __eiko_resource__: str
 
+    async def __pre__(self, ctx: HandlerContext) -> None:
+        pass
+
     async def execute(self, ctx: HandlerContext) -> None:
         raise NotImplementedError
 
     async def resolve_promises(self, ctx: HandlerContext) -> None:
         pass
 
+    async def __post__(self, ctx: HandlerContext) -> None:
+        pass
+
+    async def cleanup(self, ctx: HandlerContext) -> None:
+        pass
+
+    async def __dry_run__(self, ctx: HandlerContext) -> None:
+        ctx.info(f"Task '{ctx.name}' would execute.")
+
 
 class EikoCRUDHanlderMethodNotImplemented(Exception):
     """Raised if a method is not implemented."""
 
 
 class CRUDHandler(Handler):
     """
@@ -105,7 +118,29 @@
         raise EikoCRUDHanlderMethodNotImplemented
 
     async def update(self, ctx: HandlerContext) -> None:
         raise EikoCRUDHanlderMethodNotImplemented
 
     async def delete(self, ctx: HandlerContext) -> None:
         raise EikoCRUDHanlderMethodNotImplemented
+
+    async def __dry_run__(self, ctx: HandlerContext) -> None:
+        try:
+            logger.debug(f"Reading resource '{ctx.raw_resource.index()}'.")
+            await self.read(ctx)
+        except EikoCRUDHanlderMethodNotImplemented:
+            logger.info(f"Resource '{ctx.name}' would be created.")
+        except EikoUnresolvedPromiseError:
+            logger.info(
+                f"Resource '{ctx.name}' relies on promises that are unresolved and thus its state is unknown."
+            )
+            return
+
+        if ctx.deployed:
+            if not ctx.changes:
+                logger.info(f"Resource '{ctx.name}' is in its desired state.")
+            else:
+                logger.info(
+                    f"Resource '{ctx.name}' would be updated. (changes: {ctx.changes})"
+                )
+        else:
+            logger.info(f"Resource '{ctx.name}' would be created.")
```

### Comparing `eikobot-0.4.0/eikobot/core/lib/std/env.py` & `eikobot-0.5.0/eikobot/core/lib/std/env.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/eikobot/core/lib/std/file.py` & `eikobot-0.5.0/eikobot/core/lib/std/file.py`

 * *Files 16% similar despite different names*

```diff
@@ -104,52 +104,52 @@
 
     async def create(self, ctx: HandlerContext) -> None:
         if not isinstance(ctx.resource, FileModel):
             ctx.failed = True
             return
 
         if ctx.resource.requires_sudo:
-            ssh_exec = ctx.resource.host.execute_sudo
             sudo = "sudo "
         else:
-            ssh_exec = ctx.resource.host.execute
             sudo = ""
 
-        result = await ssh_exec(f"{sudo}mkdir -p {ctx.resource.path.parent}", ctx)
+        result = await ctx.resource.host.execute(
+            f"{sudo}mkdir -p {ctx.resource.path.parent}", ctx
+        )
         if result.returncode != 0:
             ctx.failed = True
             return
 
-        result = await ssh_exec(
+        result = await ctx.resource.host.execute(
             f'echo -n "{ctx.resource.content}" | {sudo}tee {ctx.resource.path}',
             ctx,
         )
         if result.returncode != 0:
             ctx.failed = True
             return
 
-        result = await ssh_exec(
+        result = await ctx.resource.host.execute(
             f"{sudo}chmod {ctx.resource.mode} " f"{ctx.resource.path}",
             ctx,
         )
         if result.returncode != 0:
             ctx.failed = True
             return
 
         if ctx.resource.owner is not None:
-            result = await ssh_exec(
+            result = await ctx.resource.host.execute(
                 f"{sudo}chown {ctx.resource.owner} {ctx.resource.path}",
                 ctx,
             )
             if result.returncode != 0:
                 ctx.failed = True
                 return
 
         if ctx.resource.group is not None:
-            result = await ssh_exec(
+            result = await ctx.resource.host.execute(
                 f"{sudo}chgrp {ctx.resource.group} {ctx.resource.path}",
                 ctx,
             )
             if result.returncode != 0:
                 ctx.failed = True
                 return
 
@@ -157,30 +157,32 @@
 
     async def read(self, ctx: HandlerContext) -> None:
         if not isinstance(ctx.resource, FileModel):
             ctx.failed = True
             return
 
         if ctx.resource.requires_sudo:
-            ssh_exec = ctx.resource.host.execute_sudo
             sudo = "sudo "
         else:
-            ssh_exec = ctx.resource.host.execute
             sudo = ""
 
-        cat_result = await ssh_exec(f"{sudo}cat {ctx.resource.path}", ctx)
+        cat_result = await ctx.resource.host.execute(
+            f"{sudo}cat {ctx.resource.path}", ctx
+        )
         if cat_result.returncode == 0:
             ctx.deployed = True
-            if cat_result.stdout != ctx.resource.content:
-                ctx.add_change("content", cat_result.stdout)
+            if cat_result.output != ctx.resource.content:
+                ctx.add_change("content", cat_result.output)
 
-            ls_result = await ssh_exec(f"{sudo}ls -l {ctx.resource.path}", ctx)
+            ls_result = await ctx.resource.host.execute(
+                f"{sudo}ls -l {ctx.resource.path}", ctx
+            )
             if ls_result.returncode == 0:
-                if isinstance(ls_result.stdout, str):
-                    ls_parsed = ls_result.stdout.split(" ")
+                if isinstance(ls_result.output, str):
+                    ls_parsed = ls_result.output.split(" ")
                     if parse_rwx_mode(ls_parsed[0]) != ctx.resource.mode:
                         ctx.add_change("mode", parse_rwx_mode(ls_parsed[0]))
                     if (
                         ctx.resource.owner is not None
                         and ls_parsed[2] != ctx.resource.owner
                     ):
                         ctx.add_change("owner", ls_parsed[2])
@@ -194,50 +196,44 @@
 
     async def update(self, ctx: HandlerContext) -> None:
         if not isinstance(ctx.resource, FileModel):
             ctx.failed = True
             return
 
         if ctx.resource.requires_sudo:
-            ssh_exec = ctx.resource.host.execute_sudo
             sudo = "sudo "
         else:
-            ssh_exec = ctx.resource.host.execute
             sudo = ""
 
         if ctx.changes.get("content") is not None:
-            result = await ssh_exec(
+            result = await ctx.resource.host.execute(
                 f'echo -n "{ctx.resource.content}" | {sudo}tee {ctx.resource.path}',
                 ctx,
             )
-            if result.returncode != 0:
-                ctx.failed = True
+            if result.failed():
                 return
 
         if ctx.changes.get("mode") is not None:
-            result = await ssh_exec(
+            result = await ctx.resource.host.execute(
                 f"{sudo}chmod {ctx.resource.mode} " f"{ctx.resource.path}",
                 ctx,
             )
-            if result.returncode != 0:
-                ctx.failed = True
+            if result.failed():
                 return
 
         if ctx.changes.get("owner") is not None:
-            result = await ssh_exec(
+            result = await ctx.resource.host.execute(
                 f"{sudo}chown {ctx.resource.owner} {ctx.resource.path}",
                 ctx,
             )
-            if result.returncode != 0:
-                ctx.failed = True
+            if result.failed():
                 return
 
         if ctx.changes.get("group") is not None:
-            result = await ssh_exec(
+            result = await ctx.resource.host.execute(
                 f"{sudo}chgrp {ctx.resource.group} {ctx.resource.path}",
                 ctx,
             )
-            if result.returncode != 0:
-                ctx.failed = True
+            if result.failed():
                 return
 
         ctx.deployed = True
```

### Comparing `eikobot-0.4.0/eikobot/core/lib/std/test.py` & `eikobot-0.5.0/eikobot/core/lib/std/test.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 @eiko_plugin()
 def test_raise_exception() -> None:
     raise EikoPluginException("This plugins shows that Plugin exceptions work.")
 
 
 @eiko_plugin()
 def test_python_exception() -> None:
-    raise Exception("A python exception to test the plugin exception handling.")
+    raise ValueError("A python exception to test the plugin exception handling.")
```

### Comparing `eikobot-0.4.0/eikobot/core/logger.py` & `eikobot-0.5.0/eikobot/core/logger.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/eikobot/core/plugin.py` & `eikobot-0.5.0/eikobot/core/plugin.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/eikobot.egg-info/PKG-INFO` & `eikobot-0.5.0/eikobot.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: eikobot
-Version: 0.4.0
+Version: 0.5.0
 Summary: The eikobot desired state engine.
 Author: kazaamjt
 Author-email: kazaamjt@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Utilities
+Classifier: Intended Audience :: System Administrators
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Eikobot Desired State Engine
 
 *The little Desired State Engine that made it so.*  
 
@@ -30,24 +35,23 @@
 
 Some of it's notable features are:  
 
 - Object oriented
 - sees the infrastructure as a tree of resources, rather than a flatland
 - completely stateless*
 
-The quickest way to get started is probably by doing some of the [quickstarts](https://github.com/kazaamjt/Eikobot/blob/main/docs/quickstart.md).  
+The quickest way to get started is probably by doing some of the [quickstarts](https://github.com/kazaamjt/Eikobot/blob/main/docs/quickstarts.md).  
 For a more complete idea of how the language works,
 please see the [language overview](https://github.com/kazaamjt/Eikobot/blob/main/docs/language_overview.md).  
 
 (*If the model/modules are designed well.)  
 
 ## Installation
 
-Eikobot requires python 3.10 or up and has 3 external dependencies that can be installed using pip.  
-In fact, Eikobot can be installed using pip as well.  
+Eikobot requires python 3.10 or up and can be installed using pip.  
 
 Here is an example of how to install Eikobot:  
 (This should work on most platforms, although the python command is different if you are on windows)
 
 ```bash
 python3.10 -m venv eikobot-venv
 eikobot-venv/bin/pip install eikobot
```

### Comparing `eikobot-0.4.0/eikobot.egg-info/SOURCES.txt` & `eikobot-0.5.0/eikobot.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 eikobot/__init__.py
 eikobot/__main__.py
+eikobot/py.typed
 eikobot.egg-info/PKG-INFO
 eikobot.egg-info/SOURCES.txt
 eikobot.egg-info/dependency_links.txt
 eikobot.egg-info/entry_points.txt
 eikobot.egg-info/requires.txt
 eikobot.egg-info/top_level.txt
 eikobot/core/__init__.py
@@ -30,26 +31,32 @@
 eikobot/core/compiler/definitions/_resource.py
 eikobot/core/compiler/definitions/base_model.py
 eikobot/core/compiler/definitions/base_types.py
 eikobot/core/compiler/definitions/context.py
 eikobot/core/compiler/definitions/function.py
 eikobot/core/compiler/definitions/typedef.py
 eikobot/core/lib/__init__.py
+eikobot/core/lib/docker/__init__.eiko
+eikobot/core/lib/docker/__init__.py
 eikobot/core/lib/std/__init__.eiko
 eikobot/core/lib/std/__init__.py
 eikobot/core/lib/std/env.eiko
 eikobot/core/lib/std/env.py
 eikobot/core/lib/std/file.eiko
 eikobot/core/lib/std/file.py
 eikobot/core/lib/std/regex.eiko
 eikobot/core/lib/std/regex.py
 eikobot/core/lib/std/test.eiko
 eikobot/core/lib/std/test.py
+eikobot/core/package_manager/__init__.py
+eikobot/core/package_manager/lib/eikobot-docker-0.0.2/docker/__init__.eiko
+eikobot/core/package_manager/lib/eikobot-docker-0.0.2/docker/__init__.py
 tests/test_compilation.py
 tests/test_datatypes.py
 tests/test_decorator.py
 tests/test_deployer.py
 tests/test_exporter.py
 tests/test_import.py
 tests/test_lexer.py
+tests/test_package.py
 tests/test_parser.py
 tests/test_promises.py
```

### Comparing `eikobot-0.4.0/setup.cfg` & `eikobot-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [isort]
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
 
 [mypy]
-python_version = 3.10
+python_version = 3.11
 plugins = pydantic.mypy
 warn_unused_configs = True
 disallow_subclassing_any = True
 disallow_untyped_calls = True
 disallow_untyped_defs = True
 disallow_incomplete_defs = True
 check_untyped_defs = True
@@ -193,14 +193,14 @@
 	_replace,
 	_source,
 	_make
 valid-classmethod-first-arg = cls
 valid-metaclass-classmethod-first-arg = cls
 
 [pylint.exceptions]
-overgeneral-exceptions = BaseException,
-	Exception
+overgeneral-exceptions = builtins.BaseException,
+	builtins.Exception
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `eikobot-0.4.0/setup.py` & `eikobot-0.5.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 
 import setuptools
 
 this_directory = Path(__file__).parent
 with open(this_directory / "README.md", encoding="utf-8") as f:
     long_description = f.read()
 
-VERSION = "0.4.0"
+VERSION = "0.5.0"
 REQUIRES = [
+    "aiohttp==3.8.4",
     "asyncssh==2.13.1",
     "click==8.1.3",
     "colorama==0.4.6",
     "jinja2==3.1.2",
+    "packaging==23.1",
     "pydantic==1.10.4",
 ]
 
 setuptools.setup(
     name="eikobot",
     version=VERSION,
     description="The eikobot desired state engine.",
@@ -28,15 +30,20 @@
     author="kazaamjt",
     author_email="kazaamjt@gmail.com",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
+        "Topic :: System :: Systems Administration",
+        "Topic :: Utilities",
+        "Intended Audience :: System Administrators",
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
     ],
     packages=setuptools.find_packages(),
-    package_data={"": ["**/*.eiko", "**/*.py", "requirements.xt"]},
+    package_data={"": ["**/*.eiko", "**/*.py", "py.typed"]},
     include_package_data=True,
-    python_requires=">=3.10",
+    python_requires=">=3.11",
     install_requires=REQUIRES,
     entry_points={"console_scripts": ["eikobot=eikobot.__main__:cli"]},
 )
```

### Comparing `eikobot-0.4.0/tests/test_compilation.py` & `eikobot-0.5.0/tests/test_compilation.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import pytest
 
 from eikobot.core.compiler import Compiler
 from eikobot.core.compiler._parser import Parser
 from eikobot.core.compiler.definitions._resource import EikoResourceDefinition
 from eikobot.core.compiler.definitions.base_types import (
+    EikoEnumValue,
     EikoInt,
     EikoNone,
     EikoResource,
     EikoStr,
 )
 from eikobot.core.compiler.definitions.context import CompilerContext
 from eikobot.core.compiler.definitions.typedef import EikoTypeDef
@@ -185,92 +186,107 @@
     compiler = Compiler()
     compiler.compile(eiko_inheritance_file)
 
     var_a = compiler.context.get("a")
     assert isinstance(var_a, EikoResource)
     assert var_a.type.name == "BaseRes"
     assert var_a.to_py() == {
-        "__depends_on__": [],
         "prop_1": "a",
         "prop_2": 1,
     }
 
     var_b = compiler.context.get("b")
     assert isinstance(var_b, EikoResource)
     assert var_b.type.name == "SubRes"
     assert var_b.type.super is not None
     assert var_b.type.super.name == "BaseRes"
     assert var_b.to_py() == {
-        "__depends_on__": [],
         "prop_1": "a",
         "prop_2": 1,
         "prop_3": 1,
     }
 
     var_c = compiler.context.get("c")
     assert isinstance(var_c, EikoResource)
     assert var_c.type.name == "SubSubRes"
     assert var_c.type.super is not None
     assert var_c.type.super.name == "SubRes"
     assert var_c.type.super.super is not None
     assert var_c.type.super.super.name == "BaseRes"
     assert var_c.to_py() == {
-        "__depends_on__": [],
         "prop_1": "a",
         "prop_2": 1,
         "prop_3": "a",
         "prop_4": 1,
     }
 
     var_d = compiler.context.get("d")
     assert isinstance(var_d, EikoResource)
     assert var_d.type.name == "SubResPropOverwite"
     assert var_d.type.super is not None
     assert var_d.type.super.name == "SubRes"
     assert var_d.type.super.super is not None
     assert var_d.type.super.super.name == "BaseRes"
     assert var_d.to_py() == {
-        "__depends_on__": [],
         "prop_1": "a",
         "prop_2": 1,
         "prop_3": "a",
     }
 
     var_e = compiler.context.get("e")
     assert isinstance(var_e, EikoResource)
     assert var_e.type.name == "Test"
     assert var_e.type.super is not None
     assert var_e.type.super.name == "Object"
     assert var_e.to_py() == {
-        "__depends_on__": [],
         "prop_1": var_a.to_py(),
     }
 
     var_f = compiler.context.get("f")
     assert isinstance(var_f, EikoResource)
     assert var_f.type.name == "Test"
     assert var_f.type.super is not None
     assert var_f.type.super.name == "Object"
     assert var_f.to_py() == {
-        "__depends_on__": [],
         "prop_1": var_b.to_py(),
     }
 
     var_g = compiler.context.get("g")
     assert isinstance(var_g, EikoResource)
     assert var_g.type.name == "Test"
     assert var_g.type.super is not None
     assert var_g.type.super.name == "Object"
     assert var_g.to_py() == {
-        "__depends_on__": [],
         "prop_1": var_c.to_py(),
     }
 
     var_h = compiler.context.get("h")
     assert isinstance(var_h, EikoResource)
     assert var_h.type.name == "Test"
     assert var_h.type.super is not None
     assert var_h.type.super.name == "Object"
     assert var_h.to_py() == {
-        "__depends_on__": [],
         "prop_1": var_d.to_py(),
     }
+
+
+def test_enum(eiko_enum_file: Path) -> None:
+    compiler = Compiler()
+    compiler.compile(eiko_enum_file)
+
+    var_test_1 = compiler.context.get("test_1")
+    assert isinstance(var_test_1, EikoResource)
+    assert var_test_1.type.name == "TestRes"
+    var_test_1_enum_opt_2 = var_test_1.properties.get("prop_1")
+    assert isinstance(var_test_1_enum_opt_2, EikoEnumValue)
+    assert var_test_1_enum_opt_2.value == "option_2"
+
+    var_test_2 = compiler.context.get("test_2")
+    assert isinstance(var_test_2, EikoResource)
+    assert var_test_2.type.name == "TestRes"
+    var_test_2_enum_opt_1 = var_test_2.properties.get("prop_1")
+    assert isinstance(var_test_2_enum_opt_1, EikoEnumValue)
+    assert var_test_2_enum_opt_1.value == "option_1"
+
+    var_enum_to_str = compiler.context.get("enum_to_str")
+    assert isinstance(var_enum_to_str, EikoStr)
+    assert var_enum_to_str.value == "option_3"
```

### Comparing `eikobot-0.4.0/tests/test_datatypes.py` & `eikobot-0.5.0/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/tests/test_decorator.py` & `eikobot-0.5.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/tests/test_deployer.py` & `eikobot-0.5.0/tests/test_deployer.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/tests/test_exporter.py` & `eikobot-0.5.0/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/tests/test_import.py` & `eikobot-0.5.0/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/tests/test_lexer.py` & `eikobot-0.5.0/tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.4.0/tests/test_parser.py` & `eikobot-0.5.0/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pytest
 
 from eikobot.core.compiler._parser import (
     AssignmentExprAST,
     BinOP,
     BinOpExprAST,
     CallExprAst,
+    EnumExprAst,
     FromImportExprAST,
     FStringExprAST,
     FStringLexer,
     IntExprAST,
     ListExprAST,
     Parser,
     ResourceDefinitionAST,
@@ -247,7 +248,18 @@
     assert expr_2.condition is None
 
     expr_3 = next(parse_iter)
     assert isinstance(expr_3, TypedefExprAST)
     assert expr_3.name == "IPv4Address"
     assert expr_3.super_type_expr.token.content == "str"
     assert isinstance(expr_3.condition, CallExprAst)
+
+
+def test_parse_enum(eiko_enum_file: Path) -> None:
+    parser = Parser(eiko_enum_file)
+    parse_iter = parser.parse()
+
+    expr_1 = next(parse_iter)
+    assert isinstance(expr_1, EnumExprAst)
+
+    expr_2 = next(parse_iter)
+    assert isinstance(expr_2, ResourceDefinitionAST)
```

