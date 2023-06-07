# Comparing `tmp/MCPoly-0.4.2.tar.gz` & `tmp/MCPoly-0.4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCPoly-0.4.2.tar", last modified: Wed Jun  7 15:03:58 2023, max compression
+gzip compressed data, was "MCPoly-0.4.2.1.tar", last modified: Wed Jun  7 15:30:07 2023, max compression
```

## Comparing `MCPoly-0.4.2.tar` & `MCPoly-0.4.2.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:03:58.886447 MCPoly-0.4.2/
--rw-r--r--   0 cxs454     (503) staff       (20)     1091 2023-05-03 15:22:57.000000 MCPoly-0.4.2/LICENSE
--rw-r--r--   0 cxs454     (503) staff       (20)       17 2023-05-04 08:23:11.000000 MCPoly-0.4.2/MANIFEST.in
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:03:58.871466 MCPoly-0.4.2/MCPoly/
--rw-r--r--   0 cxs454     (503) staff       (20)    14340 2023-06-02 15:40:28.000000 MCPoly-0.4.2/MCPoly/.DS_Store
--rw-r--r--   0 cxs454     (503) staff       (20)      178 2023-05-15 14:05:30.000000 MCPoly-0.4.2/MCPoly/__init__.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:03:58.874558 MCPoly-0.4.2/MCPoly/lmpset/
--rw-r--r--   0 cxs454     (503) staff       (20)     5763 2023-06-02 15:38:19.000000 MCPoly-0.4.2/MCPoly/lmpset/DATAtoXYZ.py
--rw-r--r--   0 cxs454     (503) staff       (20)     4361 2023-06-03 16:09:18.000000 MCPoly-0.4.2/MCPoly/lmpset/DATAtomolTXT.py
--rw-r--r--   0 cxs454     (503) staff       (20)      146 2023-06-03 14:29:24.000000 MCPoly-0.4.2/MCPoly/lmpset/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    55548 2023-06-05 13:00:53.000000 MCPoly-0.4.2/MCPoly/lmpset/chain.py
--rw-r--r--   0 cxs454     (503) staff       (20)    16310 2023-06-03 14:28:50.000000 MCPoly-0.4.2/MCPoly/lmpset/infchain.py
--rw-r--r--   0 cxs454     (503) staff       (20)    50843 2023-06-05 13:01:56.000000 MCPoly-0.4.2/MCPoly/lmpset/mould.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:03:58.877248 MCPoly-0.4.2/MCPoly/moldraw/
--rw-r--r--   0 cxs454     (503) staff       (20)     8966 2023-05-26 12:59:21.000000 MCPoly-0.4.2/MCPoly/moldraw/C_selection.py
--rw-r--r--   0 cxs454     (503) staff       (20)      128 2023-05-29 06:59:26.000000 MCPoly-0.4.2/MCPoly/moldraw/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    64145 2023-05-26 10:41:02.000000 MCPoly-0.4.2/MCPoly/moldraw/bind_selection.py
--rw-r--r--   0 cxs454     (503) staff       (20)    24385 2023-05-29 07:03:41.000000 MCPoly-0.4.2/MCPoly/moldraw/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)   181892 2023-05-26 12:59:34.000000 MCPoly-0.4.2/MCPoly/moldraw/molecule.py
--rw-r--r--   0 cxs454     (503) staff       (20)    98156 2023-05-26 10:40:13.000000 MCPoly-0.4.2/MCPoly/moldraw/sub_selection.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:03:58.879877 MCPoly-0.4.2/MCPoly/orcaset/
--rw-r--r--   0 cxs454     (503) staff       (20)     8635 2023-05-02 16:35:59.000000 MCPoly-0.4.2/MCPoly/orcaset/XYZtoINP.py
--rw-r--r--   0 cxs454     (503) staff       (20)      158 2023-05-11 15:49:25.000000 MCPoly-0.4.2/MCPoly/orcaset/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    16705 2023-06-07 15:01:10.000000 MCPoly-0.4.2/MCPoly/orcaset/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     7592 2023-06-07 15:00:39.000000 MCPoly-0.4.2/MCPoly/orcaset/mgui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     4842 2023-05-02 16:29:09.000000 MCPoly-0.4.2/MCPoly/orcaset/multiorca.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2072 2023-05-15 15:20:42.000000 MCPoly-0.4.2/MCPoly/orcaset/orca.py
--rw-r--r--   0 cxs454     (503) staff       (20)    18040 2023-06-07 15:00:14.000000 MCPoly-0.4.2/MCPoly/orcaset/ssgui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     8784 2023-05-11 15:46:31.000000 MCPoly-0.4.2/MCPoly/orcaset/ssorca.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2145 2023-05-09 08:28:02.000000 MCPoly-0.4.2/MCPoly/orcaset/view3dchoose.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:03:58.881344 MCPoly-0.4.2/MCPoly/sscurve/
--rw-r--r--   0 cxs454     (503) staff       (20)     1193 2023-05-02 16:03:26.000000 MCPoly-0.4.2/MCPoly/sscurve/YModulus.py
--rw-r--r--   0 cxs454     (503) staff       (20)       88 2023-05-09 08:48:45.000000 MCPoly-0.4.2/MCPoly/sscurve/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    12770 2023-05-17 15:37:43.000000 MCPoly-0.4.2/MCPoly/sscurve/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5843 2023-05-19 09:04:58.000000 MCPoly-0.4.2/MCPoly/sscurve/multiple.py
--rw-r--r--   0 cxs454     (503) staff       (20)     6832 2023-05-19 08:52:37.000000 MCPoly-0.4.2/MCPoly/sscurve/single.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:03:58.882577 MCPoly-0.4.2/MCPoly/status/
--rw-r--r--   0 cxs454     (503) staff       (20)       62 2023-05-18 16:46:40.000000 MCPoly-0.4.2/MCPoly/status/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     6202 2023-05-22 09:10:31.000000 MCPoly-0.4.2/MCPoly/status/echart.py
--rw-r--r--   0 cxs454     (503) staff       (20)    15750 2023-05-18 16:45:20.000000 MCPoly-0.4.2/MCPoly/status/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)    20682 2023-06-04 14:28:30.000000 MCPoly-0.4.2/MCPoly/status/status.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:03:58.883389 MCPoly-0.4.2/MCPoly/version/
--rw-r--r--   0 cxs454     (503) staff       (20)       23 2023-05-04 08:03:54.000000 MCPoly-0.4.2/MCPoly/version/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)       33 2023-06-07 14:58:53.000000 MCPoly-0.4.2/MCPoly/version/version.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:03:58.883773 MCPoly-0.4.2/MCPoly/view3d/
--rw-r--r--   0 cxs454     (503) staff       (20)       22 2023-04-30 18:16:37.000000 MCPoly-0.4.2/MCPoly/view3d/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     1970 2023-05-09 13:30:17.000000 MCPoly-0.4.2/MCPoly/view3d/view3d.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:03:58.884346 MCPoly-0.4.2/MCPoly/vis/
--rw-r--r--   0 cxs454     (503) staff       (20)       18 2023-05-15 14:05:55.000000 MCPoly-0.4.2/MCPoly/vis/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2071 2023-05-29 07:04:54.000000 MCPoly-0.4.2/MCPoly/vis/vis.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:03:58.872362 MCPoly-0.4.2/MCPoly.egg-info/
--rw-r--r--   0 cxs454     (503) staff       (20)     3577 2023-06-07 15:03:58.000000 MCPoly-0.4.2/MCPoly.egg-info/PKG-INFO
--rw-r--r--   0 cxs454     (503) staff       (20)     1254 2023-06-07 15:03:58.000000 MCPoly-0.4.2/MCPoly.egg-info/SOURCES.txt
--rw-r--r--   0 cxs454     (503) staff       (20)        1 2023-06-07 15:03:58.000000 MCPoly-0.4.2/MCPoly.egg-info/dependency_links.txt
--rw-r--r--   0 cxs454     (503) staff       (20)      143 2023-06-07 15:03:58.000000 MCPoly-0.4.2/MCPoly.egg-info/requires.txt
--rw-r--r--   0 cxs454     (503) staff       (20)        7 2023-06-07 15:03:58.000000 MCPoly-0.4.2/MCPoly.egg-info/top_level.txt
--rw-r--r--   0 cxs454     (503) staff       (20)     3577 2023-06-07 15:03:58.886266 MCPoly-0.4.2/PKG-INFO
--rw-r--r--   0 cxs454     (503) staff       (20)     3215 2023-05-29 11:10:40.000000 MCPoly-0.4.2/README.md
--rw-r--r--   0 cxs454     (503) staff       (20)       38 2023-06-07 15:03:58.886496 MCPoly-0.4.2/setup.cfg
--rw-r--r--   0 cxs454     (503) staff       (20)     1031 2023-06-07 14:58:41.000000 MCPoly-0.4.2/setup.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:03:58.885922 MCPoly-0.4.2/tests/
--rw-r--r--   0 cxs454     (503) staff       (20)     8625 2023-06-05 10:40:35.000000 MCPoly-0.4.2/tests/test_lmpset.py
--rw-r--r--   0 cxs454     (503) staff       (20)      799 2023-05-03 10:12:20.000000 MCPoly-0.4.2/tests/test_moldraw.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2932 2023-05-02 17:01:47.000000 MCPoly-0.4.2/tests/test_orcaset.py
--rw-r--r--   0 cxs454     (503) staff       (20)     3535 2023-05-19 13:19:19.000000 MCPoly-0.4.2/tests/test_sscurve.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5241 2023-06-05 08:11:04.000000 MCPoly-0.4.2/tests/test_status.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:30:07.708693 MCPoly-0.4.2.1/
+-rw-r--r--   0 cxs454     (503) staff       (20)     1091 2023-05-03 15:22:57.000000 MCPoly-0.4.2.1/LICENSE
+-rw-r--r--   0 cxs454     (503) staff       (20)       17 2023-05-04 08:23:11.000000 MCPoly-0.4.2.1/MANIFEST.in
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:30:07.701411 MCPoly-0.4.2.1/MCPoly/
+-rw-r--r--   0 cxs454     (503) staff       (20)    14340 2023-06-02 15:40:28.000000 MCPoly-0.4.2.1/MCPoly/.DS_Store
+-rw-r--r--   0 cxs454     (503) staff       (20)      178 2023-05-15 14:05:30.000000 MCPoly-0.4.2.1/MCPoly/__init__.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:30:07.703049 MCPoly-0.4.2.1/MCPoly/lmpset/
+-rw-r--r--   0 cxs454     (503) staff       (20)     5763 2023-06-02 15:38:19.000000 MCPoly-0.4.2.1/MCPoly/lmpset/DATAtoXYZ.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     4361 2023-06-03 16:09:18.000000 MCPoly-0.4.2.1/MCPoly/lmpset/DATAtomolTXT.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      146 2023-06-03 14:29:24.000000 MCPoly-0.4.2.1/MCPoly/lmpset/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    55548 2023-06-05 13:00:53.000000 MCPoly-0.4.2.1/MCPoly/lmpset/chain.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    16310 2023-06-03 14:28:50.000000 MCPoly-0.4.2.1/MCPoly/lmpset/infchain.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    50843 2023-06-05 13:01:56.000000 MCPoly-0.4.2.1/MCPoly/lmpset/mould.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:30:07.704100 MCPoly-0.4.2.1/MCPoly/moldraw/
+-rw-r--r--   0 cxs454     (503) staff       (20)     8966 2023-05-26 12:59:21.000000 MCPoly-0.4.2.1/MCPoly/moldraw/C_selection.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      128 2023-05-29 06:59:26.000000 MCPoly-0.4.2.1/MCPoly/moldraw/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    64145 2023-05-26 10:41:02.000000 MCPoly-0.4.2.1/MCPoly/moldraw/bind_selection.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    24385 2023-05-29 07:03:41.000000 MCPoly-0.4.2.1/MCPoly/moldraw/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)   181892 2023-05-26 12:59:34.000000 MCPoly-0.4.2.1/MCPoly/moldraw/molecule.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    98156 2023-05-26 10:40:13.000000 MCPoly-0.4.2.1/MCPoly/moldraw/sub_selection.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:30:07.705485 MCPoly-0.4.2.1/MCPoly/orcaset/
+-rw-r--r--   0 cxs454     (503) staff       (20)     8635 2023-05-02 16:35:59.000000 MCPoly-0.4.2.1/MCPoly/orcaset/XYZtoINP.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      158 2023-05-11 15:49:25.000000 MCPoly-0.4.2.1/MCPoly/orcaset/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    16705 2023-06-07 15:01:10.000000 MCPoly-0.4.2.1/MCPoly/orcaset/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     7592 2023-06-07 15:00:39.000000 MCPoly-0.4.2.1/MCPoly/orcaset/mgui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     4842 2023-05-02 16:29:09.000000 MCPoly-0.4.2.1/MCPoly/orcaset/multiorca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2072 2023-05-15 15:20:42.000000 MCPoly-0.4.2.1/MCPoly/orcaset/orca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    18040 2023-06-07 15:00:14.000000 MCPoly-0.4.2.1/MCPoly/orcaset/ssgui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     8788 2023-06-07 15:16:11.000000 MCPoly-0.4.2.1/MCPoly/orcaset/ssorca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2145 2023-05-09 08:28:02.000000 MCPoly-0.4.2.1/MCPoly/orcaset/view3dchoose.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:30:07.706195 MCPoly-0.4.2.1/MCPoly/sscurve/
+-rw-r--r--   0 cxs454     (503) staff       (20)     1193 2023-05-02 16:03:26.000000 MCPoly-0.4.2.1/MCPoly/sscurve/YModulus.py
+-rw-r--r--   0 cxs454     (503) staff       (20)       88 2023-05-09 08:48:45.000000 MCPoly-0.4.2.1/MCPoly/sscurve/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    12770 2023-05-17 15:37:43.000000 MCPoly-0.4.2.1/MCPoly/sscurve/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5843 2023-05-19 09:04:58.000000 MCPoly-0.4.2.1/MCPoly/sscurve/multiple.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     6832 2023-05-19 08:52:37.000000 MCPoly-0.4.2.1/MCPoly/sscurve/single.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:30:07.706754 MCPoly-0.4.2.1/MCPoly/status/
+-rw-r--r--   0 cxs454     (503) staff       (20)       62 2023-05-18 16:46:40.000000 MCPoly-0.4.2.1/MCPoly/status/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     6202 2023-05-22 09:10:31.000000 MCPoly-0.4.2.1/MCPoly/status/echart.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    15750 2023-05-18 16:45:20.000000 MCPoly-0.4.2.1/MCPoly/status/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    20682 2023-06-04 14:28:30.000000 MCPoly-0.4.2.1/MCPoly/status/status.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:30:07.707066 MCPoly-0.4.2.1/MCPoly/version/
+-rw-r--r--   0 cxs454     (503) staff       (20)       23 2023-05-04 08:03:54.000000 MCPoly-0.4.2.1/MCPoly/version/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)       35 2023-06-07 15:20:08.000000 MCPoly-0.4.2.1/MCPoly/version/version.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:30:07.707345 MCPoly-0.4.2.1/MCPoly/view3d/
+-rw-r--r--   0 cxs454     (503) staff       (20)       22 2023-04-30 18:16:37.000000 MCPoly-0.4.2.1/MCPoly/view3d/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     1970 2023-05-09 13:30:17.000000 MCPoly-0.4.2.1/MCPoly/view3d/view3d.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:30:07.707625 MCPoly-0.4.2.1/MCPoly/vis/
+-rw-r--r--   0 cxs454     (503) staff       (20)       18 2023-05-15 14:05:55.000000 MCPoly-0.4.2.1/MCPoly/vis/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2071 2023-05-29 07:04:54.000000 MCPoly-0.4.2.1/MCPoly/vis/vis.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:30:07.702136 MCPoly-0.4.2.1/MCPoly.egg-info/
+-rw-r--r--   0 cxs454     (503) staff       (20)     3620 2023-06-07 15:30:07.000000 MCPoly-0.4.2.1/MCPoly.egg-info/PKG-INFO
+-rw-r--r--   0 cxs454     (503) staff       (20)     1254 2023-06-07 15:30:07.000000 MCPoly-0.4.2.1/MCPoly.egg-info/SOURCES.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)        1 2023-06-07 15:30:07.000000 MCPoly-0.4.2.1/MCPoly.egg-info/dependency_links.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)      143 2023-06-07 15:30:07.000000 MCPoly-0.4.2.1/MCPoly.egg-info/requires.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)        7 2023-06-07 15:30:07.000000 MCPoly-0.4.2.1/MCPoly.egg-info/top_level.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)     3620 2023-06-07 15:30:07.708534 MCPoly-0.4.2.1/PKG-INFO
+-rw-r--r--   0 cxs454     (503) staff       (20)     3256 2023-06-07 15:29:45.000000 MCPoly-0.4.2.1/README.md
+-rw-r--r--   0 cxs454     (503) staff       (20)       38 2023-06-07 15:30:07.708742 MCPoly-0.4.2.1/setup.cfg
+-rw-r--r--   0 cxs454     (503) staff       (20)     1033 2023-06-07 15:19:29.000000 MCPoly-0.4.2.1/setup.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-07 15:30:07.708327 MCPoly-0.4.2.1/tests/
+-rw-r--r--   0 cxs454     (503) staff       (20)     8625 2023-06-05 10:40:35.000000 MCPoly-0.4.2.1/tests/test_lmpset.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      799 2023-05-03 10:12:20.000000 MCPoly-0.4.2.1/tests/test_moldraw.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2932 2023-05-02 17:01:47.000000 MCPoly-0.4.2.1/tests/test_orcaset.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     3535 2023-05-19 13:19:19.000000 MCPoly-0.4.2.1/tests/test_sscurve.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5241 2023-06-05 08:11:04.000000 MCPoly-0.4.2.1/tests/test_status.py
```

### Comparing `MCPoly-0.4.2/LICENSE` & `MCPoly-0.4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/.DS_Store` & `MCPoly-0.4.2.1/MCPoly/.DS_Store`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/lmpset/DATAtoXYZ.py` & `MCPoly-0.4.2.1/MCPoly/lmpset/DATAtoXYZ.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/lmpset/DATAtomolTXT.py` & `MCPoly-0.4.2.1/MCPoly/lmpset/DATAtomolTXT.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/lmpset/chain.py` & `MCPoly-0.4.2.1/MCPoly/lmpset/chain.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/lmpset/infchain.py` & `MCPoly-0.4.2.1/MCPoly/lmpset/infchain.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/lmpset/mould.py` & `MCPoly-0.4.2.1/MCPoly/lmpset/mould.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/moldraw/C_selection.py` & `MCPoly-0.4.2.1/MCPoly/moldraw/C_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/moldraw/bind_selection.py` & `MCPoly-0.4.2.1/MCPoly/moldraw/bind_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/moldraw/gui.py` & `MCPoly-0.4.2.1/MCPoly/moldraw/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/moldraw/molecule.py` & `MCPoly-0.4.2.1/MCPoly/moldraw/molecule.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/moldraw/sub_selection.py` & `MCPoly-0.4.2.1/MCPoly/moldraw/sub_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/orcaset/XYZtoINP.py` & `MCPoly-0.4.2.1/MCPoly/orcaset/XYZtoINP.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/orcaset/gui.py` & `MCPoly-0.4.2.1/MCPoly/orcaset/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/orcaset/mgui.py` & `MCPoly-0.4.2.1/MCPoly/orcaset/mgui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/orcaset/multiorca.py` & `MCPoly-0.4.2.1/MCPoly/orcaset/multiorca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/orcaset/orca.py` & `MCPoly-0.4.2.1/MCPoly/orcaset/orca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/orcaset/ssgui.py` & `MCPoly-0.4.2.1/MCPoly/orcaset/ssgui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/orcaset/ssorca.py` & `MCPoly-0.4.2.1/MCPoly/orcaset/ssorca.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             Program Completed.[Tue Apr 25 17:51:31 2023]
             
             The polymer is broken. Programme Completed.[Tue Apr 25 17:51:31 2023]
             [file orca_main/run.cpp, line 73453]: ORCA finished with error return - aborting the run     -> COMMAND LINES
         """
         
         print('File: {0}.xyz'.format(self.file))
-        XYZtoINP(self.file,loc=self.loc,method=method,basis_set=basis_set,opt=True,freq=freq,\
+        XYZtoINP(self.file,fileloc=self.loc,method=method,basis_set=basis_set,opt=True,freq=freq,\
                  external_force=True,aim=aim,strain=strain,maxiter=maxiter,maxcore=maxcore,corenum=corenum,\
                  electron=electron,state=state)
         os.system('cp {0}.inp {0}_0.000.inp'.format(self.file))
         keys=[]
         for key in forcestep:
             keys.append(key)
         keys.reverse()
```

