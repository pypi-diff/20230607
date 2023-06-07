# Comparing `tmp/easy_logs-1.0.0.tar.gz` & `tmp/easy_logs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_logs-1.0.0.tar", last modified: Wed Jun  7 18:31:44 2023, max compression
+gzip compressed data, was "easy_logs-1.0.1.tar", last modified: Wed Jun  7 18:39:52 2023, max compression
```

## Comparing `easy_logs-1.0.0.tar` & `easy_logs-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:31:44.491514 easy_logs-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-07 18:31:44.491514 easy_logs-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:31:44.491514 easy_logs-1.0.0/easy_logs/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-07 18:31:28.000000 easy_logs-1.0.0/easy_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-07 18:31:28.000000 easy_logs-1.0.0/easy_logs/_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-07 18:31:28.000000 easy_logs-1.0.0/easy_logs/_logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-07 18:31:28.000000 easy_logs-1.0.0/easy_logs/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:31:44.491514 easy_logs-1.0.0/easy_logs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-07 18:31:44.000000 easy_logs-1.0.0/easy_logs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-07 18:31:44.000000 easy_logs-1.0.0/easy_logs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:31:44.000000 easy_logs-1.0.0/easy_logs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 18:31:44.000000 easy_logs-1.0.0/easy_logs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:31:44.491514 easy_logs-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-07 18:31:28.000000 easy_logs-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:39:52.323553 easy_logs-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-07 18:39:52.323553 easy_logs-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:39:52.323553 easy_logs-1.0.1/easy_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-07 18:39:42.000000 easy_logs-1.0.1/easy_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-07 18:39:42.000000 easy_logs-1.0.1/easy_logs/_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-07 18:39:42.000000 easy_logs-1.0.1/easy_logs/_logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-07 18:39:42.000000 easy_logs-1.0.1/easy_logs/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:39:52.323553 easy_logs-1.0.1/easy_logs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-07 18:39:52.000000 easy_logs-1.0.1/easy_logs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-07 18:39:52.000000 easy_logs-1.0.1/easy_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:39:52.000000 easy_logs-1.0.1/easy_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 18:39:52.000000 easy_logs-1.0.1/easy_logs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:39:52.323553 easy_logs-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-07 18:39:42.000000 easy_logs-1.0.1/setup.py
```

### Comparing `easy_logs-1.0.0/PKG-INFO` & `easy_logs-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: easy_logs
-Version: 1.0.0
-Summary: My personal package for colored logs. Highly customizable.
+Version: 1.0.1
+Summary: package for easy colored logs with predefined configurations.
 Home-page: https://github.com/michalskibinski109/easy_logging
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `easy_logs-1.0.0/easy_logs/__init__.py` & `easy_logs-1.0.1/easy_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_logs-1.0.0/easy_logs/_configurations.py` & `easy_logs-1.0.1/easy_logs/_configurations.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,28 +10,25 @@
     file_name: str = None
     format: str = "%(message)s (%(filename)s:%(lineno)d)"
     datefmt: str = "%H:%M:%S"
     disable_existing_loggers: bool = False
     colored: bool = True
 
 
-_simple_logger_config = _LoggingConfig(
-    logger_name="simple_logger",
-    format="%(message)s",
-    disable_existing_loggers=True,
-    lvl=10,
-)
+class Configs:
+    simple_logger_config = _LoggingConfig(
+        logger_name="simple_logger",
+        format="%(message)s",
+        disable_existing_loggers=True,
+        lvl=10,
+    )
 
+    profesionall_logger_config = _LoggingConfig(
+        logger_name="proffesional_logger",
+        file_name="logs.log",
+        format="%(asctime)20s | %(levelname)8s | %(filename)20s :%(lineno)4d | %(message)s",
+        datefmt="%Y-%m-%d %H:%M:%S",
+    )
+    default_logger_config = _LoggingConfig()
 
-_proffesional_logger_config = _LoggingConfig(
-    logger_name="proffesional_logger",
-    file_name="logs.log",
-    format="%(asctime)20s | %(levelname)8s | %(filename)20s :%(lineno)4d | %(message)s",
-    datefmt="%Y-%m-%d %H:%M:%S",
-)
-_default_logger_config = _LoggingConfig()
 
-_LOGGERS = {
-    "simple": _simple_logger_config,
-    "proffesional": _proffesional_logger_config,
-    "default": _default_logger_config,
-}
+_LOGGERS = {name.split("_")[0]: config for name, config in Configs.__dict__.items()}
```

### Comparing `easy_logs-1.0.0/easy_logs/_logging_utils.py` & `easy_logs-1.0.1/easy_logs/_logging_utils.py`

 * *Files identical despite different names*

### Comparing `easy_logs-1.0.0/easy_logs/main.py` & `easy_logs-1.0.1/easy_logs/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging.config
 from logging import Logger, getLogger
 from pathlib import Path
 from typing import Union, Literal
-from easy_logging._logging_utils import ColoredFormatter, filter_log_record
-from _configurations import _LOGGERS
+from easy_logs._logging_utils import ColoredFormatter, filter_log_record
+from easy_logs._configurations import _LOGGERS
 
 
 class FailedToLoadLoggingConfigException(Exception):
     pass
 
 
 def get_logger(
```

### Comparing `easy_logs-1.0.0/easy_logs.egg-info/PKG-INFO` & `easy_logs-1.0.1/easy_logs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: easy-logs
-Version: 1.0.0
-Summary: My personal package for colored logs. Highly customizable.
+Version: 1.0.1
+Summary: package for easy colored logs with predefined configurations.
 Home-page: https://github.com/michalskibinski109/easy_logging
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `easy_logs-1.0.0/setup.py` & `easy_logs-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,18 +99,18 @@
 logger.info("info")
 logger.warning("warning")
 ```
 """
 
 setuptools.setup(
     name="easy_logs",
-    version="1.0.0",
+    version="1.0.1",
     author="Michał Skibiński",
     author_email="mskibinski109@gmail.com",
-    description="My personal package for colored logs. Highly customizable.",
+    description="package for easy colored logs with predefined configurations.",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     files_to_include=["easy_logs"],
     package_data={"readme": ["readme.md"]},
     url="https://github.com/michalskibinski109/easy_logging",
     packages=setuptools.find_packages(),
     classifiers=[
```

