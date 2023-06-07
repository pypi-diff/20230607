# Comparing `tmp/grpc_protoc_annotations-2.15.2.tar.gz` & `tmp/grpc_protoc_annotations-2.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpc_protoc_annotations-2.15.2.tar", last modified: Wed Jun  7 10:02:09 2023, max compression
+gzip compressed data, was "grpc_protoc_annotations-2.16.0.tar", last modified: Wed Jun  7 10:04:32 2023, max compression
```

## Comparing `grpc_protoc_annotations-2.15.2.tar` & `grpc_protoc_annotations-2.16.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nicolasm   (501) staff       (20)        0 2023-06-07 10:02:09.842611 grpc_protoc_annotations-2.15.2/
--rw-r--r--   0 nicolasm   (501) staff       (20)     1515 2022-12-20 09:43:23.000000 grpc_protoc_annotations-2.15.2/LICENSE
--rw-r--r--   0 nicolasm   (501) staff       (20)     1393 2023-06-07 10:02:09.842664 grpc_protoc_annotations-2.15.2/PKG-INFO
--rw-r--r--   0 nicolasm   (501) staff       (20)      834 2023-06-07 09:42:46.000000 grpc_protoc_annotations-2.15.2/README.md
-drwxr-xr-x   0 nicolasm   (501) staff       (20)        0 2023-06-07 10:02:09.840870 grpc_protoc_annotations-2.15.2/gen/
-drwxr-xr-x   0 nicolasm   (501) staff       (20)        0 2023-06-07 10:02:09.842162 grpc_protoc_annotations-2.15.2/gen/grpc_protoc_annotations.egg-info/
--rw-r--r--   0 nicolasm   (501) staff       (20)     1393 2023-06-07 10:02:09.000000 grpc_protoc_annotations-2.15.2/gen/grpc_protoc_annotations.egg-info/PKG-INFO
--rw-r--r--   0 nicolasm   (501) staff       (20)      443 2023-06-07 10:02:09.000000 grpc_protoc_annotations-2.15.2/gen/grpc_protoc_annotations.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasm   (501) staff       (20)        1 2023-06-07 10:02:09.000000 grpc_protoc_annotations-2.15.2/gen/grpc_protoc_annotations.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasm   (501) staff       (20)       25 2023-06-07 10:02:09.000000 grpc_protoc_annotations-2.15.2/gen/grpc_protoc_annotations.egg-info/requires.txt
--rw-r--r--   0 nicolasm   (501) staff       (20)       29 2023-06-07 10:02:09.000000 grpc_protoc_annotations-2.15.2/gen/grpc_protoc_annotations.egg-info/top_level.txt
-drwxr-xr-x   0 nicolasm   (501) staff       (20)        0 2023-06-07 10:02:09.840925 grpc_protoc_annotations-2.15.2/gen/protoc_gen_openapiv2/
-drwxr-xr-x   0 nicolasm   (501) staff       (20)        0 2023-06-07 10:02:09.842492 grpc_protoc_annotations-2.15.2/gen/protoc_gen_openapiv2/options/
--rw-r--r--   0 nicolasm   (501) staff       (20)        0 2023-06-07 10:02:05.000000 grpc_protoc_annotations-2.15.2/gen/protoc_gen_openapiv2/options/__init__.py
--rw-r--r--   0 nicolasm   (501) staff       (20)     2712 2023-06-07 10:02:05.000000 grpc_protoc_annotations-2.15.2/gen/protoc_gen_openapiv2/options/annotations_pb2.py
--rw-r--r--   0 nicolasm   (501) staff       (20)    19672 2023-06-07 10:02:05.000000 grpc_protoc_annotations-2.15.2/gen/protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--   0 nicolasm   (501) staff       (20)      104 2022-12-20 09:43:23.000000 grpc_protoc_annotations-2.15.2/pyproject.toml
--rw-r--r--   0 nicolasm   (501) staff       (20)      716 2023-06-07 10:02:09.842891 grpc_protoc_annotations-2.15.2/setup.cfg
+drwxr-xr-x   0 nicolasm   (501) staff       (20)        0 2023-06-07 10:04:32.957847 grpc_protoc_annotations-2.16.0/
+-rw-r--r--   0 nicolasm   (501) staff       (20)     1515 2022-12-20 09:43:23.000000 grpc_protoc_annotations-2.16.0/LICENSE
+-rw-r--r--   0 nicolasm   (501) staff       (20)     1393 2023-06-07 10:04:32.957901 grpc_protoc_annotations-2.16.0/PKG-INFO
+-rw-r--r--   0 nicolasm   (501) staff       (20)      834 2023-06-07 09:42:46.000000 grpc_protoc_annotations-2.16.0/README.md
+drwxr-xr-x   0 nicolasm   (501) staff       (20)        0 2023-06-07 10:04:32.955926 grpc_protoc_annotations-2.16.0/gen/
+drwxr-xr-x   0 nicolasm   (501) staff       (20)        0 2023-06-07 10:04:32.957368 grpc_protoc_annotations-2.16.0/gen/grpc_protoc_annotations.egg-info/
+-rw-r--r--   0 nicolasm   (501) staff       (20)     1393 2023-06-07 10:04:32.000000 grpc_protoc_annotations-2.16.0/gen/grpc_protoc_annotations.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasm   (501) staff       (20)      443 2023-06-07 10:04:32.000000 grpc_protoc_annotations-2.16.0/gen/grpc_protoc_annotations.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasm   (501) staff       (20)        1 2023-06-07 10:04:32.000000 grpc_protoc_annotations-2.16.0/gen/grpc_protoc_annotations.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasm   (501) staff       (20)       25 2023-06-07 10:04:32.000000 grpc_protoc_annotations-2.16.0/gen/grpc_protoc_annotations.egg-info/requires.txt
+-rw-r--r--   0 nicolasm   (501) staff       (20)       29 2023-06-07 10:04:32.000000 grpc_protoc_annotations-2.16.0/gen/grpc_protoc_annotations.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasm   (501) staff       (20)        0 2023-06-07 10:04:32.955979 grpc_protoc_annotations-2.16.0/gen/protoc_gen_openapiv2/
+drwxr-xr-x   0 nicolasm   (501) staff       (20)        0 2023-06-07 10:04:32.957712 grpc_protoc_annotations-2.16.0/gen/protoc_gen_openapiv2/options/
+-rw-r--r--   0 nicolasm   (501) staff       (20)        0 2023-06-07 10:04:27.000000 grpc_protoc_annotations-2.16.0/gen/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 nicolasm   (501) staff       (20)     2712 2023-06-07 10:04:27.000000 grpc_protoc_annotations-2.16.0/gen/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 nicolasm   (501) staff       (20)    19672 2023-06-07 10:04:27.000000 grpc_protoc_annotations-2.16.0/gen/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 nicolasm   (501) staff       (20)      104 2022-12-20 09:43:23.000000 grpc_protoc_annotations-2.16.0/pyproject.toml
+-rw-r--r--   0 nicolasm   (501) staff       (20)      716 2023-06-07 10:04:32.958145 grpc_protoc_annotations-2.16.0/setup.cfg
```

### Comparing `grpc_protoc_annotations-2.15.2/LICENSE` & `grpc_protoc_annotations-2.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grpc_protoc_annotations-2.15.2/PKG-INFO` & `grpc_protoc_annotations-2.16.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpc_protoc_annotations
-Version: 2.15.2
+Version: 2.16.0
 Summary: Provides the missing pieces for gRPC Gateway.
 Home-page: https://github.com/prosehair/grpc_protoc_annotations
 Author: Prosehair
 Author-email: nicolas@prosehair.com
 Project-URL: Bug Tracker, https://github.com/prosehair/grpc_protoc_annotations/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `grpc_protoc_annotations-2.15.2/README.md` & `grpc_protoc_annotations-2.16.0/README.md`

 * *Files identical despite different names*

