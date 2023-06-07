# Comparing `tmp/onnc-bench-4.1.9.tar.gz` & `tmp/onnc-bench-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onnc-bench-4.1.9.tar", last modified: Thu Mar  2 04:06:23 2023, max compression
+gzip compressed data, was "dist/onnc-bench-4.2.0.tar", last modified: Wed Jun  7 18:50:13 2023, max compression
```

## Comparing `onnc-bench-4.1.9.tar` & `onnc-bench-4.2.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/
--rw-r--r--   0 Ben        (501) staff       (20)     1199 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/PKG-INFO
--rw-r--r--   0 Ben        (501) staff       (20)      913 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/README.md
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/
--rwxr-xr-x   0 Ben        (501) staff       (20)      863 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/__init__.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/bench/
--rw-r--r--   0 Ben        (501) staff       (20)      794 2023-03-02 04:06:22.000000 onnc-bench-4.1.9/onnc/bench/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     1200 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/config.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/bench/core/
--rwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)       92 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/benchmark.py
--rw-r--r--   0 Ben        (501) staff       (20)      515 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/common.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/bench/core/compiler/
--rw-r--r--   0 Ben        (501) staff       (20)     1903 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/compiler/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     2092 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/compiler/builder.py
--rw-r--r--   0 Ben        (501) staff       (20)     4445 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/compiler/nnuxe.py
--rw-r--r--   0 Ben        (501) staff       (20)     2129 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/compiler/nnuxe_docker.py
--rw-r--r--   0 Ben        (501) staff       (20)    12019 2023-02-09 04:31:37.000000 onnc-bench-4.1.9/onnc/bench/core/compiler/onnc_saas.py
--rw-r--r--   0 Ben        (501) staff       (20)     1009 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/compiler/saas_config.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/bench/core/dataset/
--rw-r--r--   0 Ben        (501) staff       (20)      574 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/dataset/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     3048 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/dataset/dataset.py
--rw-r--r--   0 Ben        (501) staff       (20)     7394 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/dataset/identifier.py
--rw-r--r--   0 Ben        (501) staff       (20)      661 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/dataset/layout.py
--rw-r--r--   0 Ben        (501) staff       (20)     2220 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/dataset/operation.py
--rw-r--r--   0 Ben        (501) staff       (20)     1456 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/dataset/preprocessor.py
--rw-r--r--   0 Ben        (501) staff       (20)     8189 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/dataset/serializer.py
--rw-r--r--   0 Ben        (501) staff       (20)     2419 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/dataset/transformer.py
--rw-r--r--   0 Ben        (501) staff       (20)     5077 2023-02-09 04:31:37.000000 onnc-bench-4.1.9/onnc/bench/core/deployment.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/bench/core/evaluator/
--rw-r--r--   0 Ben        (501) staff       (20)      697 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/evaluator/__init__.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/bench/core/model/
--rw-r--r--   0 Ben        (501) staff       (20)     1129 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/model/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     3759 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/model/dtype_map.py
--rw-r--r--   0 Ben        (501) staff       (20)    10557 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/model/identifier.py
--rw-r--r--   0 Ben        (501) staff       (20)    14313 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/model/meta.py
--rw-r--r--   0 Ben        (501) staff       (20)     3995 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/model/model.py
--rw-r--r--   0 Ben        (501) staff       (20)     6705 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/model/serializer.py
--rw-r--r--   0 Ben        (501) staff       (20)      577 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/core/model/transformer.py
--rw-r--r--   0 Ben        (501) staff       (20)     7347 2023-03-02 04:05:22.000000 onnc-bench-4.1.9/onnc/bench/core/modelpackage.py
--rw-r--r--   0 Ben        (501) staff       (20)     6308 2023-02-09 04:09:54.000000 onnc-bench-4.1.9/onnc/bench/project.py
--rw-r--r--   0 Ben        (501) staff       (20)      279 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/bench/utils.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/forest/
--rw-r--r--   0 Ben        (501) staff       (20)      295 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/__init__.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/forest/core/
--rwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/core/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)      748 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/core/binding_helper.py
--rw-r--r--   0 Ben        (501) staff       (20)     1667 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/core/options.py
--rw-r--r--   0 Ben        (501) staff       (20)     4244 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/core/runtime.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/forest/proxies/
--rw-r--r--   0 Ben        (501) staff       (20)     1754 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/proxies/__init__.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/forest/proxies/zerorpc/
--rw-r--r--   0 Ben        (501) staff       (20)        0 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/proxies/zerorpc/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     2294 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/proxies/zerorpc/runtime.py
--rw-r--r--   0 Ben        (501) staff       (20)     2388 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/proxies/zerorpc/runtime_server.py
--rw-r--r--   0 Ben        (501) staff       (20)      482 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/proxies/zerorpc/utils.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/forest/runtimes/
--rwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/runtimes/__init__.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/forest/runtimes/onnx/
--rw-r--r--   0 Ben        (501) staff       (20)        0 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/runtimes/onnx/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     2069 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/runtimes/onnx/runtime.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/forest/runtimes/openvino/
--rwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/runtimes/openvino/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     4931 2023-02-09 03:59:48.000000 onnc-bench-4.1.9/onnc/forest/runtimes/openvino/runtime.py
--rw-r--r--   0 Ben        (501) staff       (20)     6455 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/runtimes/openvino/utils.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/forest/runtimes/tensorrt/
--rwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/runtimes/tensorrt/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     3623 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/runtimes/tensorrt/runtime.py
--rw-r--r--   0 Ben        (501) staff       (20)     2930 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/runtimes/tensorrt/utils.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc/forest/utils/
--rwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/utils/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)      510 2023-02-09 01:54:37.000000 onnc-bench-4.1.9/onnc/forest/utils/load_img.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/onnc_bench.egg-info/
--rw-r--r--   0 Ben        (501) staff       (20)     1199 2023-03-02 04:06:22.000000 onnc-bench-4.1.9/onnc_bench.egg-info/PKG-INFO
--rw-r--r--   0 Ben        (501) staff       (20)     1985 2023-03-02 04:06:22.000000 onnc-bench-4.1.9/onnc_bench.egg-info/SOURCES.txt
--rw-r--r--   0 Ben        (501) staff       (20)        1 2023-03-02 04:06:22.000000 onnc-bench-4.1.9/onnc_bench.egg-info/dependency_links.txt
--rw-r--r--   0 Ben        (501) staff       (20)       48 2023-03-02 04:06:22.000000 onnc-bench-4.1.9/onnc_bench.egg-info/requires.txt
--rw-r--r--   0 Ben        (501) staff       (20)        5 2023-03-02 04:06:22.000000 onnc-bench-4.1.9/onnc_bench.egg-info/top_level.txt
--rw-r--r--   0 Ben        (501) staff       (20)       38 2023-03-02 04:06:23.000000 onnc-bench-4.1.9/setup.cfg
--rw-r--r--   0 Ben        (501) staff       (20)      858 2023-03-02 04:06:22.000000 onnc-bench-4.1.9/setup.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      991 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/PKG-INFO
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      725 2023-05-22 10:00:39.000000 onnc-bench-4.2.0/README.md
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)      863 2023-02-07 10:13:51.000000 onnc-bench-4.2.0/onnc/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/bench/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      794 2023-06-07 18:50:12.000000 onnc-bench-4.2.0/onnc/bench/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1213 2023-06-01 09:39:05.000000 onnc-bench-4.2.0/onnc/bench/config.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/bench/core/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-05-19 06:51:56.000000 onnc-bench-4.2.0/onnc/bench/core/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       92 2022-05-19 06:51:56.000000 onnc-bench-4.2.0/onnc/bench/core/benchmark.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      515 2022-07-05 06:10:59.000000 onnc-bench-4.2.0/onnc/bench/core/common.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1811 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1838 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/builder.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3886 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/nnuxe.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2129 2022-09-22 04:18:54.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/nnuxe_docker.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)    11856 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/onnc_saas.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1009 2022-07-05 06:10:59.000000 onnc-bench-4.2.0/onnc/bench/core/compiler/saas_config.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      574 2022-07-12 05:47:39.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3048 2022-10-27 02:52:35.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/dataset.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     7431 2023-05-17 08:52:59.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/identifier.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      661 2022-05-19 06:51:56.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/layout.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2220 2022-10-19 15:48:12.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/operation.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1456 2022-10-25 08:05:07.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/preprocessor.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     8188 2023-05-17 08:46:00.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/serializer.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2419 2022-05-19 06:51:56.000000 onnc-bench-4.2.0/onnc/bench/core/dataset/transformer.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4005 2023-05-22 10:27:59.000000 onnc-bench-4.2.0/onnc/bench/core/deployment.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/bench/core/evaluator/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      697 2022-05-19 06:51:56.000000 onnc-bench-4.2.0/onnc/bench/core/evaluator/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/bench/core/model/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1122 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/model/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3759 2023-06-01 11:15:50.000000 onnc-bench-4.2.0/onnc/bench/core/model/dtype_map.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     9880 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/model/identifier.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)    15409 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/model/meta.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4573 2023-05-17 08:09:57.000000 onnc-bench-4.2.0/onnc/bench/core/model/model.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     6772 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/core/model/serializer.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      577 2022-05-19 06:51:56.000000 onnc-bench-4.2.0/onnc/bench/core/model/transformer.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     7347 2023-05-17 08:56:50.000000 onnc-bench-4.2.0/onnc/bench/core/modelpackage.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     6253 2023-06-07 17:45:11.000000 onnc-bench-4.2.0/onnc/bench/project.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      279 2022-07-28 03:03:26.000000 onnc-bench-4.2.0/onnc/bench/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      295 2022-07-28 03:03:26.000000 onnc-bench-4.2.0/onnc/forest/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/core/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.2.0/onnc/forest/core/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      748 2022-09-21 03:34:59.000000 onnc-bench-4.2.0/onnc/forest/core/binding_helper.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1667 2022-09-19 02:11:04.000000 onnc-bench-4.2.0/onnc/forest/core/options.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4244 2022-10-21 04:37:40.000000 onnc-bench-4.2.0/onnc/forest/core/runtime.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/proxies/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1754 2022-09-19 02:11:04.000000 onnc-bench-4.2.0/onnc/forest/proxies/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2022-09-19 02:11:04.000000 onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2294 2022-09-19 02:11:04.000000 onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/runtime.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2388 2022-09-19 02:11:04.000000 onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/runtime_server.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      482 2022-09-19 02:11:04.000000 onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/runtimes/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.2.0/onnc/forest/runtimes/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/runtimes/onnx/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-02-07 10:13:51.000000 onnc-bench-4.2.0/onnc/forest/runtimes/onnx/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2069 2022-10-25 08:05:07.000000 onnc-bench-4.2.0/onnc/forest/runtimes/onnx/runtime.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/runtimes/openvino/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.2.0/onnc/forest/runtimes/openvino/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4819 2023-05-19 03:28:04.000000 onnc-bench-4.2.0/onnc/forest/runtimes/openvino/runtime.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     6455 2022-07-05 06:10:59.000000 onnc-bench-4.2.0/onnc/forest/runtimes/openvino/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/runtimes/tensorrt/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.2.0/onnc/forest/runtimes/tensorrt/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3623 2022-10-25 08:05:07.000000 onnc-bench-4.2.0/onnc/forest/runtimes/tensorrt/runtime.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2930 2022-07-26 09:00:19.000000 onnc-bench-4.2.0/onnc/forest/runtimes/tensorrt/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc/forest/utils/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.2.0/onnc/forest/utils/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      510 2022-07-05 06:10:59.000000 onnc-bench-4.2.0/onnc/forest/utils/load_img.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc_bench.egg-info/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      991 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc_bench.egg-info/PKG-INFO
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1985 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc_bench.egg-info/SOURCES.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        1 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc_bench.egg-info/dependency_links.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      291 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc_bench.egg-info/requires.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        5 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/onnc_bench.egg-info/top_level.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       38 2023-06-07 18:50:13.000000 onnc-bench-4.2.0/setup.cfg
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1324 2023-06-07 18:50:12.000000 onnc-bench-4.2.0/setup.py
```

### Comparing `onnc-bench-4.1.9/PKG-INFO` & `onnc-bench-4.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: onnc-bench
-Version: 4.1.9
+Version: 4.2.0
 Summary: ONNC-bench is a Python wrapper of ONNC
 Home-page: https://www.skymizer.com
 Author: The Skymizer Team
 Author-email: hello@skymizer.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # ONNC-bench
 
 ONNC-bench is a Python wrapper of ONNC
 
 ## Installation
 
 ### Using pip