### Comparing `MCPoly-0.4.2/MCPoly/orcaset/view3dchoose.py` & `MCPoly-0.4.2.1/MCPoly/orcaset/view3dchoose.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/sscurve/YModulus.py` & `MCPoly-0.4.2.1/MCPoly/sscurve/YModulus.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/sscurve/gui.py` & `MCPoly-0.4.2.1/MCPoly/sscurve/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/sscurve/multiple.py` & `MCPoly-0.4.2.1/MCPoly/sscurve/multiple.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/sscurve/single.py` & `MCPoly-0.4.2.1/MCPoly/sscurve/single.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/status/echart.py` & `MCPoly-0.4.2.1/MCPoly/status/echart.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/status/gui.py` & `MCPoly-0.4.2.1/MCPoly/status/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/status/status.py` & `MCPoly-0.4.2.1/MCPoly/status/status.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/view3d/view3d.py` & `MCPoly-0.4.2.1/MCPoly/view3d/view3d.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly/vis/vis.py` & `MCPoly-0.4.2.1/MCPoly/vis/vis.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/MCPoly.egg-info/PKG-INFO` & `MCPoly-0.4.2.1/MCPoly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCPoly
-Version: 0.4.2
+Version: 0.4.2.1
 Summary: Useful tools for Computational Chemistry for polymers
 Home-page: https://github.com/Omicron-Fluor/MCPoly/
 Author: Omicron Fluor
 Author-email: cxs454@student.bham.ac.uk
 License: MIT
 Keywords: ORCA,Mechanical Property,Computational Chemistry
 Description-Content-Type: text/markdown
