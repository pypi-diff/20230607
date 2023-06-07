# Comparing `tmp/multi_channel_pytorch-0.1.0.tar.gz` & `tmp/multi_channel_pytorch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_channel_pytorch-0.1.0.tar", max compression
+gzip compressed data, was "multi_channel_pytorch-0.2.0.tar", max compression
```

## Comparing `multi_channel_pytorch-0.1.0.tar` & `multi_channel_pytorch-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35821 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.1.0/multi_channel_pytorch/__init__.py
--rw-r--r--   0        0        0     5291 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.1.0/multi_channel_pytorch/injection.py
--rw-r--r--   0        0        0      807 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.1.0/multi_channel_pytorch/multify.py
--rw-r--r--   0        0        0       89 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.1.0/multi_channel_pytorch/utils.py
--rw-r--r--   0        0        0      527 2023-06-07 09:16:16.339184 multi_channel_pytorch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.1.0/README.md
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 multi_channel_pytorch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35821 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.2.0/multi_channel_pytorch/__init__.py
+-rw-r--r--   0        0        0     7807 2023-06-07 10:47:31.805147 multi_channel_pytorch-0.2.0/multi_channel_pytorch/injection.py
+-rw-r--r--   0        0        0      807 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.2.0/multi_channel_pytorch/multify.py
+-rw-r--r--   0        0        0       89 2023-06-07 09:12:12.630108 multi_channel_pytorch-0.2.0/multi_channel_pytorch/utils.py
+-rw-r--r--   0        0        0      527 2023-06-07 10:49:10.100826 multi_channel_pytorch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2090 2023-06-07 10:36:27.173678 multi_channel_pytorch-0.2.0/README.md
+-rw-r--r--   0        0        0     2716 1970-01-01 00:00:00.000000 multi_channel_pytorch-0.2.0/PKG-INFO
```

### Comparing `multi_channel_pytorch-0.1.0/LICENSE` & `multi_channel_pytorch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multi_channel_pytorch-0.1.0/multi_channel_pytorch/multify.py` & `multi_channel_pytorch-0.2.0/multi_channel_pytorch/multify.py`

 * *Files identical despite different names*

### Comparing `multi_channel_pytorch-0.1.0/pyproject.toml` & `multi_channel_pytorch-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multi-channel-pytorch"
-version = "0.1.0"
+version = "0.2.0"
 description = "Library for adding multi channel functionality to PyTorch models."
 license = "GPL-3.0-only"
 authors = ["Timo Michel <timo.michel1996@outlook.de>"]
 readme = "README.md"
 repository = "https://github.com/Timom1996/multi-channel-pytorch"
 packages = [{include = "multi_channel_pytorch"}]
```

