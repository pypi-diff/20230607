# Comparing `tmp/moonlight-0.0.8.tar.gz` & `tmp/moonlight-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonlight-0.0.8.tar", max compression
+gzip compressed data, was "moonlight-0.0.9.tar", max compression
```

## Comparing `moonlight-0.0.8.tar` & `moonlight-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-03-13 10:38:43.787671 moonlight-0.0.8/LICENSE
--rw-r--r--   0        0        0      171 2023-03-13 10:38:43.787780 moonlight-0.0.8/README.md
--rw-r--r--   0        0        0      412 2023-03-13 14:01:22.903798 moonlight-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3732 2023-03-13 14:01:44.592424 moonlight-0.0.8/src/moonlight/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 10:38:43.787932 moonlight-0.0.8/src/moonlight/jar/__init__.py
--rw-r--r--   0        0        0   337864 2023-03-13 10:32:46.282432 moonlight-0.0.8/src/moonlight/jar/antlr4-runtime.jar
--rw-r--r--   0        0        0   432208 2023-03-13 10:40:03.118331 moonlight-0.0.8/src/moonlight/jar/engine.jar
--rw-r--r--   0        0        0   162822 2023-03-13 10:40:03.079722 moonlight-0.0.8/src/moonlight/jar/script.jar
--rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 moonlight-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-13 10:38:43.787671 moonlight-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1709 2023-03-14 09:59:57.329279 moonlight-0.0.9/README.md
+-rw-r--r--   0        0        0      412 2023-03-14 10:02:09.242036 moonlight-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3732 2023-03-13 14:01:44.592424 moonlight-0.0.9/src/moonlight/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 10:38:43.787932 moonlight-0.0.9/src/moonlight/jar/__init__.py
+-rw-r--r--   0        0        0   337864 2023-03-13 10:32:46.282432 moonlight-0.0.9/src/moonlight/jar/antlr4-runtime.jar
+-rw-r--r--   0        0        0   432208 2023-03-13 10:40:03.118331 moonlight-0.0.9/src/moonlight/jar/engine.jar
+-rw-r--r--   0        0        0   162822 2023-03-13 10:40:03.079722 moonlight-0.0.9/src/moonlight/jar/script.jar
+-rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 moonlight-0.0.9/PKG-INFO
```

### Comparing `moonlight-0.0.8/LICENSE` & `moonlight-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `moonlight-0.0.8/src/moonlight/__init__.py` & `moonlight-0.0.9/src/moonlight/__init__.py`

 * *Files identical despite different names*

### Comparing `moonlight-0.0.8/src/moonlight/jar/antlr4-runtime.jar` & `moonlight-0.0.9/src/moonlight/jar/antlr4-runtime.jar`

 * *Files identical despite different names*

### Comparing `moonlight-0.0.8/src/moonlight/jar/engine.jar` & `moonlight-0.0.9/src/moonlight/jar/engine.jar`

 * *Files identical despite different names*

### Comparing `moonlight-0.0.8/src/moonlight/jar/script.jar` & `moonlight-0.0.9/src/moonlight/jar/script.jar`

 * *Files identical despite different names*