+
 ```
 pip install onnc-bench
 ```
 
 ## Python API Example
+
 Here is an example to show how to use ONNC python API
+
 ```
 from onnc.bench import login, Project
 # Setup your ONNC API key
 api_key = "Your API KEY"
 login(api_key)
 
 # Instantiate a projct
@@ -37,23 +39,10 @@
 # Compile the model and optmize to `CMSIS-NN` backend
 project.compile(target='CMSIS-NN-DEFAULT')
 
 
 # Save the compiled model
 deployment = project.save('./output')
 
-print(deployment.report)
-
-{
-    'sram_size': 2490,
-    'flash_size': 101970
-}
 ```
 
-The report shows we need:
-    2,490 bytes of SRAM
-  101,970 bytes of ROM
-to run this model on a CortexM device.
-
 Please Check https://docs-tinyonnc.skymizer.com/index.html for the full documents.
-
-
```

### Comparing `onnc-bench-4.1.9/README.md` & `onnc-bench-4.2.0/onnc_bench.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,33 @@
+Metadata-Version: 2.1
+Name: onnc-bench
+Version: 4.2.0
+Summary: ONNC-bench is a Python wrapper of ONNC
+Home-page: https://www.skymizer.com
+Author: The Skymizer Team
+Author-email: hello@skymizer.com
+License: Apache License 2.0
+Description-Content-Type: text/markdown
+
 # ONNC-bench
 
 ONNC-bench is a Python wrapper of ONNC
 
 ## Installation
 
 ### Using pip
+
 ```
 pip install onnc-bench
 ```
 
 ## Python API Example
+
 Here is an example to show how to use ONNC python API
+
 ```
 from onnc.bench import login, Project
 # Setup your ONNC API key
 api_key = "Your API KEY"
 login(api_key)
 
 # Instantiate a projct
@@ -26,21 +39,10 @@
 # Compile the model and optmize to `CMSIS-NN` backend
 project.compile(target='CMSIS-NN-DEFAULT')
 
 
 # Save the compiled model
 deployment = project.save('./output')
 
-print(deployment.report)
-
-{
-    'sram_size': 2490,
-    'flash_size': 101970
-}
 ```
 