@@ -13,18 +13,19 @@
 # MCPoly
 Some methods to deal with some manipulation of computational chemistry, mostly about mechanical properties of polymers.
 ![](./reference/function.png)
 
 ## Overview
 `MCPoly` is a Python library to make some steps of computational chemistry easier. It includes some functions of drawing molecule structures, creating proper .xyz , .inp , .mol and .data file, which specialised for using ORCA and LAMMPS, and some functions for researching the mechanical property of some polymers.
 
-## Updated in v0.4.1.2(29.05.23)
+## Updated in v0.4.2.1(07.06.23)
 1. BIG UPDATE: Molecule Designer GUI is included in this package. You can now use it to draw molecule with 3D view at the same time.
 <img src="https://github.com/Omicron-Fluor/MCPoly/blob/main/reference/moldraw_gui.png">
 2. Add 'chain' in 'lmpset' package. You can now use it to convert periodic polymer structure input data now.
+3. Fix some bugs about ORCA Calculations
 
 ## Updated in v0.3.0 (19.05.23)
 1. BIG UPDATE: Now status package can be used to see energy and gibbs free energy by .energy and .gibbs.
 2. BIG UPDATE: The new Reaction Diagram GUI is included in this package. You can use it to merge some tables and sea the relevant reaction diagram as a reference.
 <img src="https://github.com/Omicron-Fluor/MCPoly/blob/main/reference/status_gui.png">
 3. Fix some bugs about availability of Stress-Strain Curve Output.
