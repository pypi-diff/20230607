# Comparing `tmp/eikobot-0.5.0.tar.gz` & `tmp/eikobot-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eikobot-0.5.0.tar", last modified: Wed Jun  7 14:02:39 2023, max compression
+gzip compressed data, was "eikobot-0.5.1.tar", last modified: Wed Jun  7 15:29:15 2023, max compression
```

## Comparing `eikobot-0.5.0.tar` & `eikobot-0.5.1.tar`

### file list

```diff
@@ -1,77 +1,69 @@
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.167419 eikobot-0.5.0/
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1059 2023-06-05 11:53:10.000000 eikobot-0.5.0/LICENSE
--rw-r--r--   0 yaron     (1000) yaron     (1000)     3252 2023-06-07 14:02:39.167419 eikobot-0.5.0/PKG-INFO
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2644 2023-06-07 14:01:19.000000 eikobot-0.5.0/README.md
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/
--rw-r--r--   0 yaron     (1000) yaron     (1000)      159 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     6055 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/__main__.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/
--rw-r--r--   0 yaron     (1000) yaron     (1000)       39 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/__init__.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/compiler/
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1263 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    85130 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/_parser.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1666 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/_token.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2420 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/decorator.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/compiler/definitions/
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2786 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/_resource.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1593 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/base_model.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    35673 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/base_types.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    12465 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/context.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    12376 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/function.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2777 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/definitions/typedef.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     8553 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/importlib.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     9149 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/lexer.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      306 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/compiler/misc.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     8779 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/compiler/ops.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2828 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/deployer.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2893 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/errors.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     8016 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/exporter.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     4755 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/handlers.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      395 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/helpers.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/lib/
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/__init__.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/lib/docker/
--rw-r--r--   0 yaron     (1000) yaron     (1000)      974 2023-06-04 18:43:55.000000 eikobot-0.5.0/eikobot/core/lib/docker/__init__.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)     4771 2023-06-07 10:53:48.000000 eikobot-0.5.0/eikobot/core/lib/docker/__init__.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/lib/std/
--rw-r--r--   0 yaron     (1000) yaron     (1000)      819 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/lib/std/__init__.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)    14244 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/lib/std/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/std/env.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1486 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/std/env.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      316 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/std/file.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)     6997 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/lib/std/file.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/std/regex.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)      325 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/std/regex.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)       50 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/lib/std/test.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)      520 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/lib/std/test.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2248 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/logger.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot/core/package_manager/
--rw-r--r--   0 yaron     (1000) yaron     (1000)    10302 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/core/package_manager/__init__.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.159419 eikobot-0.5.0/eikobot/core/package_manager/lib/
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.159419 eikobot-0.5.0/eikobot/core/package_manager/lib/eikobot-docker-0.0.2/
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.167419 eikobot-0.5.0/eikobot/core/package_manager/lib/eikobot-docker-0.0.2/docker/
--rw-r--r--   0 yaron     (1000) yaron     (1000)      974 2023-06-04 18:43:55.000000 eikobot-0.5.0/eikobot/core/package_manager/lib/eikobot-docker-0.0.2/docker/__init__.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)     4771 2023-06-07 10:53:48.000000 eikobot-0.5.0/eikobot/core/package_manager/lib/eikobot-docker-0.0.2/docker/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      803 2023-06-05 11:53:10.000000 eikobot-0.5.0/eikobot/core/plugin.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:01:19.000000 eikobot-0.5.0/eikobot/py.typed
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.163419 eikobot-0.5.0/eikobot.egg-info/
--rw-r--r--   0 yaron     (1000) yaron     (1000)     3252 2023-06-07 14:02:39.000000 eikobot-0.5.0/eikobot.egg-info/PKG-INFO
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1885 2023-06-07 14:02:39.000000 eikobot-0.5.0/eikobot.egg-info/SOURCES.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)        1 2023-06-07 14:02:39.000000 eikobot-0.5.0/eikobot.egg-info/dependency_links.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)       49 2023-06-07 14:02:39.000000 eikobot-0.5.0/eikobot.egg-info/entry_points.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)      108 2023-06-07 14:02:39.000000 eikobot-0.5.0/eikobot.egg-info/requires.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)        8 2023-06-07 14:02:39.000000 eikobot-0.5.0/eikobot.egg-info/top_level.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)     4076 2023-06-07 14:02:39.167419 eikobot-0.5.0/setup.cfg
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1401 2023-06-07 14:01:19.000000 eikobot-0.5.0/setup.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:02:39.167419 eikobot-0.5.0/tests/
--rw-r--r--   0 yaron     (1000) yaron     (1000)     8976 2023-06-07 14:01:19.000000 eikobot-0.5.0/tests/test_compilation.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2792 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_datatypes.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      750 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_decorator.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     5979 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_deployer.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1350 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_exporter.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2353 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_import.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    16877 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_lexer.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      921 2023-06-07 14:01:19.000000 eikobot-0.5.0/tests/test_package.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     9776 2023-06-07 14:01:19.000000 eikobot-0.5.0/tests/test_parser.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      409 2023-06-05 11:53:10.000000 eikobot-0.5.0/tests/test_promises.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.464075 eikobot-0.5.1/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1059 2023-06-05 11:53:10.000000 eikobot-0.5.1/LICENSE
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     3252 2023-06-07 15:29:15.464075 eikobot-0.5.1/PKG-INFO
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2644 2023-06-07 14:01:19.000000 eikobot-0.5.1/README.md
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.460075 eikobot-0.5.1/eikobot/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      159 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     6055 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/__main__.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.460075 eikobot-0.5.1/eikobot/core/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)       39 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/__init__.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.460075 eikobot-0.5.1/eikobot/core/compiler/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1263 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    85130 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/_parser.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1666 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/_token.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2420 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/decorator.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.464075 eikobot-0.5.1/eikobot/core/compiler/definitions/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2786 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/_resource.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1593 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/base_model.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    35673 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/base_types.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    12465 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/context.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    12376 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/function.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2777 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/typedef.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     8553 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/importlib.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     9149 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/lexer.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      306 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/misc.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     8779 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/ops.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2828 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/deployer.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2893 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/errors.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     8016 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/exporter.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     4755 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/handlers.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      395 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/helpers.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.464075 eikobot-0.5.1/eikobot/core/lib/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/__init__.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.464075 eikobot-0.5.1/eikobot/core/lib/std/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      819 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/lib/std/__init__.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    14244 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/lib/std/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/std/env.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1486 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/std/env.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      316 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/std/file.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     6997 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/lib/std/file.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/std/regex.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      325 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/std/regex.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)       50 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/std/test.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      520 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/lib/std/test.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2248 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/logger.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.464075 eikobot-0.5.1/eikobot/core/package_manager/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    10663 2023-06-07 15:28:36.000000 eikobot-0.5.1/eikobot/core/package_manager/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      803 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/plugin.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/py.typed
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.460075 eikobot-0.5.1/eikobot.egg-info/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     3252 2023-06-07 15:29:15.000000 eikobot-0.5.1/eikobot.egg-info/PKG-INFO
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1663 2023-06-07 15:29:15.000000 eikobot-0.5.1/eikobot.egg-info/SOURCES.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        1 2023-06-07 15:29:15.000000 eikobot-0.5.1/eikobot.egg-info/dependency_links.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)       49 2023-06-07 15:29:15.000000 eikobot-0.5.1/eikobot.egg-info/entry_points.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      108 2023-06-07 15:29:15.000000 eikobot-0.5.1/eikobot.egg-info/requires.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        8 2023-06-07 15:29:15.000000 eikobot-0.5.1/eikobot.egg-info/top_level.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     4076 2023-06-07 15:29:15.464075 eikobot-0.5.1/setup.cfg
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1401 2023-06-07 15:24:36.000000 eikobot-0.5.1/setup.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.464075 eikobot-0.5.1/tests/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     8976 2023-06-07 14:01:19.000000 eikobot-0.5.1/tests/test_compilation.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2792 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_datatypes.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      750 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_decorator.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     5979 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_deployer.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1350 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_exporter.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2353 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_import.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    16877 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_lexer.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      921 2023-06-07 14:01:19.000000 eikobot-0.5.1/tests/test_package.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     9776 2023-06-07 14:01:19.000000 eikobot-0.5.1/tests/test_parser.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      409 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_promises.py
```

### Comparing `eikobot-0.5.0/LICENSE` & `eikobot-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/PKG-INFO` & `eikobot-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eikobot
-Version: 0.5.0
+Version: 0.5.1
 Summary: The eikobot desired state engine.
 Author: kazaamjt
 Author-email: kazaamjt@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eikobot-0.5.0/README.md` & `eikobot-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/__main__.py` & `eikobot-0.5.1/eikobot/__main__.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/__init__.py` & `eikobot-0.5.1/eikobot/core/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/_parser.py` & `eikobot-0.5.1/eikobot/core/compiler/_parser.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/_token.py` & `eikobot-0.5.1/eikobot/core/compiler/_token.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/decorator.py` & `eikobot-0.5.1/eikobot/core/compiler/decorator.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/definitions/_resource.py` & `eikobot-0.5.1/eikobot/core/compiler/definitions/_resource.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/definitions/base_model.py` & `eikobot-0.5.1/eikobot/core/compiler/definitions/base_model.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/definitions/base_types.py` & `eikobot-0.5.1/eikobot/core/compiler/definitions/base_types.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/definitions/context.py` & `eikobot-0.5.1/eikobot/core/compiler/definitions/context.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/definitions/function.py` & `eikobot-0.5.1/eikobot/core/compiler/definitions/function.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/definitions/typedef.py` & `eikobot-0.5.1/eikobot/core/compiler/definitions/typedef.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/importlib.py` & `eikobot-0.5.1/eikobot/core/compiler/importlib.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/lexer.py` & `eikobot-0.5.1/eikobot/core/compiler/lexer.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/compiler/ops.py` & `eikobot-0.5.1/eikobot/core/compiler/ops.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/deployer.py` & `eikobot-0.5.1/eikobot/core/deployer.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/errors.py` & `eikobot-0.5.1/eikobot/core/errors.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/exporter.py` & `eikobot-0.5.1/eikobot/core/exporter.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/handlers.py` & `eikobot-0.5.1/eikobot/core/handlers.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/lib/std/__init__.eiko` & `eikobot-0.5.1/eikobot/core/lib/std/__init__.eiko`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/lib/std/__init__.py` & `eikobot-0.5.1/eikobot/core/lib/std/__init__.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/lib/std/env.py` & `eikobot-0.5.1/eikobot/core/lib/std/env.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/lib/std/file.py` & `eikobot-0.5.1/eikobot/core/lib/std/file.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/lib/std/test.py` & `eikobot-0.5.1/eikobot/core/lib/std/test.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/logger.py` & `eikobot-0.5.1/eikobot/core/logger.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot/core/package_manager/__init__.py` & `eikobot-0.5.1/eikobot/core/package_manager/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -188,15 +188,16 @@
     _construct_pkg_index()
     if pkg_def.startswith("http://") or pkg_def.startswith("https://"):
         _download_pkg(pkg_def)
 
     elif pkg_def.endswith(".eiko.tar.gz"):
         _install_pkg_from_path(Path(pkg_def))
 
-    raise EikoPackageError("Failed to properly parse package url or path.")
+    else:
+        raise EikoPackageError("Failed to properly parse package url or path.")
 
 
 def _download_pkg(url: str) -> None:
     if url.endswith(".eiko.tar.gz"):
         logger.debug("Directly downloading package.")
         asyncio.run(_download_to_cache(url))
 
@@ -284,17 +285,25 @@
             check=True,
         )
 
     logger.debug("Installing requirements.")
     for req in pkg_data.requires:
         install_pkg(req)
 
-    os.symlink(
-        pkg_lib_path / pkg_data.source_dir, INTERNAL_LIB_PATH / pkg_data.source_dir
-    )
+    try:
+        os.symlink(
+            pkg_lib_path / pkg_data.source_dir, INTERNAL_LIB_PATH / pkg_data.source_dir
+        )
+    except FileExistsError:
+        # This is a bug in the package index
+        # I have no idea what causes it, but this is hack around the issue.
+        os.remove(INTERNAL_LIB_PATH / pkg_data.source_dir)
+        os.symlink(
+            pkg_lib_path / pkg_data.source_dir, INTERNAL_LIB_PATH / pkg_data.source_dir
+        )
 
     if pkg_data.version is None:
         logger.info(f"Installed '{pkg_data.name}'.")
     else:
         logger.info(f"Installed '{pkg_data.name}=={pkg_data.version}'.")
```