-The report shows we need:
-    2,490 bytes of SRAM
-  101,970 bytes of ROM
-to run this model on a CortexM device.
-
 Please Check https://docs-tinyonnc.skymizer.com/index.html for the full documents.
```

### Comparing `onnc-bench-4.1.9/onnc/__init__.py` & `onnc-bench-4.2.0/onnc/__init__.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/__init__.py` & `onnc-bench-4.2.0/onnc/bench/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,8 +24,8 @@
              level="INFO")
 
 sentry_sdk.init(
     "https://da9cdf5759874504940714a91657de21@o304393.ingest.sentry.io/5901378",
     traces_sample_rate=1.0)
 fpath = os.path.dirname(os.path.abspath(__file__))
 
-__version__= "4.1.9"
+__version__= "4.2.0"
```

### Comparing `onnc-bench-4.1.9/onnc/bench/config.py` & `onnc-bench-4.2.0/onnc/bench/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 api_url = "api.onnc.skymizer.com"
 api_port = 443
 
 image_name = 'registry.skymizer.com/nnuxe/nnuxe/nnuxe_image'
 image_tag = "v0.0.4-test"
 
 default_builder: IBuilder
-try:
-    if os.environ['BENCH_COMPILER'] == "NNUXE":
-        from .core.compiler.nnuxe import NNUXEBuilder
 
-        default_builder = NNUXEBuilder
-        default_builder_params = []
-    elif os.environ['BENCH_COMPILER'] == "NNUXE_DOCKER":
-        from .core.compiler.nnuxe_docker import NNUXEDockerBuilder
+if os.environ.get('BENCH_COMPILER') == "NNUXE":
+    from .core.compiler.nnuxe import NNUXEBuilder
+    default_builder = NNUXEBuilder
+    default_builder_params = []
+elif os.environ.get('BENCH_COMPILER') == "NNUXE_DOCKER":
+    from .core.compiler.nnuxe_docker import NNUXEDockerBuilder
 
-        default_builder = NNUXEDockerBuilder
-        default_builder_params = [image_name, image_tag]
-    else:
-        default_builder = ONNCSaaSBuilder
-        default_builder_params = [api_protocol, api_url, api_port]
-except KeyError:
+    default_builder = NNUXEDockerBuilder
+    default_builder_params = [image_name, image_tag]
+elif os.environ.get('BENCH_COMPILER') == "NNUXE_SAAS":
     default_builder = ONNCSaaSBuilder
     default_builder_params = [api_protocol, api_url, api_port]
+else:
+    from .core.compiler.nnuxe import NNUXEBuilder
+    default_builder = NNUXEBuilder
+    default_builder_params = []
```

### Comparing `onnc-bench-4.1.9/onnc/bench/core/common.py` & `onnc-bench-4.2.0/onnc/bench/core/common.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/core/compiler/__init__.py` & `onnc-bench-4.2.0/onnc/bench/core/compiler/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,12 @@
             raise TypeError("dataset.src should be str or path, "
                             f"not {type(dataset.src)}")
         self.compilation_id: str  # SaaS compilation_id
         self.model_path = model.src
         self.sample_path = dataset.src
         self.model_meta = self.get_model_meta(model, inputs_as_nchw)
         self.sample_meta = self.get_dataset_meta(dataset)
-        self.calibrator_params: Dict[str, Any]
-        self.compiler_params: Dict[str, Any]
 
 
 from .onnc_saas import ONNCSaaSBuilder
 from .nnuxe import NNUXEBuilder
 from .nnuxe_docker import NNUXEDockerBuilder