```

### Comparing `MCPoly-0.4.2/MCPoly.egg-info/SOURCES.txt` & `MCPoly-0.4.2.1/MCPoly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/PKG-INFO` & `MCPoly-0.4.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCPoly
-Version: 0.4.2
+Version: 0.4.2.1
 Summary: Useful tools for Computational Chemistry for polymers
 Home-page: https://github.com/Omicron-Fluor/MCPoly/
 Author: Omicron Fluor
 Author-email: cxs454@student.bham.ac.uk
 License: MIT
 Keywords: ORCA,Mechanical Property,Computational Chemistry
 Description-Content-Type: text/markdown
@@ -13,18 +13,19 @@
 # MCPoly
 Some methods to deal with some manipulation of computational chemistry, mostly about mechanical properties of polymers.
 ![](./reference/function.png)
 
 ## Overview
 `MCPoly` is a Python library to make some steps of computational chemistry easier. It includes some functions of drawing molecule structures, creating proper .xyz , .inp , .mol and .data file, which specialised for using ORCA and LAMMPS, and some functions for researching the mechanical property of some polymers.
 
-## Updated in v0.4.1.2(29.05.23)
+## Updated in v0.4.2.1(07.06.23)
 1. BIG UPDATE: Molecule Designer GUI is included in this package. You can now use it to draw molecule with 3D view at the same time.
 <img src="https://github.com/Omicron-Fluor/MCPoly/blob/main/reference/moldraw_gui.png">
 2. Add 'chain' in 'lmpset' package. You can now use it to convert periodic polymer structure input data now.