### Comparing `eikobot-0.5.0/eikobot/core/plugin.py` & `eikobot-0.5.1/eikobot/core/plugin.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/eikobot.egg-info/PKG-INFO` & `eikobot-0.5.1/eikobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eikobot
-Version: 0.5.0
+Version: 0.5.1
 Summary: The eikobot desired state engine.
 Author: kazaamjt
 Author-email: kazaamjt@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eikobot-0.5.0/eikobot.egg-info/SOURCES.txt` & `eikobot-0.5.1/eikobot.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -31,29 +31,25 @@
 eikobot/core/compiler/definitions/_resource.py
 eikobot/core/compiler/definitions/base_model.py
 eikobot/core/compiler/definitions/base_types.py
 eikobot/core/compiler/definitions/context.py
 eikobot/core/compiler/definitions/function.py
 eikobot/core/compiler/definitions/typedef.py
 eikobot/core/lib/__init__.py
-eikobot/core/lib/docker/__init__.eiko
-eikobot/core/lib/docker/__init__.py
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
 eikobot/core/package_manager/__init__.py
-eikobot/core/package_manager/lib/eikobot-docker-0.0.2/docker/__init__.eiko
-eikobot/core/package_manager/lib/eikobot-docker-0.0.2/docker/__init__.py
 tests/test_compilation.py
 tests/test_datatypes.py
 tests/test_decorator.py
 tests/test_deployer.py
 tests/test_exporter.py
 tests/test_import.py
 tests/test_lexer.py