```

### Comparing `onnc-bench-4.1.9/onnc/bench/core/compiler/builder.py` & `onnc-bench-4.2.0/onnc/bench/core/compiler/builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,19 +34,14 @@
         """
 
         compilation = Compilation(model, dataset, inputs_as_nchw)
         _internal_cid = id(model.src)
         self._compilations[_internal_cid] = compilation
         return _internal_cid
 
-    def set_compilations_params(self, model_id: int, compile_params: Dict,
-        calibrator_params:Dict):
-        self._compilations[model_id].calibrator_params = calibrator_params
-        self._compilations[model_id].compiler_params = compile_params
-
     @abstractmethod
     def build(self, target, converter_params: Dict = {}) -> Any:
         """build a project witch contains multiple models
 
         for model in model_ids:
             ...
         """
```

### Comparing `onnc-bench-4.1.9/onnc/bench/core/compiler/nnuxe.py` & `onnc-bench-4.2.0/onnc/bench/core/compiler/nnuxe.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 class NNUXEBuilder(IBuilder):
     BUILDER_NAME = "NNUXEBuilder"
 
     def __init__(self):
         self._compilations: Dict[int, Compilation] = {}
         self.output_path: str = ""
 
-
     def _compile(self,
                  model_name,
                  model_path: str,
                  sample_path: str,
                  params_path: str,
                  output_path: str,
                  local_nnuxe: bool = True):
@@ -46,31 +45,29 @@
                       report,
                       local_nnuxe=local_nnuxe)
         return report
 
     def build(self, target: str, converter_params={}) -> Dict:
 
         compilation_list = []
-        params = {}
-        res = {}
+
+
         # Upload files and create compilation
         for iternal_cid in self._compilations:
+            params = {}
             compilation = self._compilations[iternal_cid]
-
-            compilation.compiler_params['target'] = target
-
+            params["target"] = target
             params["model_meta"] = compilation.model_meta
             params["sample_meta"] = compilation.sample_meta
-            params["compiler_params"] = compilation.compiler_params
-            params["calibrator_params"] = compilation.calibrator_params
             params["converter_params"] = converter_params
             compilation_list.append(
                 (compilation.model_path, compilation.sample_path, params))
         output_path = get_tmp_path()
         os.makedirs(output_path, exist_ok=True)
+        res = {}
         for idx, compi in enumerate(compilation_list):
             model_path = compi[0]
             sample_path = compi[1]
             params = compi[2]
             params_path = get_tmp_path()
             open(params_path, 'w').write(json.dumps(params))
             report = self._compile(f'model_{idx}', model_path, sample_path,
@@ -83,47 +80,35 @@
 
             logger.debug(params)
 
         self.output_path = output_path
 
         return res
 
-    def save(self, output: Path) -> Union[Dict, Deployment]:
-        res = {}
+    def save(self, output: Path) -> Deployment:
         shutil.rmtree(output, ignore_errors=True)
         shutil.copytree(self.output_path, output)
-        shutil.rmtree(self.output_path, ignore_errors=True)
-
-        for i in os.listdir(output):
-            try:
-                out = Path(os.path.join(output, i))
-                deployment = Deployment(out)
-            except Exception as e:
-                deployment = Deployment(None)
-
-            res[i] = deployment
-        return res
-        # return Deployment(None, report=res, logs=res)
+        return Deployment(output)
 
     @property
     def supported_devices(self) -> Dict:
         devices = {
             'CMSIS-NN': 'CMSIS-NN',
             'ANDES-LIBNN': 'ANDES-LIBNN',
             'NVDLA-NV-SMALL': 'NVDLA-NV-SMALL',
             'NVDLA-NV-LARGE': 'NVDLA-NV-LARGE',
             'NVDLA-NV-FULL': 'NVDLA-NV-FULL',
             'CMSIS-NN-DEFAULT': 'CMSIS-NN-DEFAULT',
             'NVDLA-NV-SMALL-DEFAULT': 'NVDLA-NV-SMALL-DEFAULT',
             'NVDLA-NV-LARGE-DEFAULT': 'NVDLA-NV-LARGE-DEFAULT',
             'NVDLA-NV-FULL-DEFAULT': 'NVDLA-NV-FULL-DEFAULT',
-            'NVIDIA-TENSORRT-FP32' : 'NVIDIA-TENSORRT-FP32',
-            'NVIDIA-TENSORRT-FP16' : 'NVIDIA-TENSORRT-FP16',
-            'NVIDIA-TENSORRT-INT8' : 'NVIDIA-TENSORRT-INT8',
-            'RELAYIR' : 'RELAYIR',
+            'NVIDIA-TENSORRT-FP32': 'NVIDIA-TENSORRT-FP32',
+            'NVIDIA-TENSORRT-FP16': 'NVIDIA-TENSORRT-FP16',
+            'NVIDIA-TENSORRT-INT8': 'NVIDIA-TENSORRT-INT8',
+            'RELAYIR': 'RELAYIR',
             "INTEL-OPENVINO-CPU-FP32": "INTEL-OPENVINO-CPU-FP32",
             "FIXED_ONNX": "FIXED_ONNX",
             "ONNX": "ONNX",
             "ONNC-IN2O3": "ONNC-IN2O3",
             "GenericONNC": "GenericONNC"
         }
         return devices
```

### Comparing `onnc-bench-4.1.9/onnc/bench/core/compiler/nnuxe_docker.py` & `onnc-bench-4.2.0/onnc/bench/core/compiler/nnuxe_docker.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/core/compiler/onnc_saas.py` & `onnc-bench-4.2.0/onnc/bench/core/compiler/onnc_saas.py`

 * *Files 7% similar despite different names*

```diff
@@ -236,22 +236,18 @@
         if not converter_params:
             params = {}
         saas_compilations = []
 
         # Upload files and create compilation
         for iternal_cid in self._compilations:
             compilation = self._compilations[iternal_cid]
-
-            compilation.compiler_params['target'] = target
-
             params = {}
+            params["target"] = target
             params["model_meta"] = compilation.model_meta
             params["sample_meta"] = compilation.sample_meta
-            params["compiler_params"] = compilation.compiler_params
-            params["calibrator_params"] = compilation.calibrator_params
             params["converter_params"] = converter_params
 
             data = self._saas_create_compilation(compilation.model_path,
                                                  compilation.sample_path,
                                                  params)
             # saas_compilations.append(cr.data["id"])
             saas_compilations.append(data)
```

### Comparing `onnc-bench-4.1.9/onnc/bench/core/compiler/saas_config.py` & `onnc-bench-4.2.0/onnc/bench/core/compiler/saas_config.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/core/dataset/__init__.py` & `onnc-bench-4.2.0/onnc/bench/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/core/dataset/dataset.py` & `onnc-bench-4.2.0/onnc/bench/core/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/core/dataset/identifier.py` & `onnc-bench-4.2.0/onnc/bench/core/dataset/identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 class IdentifierRegistry(type):
 
     REGISTRY: List = []
 
     def __new__(cls, name, bases, attrs):
         new_cls = type.__new__(cls, name, bases, attrs)
-        cls.REGISTRY.append(new_cls)
+        if name != "Identifier":
+            cls.REGISTRY.append(new_cls)
         return new_cls
 
 
 class Identifier(metaclass=IdentifierRegistry):
 
     FORMAT: DatasetFormat = DatasetFormat.NON_SPECIFIED
```

### Comparing `onnc-bench-4.1.9/onnc/bench/core/dataset/layout.py` & `onnc-bench-4.2.0/onnc/bench/core/dataset/layout.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/core/dataset/operation.py` & `onnc-bench-4.2.0/onnc/bench/core/dataset/operation.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/core/dataset/preprocessor.py` & `onnc-bench-4.2.0/onnc/bench/core/dataset/preprocessor.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/core/dataset/serializer.py` & `onnc-bench-4.2.0/onnc/bench/core/dataset/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 def serialize(dataset: Dataset, dest: Path) -> Dataset:
     for serializer in Serializer.REGISTRY:
         if serializer.is_me(dataset):
             return serializer().serialize(dataset, dest)
 
-    raise NotImplementedError(f"Unalble to identify {dataset.src}")
+    raise NotImplementedError(f"Unable to identify {dataset.src}")
 
 
 class FileSerializer(Serializer):
 
     FORMAT: DatasetFormat = DatasetFormat.NON_SPECIFIED
 
     def transform(self, dataset: Dataset):
```

### Comparing `onnc-bench-4.1.9/onnc/bench/core/dataset/transformer.py` & `onnc-bench-4.2.0/onnc/bench/core/dataset/transformer.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/core/deployment.py` & `onnc-bench-4.2.0/onnc/bench/core/deployment.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,65 +6,46 @@
 from os.path import abspath
 
 from onnc.bench.core.model.model import Model
 
 
 class Deployment:
     """
-    Deployment is a container class for built artifacts and reports
+    Deployment describes the output directory of a compilation results.
+        ├── base_path
+        │   └── model_0
+        │       ├── build
+        │       │   └── model
+        │       ├── report.json
+        │       └── working_dir
     """
     META_FNAME = Path('.deployment.json')
 
-    def __init__(self, path: Union[None, Path], report=None, logs=None):
-        self._compiled_files: List = []
-        self._report = report
-        self._compile_logs = logs
-        if path:
-            self.base_path = Path(path)
-            self.report_path = self.base_path / Path('report.json')
-        else:
-            self.base_path = Path("")
-            self.report_path = Path('report.json')
-
-    def __str__(self):
-        try:
-            with open(self.report_path, 'r') as f:
-                report = json.load(f)
-            return json.dumps(report, sort_keys=True, indent=2)
-        except:
-            return "{}"
-
-    def __repr__(self):
-        return json.dumps(self.meta, sort_keys=True, indent=2)
-
-    @property
-    def report(self) -> Dict:
-        if not self._report:
-            if os.path.exists(self.report_path):
-                with open(self.report_path, 'r') as f:
-                    return dict(json.load(f)["metrics"])
-        else:
-            return self._report
+    def __init__(self, base_path: Path):
 
-        return {}
+        if not os.path.isdir(base_path):
+            raise FileNotFoundError(f'"{base_path}" is not an exist dir')
+        self.base_path = Path(base_path)
+        self.report_paths = list(self.base_path.rglob("**/report.json"))
+        if len(self.report_paths) == 0:
+            raise FileNotFoundError(
+                'A deployment dir should contain at least one model_N/report.json'
+                'but not found in {}'.format(self.base_path)
+            )
 
     @property
-    def compiled_files(self):
-        if os.path.exists(self.base_path):
-            model_src = self.base_path / Path('build')
-            if model_src.exists():
-                files = []
-                # list all files recursively
-                for i in os.walk(model_src):
-                    if len(i[2]) > 0:
-                        for j in i[2]:
-                            files.append(os.path.join(i[0], j))
-                return files
+    def reports(self):
+        res = []
+        for report_path in self.report_paths:
+            with open(report_path, 'r') as f:
+                report = json.load(f)
+                # res.append(json.dumps(report, sort_keys=True, indent=2))
+                res.append(report)
+        return res
 
-        return []
     @property
     def loadable(self):
         if len(self.loadables) > 1:
             raise ValueError("Error: Compilation result contains multiple "
                              "models, use loadables instead.")
         elif len(self.loadables) == 0:
             raise ValueError("Error: No loadable found "
@@ -75,14 +56,25 @@
     def loadables(self) -> List[Model]:
 
         if not os.path.exists(self.base_path):
             raise Exception(f'Deployment base_path is not a directory: '
                             f'{self.base_path}.')
         res = []
         for sub_model_root in os.listdir(self.base_path):
+            """
+            └── self.base_path
+                └── model_0    <------ sub_model_root
+                │    ├── build
+                │    │   ├── by_product
+                │    │   └── model.xxx
+                │    ├── report.json
+                │    └── working_dir
+                │        └── asdf.txt
+
+            """
             root = self.base_path / sub_model_root
             if not os.path.isdir(root / "build"):
                 raise Exception(f'Invalid deployment subdir {root}: '
                                 f'Missing model directory')
             model_to_add = None
             if os.path.isdir(root / "build/model"):
                 """