+3. Fix some bugs about ORCA Calculations
 
 ## Updated in v0.3.0 (19.05.23)
 1. BIG UPDATE: Now status package can be used to see energy and gibbs free energy by .energy and .gibbs.
 2. BIG UPDATE: The new Reaction Diagram GUI is included in this package. You can use it to merge some tables and sea the relevant reaction diagram as a reference.
 <img src="https://github.com/Omicron-Fluor/MCPoly/blob/main/reference/status_gui.png">
 3. Fix some bugs about availability of Stress-Strain Curve Output.
```

### Comparing `MCPoly-0.4.2/README.md` & `MCPoly-0.4.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # MCPoly
 Some methods to deal with some manipulation of computational chemistry, mostly about mechanical properties of polymers.
 ![](./reference/function.png)
 
 ## Overview
 `MCPoly` is a Python library to make some steps of computational chemistry easier. It includes some functions of drawing molecule structures, creating proper .xyz , .inp , .mol and .data file, which specialised for using ORCA and LAMMPS, and some functions for researching the mechanical property of some polymers.
 
-## Updated in v0.4.1.2(29.05.23)
+## Updated in v0.4.2.1(07.06.23)
 1. BIG UPDATE: Molecule Designer GUI is included in this package. You can now use it to draw molecule with 3D view at the same time.
 <img src="https://github.com/Omicron-Fluor/MCPoly/blob/main/reference/moldraw_gui.png">
 2. Add 'chain' in 'lmpset' package. You can now use it to convert periodic polymer structure input data now.
