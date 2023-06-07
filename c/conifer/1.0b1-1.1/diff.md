# Comparing `tmp/conifer-1.0b1.tar.gz` & `tmp/conifer-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conifer-1.0b1.tar", last modified: Mon Apr  3 10:50:48 2023, max compression
+gzip compressed data, was "conifer-1.1.tar", last modified: Wed Jun  7 14:16:15 2023, max compression
```

## Comparing `conifer-1.0b1.tar` & `conifer-1.1.tar`

### file list

```diff
@@ -1,105 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.923896 conifer-1.0b1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.903896 conifer-1.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.911896 conifer-1.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-03 10:50:33.000000 conifer-1.0b1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-03 10:50:33.000000 conifer-1.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-03 10:50:33.000000 conifer-1.0b1/Jenkinsfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 10:50:33.000000 conifer-1.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-03 10:50:33.000000 conifer-1.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-03 10:50:48.923896 conifer-1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-03 10:50:33.000000 conifer-1.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.911896 conifer-1.0b1/conifer/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.911896 conifer-1.0b1/conifer/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.911896 conifer-1.0b1/conifer/backends/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/cpp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.911896 conifer-1.0b1/conifer/backends/cpp/include/
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/cpp/include/conifer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.911896 conifer-1.0b1/conifer/backends/cpp/template/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/cpp/template/bridge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/cpp/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.911896 conifer-1.0b1/conifer/backends/vhdl/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.915896 conifer-1.0b1/conifer/backends/vhdl/firmware/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/firmware/AddReduce.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/firmware/BDT.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/firmware/BDTTestbench.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/firmware/BDTTop.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/firmware/Constants.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/firmware/SimulationInput.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/firmware/SimulationOutput.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/firmware/TestUtil.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/firmware/Tree.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/firmware/Types.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.915896 conifer-1.0b1/conifer/backends/vhdl/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/scripts/ghdl_compile.sh
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/scripts/modelsim_compile.sh
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/scripts/synth.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/scripts/xsim_compile.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/simulators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/vhdl/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.915896 conifer-1.0b1/conifer/backends/xilinxhls/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/xilinxhls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.915896 conifer-1.0b1/conifer/backends/xilinxhls/firmware/
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/xilinxhls/firmware/BDT_rolled.h
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/xilinxhls/firmware/BDT_unrolled.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.919896 conifer-1.0b1/conifer/backends/xilinxhls/hls-template/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/xilinxhls/hls-template/bridge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/xilinxhls/hls-template/build_prj.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.919896 conifer-1.0b1/conifer/backends/xilinxhls/hls-template/firmware/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/xilinxhls/hls-template/firmware/BDT_rolled.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/xilinxhls/hls-template/firmware/BDT_unrolled.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/xilinxhls/hls-template/firmware/myproject.h
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/xilinxhls/hls-template/myproject_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22013 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/backends/xilinxhls/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.919896 conifer-1.0b1/conifer/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/converters/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/converters/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/converters/tf_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/converters/tmva.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/converters/xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.919896 conifer-1.0b1/conifer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/utils/fixed_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/utils/fixed_point_conversions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.911896 conifer-1.0b1/conifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-03 10:50:48.000000 conifer-1.0b1/conifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-03 10:50:48.000000 conifer-1.0b1/conifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 10:50:48.000000 conifer-1.0b1/conifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-03 10:50:48.000000 conifer-1.0b1/conifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-03 10:50:48.000000 conifer-1.0b1/conifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    28385 2023-04-03 10:50:33.000000 conifer-1.0b1/conifer_v1.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.907896 conifer-1.0b1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.919896 conifer-1.0b1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-03 10:50:33.000000 conifer-1.0b1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-03 10:50:33.000000 conifer-1.0b1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.923896 conifer-1.0b1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-03 10:50:33.000000 conifer-1.0b1/examples/pruned_xgboost_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-03 10:50:33.000000 conifer-1.0b1/examples/sklearn_RandomForest.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-03 10:50:33.000000 conifer-1.0b1/examples/sklearn_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-03 10:50:33.000000 conifer-1.0b1/examples/sklearn_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-03 10:50:33.000000 conifer-1.0b1/examples/sklearn_to_cpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-03 10:50:33.000000 conifer-1.0b1/examples/sklearn_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-03 10:50:33.000000 conifer-1.0b1/examples/sklearn_to_vhdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-03 10:50:33.000000 conifer-1.0b1/examples/tf_df_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-03 10:50:33.000000 conifer-1.0b1/examples/tf_df_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-03 10:50:33.000000 conifer-1.0b1/examples/xgboost_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-03 10:50:33.000000 conifer-1.0b1/examples/xgboost_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-03 10:50:33.000000 conifer-1.0b1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 10:50:48.923896 conifer-1.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-03 10:50:33.000000 conifer-1.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 10:50:48.923896 conifer-1.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-03 10:50:33.000000 conifer-1.0b1/tests/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-03 10:50:33.000000 conifer-1.0b1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-03 10:50:33.000000 conifer-1.0b1/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-03 10:50:33.000000 conifer-1.0b1/tests/test_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-03 10:50:33.000000 conifer-1.0b1/tests/test_onnx_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-03 10:50:33.000000 conifer-1.0b1/tests/test_save_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-03 10:50:33.000000 conifer-1.0b1/tests/test_skl_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-03 10:50:33.000000 conifer-1.0b1/tests/test_tf_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-03 10:50:33.000000 conifer-1.0b1/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.667023 conifer-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.635023 conifer-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.639023 conifer-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-07 14:16:04.000000 conifer-1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 14:16:04.000000 conifer-1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 14:16:04.000000 conifer-1.1/Jenkinsfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 14:16:04.000000 conifer-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-07 14:16:04.000000 conifer-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-07 14:16:15.667023 conifer-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-07 14:16:04.000000 conifer-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.643023 conifer-1.1/conifer/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-07 14:16:04.000000 conifer-1.1/conifer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.643023 conifer-1.1/conifer/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.643023 conifer-1.1/conifer/backends/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/cpp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.643023 conifer-1.1/conifer/backends/cpp/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/cpp/include/conifer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.643023 conifer-1.1/conifer/backends/cpp/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/cpp/template/bridge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/cpp/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.647023 conifer-1.1/conifer/backends/fpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.647023 conifer-1.1/conifer/backends/fpu/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/build_bit.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/build_hls.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/changes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/fpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/src/fpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22375 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/fpu/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.647023 conifer-1.1/conifer/backends/vhdl/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.651023 conifer-1.1/conifer/backends/vhdl/firmware/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/AddReduce.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/BDT.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/BDTTestbench.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/BDTTop.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/Constants.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/SimulationInput.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/SimulationOutput.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/TestUtil.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/Tree.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/firmware/Types.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.651023 conifer-1.1/conifer/backends/vhdl/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/scripts/ghdl_compile.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/scripts/modelsim_compile.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/scripts/synth.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/scripts/xsim_compile.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/simulators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/vhdl/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.655023 conifer-1.1/conifer/backends/xilinxhls/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.655023 conifer-1.1/conifer/backends/xilinxhls/firmware/
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/firmware/BDT_rolled.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/firmware/BDT_unrolled.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.655023 conifer-1.1/conifer/backends/xilinxhls/hls-template/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/hls-template/bridge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/hls-template/build_prj.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.655023 conifer-1.1/conifer/backends/xilinxhls/hls-template/firmware/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/hls-template/firmware/BDT_rolled.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/hls-template/firmware/BDT_unrolled.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/hls-template/firmware/myproject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/hls-template/myproject_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22013 2023-06-07 14:16:04.000000 conifer-1.1/conifer/backends/xilinxhls/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.659023 conifer-1.1/conifer/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-07 14:16:04.000000 conifer-1.1/conifer/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-07 14:16:04.000000 conifer-1.1/conifer/converters/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-07 14:16:04.000000 conifer-1.1/conifer/converters/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-06-07 14:16:04.000000 conifer-1.1/conifer/converters/tf_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-07 14:16:04.000000 conifer-1.1/conifer/converters/tmva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-07 14:16:04.000000 conifer-1.1/conifer/converters/xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-06-07 14:16:04.000000 conifer-1.1/conifer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.659023 conifer-1.1/conifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:16:04.000000 conifer-1.1/conifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-07 14:16:04.000000 conifer-1.1/conifer/utils/fixed_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-07 14:16:04.000000 conifer-1.1/conifer/utils/fixed_point_conversions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-07 14:16:04.000000 conifer-1.1/conifer/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.643023 conifer-1.1/conifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-07 14:16:15.000000 conifer-1.1/conifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 14:16:15.000000 conifer-1.1/conifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:16:15.000000 conifer-1.1/conifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 14:16:15.000000 conifer-1.1/conifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 14:16:15.000000 conifer-1.1/conifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    28385 2023-06-07 14:16:04.000000 conifer-1.1/conifer_v1.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.639023 conifer-1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.659023 conifer-1.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-07 14:16:04.000000 conifer-1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-07 14:16:04.000000 conifer-1.1/docs/source/fpu.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-07 14:16:04.000000 conifer-1.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.663023 conifer-1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-07 14:16:04.000000 conifer-1.1/examples/build_fpu_alveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-07 14:16:04.000000 conifer-1.1/examples/build_fpu_pynq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-07 14:16:04.000000 conifer-1.1/examples/pruned_xgboost_to_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_RandomForest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_to_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_to_fpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_to_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-07 14:16:04.000000 conifer-1.1/examples/sklearn_to_vhdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 14:16:04.000000 conifer-1.1/examples/tf_df_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-07 14:16:04.000000 conifer-1.1/examples/tf_df_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-07 14:16:04.000000 conifer-1.1/examples/xgboost_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-07 14:16:04.000000 conifer-1.1/examples/xgboost_to_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:16:04.000000 conifer-1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:16:15.667023 conifer-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-07 14:16:04.000000 conifer-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:16:15.667023 conifer-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 14:16:04.000000 conifer-1.1/tests/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-07 14:16:04.000000 conifer-1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-07 14:16:04.000000 conifer-1.1/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-07 14:16:04.000000 conifer-1.1/tests/test_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-07 14:16:04.000000 conifer-1.1/tests/test_onnx_to_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-07 14:16:04.000000 conifer-1.1/tests/test_save_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 14:16:04.000000 conifer-1.1/tests/test_skl_to_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-07 14:16:04.000000 conifer-1.1/tests/test_tf_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-07 14:16:04.000000 conifer-1.1/tests/util.py
```

### Comparing `conifer-1.0b1/.github/workflows/python-publish.yml` & `conifer-1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/Jenkinsfile` & `conifer-1.1/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/LICENSE` & `conifer-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/__init__.py` & `conifer-1.1/conifer/backends/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 vitishls._tool = 'vitishls'
 SPEC_XILINXHLS.loader.exec_module(vitishls)
 
 del SPEC_XILINXHLS
 
 from conifer.backends import vhdl
 from conifer.backends import cpp