@@ -102,53 +94,17 @@
                 raise Exception(
                     f"Unrecognized deployment subdir "
                     f"abspath{root}, plz contacts developers to fix it.")
             else:
                 res.append(model_to_add)
         return res
 
-    @property
-    def compile_logs(self):
-        if not self._compile_logs:
-            if os.path.exists(self.report_path):
-                with open(self.report_path, 'r') as f:
-                    return json.load(f)["logs"]
-        else:
-            return self._compile_logs
-
-        return []
-
-    @property
-    def meta(self):
-        return {
-            "base_path": str(self.base_path),
-            "compiled_files": [str(x) for x in self.compiled_files],
-            "report_path": str(self.report_path),
-            "report": self.report
-        }
-
-    def save(self):
-        _path = self.base_path / self.META_FNAME
-        open(_path, 'w').write(json.dumps(self.meta, sort_keys=True, indent=4))
-
-    def load(self):
-        meta = json.loads(open(self.base_path / self.META_FNAME, 'r').read())
-
-        self.base_path = meta["base_path"]
-        self.report_path = meta["report_path"]
-
-    def load_raw(self):
-        """Scan folder and construct the object"""
-        pass
-
     def deploy(self, target: Path):
         """Copy the deployment folder to target
 
         Copy the deployment folder to target and reconstruct the meta
 
         """
         shutil.copytree(self.base_path, target)
         if os.path.exists(target / self.META_FNAME):
             os.remove(target / self.META_FNAME)