+3. Fix some bugs about ORCA Calculations
 
 ## Updated in v0.3.0 (19.05.23)
 1. BIG UPDATE: Now status package can be used to see energy and gibbs free energy by .energy and .gibbs.
 2. BIG UPDATE: The new Reaction Diagram GUI is included in this package. You can use it to merge some tables and sea the relevant reaction diagram as a reference.
 <img src="https://github.com/Omicron-Fluor/MCPoly/blob/main/reference/status_gui.png">
 3. Fix some bugs about availability of Stress-Strain Curve Output.
```

### Comparing `MCPoly-0.4.2/setup.py` & `MCPoly-0.4.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='MCPoly',
-    version='0.4.2',
+    version='0.4.2.1',
     description='Useful tools for Computational Chemistry for polymers',
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=['MCPoly','MCPoly.lmpset','MCPoly.moldraw','MCPoly.orcaset','MCPoly.sscurve','MCPoly.status','MCPoly.view3d','MCPoly.version','MCPoly.vis'],
     author='Omicron Fluor',
     author_email='cxs454@student.bham.ac.uk',
```

### Comparing `MCPoly-0.4.2/tests/test_lmpset.py` & `MCPoly-0.4.2.1/tests/test_lmpset.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/tests/test_moldraw.py` & `MCPoly-0.4.2.1/tests/test_moldraw.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/tests/test_orcaset.py` & `MCPoly-0.4.2.1/tests/test_orcaset.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/tests/test_sscurve.py` & `MCPoly-0.4.2.1/tests/test_sscurve.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2/tests/test_status.py` & `MCPoly-0.4.2.1/tests/test_status.py`

 * *Files identical despite different names*