+from conifer.backends import fpu
 
 _backend_map = {'xilinxhls' : xilinxhls,
                 'vivadohls' : vivadohls,
                 'vitishls'  : vitishls,
                 'vhdl'      : vhdl,
-                'cpp'       : cpp}
+                'cpp'       : cpp,
+                'fpu'       : fpu,}
 
 def get_backend(backend):
   '''Get backend object from string'''
   backend_obj = _backend_map.get(backend)
   if backend_obj is None:
     raise RuntimeError(f'No backend "{backend}" found. Options are {[k for k in _backend_map.keys()]}')
   return backend_obj
```

### Comparing `conifer-1.0b1/conifer/backends/common.py` & `conifer-1.1/conifer/backends/common.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/cpp/include/conifer.h` & `conifer-1.1/conifer/backends/cpp/include/conifer.h`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/cpp/writer.py` & `conifer-1.1/conifer/backends/cpp/writer.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/firmware/AddReduce.vhd` & `conifer-1.1/conifer/backends/vhdl/firmware/AddReduce.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/firmware/BDT.vhd` & `conifer-1.1/conifer/backends/vhdl/firmware/BDT.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/firmware/BDTTestbench.vhd` & `conifer-1.1/conifer/backends/vhdl/firmware/BDTTestbench.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/firmware/BDTTop.vhd` & `conifer-1.1/conifer/backends/vhdl/firmware/BDTTop.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/firmware/SimulationInput.vhd` & `conifer-1.1/conifer/backends/vhdl/firmware/SimulationInput.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/firmware/SimulationOutput.vhd` & `conifer-1.1/conifer/backends/vhdl/firmware/SimulationOutput.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/firmware/TestUtil.vhd` & `conifer-1.1/conifer/backends/vhdl/firmware/TestUtil.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/firmware/Tree.vhd` & `conifer-1.1/conifer/backends/vhdl/firmware/Tree.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/firmware/Types.vhd` & `conifer-1.1/conifer/backends/vhdl/firmware/Types.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/scripts/ghdl_compile.sh` & `conifer-1.1/conifer/backends/vhdl/scripts/ghdl_compile.sh`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/scripts/modelsim_compile.sh` & `conifer-1.1/conifer/backends/vhdl/scripts/modelsim_compile.sh`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/simulators.py` & `conifer-1.1/conifer/backends/vhdl/simulators.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/vhdl/writer.py` & `conifer-1.1/conifer/backends/vhdl/writer.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/xilinxhls/firmware/BDT_rolled.h` & `conifer-1.1/conifer/backends/xilinxhls/firmware/BDT_rolled.h`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/xilinxhls/firmware/BDT_unrolled.h` & `conifer-1.1/conifer/backends/xilinxhls/firmware/BDT_unrolled.h`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/xilinxhls/hls-template/bridge.cpp` & `conifer-1.1/conifer/backends/xilinxhls/hls-template/bridge.cpp`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/xilinxhls/hls-template/build_prj.tcl` & `conifer-1.1/conifer/backends/xilinxhls/hls-template/build_prj.tcl`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/xilinxhls/hls-template/myproject_test.cpp` & `conifer-1.1/conifer/backends/xilinxhls/hls-template/myproject_test.cpp`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/backends/xilinxhls/writer.py` & `conifer-1.1/conifer/backends/xilinxhls/writer.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/converters/__init__.py` & `conifer-1.1/conifer/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/converters/onnx.py` & `conifer-1.1/conifer/converters/onnx.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/converters/sklearn.py` & `conifer-1.1/conifer/converters/sklearn.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/converters/tf_df.py` & `conifer-1.1/conifer/converters/tf_df.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/converters/tmva.py` & `conifer-1.1/conifer/converters/tmva.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/converters/xgboost.py` & `conifer-1.1/conifer/converters/xgboost.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/model.py` & `conifer-1.1/conifer/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from conifer import __version__ as version
+from packaging.version import Version
 import numpy as np
 import os
 import json
 import copy
 import datetime
 import platform
 import getpass