-        deployment = Deployment(target)
-
-        return deployment
+        return Deployment(target)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `onnc-bench-4.1.9/onnc/bench/core/evaluator/__init__.py` & `onnc-bench-4.2.0/onnc/bench/core/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/core/model/dtype_map.py` & `onnc-bench-4.2.0/onnc/bench/core/model/dtype_map.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/core/model/identifier.py` & `onnc-bench-4.2.0/onnc/bench/core/model/identifier.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import zipfile
 from enum import Enum
 import inspect
 from pathlib import Path
 from typing import List, Union
 from onnc.bench.core.model.model import Model
 from onnc.bench.core.dataset.dataset import Dataset
+from onnc.bench.core.model.model import SrcType
 # from typing import TYPE_CHECKING
 
 # if TYPE_CHECKING:
 #     from . import Model
 
 from . import ModelFormat
 
@@ -29,83 +30,71 @@
 
 class IdentifierRegistry(type):
 
     REGISTRY: List = []
 
     def __new__(cls, name, bases, attrs):
         new_cls = type.__new__(cls, name, bases, attrs)
-        cls.REGISTRY.append(new_cls)
+        if name != "Identifier":
+            cls.REGISTRY.append(new_cls)
         return new_cls
 
 
 class Identifier(metaclass=IdentifierRegistry):
 
     FORMAT = ModelFormat.NON_SPECIFIED
 
     @classmethod
     def is_me(cls, model: Model) -> bool:
         pass
 
 
 def identify(model: Model) -> ModelFormat:
     for identifier in Identifier.REGISTRY:
-        if identifier.is_me(model):
+        if model.format == identifier.FORMAT:
             return identifier.FORMAT
-    raise NotImplementedError(f"Unable to identify {model.src}")
+        elif identifier.is_me(model):
+            return identifier.FORMAT
+
+    raise NotImplementedError(
+        f"Unable to identify {model.src}. Maybe it doesn't exist, plz check.")
 
 
 class H5(Identifier):
     """
     Use file extension and magic number to identify the file
     """
     FORMAT = ModelFormat.H5
 
     @classmethod
     def is_me(cls, model: Model) -> bool:
-        if model.format == cls.FORMAT:
-            return True
-
-        if isinstance(model.src, str):
-            path = Path(model.src)
-        else:
-            path = model.src
-
-        if not (isinstance(path, Path) and path.exists() and path.is_file()):
+        if model.get_src_type() != SrcType.FILE:
             return False
-        if str(path).lower().endswith('.h5'):
+        if str(model.src).lower().endswith('.h5'):
             return True
-        with open(path, 'rb') as f:
+        with open(model.src, 'rb') as f:
             r = f.read(8) == bytes.fromhex('894844460d0a1a0a')
             return r
 
 
 class ONNX(Identifier):
     """
     Use file extension and magic number to identify the file
     """
     FORMAT = ModelFormat.ONNX
 
     @classmethod
     def is_me(cls, model: Model):
-        if model.format == cls.FORMAT:
-            return True
-
-        if isinstance(model.src, str):
-            path = Path(model.src)
-        else:
-            path = model.src
-
-        if not (isinstance(path, Path) and path.exists() and path.is_file()):
+        if model.get_src_type() != SrcType.FILE:
             return False
-        if str(path).lower().endswith('.onnx'):
+        if str(model.src).lower().endswith('.onnx'):
             return True
-
         import onnx
         try:
-            onnx.checker.check_model(str(path))
+            onnx.checker.check_model(str(model.src))
         except onnx.onnx_cpp2py_export.checker.ValidationError:
             return False
         return True
 
 
 class PTH(Identifier):
     """
@@ -116,31 +105,23 @@
     number, then get the file list and check if it match torch strucutre
     """
     FORMAT = ModelFormat.PTH
 
     @classmethod
     def is_me(cls, model: Model):
 
-        if model.format == cls.FORMAT:
-            return True
-
-        if isinstance(model.src, str):
-            path = Path(model.src)
-        else:
-            path = model.src
-
-        if not (isinstance(path, Path) and path.exists() and path.is_file()):
+        if model.get_src_type() != SrcType.FILE:
             return False
 
-        with open(path, 'rb') as f:
+        with open(model.src, 'rb') as f:
             if not f.read(4) == bytes.fromhex('504b0304'):
                 return False
 
         try:
-            z = zipfile.ZipFile(path)
+            z = zipfile.ZipFile(model.src)
             file_names = '|'.join(z.namelist())
             return ('code/__torch__' not in file_names) and \
                    'data.pkl' in file_names and \
                    'data/' in file_names
         except OSError:
             return False
 
@@ -153,31 +134,21 @@
     number, then get the file list and check if it match torch strucutre
     """
     FORMAT = ModelFormat.TORCH_TRACED
 
     @classmethod
     def is_me(cls, model: Model):
 
-        if model.format == cls.FORMAT:
-            return True
-
-        if isinstance(model.src, str):
-            path = Path(model.src)
-        else:
-            path = model.src
-
-        if not (isinstance(path, Path) and path.exists() and path.is_file()):
+        if model.get_src_type() != SrcType.FILE:
             return False
-
-        with open(path, 'rb') as f:
+        with open(model.src, 'rb') as f:
             if not f.read(4) == bytes.fromhex('504b0304'):
                 return False
-
         try:
-            z = zipfile.ZipFile(path)
+            z = zipfile.ZipFile(model.src)
             file_names = '|'.join(z.namelist())
             return 'code/__torch__' in file_names and \
                    'data.pkl' in file_names and \
                    'data/' in file_names
         except OSError:
             return False
 
@@ -187,68 +158,51 @@
     Use file extension and magic number to identify the file
     """
 
     FORMAT = ModelFormat.PB
 
     @classmethod
     def is_me(cls, model: Model):
-
-        if model.format == cls.FORMAT:
-            return True
-
-        if isinstance(model.src, str):
-            path = Path(model.src)
-        else:
-            path = model.src
-
-        if not (isinstance(path, Path) and path.exists() and path.is_file()):
+        if model.get_src_type() != SrcType.FILE:
             return False
-
         # I dont find such pattern in:
         # 1. https://github.com/chen0040/java-tensorflow-samples/blob/master/audio-classifier/src/main/resources/tf_models/resnet-v2.pb
         # 2. https://github.com/bugra/putting-tensorflow-2-models-to-production/blob/master/models/resnet/1538687457/saved_model.pb
         # 3. https://github.com/U-t-k-a-r-s-h/Auto-Labeling-tool-using-Tensorflow/blob/master/Mobilenet.pb
         # 4. https://codechina.csdn.net/shy_201992/human-pose-estimation-opencv/-/blob/master/graph_opt.pb
         #
         # with open(path, 'rb') as f:
         #     if f.read(8) == 'PBDEMS2\0':
         #         return True
 
         # check if 'dtype' exists in the first 1k of the file.
-        with open(path, 'rb') as f:
+        with open(model.src, 'rb') as f:
             if bytes.fromhex('0A05647479706512') in f.read(1024):
                 return True
 
-        return str(path).lower().endswith('.pb')
+        return str(model.src).lower().endswith('.pb')
 
 
 class TFLITE(Identifier):
     """
     Use file extension and magic number to identify the file
     """
 
     FORMAT = ModelFormat.TFLITE
 
     @classmethod
     def is_me(cls, model: Model):
 
-        if model.format == cls.FORMAT:
-            return True
-
-        if isinstance(model.src, str):
-            path = Path(model.src)
-        else:
-            path = model.src
+        if model.get_src_type() != SrcType.FILE:
+            return False
 
-        if str(path).lower().endswith(".tflite"):
+        if str(model.src).lower().endswith(".tflite"):
             return True
-        if not (isinstance(path, Path) and path.exists() and path.is_file()):
-            return False
 
-        with open(path, 'rb') as f:
+        with open(model.src, 'rb') as f:
             if bytes.fromhex('1C00000054464C33') in f.read(8):
                 return True
 
         return False
 
 
 class SavedModel(Identifier):
@@ -257,149 +211,145 @@
     """
 
     FORMAT = ModelFormat.SAVED_MODEL
 
     @classmethod
     def is_me(cls, model: Model):
 
-        if model.format == cls.FORMAT:
-            return True
-
-        if isinstance(model.src, str):
-            path = Path(model.src)
-        else:
-            path = model.src
-
-        if not (isinstance(path, Path) and path.exists()):
+        if model.get_src_type() != SrcType.DIR:
             return False
 
-        if path.is_dir():
-            return (os.path.exists(os.path.join(path, 'saved_model.pb')) and
-                    os.path.exists(os.path.join(path, 'variables')))
-        return False
+        return (os.path.exists(os.path.join(model.src, 'saved_model.pb')) and
+                os.path.exists(os.path.join(model.src, 'variables')))
 
 
 class ZippedSavedModel(Identifier):
     """
     Use directory pattern to identify the file
     """
 
     FORMAT = ModelFormat.ZIPPED_SAVED_MODEL
 
     @classmethod
     def is_me(cls, model: Model) -> bool:
 
-        if model.format == cls.FORMAT:
-            return True
-
-        if isinstance(model.src, str):
-            path = Path(model.src)
-        else:
-            path = model.src
-
-        if not (isinstance(path, Path) and path.exists()):
+        if model.get_src_type() != SrcType.FILE:
+            return False
+        try:
+            z = zipfile.ZipFile(model.src)
+            file_names = '|'.join(z.namelist())
+            return 'saved_model.pb' in file_names and 'variables' in file_names
+        except Exception:
             return False
-
-        if path.is_file():
-            try:
-                z = zipfile.ZipFile(path)
-                file_names = '|'.join(z.namelist())
-                return 'saved_model.pb' in file_names and 'variables' in file_names
-            except OSError:
-                return False
-            except zipfile.BadZipFile:
-                return False
-        return False
 
 
 class TFKerasModel(Identifier):
     ''' Use python MRO to check if it contains specific str
     '''
 
     FORMAT = ModelFormat.TF_KERAS_MODEL
 
     @classmethod
     def is_me(cls, model: Model):
-
-        if model.format == cls.FORMAT:
-            return True
-
+        if model.get_src_type() != SrcType.OBJ:
+            return False
         return _check_object_type('tensorflow.python.keras', model.src)
 
 
 class TFSession(Identifier):
     ''' Use python MRO to check if it contains specific str
     '''
     FORMAT = ModelFormat.TF_SESSION
 
     @classmethod
     def is_me(cls, model: Model):
-
-        if model.format == cls.FORMAT:
-            return True
-
+        if model.get_src_type() != SrcType.OBJ:
+            return False
         return _check_object_type('tensorflow.python.client.session.Session',
                                   model.src)
 
 
 class KerasModel(Identifier):
     '''Use python MRO to check if it contains specific str
     Keras 2.5.0 Serializer
     '''
 
     FORMAT = ModelFormat.KERAS_MODEL
 
     @classmethod
     def is_me(cls, model: Model):
-
-        if model.format == cls.FORMAT:
-            return True
-
+        if model.get_src_type() != SrcType.OBJ:
+            return False
         return _check_object_type('keras.', model.src)
 
 
 class PytorchModel(Identifier):
     """Use python MRO to check if it contains specific str"""
 
     FORMAT = ModelFormat.PT_NN_MODULE
 
     @classmethod
     def is_me(cls, model: Model):
 
-        if model.format == cls.FORMAT:
-            return True
-
-        if _check_object_type('torch.nn.module', model.src):
-            return True
-
-        elif _check_object_type('torchvision.models.', model.src):
-            return True
-
-        else:
+        if model.get_src_type() != SrcType.OBJ:
             return False
 
+        return (_check_object_type('torch.nn.module', model.src) or
+                _check_object_type('torchvision.models.', model.src))
+
 
 class OpenvinoIRDir(Identifier):
     FORMAT = ModelFormat.OPENVINO_IRDIR
 
     @classmethod
     def is_me(cls, model: Model):
-        model_path = model.src
-        if not os.path.isdir(model_path):
+        if model.get_src_type() != SrcType.DIR:
             return False
+        model_path = model.src
         files = glob.glob(f"{model_path}/*")
 
         return (any([f.endswith(".xml") for f in files]) and
                 any([f.endswith(".bin") for f in files]) and
                 any([f.endswith(".mapping") for f in files]))
 
 
 class TensorrtPLAN(Identifier):
     FORMAT = ModelFormat.TRT_PLAN
 
     @classmethod
     def is_me(cls, model: Model):
+        if model.get_src_type() != SrcType.FILE:
+            return False
+        return str(model.src).endswith(".plan") or str(
+            model.src).endswith(".engine")
+
+class CaffeDir(Identifier):
+    FORMAT = ModelFormat.CAFFE_DIR
+
+    @classmethod
+    def is_me(cls, model: Model):
+        if model.get_src_type() != SrcType.DIR:
+            return False
         model_path = model.src
-        if not os.path.isfile(model_path):
+        files = glob.glob(f"{model_path}/*")
+
+        return (any([f.endswith(".caffemodel") for f in files]) and
+                any([f.endswith(".prototxt") for f in files]))
+
+class ZippedCaffeDir(Identifier):
+    """
+    Use directory pattern to identify the file
+    """
+
+    FORMAT = ModelFormat.ZIPPED_CAFFE_DIR
+    @classmethod
+    def is_me(cls, model: Model) -> bool:
+
+        if model.get_src_type() != SrcType.FILE:
+            return False
+        try:
+            z = zipfile.ZipFile(model.src)
+            files = z.namelist()
+            return (any([f.endswith(".caffemodel") for f in files]) and
+                any([f.endswith(".prototxt") for f in files]))
+        except Exception:
             return False
-        return str(model_path).endswith(".plan") or str(model_path).endswith(
-            ".engine")
```