```

### Comparing `eikobot-0.5.0/setup.cfg` & `eikobot-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/setup.py` & `eikobot-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import setuptools
 
 this_directory = Path(__file__).parent
 with open(this_directory / "README.md", encoding="utf-8") as f:
     long_description = f.read()
 
-VERSION = "0.5.0"
+VERSION = "0.5.1"
 REQUIRES = [
     "aiohttp==3.8.4",
     "asyncssh==2.13.1",
     "click==8.1.3",
     "colorama==0.4.6",
     "jinja2==3.1.2",
     "packaging==23.1",
```

### Comparing `eikobot-0.5.0/tests/test_compilation.py` & `eikobot-0.5.1/tests/test_compilation.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/tests/test_datatypes.py` & `eikobot-0.5.1/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/tests/test_decorator.py` & `eikobot-0.5.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/tests/test_deployer.py` & `eikobot-0.5.1/tests/test_deployer.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/tests/test_exporter.py` & `eikobot-0.5.1/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/tests/test_import.py` & `eikobot-0.5.1/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/tests/test_lexer.py` & `eikobot-0.5.1/tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/tests/test_package.py` & `eikobot-0.5.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.0/tests/test_parser.py` & `eikobot-0.5.1/tests/test_parser.py`

 * *Files identical despite different names*