### Comparing `grpc_protoc_annotations-2.15.2/gen/grpc_protoc_annotations.egg-info/PKG-INFO` & `grpc_protoc_annotations-2.16.0/gen/grpc_protoc_annotations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpc-protoc-annotations
-Version: 2.15.2
+Version: 2.16.0
 Summary: Provides the missing pieces for gRPC Gateway.
 Home-page: https://github.com/prosehair/grpc_protoc_annotations
 Author: Prosehair
 Author-email: nicolas@prosehair.com
 Project-URL: Bug Tracker, https://github.com/prosehair/grpc_protoc_annotations/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `grpc_protoc_annotations-2.15.2/gen/protoc_gen_openapiv2/options/annotations_pb2.py` & `grpc_protoc_annotations-2.16.0/gen/protoc_gen_openapiv2/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `grpc_protoc_annotations-2.15.2/gen/protoc_gen_openapiv2/options/openapiv2_pb2.py` & `grpc_protoc_annotations-2.16.0/gen/protoc_gen_openapiv2/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `grpc_protoc_annotations-2.15.2/setup.cfg` & `grpc_protoc_annotations-2.16.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = grpc_protoc_annotations
-version = 2.15.2
+version = 2.16.0
 author = Prosehair
 author_email = nicolas@prosehair.com
 description = Provides the missing pieces for gRPC Gateway.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/prosehair/grpc_protoc_annotations
 project_urls =
```