### Comparing `onnc-bench-4.1.9/onnc/bench/core/model/meta.py` & `onnc-bench-4.2.0/onnc/bench/core/model/meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 class MetadataRetriverRegistry(type):
 
     REGISTRY: List = []
 
     def __new__(cls, name, bases, attrs):
         new_cls = type.__new__(cls, name, bases, attrs)
-        cls.REGISTRY.append(new_cls)
+        if name != "MetadataRetriver":
+            cls.REGISTRY.append(new_cls)
         return new_cls
 
 
 class ModelMeta:
 
     def __init__(self, inputs: List[Tensor], outputs: List[Tensor]):
         self.inputs = inputs
@@ -58,15 +59,15 @@
 
 
 def retrieve_model_metadata(model: Model) -> ModelMeta:
     for metadataretriever in MetadataRetriver.REGISTRY:
         if metadataretriever.is_me(model):
             return metadataretriever().retrieve(model)
 
-    raise NotImplementedError(f"Unalble to retrieve metadata of {model.format}")
+    raise NotImplementedError(f"Unable to retrieve metadata of {model.format}")
 
 
 class H5(MetadataRetriver):
 
     FORMAT = ModelFormat.H5
 
     from .dtype_map import TF_map
@@ -183,40 +184,34 @@
             graph_def.ParseFromString(f.read())
         with tf.Graph().as_default() as graph:
             tf.import_graph_def(graph_def)
 
         ops = graph.get_operations()
         return ops
 
-    def analyze_inputs_outputs(graph):
-
-        inputs = []
-        for op in ops:
-            if len(op.inputs) == 0 and op.type != 'Const':
-                inputs.append(op)
-            else:
-                for input_tensor in op.inputs:
-                    if input_tensor.op in outputs_set:
-                        outputs_set.remove(input_tensor.op)
-        outputs = list(outputs_set)
-        return (inputs, outputs)
-
     def retrieve_inputs(self, model: Model) -> List[Tensor]:
         import tensorflow as tf
         ops = self._load_graph(model.src)
         inputs = []
         for op in ops:
             if len(op.inputs) == 0 and op.type != 'Const':
                 inputs.append(op)
 
-        return [
-            Tensor(name=x.name,
-                   shape=tuple(xx if xx else -1 for xx in x.outputs[0].shape),
-                   dtype=self.TF_map.map(x.outputs[0].dtype)) for x in inputs
-        ]
+        res = []
+        """
+        Eliminating "/" in the name is still under experiment
+        This bug happens when converting bert-squad-384.pb which's input
+        should be "logits" but is "import/logits" in the graph
+        """
+        for x in inputs:
+            res.append(
+                Tensor(name=x.name.split("/")[-1],
+                       shape=tuple(xx if xx else -1 for xx in x.outputs[0].shape),
+                       dtype=self.TF_map.map(x.outputs[0].dtype)))
+        return res
         """
         >>> [x.size for x in graph_def.node[0].attr['shape'].shape.dim]
         [-1, 96, 96, 3]
         """
 
     def retrieve_outputs(self, model: Model) -> List[Tensor]:
         import tensorflow as tf
@@ -229,20 +224,26 @@
                 inputs.append(op)
             else:
                 for input_tensor in op.inputs:
                     if input_tensor.op in outputs_set:
                         outputs_set.remove(input_tensor.op)
 
         outputs = list(outputs_set)
-
-        return [
-            Tensor(name=x.name,
-                   shape=tuple(xx if xx else -1 for xx in x.outputs[0].shape),
-                   dtype=self.TF_map.map(x.outputs[0].dtype)) for x in outputs
-        ]
+        res = []
+        """
+        Eliminating "/" in the name is still under experiment
+        This bug happens when converting bert-squad-384.pb which's input
+        should be "logits" but is "import/logits" in the graph
+        """
+        for x in outputs:
+            res.append(
+                Tensor(name=x.name.split("/")[-1],
+                       shape=tuple(xx if xx else -1 for xx in x.outputs[0].shape),
+                       dtype=self.TF_map.map(x.outputs[0].dtype)))
+        return res
 
 
 class SavedModel(MetadataRetriver):
 
     FORMAT = ModelFormat.SAVED_MODEL
 
     from .dtype_map import TF_map
@@ -432,7 +433,34 @@
         res = []
         for i in interpreter.get_output_details():
             res.append(
                 Tensor(i["name"],
                        tuple(-1 if not s else int(s) for s in i["shape"]),
                        self._dtype_map.map(i['dtype'])))
         return res
+
+class CaffeDir(MetadataRetriver):
+    FORMAT = ModelFormat.CAFFE_DIR
+    def retrieve_inputs(self, model: Model) -> List[Tensor]:
+        return []
+    def retrieve_outputs(self, model: Model) -> List[Tensor]:
+        return []
+
+
+class ZippedSavedModel(CaffeDir):
+
+    FORMAT = ModelFormat.ZIPPED_CAFFE_DIR
+
+    def retrieve_inputs(self, model: Model) -> List[Tensor]:
+        temp = get_tmp_path()
+
+        with zipfile.ZipFile(model.src,
+                             'r') as zip_ref:  # type: ignore[arg-type]
+            zip_ref.extractall(temp)
+        return super().retrieve_inputs(Model(temp))
+
+    def retrieve_outputs(self, model: Model) -> List[Tensor]:
+        temp = get_tmp_path()
+        with zipfile.ZipFile(model.src,
+                             'r') as zip_ref:  # type: ignore[arg-type]
+            zip_ref.extractall(temp)
+        return super().retrieve_outputs(Model(temp))
```

### Comparing `onnc-bench-4.1.9/onnc/bench/core/model/model.py` & `onnc-bench-4.2.0/onnc/bench/core/model/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union, Tuple, Any, List, Type, Dict, Optional
 from dataclasses import dataclass
 from pathlib import Path
 from collections import OrderedDict
 from loguru import logger
-from enum import Enum
+from enum import Enum, auto
 
 from . import ModelFormat, ModelDataType
 from ..common import get_class_name
 
 
 @dataclass
 class Tensor:
@@ -23,14 +23,20 @@
                 self.shape,
             "type":
                 self.dtype.name
                 if isinstance(self.dtype, ModelDataType) else None
         }
 
 