@@ -54,15 +55,21 @@
         vals = {}
         for key in self._config_fields:
             vals[key] = getattr(self, key, None)
         assert not (None in vals.values()), f'Missing some required configuration, have: {vals}'
         assert get_backend(self.backend) is not None, f'Backend {self.backend} not found'
 
     def _to_dict(self):
-        dictionary = {k : getattr(self, k) for k in self._config_fields}
+        dictionary = {}
+        for k in self._config_fields:
+            if hasattr(getattr(self, k), '_to_dict'):
+                v = getattr(self, k)._to_dict()
+            else:
+                v = getattr(self, k)
+            dictionary[k] = v
         return dictionary
 
     def _log(self, logger):
         logger.info(f'Configuration: {self._to_dict()}')
 
     def default_config():
         return copy.deepcopy(ConfigBase._defaults)
@@ -210,22 +217,22 @@
     def __init__(self):
         self.version = version
         self.time = datetime.datetime.now()
         self.host = platform.node()
         self.user = getpass.getuser()
 
     def _to_dict(self):
-        return {'version' : self.version,
+        return {'version' : str(self.version),
                 'host'    : self.host,
                 'user'    : self.user,
                 'time'    : self.time.timestamp()}
 
     def _from_dict(d):
         mmd = ModelMetaData()
-        mmd.version = d.get('version', None)
+        mmd.version = Version(d.get('version', None))
         mmd.host = d.get('host', None)
         mmd.user = d.get('user', None)
         mmd.time = datetime.datetime.fromtimestamp(d.get('time', 0))
         return mmd
 
 def make_model(ensembleDict, config):
     from conifer.backends import get_backend
```

### Comparing `conifer-1.0b1/conifer/utils/fixed_point.py` & `conifer-1.1/conifer/utils/fixed_point.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import numpy as np
+from conifer.utils.misc import _ap_include
 import logging
 logger = logging.getLogger(__name__)
 
 class FixedPointConverter:
   '''
   A Python wrapper around ap_fixed types to easily emulate the correct number representations
   '''
@@ -31,15 +32,15 @@
         newline =  f"typedef {type_string} T;\n"
       fout.write(newline)
     fin.close()
     fout.close()
 
     curr_dir = os.getcwd()
     os.chdir(cpp_filedir)
-    cmd = f"g++ -O3 -shared -std=c++11 -fPIC $(python3 -m pybind11 --includes) -I/cvmfs/cms.cern.ch/slc7_amd64_gcc900/external/hls/2019.08/include/ {self.sani_type}.cpp -o {self.sani_type}.so"
+    cmd = f"g++ -O3 -shared -std=c++11 -fPIC $(python3 -m pybind11 --includes) {_ap_include()} {self.sani_type}.cpp -o {self.sani_type}.so"
     logger.debug(f'Compiling with command {cmd}')
     try:
       ret_val = os.system(cmd)
       if ret_val != 0:
         raise Exception(f'Failed to compile FixedPointConverter {self.sani_type}.cpp')
     finally:
       os.chdir(curr_dir)
```

### Comparing `conifer-1.0b1/conifer/utils/fixed_point_conversions.cpp` & `conifer-1.1/conifer/utils/fixed_point_conversions.cpp`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer/utils/misc.py` & `conifer-1.1/conifer/utils/misc.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/conifer.egg-info/SOURCES.txt` & `conifer-1.1/conifer.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,24 @@
 conifer.egg-info/top_level.txt
 conifer/backends/__init__.py
 conifer/backends/common.py
 conifer/backends/cpp/__init__.py
 conifer/backends/cpp/writer.py
 conifer/backends/cpp/include/conifer.h
 conifer/backends/cpp/template/bridge.cpp
+conifer/backends/fpu/__init__.py
+conifer/backends/fpu/runtime.py
+conifer/backends/fpu/writer.py
+conifer/backends/fpu/src/LICENSE
+conifer/backends/fpu/src/README.md
+conifer/backends/fpu/src/build_bit.tcl
+conifer/backends/fpu/src/build_hls.tcl
+conifer/backends/fpu/src/changes.txt
+conifer/backends/fpu/src/fpu.cpp
+conifer/backends/fpu/src/fpu.h
 conifer/backends/vhdl/__init__.py
 conifer/backends/vhdl/simulators.py
 conifer/backends/vhdl/writer.py
 conifer/backends/vhdl/firmware/AddReduce.vhd
 conifer/backends/vhdl/firmware/BDT.vhd
 conifer/backends/vhdl/firmware/BDTTestbench.vhd
 conifer/backends/vhdl/firmware/BDTTop.vhd
@@ -54,20 +64,24 @@
 conifer/converters/tmva.py
 conifer/converters/xgboost.py
 conifer/utils/__init__.py
 conifer/utils/fixed_point.py
 conifer/utils/fixed_point_conversions.cpp
 conifer/utils/misc.py
 docs/source/conf.py
+docs/source/fpu.rst
 docs/source/index.rst
+examples/build_fpu_alveo.py
+examples/build_fpu_pynq.py
 examples/pruned_xgboost_to_hls.py
 examples/sklearn_RandomForest.py
 examples/sklearn_multiclass.py
 examples/sklearn_regression.py
 examples/sklearn_to_cpp.py
+examples/sklearn_to_fpu.py
 examples/sklearn_to_hls.py
 examples/sklearn_to_vhdl.py
 examples/tf_df_binary.py
 examples/tf_df_multiclass.py
 examples/xgboost_multiclass.py
 examples/xgboost_to_hls.py
 tests/cleanup.sh
```

### Comparing `conifer-1.0b1/conifer_v1.png` & `conifer-1.1/conifer_v1.png`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/docs/source/conf.py` & `conifer-1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/examples/pruned_xgboost_to_hls.py` & `conifer-1.1/examples/pruned_xgboost_to_hls.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/examples/sklearn_RandomForest.py` & `conifer-1.1/examples/sklearn_RandomForest.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/examples/sklearn_multiclass.py` & `conifer-1.1/examples/sklearn_multiclass.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/examples/sklearn_regression.py` & `conifer-1.1/examples/sklearn_regression.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/examples/sklearn_to_cpp.py` & `conifer-1.1/examples/sklearn_to_cpp.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/examples/sklearn_to_hls.py` & `conifer-1.1/examples/sklearn_to_hls.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/examples/sklearn_to_vhdl.py` & `conifer-1.1/examples/sklearn_to_vhdl.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/examples/tf_df_binary.py` & `conifer-1.1/examples/tf_df_binary.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/examples/tf_df_multiclass.py` & `conifer-1.1/examples/tf_df_multiclass.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/examples/xgboost_multiclass.py` & `conifer-1.1/examples/xgboost_multiclass.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/examples/xgboost_to_hls.py` & `conifer-1.1/examples/xgboost_to_hls.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/setup.py` & `conifer-1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,10 +18,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     python_requires='>=3.8',
     install_requires=[
         'numpy',
         'pybind11',
+        'packaging',
     ],
     include_package_data=True,
 )
```

### Comparing `conifer-1.0b1/tests/test_backends.py` & `conifer-1.1/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/tests/test_multiclass.py` & `conifer-1.1/tests/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/tests/test_onnx_to_hls.py` & `conifer-1.1/tests/test_onnx_to_hls.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/tests/test_save_load.py` & `conifer-1.1/tests/test_save_load.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/tests/test_tf_df.py` & `conifer-1.1/tests/test_tf_df.py`

 * *Files identical despite different names*

### Comparing `conifer-1.0b1/tests/util.py` & `conifer-1.1/tests/util.py`

 * *Files identical despite different names*