+class SrcType(Enum):
+    OBJ = auto()
+    FILE = auto()
+    DIR = auto()
+
+
 class Model():
 
     def __init__(self,
                  src: Union[str, Path, object],
                  format=ModelFormat.NON_SPECIFIED,
                  inputs: List[Union[List, Tuple, Tensor]] = None,
                  outputs: List[Union[List, Tuple, Tensor]] = None,
@@ -39,15 +45,15 @@
         Do not put identify_format in Model. Make sure
         (MVC) control and model are separated.
         """
         if not inputs:
             inputs = []
         if not outputs:
             outputs = []
-        if isinstance(src,str):
+        if isinstance(src, str):
             self.src = Path(src)
         else:
             self.src = src
         self.inputs: List[Tensor] = inputs
         self.outputs: List = outputs
         self.format = format
         self.batch_dim: int = batch_dim
@@ -60,14 +66,34 @@
         else:
             self._name = str(type(object))
 
     @property
     def name(self) -> str:
         return self._name
 
+    def get_src_type(self) -> SrcType:
+        """
+          Return type of self.src
+          Return None if self.src is not a valid path
+        """
+
+        if isinstance(self.src, str):
+            path = Path(self.src)
+        elif isinstance(self.src, Path):
+            path = self.src
+        else:
+            return SrcType.OBJ
+
+        if path.is_dir():
+            return SrcType.DIR
+        elif path.is_file():
+            return SrcType.FILE
+        else:
+            return None
+
     def set_name(self, _name: str):
         self._name = _name
 
     def set_batch_dim(self, _batch_dim: Optional[int]):
         if _batch_dim is not None:
             assert _batch_dim >= 0
         self.batch_dim = _batch_dim
```

### Comparing `onnc-bench-4.1.9/onnc/bench/core/model/serializer.py` & `onnc-bench-4.2.0/onnc/bench/core/model/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,23 @@
         return m
 
 
 def serializer_selector(model: Model) -> Serializer:
     for serializer in Serializer.REGISTRY:
         if serializer.is_me(model):
             return serializer
-    raise NotImplementedError(f"Unalble to serialize {model}")
+    raise NotImplementedError(f"Unable to serialize {model}")
 
 
 def serialize(model: Model, dest: Path) -> Model:
     for serializer in Serializer.REGISTRY:
         if serializer.is_me(model):
             return serializer().serialize(model, dest)
 
-    raise NotImplementedError(f"Unalble to serialize {model}")
+    raise NotImplementedError(f"Unable to serialize {model}")
 
 
 class FileSerializer(Serializer):
 
     FORMAT: ModelFormat = ModelFormat.NON_SPECIFIED
 
     def transform(self, model: Model):
@@ -105,14 +105,19 @@
     def serialize(self, model: Model, dest: Path) -> Model:
         # return super().serialize(model, dest)
         self.add_param('dest', dest)  # type: ignore[attr-defined]
         m = self.transform(model)
         return m
 
 
+class CaffeDir(DirSerializer):
+
+    FORMAT = ModelFormat.CAFFE_DIR
+
+
 class H5(FileSerializer):
 
     FORMAT = ModelFormat.H5
 
 
 class ONNX(FileSerializer):
```

### Comparing `onnc-bench-4.1.9/onnc/bench/core/model/transformer.py` & `onnc-bench-4.2.0/onnc/bench/core/model/transformer.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/core/modelpackage.py` & `onnc-bench-4.2.0/onnc/bench/core/modelpackage.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/bench/project.py` & `onnc-bench-4.2.0/onnc/bench/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,15 @@
                                      sample_format, model_inputs, model_outputs,
                                      batch_dim)
         serialized_model, serialized_dataset = model_package.serialize()
 
         model_id = self.builder.prepare_model(serialized_model,
                                               serialized_dataset,
                                               inputs_as_nchw)
-        self.builder.set_compilations_params(model_id,compile_params={},
-            calibrator_params={})
+        return serialized_model, serialized_dataset
 
     def compile(self, target: str, converter_params: Dict = None):
         """Trigger the compilation process and transform the given
         model into C function calls.
 
         :param str device:
             The name of the supported SoC board, for example, NUMAKER_IOT_M487.
```

### Comparing `onnc-bench-4.1.9/onnc/forest/core/binding_helper.py` & `onnc-bench-4.2.0/onnc/forest/core/binding_helper.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/forest/core/options.py` & `onnc-bench-4.2.0/onnc/forest/core/options.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/forest/core/runtime.py` & `onnc-bench-4.2.0/onnc/forest/core/runtime.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/forest/proxies/__init__.py` & `onnc-bench-4.2.0/onnc/forest/proxies/__init__.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/forest/proxies/zerorpc/runtime.py` & `onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/runtime.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/forest/proxies/zerorpc/runtime_server.py` & `onnc-bench-4.2.0/onnc/forest/proxies/zerorpc/runtime_server.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/forest/runtimes/onnx/runtime.py` & `onnc-bench-4.2.0/onnc/forest/runtimes/onnx/runtime.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/forest/runtimes/openvino/runtime.py` & `onnc-bench-4.2.0/onnc/forest/runtimes/openvino/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,16 +68,14 @@
         model = self.core.read_model(xml_path)
 
         # This step is belong to `materialize`
         # However, bind_input() need to use compiled_model
         # to create InferRequest, so, it is a workaround
         # and materialize the model in the step `load`
         self._compiled_model = self.core.compile_model(model, self.device)
-        print("self._compiled_model",
-              self._compiled_model.get_property("INFERENCE_NUM_THREADS"))
 
     def create_infer_request(self):
 
         infer_request = self._compiled_model.create_infer_request()
         return infer_request
 
     def _create_infer_request(self):
```

### Comparing `onnc-bench-4.1.9/onnc/forest/runtimes/openvino/utils.py` & `onnc-bench-4.2.0/onnc/forest/runtimes/openvino/utils.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/forest/runtimes/tensorrt/runtime.py` & `onnc-bench-4.2.0/onnc/forest/runtimes/tensorrt/runtime.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc/forest/runtimes/tensorrt/utils.py` & `onnc-bench-4.2.0/onnc/forest/runtimes/tensorrt/utils.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/onnc_bench.egg-info/SOURCES.txt` & `onnc-bench-4.2.0/onnc_bench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.1.9/setup.py` & `onnc-bench-4.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,21 +6,35 @@
 # The directory containing this file
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
+
+def load_req(path):
+    with open(path) as f:
+        requirements = f.read().splitlines()
+        # this is a workaround for the fact that pip set doesn't support intuitive whl install
+        for i in range(len(requirements)):
+            if "{CWD}" in requirements[i]:
+                requirements[i] = requirements[i].replace("{CWD}", os.getcwd())
+    return [r for r in requirements if r and r[0] != '#']
+
+
 # This call to setup() does all the work
 setup(name="onnc-bench",
-      version="4.1.9",
+      version="4.2.0",
       description="ONNC-bench is a Python wrapper of ONNC",
       long_description=README,
       long_description_content_type="text/markdown",
       url="https://www.skymizer.com",
       author="The Skymizer Team",
       author_email="hello@skymizer.com",
       license="Apache License 2.0",
       packages=find_packages(),
       package_data={"onnc": ["*"]},
       data_files=[],
-      install_requires=["requests", "numpy", "onnx", "loguru", "sentry-sdk", "packaging"])
+      install_requires=[
+          "requests", "numpy", "onnx", "loguru",
+          "sentry-sdk", "packaging"] + load_req("requirements.txt")
+)
```

