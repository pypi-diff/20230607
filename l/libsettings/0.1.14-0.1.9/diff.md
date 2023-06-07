# Comparing `tmp/libsettings-0.1.14.tar.gz` & `tmp/libsettings-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsettings-0.1.14.tar", last modified: Wed Jun  7 07:13:04 2023, max compression
+gzip compressed data, was "dist/libsettings-0.1.9.tar", last modified: Tue Feb 19 11:00:47 2019, max compression
```

## Comparing `libsettings-0.1.14.tar` & `libsettings-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:13:04.336077 libsettings-0.1.14/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-07 07:12:35.000000 libsettings-0.1.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-07 07:12:35.000000 libsettings-0.1.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-07 07:13:04.336077 libsettings-0.1.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-07 07:12:35.000000 libsettings-0.1.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:13:04.332077 libsettings-0.1.14/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:13:04.336077 libsettings-0.1.14/include/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/internal/request_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/internal/setting_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/internal/setting_def.h
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/internal/setting_macros.h
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/internal/setting_sbp_cb.h
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/internal/setting_type.h
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/internal/setting_type_enum.h
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/internal/setting_type_float.h
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/internal/setting_type_int.h
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/internal/setting_type_str.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:13:04.336077 libsettings-0.1.14/include/libsettings/
--rw-r--r--   0 runner    (1001) docker     (123)    21424 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/libsettings/settings.h
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/libsettings/settings_declspec.h
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-07 07:12:35.000000 libsettings-0.1.14/include/libsettings/settings_util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:13:04.336077 libsettings-0.1.14/libsettings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-07 07:13:04.000000 libsettings-0.1.14/libsettings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-07 07:13:04.000000 libsettings-0.1.14/libsettings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:13:04.000000 libsettings-0.1.14/libsettings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 07:13:04.000000 libsettings-0.1.14/libsettings.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:13:04.336077 libsettings-0.1.14/python/
--rw-r--r--   0 runner    (1001) docker     (123)   713145 2023-06-07 07:12:57.000000 libsettings-0.1.14/python/libsettings.c
--rw-r--r--   0 runner    (1001) docker     (123)    13482 2023-06-07 07:12:35.000000 libsettings-0.1.14/python/libsettings.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 07:13:04.336077 libsettings-0.1.14/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2188 2023-06-07 07:12:35.000000 libsettings-0.1.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:13:04.336077 libsettings-0.1.14/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-07 07:12:35.000000 libsettings-0.1.14/src/request_state.c
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-06-07 07:12:35.000000 libsettings-0.1.14/src/setting_data.c
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-06-07 07:12:35.000000 libsettings-0.1.14/src/setting_sbp_cb.c
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-07 07:12:35.000000 libsettings-0.1.14/src/setting_type.c
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-07 07:12:35.000000 libsettings-0.1.14/src/setting_type_enum.c
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-07 07:12:35.000000 libsettings-0.1.14/src/setting_type_float.c
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-07 07:12:35.000000 libsettings-0.1.14/src/setting_type_int.c
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-07 07:12:35.000000 libsettings-0.1.14/src/setting_type_str.c
--rw-r--r--   0 runner    (1001) docker     (123)    25348 2023-06-07 07:12:35.000000 libsettings-0.1.14/src/settings.c
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-07 07:12:35.000000 libsettings-0.1.14/src/settings_util.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:13:04.332077 libsettings-0.1.14/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:13:04.332077 libsettings-0.1.14/third_party/libswiftnav/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:13:04.336077 libsettings-0.1.14/third_party/libswiftnav/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-07 07:12:50.000000 libsettings-0.1.14/third_party/libswiftnav/src/logging.c
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-07 07:12:50.000000 libsettings-0.1.14/third_party/libswiftnav/src/logging_common.c
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:47.000000 libsettings-0.1.9/
+-rw-r--r--   0 pasi      (1003) users      (100)    18092 2018-11-30 10:08:33.000000 libsettings-0.1.9/LICENSE
+-rwxr-xr-x   0 pasi      (1003) users      (100)     2263 2019-02-19 11:00:39.000000 libsettings-0.1.9/setup.py
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:46.000000 libsettings-0.1.9/include/
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:46.000000 libsettings-0.1.9/include/internal/
+-rw-r--r--   0 pasi      (1003) users      (100)      864 2019-01-24 07:23:50.000000 libsettings-0.1.9/include/internal/setting_type_str.h
+-rw-r--r--   0 pasi      (1003) users      (100)     1651 2019-02-14 08:28:30.000000 libsettings-0.1.9/include/internal/setting_sbp_cb.h
+-rw-r--r--   0 pasi      (1003) users      (100)      864 2019-01-24 07:23:50.000000 libsettings-0.1.9/include/internal/setting_type_int.h
+-rw-r--r--   0 pasi      (1003) users      (100)     1586 2019-02-05 07:39:20.000000 libsettings-0.1.9/include/internal/request_state.h
+-rw-r--r--   0 pasi      (1003) users      (100)      953 2019-01-24 07:23:50.000000 libsettings-0.1.9/include/internal/setting_type_float.h
+-rw-r--r--   0 pasi      (1003) users      (100)     1449 2019-02-14 08:28:30.000000 libsettings-0.1.9/include/internal/setting_def.h
+-rw-r--r--   0 pasi      (1003) users      (100)     2469 2019-01-24 07:23:50.000000 libsettings-0.1.9/include/internal/setting_type.h
+-rw-r--r--   0 pasi      (1003) users      (100)     4684 2019-02-08 11:38:25.000000 libsettings-0.1.9/include/internal/setting_data.h
+-rw-r--r--   0 pasi      (1003) users      (100)      968 2019-01-24 07:23:50.000000 libsettings-0.1.9/include/internal/setting_type_enum.h
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:46.000000 libsettings-0.1.9/include/libsettings/
+-rw-r--r--   0 pasi      (1003) users      (100)     2815 2019-02-05 07:39:20.000000 libsettings-0.1.9/include/libsettings/settings_util.h
+-rw-r--r--   0 pasi      (1003) users      (100)    21511 2019-02-19 08:43:46.000000 libsettings-0.1.9/include/libsettings/settings.h
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:47.000000 libsettings-0.1.9/src/
+-rw-r--r--   0 pasi      (1003) users      (100)     3043 2019-01-24 07:23:50.000000 libsettings-0.1.9/src/request_state.c
+-rw-r--r--   0 pasi      (1003) users      (100)      945 2019-01-24 07:23:50.000000 libsettings-0.1.9/src/setting_type_str.c
+-rw-r--r--   0 pasi      (1003) users      (100)    27829 2019-02-19 08:43:46.000000 libsettings-0.1.9/src/settings.c
+-rw-r--r--   0 pasi      (1003) users      (100)     1827 2019-01-24 07:23:50.000000 libsettings-0.1.9/src/setting_type_enum.c
+-rw-r--r--   0 pasi      (1003) users      (100)     6848 2019-02-08 11:38:25.000000 libsettings-0.1.9/src/setting_data.c
+-rw-r--r--   0 pasi      (1003) users      (100)     1765 2019-01-16 07:59:11.000000 libsettings-0.1.9/src/setting_type.c
+-rw-r--r--   0 pasi      (1003) users      (100)     1469 2019-01-24 07:23:50.000000 libsettings-0.1.9/src/setting_type_int.c
+-rw-r--r--   0 pasi      (1003) users      (100)     2260 2019-02-05 07:39:20.000000 libsettings-0.1.9/src/settings_util.c
+-rw-r--r--   0 pasi      (1003) users      (100)    12384 2019-02-13 09:09:28.000000 libsettings-0.1.9/src/setting_sbp_cb.c
+-rw-r--r--   0 pasi      (1003) users      (100)     1174 2019-01-24 07:23:50.000000 libsettings-0.1.9/src/setting_type_float.c
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:47.000000 libsettings-0.1.9/python/
+-rw-r--r--   0 pasi      (1003) users      (100)   589030 2019-02-19 08:52:23.000000 libsettings-0.1.9/python/libsettings.c
+-rw-r--r--   0 pasi      (1003) users      (100)    10248 2019-02-13 09:09:28.000000 libsettings-0.1.9/python/libsettings.pyx
+-rw-r--r--   0 pasi      (1003) users      (100)        7 2019-02-05 09:12:05.000000 libsettings-0.1.9/requirements-unix.txt
+-rw-r--r--   0 pasi      (1003) users      (100)       20 2019-02-05 09:12:05.000000 libsettings-0.1.9/requirements-win-cp35-cp36-cp37.txt
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:47.000000 libsettings-0.1.9/libsettings.egg-info/
+-rw-r--r--   0 pasi      (1003) users      (100)        1 2019-02-19 11:00:46.000000 libsettings-0.1.9/libsettings.egg-info/dependency_links.txt
+-rw-r--r--   0 pasi      (1003) users      (100)       12 2019-02-19 11:00:46.000000 libsettings-0.1.9/libsettings.egg-info/top_level.txt
+-rw-r--r--   0 pasi      (1003) users      (100)      946 2019-02-19 11:00:46.000000 libsettings-0.1.9/libsettings.egg-info/PKG-INFO
+-rw-r--r--   0 pasi      (1003) users      (100)     1896 2019-02-19 11:00:46.000000 libsettings-0.1.9/libsettings.egg-info/SOURCES.txt
+-rw-r--r--   0 pasi      (1003) users      (100)       83 2019-02-05 09:12:05.000000 libsettings-0.1.9/requirements-win-cp27-cp34.txt
+-rw-r--r--   0 pasi      (1003) users      (100)      946 2019-02-19 11:00:47.000000 libsettings-0.1.9/PKG-INFO
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:46.000000 libsettings-0.1.9/libswiftnav/
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:46.000000 libsettings-0.1.9/libswiftnav/include/
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:47.000000 libsettings-0.1.9/libswiftnav/include/swiftnav/
+-rw-r--r--   0 pasi      (1003) users      (100)    10813 2019-02-15 07:15:18.000000 libsettings-0.1.9/libswiftnav/include/swiftnav/logging.h
+-rw-r--r--   0 pasi      (1003) users      (100)     2169 2019-02-15 07:15:18.000000 libsettings-0.1.9/libswiftnav/include/swiftnav/common.h
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:47.000000 libsettings-0.1.9/libswiftnav/src/
+-rw-r--r--   0 pasi      (1003) users      (100)     2090 2019-02-15 07:15:18.000000 libsettings-0.1.9/libswiftnav/src/logging.c
+-rw-r--r--   0 pasi      (1003) users      (100)     1339 2019-02-15 07:15:18.000000 libsettings-0.1.9/libswiftnav/src/logging_common.c
+-rw-r--r--   0 pasi      (1003) users      (100)      306 2019-02-19 10:15:46.000000 libsettings-0.1.9/MANIFEST.in
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:46.000000 libsettings-0.1.9/libsbp/
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:46.000000 libsettings-0.1.9/libsbp/c/
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:46.000000 libsettings-0.1.9/libsbp/c/include/
+drwxr-xr-x   0 pasi      (1003) users      (100)        0 2019-02-19 11:00:47.000000 libsettings-0.1.9/libsbp/c/include/libsbp/
+-rw-r--r--   0 pasi      (1003) users      (100)     1022 2019-02-08 06:58:45.000000 libsettings-0.1.9/libsbp/c/include/libsbp/version.h
+-rw-r--r--   0 pasi      (1003) users      (100)     2240 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/ndb.h
+-rw-r--r--   0 pasi      (1003) users      (100)     6313 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/file_io.h
+-rw-r--r--   0 pasi      (1003) users      (100)     9419 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/tracking.h
+-rw-r--r--   0 pasi      (1003) users      (100)     1546 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/sbas.h
+-rw-r--r--   0 pasi      (1003) users      (100)     3449 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/gnss.h
+-rw-r--r--   0 pasi      (1003) users      (100)     1701 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/ext_events.h
+-rw-r--r--   0 pasi      (1003) users      (100)     4179 2019-02-05 09:08:14.000000 libsettings-0.1.9/libsbp/c/include/libsbp/system.h
+-rw-r--r--   0 pasi      (1003) users      (100)     7638 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/ssr.h
+-rw-r--r--   0 pasi      (1003) users      (100)     7172 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/linux.h
+-rw-r--r--   0 pasi      (1003) users      (100)      697 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/edc.h
+-rw-r--r--   0 pasi      (1003) users      (100)     1879 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/vehicle.h
+-rw-r--r--   0 pasi      (1003) users      (100)     6535 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/flash.h
+-rw-r--r--   0 pasi      (1003) users      (100)     5057 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/orientation.h
+-rw-r--r--   0 pasi      (1003) users      (100)    25720 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/navigation.h
+-rw-r--r--   0 pasi      (1003) users      (100)    50537 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/observation.h
+-rw-r--r--   0 pasi      (1003) users      (100)     2429 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/imu.h
+-rw-r--r--   0 pasi      (1003) users      (100)     3703 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/bootload.h
+-rw-r--r--   0 pasi      (1003) users      (100)     5852 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/acquisition.h
+-rw-r--r--   0 pasi      (1003) users      (100)     3426 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/sbp.h
+-rw-r--r--   0 pasi      (1003) users      (100)     2553 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/logging.h
+-rw-r--r--   0 pasi      (1003) users      (100)     1582 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/mag.h
+-rw-r--r--   0 pasi      (1003) users      (100)    15146 2019-02-05 09:08:14.000000 libsettings-0.1.9/libsbp/c/include/libsbp/piksi.h
+-rw-r--r--   0 pasi      (1003) users      (100)     1268 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/user.h
+-rw-r--r--   0 pasi      (1003) users      (100)     8726 2019-02-05 09:08:14.000000 libsettings-0.1.9/libsbp/c/include/libsbp/settings.h
+-rw-r--r--   0 pasi      (1003) users      (100)     2104 2018-11-21 08:02:28.000000 libsettings-0.1.9/libsbp/c/include/libsbp/common.h
+-rw-r--r--   0 pasi      (1003) users      (100)       38 2019-02-19 11:00:47.000000 libsettings-0.1.9/setup.cfg
+-rw-r--r--   0 pasi      (1003) users      (100)     3533 2019-02-08 11:38:25.000000 libsettings-0.1.9/README.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `libsettings-0.1.14/LICENSE` & `libsettings-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `libsettings-0.1.14/PKG-INFO` & `libsettings-0.1.9/libsettings.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: libsettings
-Version: 0.1.14
+Version: 0.1.9
 Summary: Open source SwiftNav settings API library.
 Home-page: https://github.com/swift-nav/libsettings
 Author: Swift Navigation
 Author-email: dev@swift-nav.com
+License: UNKNOWN
+Description: UNKNOWN
 Platform: linux
 Platform: osx
 Platform: win32
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE
```

### Comparing `libsettings-0.1.14/include/internal/setting_data.h` & `libsettings-0.1.9/include/internal/setting_data.h`

 * *Files 5% similar despite different names*

```diff
@@ -51,76 +51,81 @@
  * @param type: type identifier
  * @param notify: optional notification callback
  * @param notify_context: optional data reference to pass during notification
  * @param readonly: set to true to disable value updates
  * @param watchonly: set to true to indicate a non-owned setting watch
  * @return the newly created setting, NULL if failed
  */
-setting_data_t *setting_data_create(type_data_t *type_list, const char *section,
-                                    const char *name, void *var, size_t var_len,
+setting_data_t *setting_data_create(type_data_t *type_list,
+                                    const char *section,
+                                    const char *name,
+                                    void *var,
+                                    size_t var_len,
                                     settings_type_t type,
                                     settings_notify_fn notify,
-                                    void *notify_context, bool readonly,
+                                    void *notify_context,
+                                    bool readonly,
                                     bool watchonly);
 
 /**
  * @brief setting_data_destroy - deinit for settings data
  * @param setting_data: setting to deinit
  */
 void setting_data_destroy(setting_data_t *setting_data);
 
 /**
- * @brief setting_data_update_value - process value string and update internal
- * data on success
+ * @brief setting_data_update_value - process value string and update internal data
+ * on success
  * @param setting_data: setting to update
  * @param value: value string to evaluate
  * @return result of updating the value
  */
-settings_write_res_t setting_data_update_value(setting_data_t *setting_data,
-                                               const char *value);
+settings_write_res_t setting_data_update_value(setting_data_t *setting_data, const char *value);
 
 /**
  * @brief setting_data_format - formats a fully formed setting message
  * payload
  * @param setting_data: the setting to format
  * @param type: flag to indicate if type data shall be formatted
  * @param buf: buffer to hold formatted setting string
  * @param len: length of the destination buffer
  * @param msg_hdr_len: length of the msg header
  * @return number of bytes written to the buffer, -1 in case of failure
  */
-int setting_data_format(setting_data_t *setting_data, bool type, char *buf,
-                        int blen, uint8_t *msg_hdr_len);
+int setting_data_format(setting_data_t *setting_data,
+                        bool type,
+                        char *buf,
+                        int blen,
+                        uint8_t *msg_hdr_len);
 
 /**
  * @brief setting_data_append - appends setting data to end of setting data list
  * @param data_list: setting data list
  * @param setting_data: data to append
  * @return
  */
-void setting_data_append(setting_data_t **data_list,
-                         setting_data_t *setting_data);
+void setting_data_append(setting_data_t **data_list, setting_data_t *setting_data);
 
 /**
  * @brief setting_data_list_remove - remove a setting from the setting data list
  * @param data_list: setting data list
  * @param setting_data: setting to remove
  */
-void setting_data_remove(setting_data_t **data_list,
-                         setting_data_t **setting_data);
+void setting_data_remove(setting_data_t **data_list, setting_data_t **setting_data);
 
 /**
  * @brief setting_data_lookup - retrieves setting node from settings data list
  * @param data_list: setting data list
  * @param section: setting section string to match
  * @param name: setting name string to match
  * @return the setting type entry if a match is found, otherwise NULL
  */
 setting_data_t *setting_data_lookup(setting_data_t *data_list,
-                                    const char *section, const char *name);
+                                    const char *section,
+                                    const char *name);
 
 /**
  * @brief setting_data_free - free the setting data list
  * @param data_list: setting data list to free
  */
 void setting_data_free(setting_data_t *data_list);
```

### Comparing `libsettings-0.1.14/include/internal/setting_def.h` & `libsettings-0.1.9/include/internal/setting_def.h`

 * *Files 19% similar despite different names*

```diff
@@ -11,30 +11,34 @@
  */
 
 #ifndef LIBSETTINGS_SETTING_DEF_H
 #define LIBSETTINGS_SETTING_DEF_H
 
 #include <libsettings/settings.h>
 
-#include <internal/setting_data.h>
-#include <internal/setting_type.h>
-
 typedef struct setting_sbp_cb_s setting_sbp_cb_t;
 
 /**
  * @brief Settings Context
  *
  * This is the main context for managing client interactions with
  * the settings manager. It implements the client messaging context
  * as well as the list of types and settings necessary to perform
  * the registration, watching and callback functionality of the client.
  */
 struct settings_s {
   type_data_t *type_data_list;
   setting_data_t *setting_data_list;
-  request_state_t *req_list;
+  request_state_t request_state;
   setting_sbp_cb_t *sbp_cb_list;
   settings_api_t client_iface;
   uint16_t sender_id;
+  /* TODO: make independent structure of these */
+  char resp_section[SETTINGS_BUFLEN];
+  char resp_name[SETTINGS_BUFLEN];
+  char resp_value[SETTINGS_BUFLEN];
+  char resp_type[SETTINGS_BUFLEN];
+  bool read_by_idx_done;
+  settings_write_res_t status;
 };
 
 #endif /* LIBSETTINGS_SETTING_DEF_H */
```

### Comparing `libsettings-0.1.14/include/internal/setting_sbp_cb.h` & `libsettings-0.1.9/include/internal/setting_sbp_cb.h`

 * *Files identical despite different names*

### Comparing `libsettings-0.1.14/include/internal/setting_type.h` & `libsettings-0.1.9/include/internal/setting_type.h`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,16 @@
 #ifndef LIBSETTINGS_SETTING_TYPE_H
 #define LIBSETTINGS_SETTING_TYPE_H
 
 #include <stdbool.h>
 
 #include <libsettings/settings.h>
 
-typedef int (*to_string_fn)(const void *priv, char *str, int slen,
-                            const void *blob, int blen);
-typedef bool (*from_string_fn)(const void *priv, void *blob, int blen,
-                               const char *str);
+typedef int (*to_string_fn)(const void *priv, char *str, int slen, const void *blob, int blen);
+typedef bool (*from_string_fn)(const void *priv, void *blob, int blen, const char *str);
 typedef int (*format_type_fn)(const void *priv, char *str, int slen);
 
 /**
  * @brief Type Data
  *
  * This structure encapsulates the codec for values of a given type
  * which the settings context uses to build a list of known types
@@ -56,17 +54,20 @@
  * @param to_string: serialization method
  * @param from_string: deserialization method
  * @param format_type: ?
  * @param priv: private data used in ser/des methods
  * @param type: type enum that is used to identify this type
  * @return
  */
-int type_register(type_data_t **data_list, to_string_fn to_string,
-                  from_string_fn from_string, format_type_fn format_type,
-                  const void *priv, settings_type_t *type);
+int type_register(type_data_t **data_list,
+                  to_string_fn to_string,
+                  from_string_fn from_string,
+                  format_type_fn format_type,
+                  const void *priv,
+                  settings_type_t *type);
 
 /**
  * @brief type_data_free - free type data list
  * @param data_list: type data list to free
  */
 void type_data_free(type_data_t *data_list);
```

### Comparing `libsettings-0.1.14/include/internal/setting_type_enum.h` & `libsettings-0.1.9/include/internal/setting_type_enum.h`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 #define LIBSETTINGS_ENUM_TAG "enum:"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 int enum_format_type(const void *priv, char *str, int slen);
-int enum_to_string(const void *priv, char *str, int slen, const void *blob,
-                   int blen);
+int enum_to_string(const void *priv, char *str, int slen, const void *blob, int blen);
 bool enum_from_string(const void *priv, void *blob, int blen, const char *str);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* LIBSETTINGS_SETTING_TYPE_ENUM_H */
```

### Comparing `libsettings-0.1.14/include/internal/setting_type_float.h` & `libsettings-0.1.9/include/internal/setting_type_float.h`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 #define SETTINGS_FLOAT_PRECISION 12
 #define SETTINGS_FLOAT_PRECISION_STR "12"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-int float_to_string(const void *priv, char *str, int slen, const void *blob,
-                    int blen);
+int float_to_string(const void *priv, char *str, int slen, const void *blob, int blen);
 bool float_from_string(const void *priv, void *blob, int blen, const char *str);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* LIBSETTINGS_SETTING_TYPE_FLOAT_H */
```

### Comparing `libsettings-0.1.14/include/internal/setting_type_int.h` & `libsettings-0.1.9/include/internal/setting_type_int.h`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 
 #include <stdbool.h>
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-int int_to_string(const void *priv, char *str, int slen, const void *blob,
-                  int blen);
+int int_to_string(const void *priv, char *str, int slen, const void *blob, int blen);
 bool int_from_string(const void *priv, void *blob, int blen, const char *str);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* LIBSETTINGS_SETTING_TYPE_INT_H */
```

### Comparing `libsettings-0.1.14/include/internal/setting_type_str.h` & `libsettings-0.1.9/include/internal/setting_type_str.h`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 
 #include <stdbool.h>
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-int str_to_string(const void *priv, char *str, int slen, const void *blob,
-                  int blen);
+int str_to_string(const void *priv, char *str, int slen, const void *blob, int blen);
 bool str_from_string(const void *priv, void *blob, int blen, const char *str);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* LIBSETTINGS_SETTING_TYPE_STR_H */
```

### Comparing `libsettings-0.1.14/include/libsettings/settings.h` & `libsettings-0.1.9/include/libsettings/settings.h`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,23 @@
 #define LIBSETTINGS_SETTINGS_H
 
 #include <inttypes.h>
 #include <stddef.h>
 
 #include <libsbp/sbp.h>
 
-#include <libsettings/settings_declspec.h>
+#if defined(_MSC_VER)
+#define LIBSETTINGS_EXPORT __declspec(dllexport)
+#define LIBSETTINGS_IMPORT __declspec(dllimport)
+#elif defined(__GNUC__)
+#define LIBSETTINGS_EXPORT __attribute__((visibility("default")))
+#define LIBSETTINGS_IMPORT
+#else
+#pragma error Unknown dynamic link import / export semantics.
+#endif
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 /**
  * @brief   Settings type.
@@ -42,15 +50,14 @@
  * @struct  settings_t
  *
  * @brief   Opaque context for settings.
  */
 typedef struct settings_s settings_t;
 
 #define SETTINGS_BUFLEN 255
-#define MAX_SETTING_WRITE_LEN 252
 
 /**
  * @brief   Standard settings type definitions.
  */
 enum {
   SETTINGS_TYPE_INT,    /**< Integer. 8, 16, or 32 bits.                   */
   SETTINGS_TYPE_FLOAT,  /**< Float. Single or double precision.            */
@@ -58,19 +65,17 @@
   SETTINGS_TYPE_BOOL    /**< Boolean.                                      */
 };
 
 /**
  * @brief Settings register error codes
  */
 typedef enum settings_reg_res_e {
-  SETTINGS_REG_OK = 0, /**< Setting registered, requested value used */
-  SETTINGS_REG_OK_PERM =
-      1, /**< Setting registered, permanent storage value found and returned */
-  SETTINGS_REG_REGISTERED =
-      2, /**< Setting is already registered, value from memory returned */
+  SETTINGS_REG_OK = 0,      /**< Setting registered, requested value used */
+  SETTINGS_REG_OK_PERM = 1, /**< Setting registered, permanent storage value found and returned */
+  SETTINGS_REG_REGISTERED = 2,   /**< Setting is already registered, value from memory returned */
   SETTINGS_REG_PARSE_FAILED = 3, /**< Could not parse setting */
 } settings_reg_res_t;
 
 /**
  * @brief Settings write error codes
  */
 typedef enum settings_write_res_e {
@@ -81,56 +86,47 @@
   /* READ_ONLY:MODIFY_DISABLED ~= Permanent:Temporary */
   SETTINGS_WR_READ_ONLY = 4,       /**< Setting is read only          */
   SETTINGS_WR_MODIFY_DISABLED = 5, /**< Setting is not modifiable     */
   SETTINGS_WR_SERVICE_FAILED = 6,  /**< System failure during setting */
   SETTINGS_WR_TIMEOUT = 7,         /**< Request wasn't replied in time */
 } settings_write_res_t;
 
-typedef int (*settings_send_t)(void *ctx, uint16_t msg_type, uint8_t len,
-                               uint8_t *payload);
-typedef int (*settings_send_from_t)(void *ctx, uint16_t msg_type, uint8_t len,
-                                    uint8_t *payload, uint16_t sbp_sender_id);
+typedef int (*settings_send_t)(void *ctx, uint16_t msg_type, uint8_t len, uint8_t *payload);
+typedef int (*settings_send_from_t)(void *ctx,
+                                    uint16_t msg_type,
+                                    uint8_t len,
+                                    uint8_t *payload,
+                                    uint16_t sbp_sender_id);
 
 typedef int (*settings_wait_init_t)(void *ctx);
 typedef int (*settings_wait_t)(void *ctx, int timeout_ms);
 typedef int (*settings_wait_deinit_t)(void *ctx);
 typedef void (*settings_signal_t)(void *ctx);
 
-typedef int (*settings_wait_thd_t)(void *event, int timeout_ms);
-typedef void (*settings_signal_thd_t)(void *event);
-
-typedef void (*settings_lock_t)(void *ctx);
-typedef void (*settings_unlock_t)(void *ctx);
-
-typedef int (*settings_reg_cb_t)(void *ctx, uint16_t msg_type,
-                                 sbp_msg_callback_t cb, void *cb_context,
+typedef int (*settings_reg_cb_t)(void *ctx,
+                                 uint16_t msg_type,
+                                 sbp_msg_callback_t cb,
+                                 void *cb_context,
                                  sbp_msg_callbacks_node_t **node);
 typedef int (*settings_unreg_cb_t)(void *ctx, sbp_msg_callbacks_node_t **node);
 
 typedef void (*settings_log_t)(int priority, const char *format, ...);
-typedef void (*settings_log_preformatted_t)(int priority, const char *format);
 
 typedef struct settings_api_s {
   void *ctx;
   settings_send_t send;
   settings_send_from_t send_from;
-  settings_wait_init_t
-      wait_init; /* Optional, needed if wait uses semaphores etc */
+  settings_wait_init_t wait_init; /* Optional, needed if wait uses semaphores etc */
   settings_wait_t wait;
-  settings_wait_deinit_t
-      wait_deinit; /* Optional, needed if wait uses semaphores etc */
+  settings_wait_deinit_t wait_deinit; /* Optional, needed if wait uses semaphores etc */
   settings_signal_t signal;
-  settings_wait_t wait_thd;     /* Required for multithreading */
-  settings_signal_t signal_thd; /* Required for multithreading */
-  settings_lock_t lock;         /* Required for multithreading */
-  settings_unlock_t unlock;     /* Required for multithreading */
   settings_reg_cb_t register_cb;
   settings_unreg_cb_t unregister_cb;
   settings_log_t log;
-  settings_log_preformatted_t log_preformatted;
+  bool log_preformat;
 } settings_api_t;
 
 /**
  * @brief   Settings notify callback.
  * @details Signature of a user-provided callback function to be executed
  *          after a setting value is updated.
  *
@@ -149,43 +145,42 @@
 /**
  * @brief   Create a settings context.
  * @details Create and initialize a settings context.
  *
  * @return                  Pointer to the created context, or NULL if the
  *                          operation failed.
  */
-LIBSETTINGS_DECLSPEC settings_t *settings_create(uint16_t sender_id,
-                                                 settings_api_t *api_impl);
+LIBSETTINGS_EXPORT settings_t *settings_create(uint16_t sender_id, settings_api_t *api_impl);
 
 /**
  * @brief   Destroy a settings context.
  * @details Deinitialize and destroy a settings context.
  *
  * @note    The context pointer will be set to NULL by this function.
  *
  * @param[inout] ctx        Double pointer to the context to destroy.
  */
-LIBSETTINGS_DECLSPEC void settings_destroy(settings_t **ctx);
+LIBSETTINGS_EXPORT void settings_destroy(settings_t **ctx);
 
 /**
  * @brief   Register an enum type.
  * @details Register an enum as a settings type.
  *
  * @param[in] ctx           Pointer to the context to use.
  * @param[in] enum_names    Null-terminated array of strings corresponding to
  *                          the possible enum values.
  * @param[out] type         Pointer to be set to the allocated settings type.
  *
  * @return                  The operation result.
  * @retval 0                The enum type was registered successfully.
  * @retval -1               An error occurred.
  */
-LIBSETTINGS_DECLSPEC int settings_register_enum(settings_t *ctx,
-                                                const char *const enum_names[],
-                                                settings_type_t *type);
+LIBSETTINGS_EXPORT int settings_register_enum(settings_t *ctx,
+                                              const char *const enum_names[],
+                                              settings_type_t *type);
 
 /**
  * @brief   Register a setting.
  * @details Register a persistent, user-facing setting.
  *
  * @note    The specified notify function will be executed from this function
  *          during initial registration.
@@ -201,18 +196,22 @@
  *                          written and during initial registration.
  * @param[in] notify_context Context passed to the notify function.
  *
  * @return                  The operation result.
  * @retval 0                The setting was registered successfully.
  * @retval -1               An error occurred.
  */
-LIBSETTINGS_DECLSPEC int settings_register_setting(
-    settings_t *ctx, const char *section, const char *name, void *var,
-    size_t var_len, settings_type_t type, settings_notify_fn notify,
-    void *notify_context);
+LIBSETTINGS_EXPORT int settings_register_setting(settings_t *ctx,
+                                                 const char *section,
+                                                 const char *name,
+                                                 void *var,
+                                                 size_t var_len,
+                                                 settings_type_t type,
+                                                 settings_notify_fn notify,
+                                                 void *notify_context);
 
 /**
  * @brief   Register a read-only setting.
  * @details Register a read-only, user-facing setting.
  *
  * @param[in] ctx           Pointer to the context to use.
  * @param[in] section       String describing the setting section.
@@ -222,17 +221,20 @@
  * @param[in] var_len       Size of the setting variable.
  * @param[in] type          Type of the setting.
  *
  * @return                  The operation result.
  * @retval 0                The setting was registered successfully.
  * @retval -1               An error occurred.
  */
-LIBSETTINGS_DECLSPEC int settings_register_readonly(
-    settings_t *ctx, const char *section, const char *name, const void *var,
-    size_t var_len, settings_type_t type);
+LIBSETTINGS_EXPORT int settings_register_readonly(settings_t *ctx,
+                                                  const char *section,
+                                                  const char *name,
+                                                  const void *var,
+                                                  size_t var_len,
+                                                  settings_type_t type);
 
 /**
  * @brief   Create and add a watch only setting.
  * @details Create and add a watch only setting.
  *
  * @param[in] ctx           Pointer to the context to use.
  * @param[in] section       String describing the setting section.
@@ -245,251 +247,242 @@
  *                          updated by a write response
  * @param[in] notify_context Context passed to the notify function.
  *
  * @return                  The operation result.
  * @retval 0                The setting was registered successfully.
  * @retval -1               An error occurred.
  */
-LIBSETTINGS_DECLSPEC int settings_register_watch(
-    settings_t *ctx, const char *section, const char *name, void *var,
-    size_t var_len, settings_type_t type, settings_notify_fn notify,
-    void *notify_context);
+LIBSETTINGS_EXPORT int settings_register_watch(settings_t *ctx,
+                                               const char *section,
+                                               const char *name,
+                                               void *var,
+                                               size_t var_len,
+                                               settings_type_t type,
+                                               settings_notify_fn notify,
+                                               void *notify_context);
 
 /**
  * @brief   Write a new value for registered setting.
  * @details Call will block until write response or internal timeout.
- *          In case of multithreading, caller shall provide event object
- *          that shall be used for waiting in wait_thd API function and
- *          signaled in signal_thd API function. Also lock and unlock API
- *          function implementations are mandatory when multithreading.
  *
  * @param[in] ctx           Pointer to the context to use.
- * @param[in] event         Request specific event object.
  * @param[in] section       String describing the setting section.
  * @param[in] name          String describing the setting name.
  * @param[in] value         Address of the value variable.
  * @param[in] value_len     Size of the value variable.
  * @param[in] type          Type of the setting.
  *
  * @return                  The operation result.
  * @retval -1               Sending of the request failed.
  * @retval 0                The setting was written successfully.
  * @retval >0               Response returned an error @see settings_write_res_t
  */
-LIBSETTINGS_DECLSPEC settings_write_res_t settings_write(
-    settings_t *ctx, void *event, const char *section, const char *name,
-    const void *value, size_t value_len, settings_type_t type);
+LIBSETTINGS_EXPORT settings_write_res_t settings_write(settings_t *ctx,
+                                                       const char *section,
+                                                       const char *name,
+                                                       const void *value,
+                                                       size_t value_len,
+                                                       settings_type_t type);
 
 /**
  * @brief   Write a new value for registered setting of type int.
  * @details Call will block until write response or internal timeout.
- *          In case of multithreading, caller shall provide event object
- *          that shall be used for waiting in wait_thd API function and
- *          signaled in signal_thd API function. Also lock and unlock API
- *          function implementations are mandatory when multithreading.
  *
  * @param[in] ctx           Pointer to the context to use.
- * @param[in] event         Request specific event object.
  * @param[in] section       String describing the setting section.
  * @param[in] name          String describing the setting name.
  * @param[in] value         Value to be written.
  *
  * @return                  The operation result.
  * @retval -1               Sending of the request failed.
  * @retval 0                The setting was written successfully.
  * @retval >0               Response returned an error @see settings_write_res_t
  */
-LIBSETTINGS_DECLSPEC settings_write_res_t
-settings_write_int(settings_t *ctx, void *event, const char *section,
-                   const char *name, int value);
+LIBSETTINGS_EXPORT settings_write_res_t settings_write_int(settings_t *ctx,
+                                                           const char *section,
+                                                           const char *name,
+                                                           int value);
 
 /**
  * @brief   Write a new value for registered setting of type float.
  * @details Call will block until write response or internal timeout.
- *          In case of multithreading, caller shall provide event object
- *          that shall be used for waiting in wait_thd API function and
- *          signaled in signal_thd API function. Also lock and unlock API
- *          function implementations are mandatory when multithreading.
  *
  * @param[in] ctx           Pointer to the context to use.
- * @param[in] event         Request specific event object.
  * @param[in] section       String describing the setting section.
  * @param[in] name          String describing the setting name.
  * @param[in] value         Value to be written.
  *
  * @return                  The operation result.
  * @retval -1               Sending of the request failed.
  * @retval 0                The setting was written successfully.
  * @retval >0               Response returned an error @see settings_write_res_t
  */
-LIBSETTINGS_DECLSPEC settings_write_res_t
-settings_write_float(settings_t *ctx, void *event, const char *section,
-                     const char *name, float value);
+LIBSETTINGS_EXPORT settings_write_res_t settings_write_float(settings_t *ctx,
+                                                             const char *section,
+                                                             const char *name,
+                                                             float value);
 
 /**
  * @brief   Write a new value for registered setting of type str.
  * @details Call will block until write response or internal timeout.
- *          In case of multithreading, caller shall provide event object
- *          that shall be used for waiting in wait_thd API function and
- *          signaled in signal_thd API function. Also lock and unlock API
- *          function implementations are mandatory when multithreading.
  *
  * @param[in] ctx           Pointer to the context to use.
- * @param[in] event         Request specific event object.
  * @param[in] section       String describing the setting section.
  * @param[in] name          String describing the setting name.
  * @param[in] str           Value to be written.
  *
  * @return                  The operation result.
  * @retval -1               Sending of the request failed.
  * @retval 0                The setting was written successfully.
  * @retval >0               Response returned an error @see settings_write_res_t
  */
-LIBSETTINGS_DECLSPEC settings_write_res_t
-settings_write_str(settings_t *ctx, void *event, const char *section,
-                   const char *name, const char *str);
+LIBSETTINGS_EXPORT settings_write_res_t settings_write_str(settings_t *ctx,
+                                                           const char *section,
+                                                           const char *name,
+                                                           const char *str);
 
 /**
  * @brief   Write a new value for registered setting of type bool.
  * @details Call will block until write response or internal timeout.
- *          In case of multithreading, caller shall provide event object
- *          that shall be used for waiting in wait_thd API function and
- *          signaled in signal_thd API function. Also lock and unlock API
- *          function implementations are mandatory when multithreading.
  *
  * @param[in] ctx           Pointer to the context to use.
- * @param[in] event         Request specific event object.
  * @param[in] section       String describing the setting section.
  * @param[in] name          String describing the setting name.
  * @param[in] value         Value to be written.
  *
  * @return                  The operation result.
  * @retval -1               Sending of the request failed.
  * @retval 0                The setting was written successfully.
  * @retval >0               Response returned an error @see settings_write_res_t
  */
-LIBSETTINGS_DECLSPEC settings_write_res_t
-settings_write_bool(settings_t *ctx, void *event, const char *section,
-                    const char *name, bool value);
+LIBSETTINGS_EXPORT settings_write_res_t settings_write_bool(settings_t *ctx,
+                                                            const char *section,
+                                                            const char *name,
+                                                            bool value);
 
 /**
  * @brief   Read value of registered setting.
  * @details Call will block until read response or internal timeout.
  *
  * @param[in] ctx           Pointer to the context to use.
  * @param[in] section       String describing the setting section.
  * @param[in] name          String describing the setting name.
- * @param[in] value         Address of the variable where the read value shall
- * be written.
+ * @param[in] value         Address of the variable where the read value shall be written.
  * @param[in] value_len     Size of the value variable.
  * @param[in] type          Type of the setting.
  *
  * @return                  The operation result.
  * @retval 0                The setting was read successfully. Error otherwise.
  */
-LIBSETTINGS_DECLSPEC int settings_read(settings_t *ctx, const char *section,
-                                       const char *name, void *value,
-                                       size_t value_len, settings_type_t type);
+LIBSETTINGS_EXPORT int settings_read(settings_t *ctx,
+                                     const char *section,
+                                     const char *name,
+                                     void *value,
+                                     size_t value_len,
+                                     settings_type_t type);
 
 /**
  * @brief   Read value of registered setting of type int.
  * @details Call will block until read response or internal timeout.
  *
  * @param[in] ctx           Pointer to the context to use.
  * @param[in] section       String describing the setting section.
  * @param[in] name          String describing the setting name.
- * @param[out] value        Address of the variable where the read value shall
- * be written.
+ * @param[out] value        Address of the variable where the read value shall be written.
  *
  * @return                  The operation result.
  * @retval 0                The setting was read successfully. Error otherwise.
  */
-LIBSETTINGS_DECLSPEC int settings_read_int(settings_t *ctx, const char *section,
-                                           const char *name, int *value);
+LIBSETTINGS_EXPORT int settings_read_int(settings_t *ctx,
+                                         const char *section,
+                                         const char *name,
+                                         int *value);
 
 /**
  * @brief   Read value of registered setting of type float.
  * @details Call will block until read response or internal timeout.
  *
  * @param[in] ctx           Pointer to the context to use.
  * @param[in] section       String describing the setting section.
  * @param[in] name          String describing the setting name.
- * @param[out] value        Address of the variable where the read value shall
- * be written.
+ * @param[out] value        Address of the variable where the read value shall be written.
  *
  * @return                  The operation result.
  * @retval 0                The setting was read successfully. Error otherwise.
  */
-LIBSETTINGS_DECLSPEC int settings_read_float(settings_t *ctx,
-                                             const char *section,
-                                             const char *name, float *value);
+LIBSETTINGS_EXPORT int settings_read_float(settings_t *ctx,
+                                           const char *section,
+                                           const char *name,
+                                           float *value);
 
 /**
  * @brief   Read value of registered setting of type str.
  * @details Call will block until read response or internal timeout.
  *
  * @param[in] ctx           Pointer to the context to use.
  * @param[in] section       String describing the setting section.
  * @param[in] name          String describing the setting name.
- * @param[out] str          Address of the variable where the read value shall
- * be written.
+ * @param[out] str          Address of the variable where the read value shall be written.
  * @param[in] str_len       Size of the str buffer.
  *
  * @return                  The operation result.
  * @retval 0                The setting was read successfully. Error otherwise.
  */
-LIBSETTINGS_DECLSPEC int settings_read_str(settings_t *ctx, const char *section,
-                                           const char *name, char *str,
-                                           size_t str_len);
+LIBSETTINGS_EXPORT int settings_read_str(settings_t *ctx,
+                                         const char *section,
+                                         const char *name,
+                                         char *str,
+                                         size_t str_len);
 
 /**
  * @brief   Read value of registered setting of type bool.
  * @details Call will block until read response or internal timeout.
  *
  * @param[in] ctx           Pointer to the context to use.
  * @param[in] section       String describing the setting section.
  * @param[in] name          String describing the setting name.
- * @param[out] value        Address of the variable where the read value shall
- * be written.
+ * @param[out] value        Address of the variable where the read value shall be written.
  *
  * @return                  The operation result.
  * @retval 0                The setting was read successfully. Error otherwise.
  */
-LIBSETTINGS_DECLSPEC int settings_read_bool(settings_t *ctx,
-                                            const char *section,
-                                            const char *name, bool *value);
+LIBSETTINGS_EXPORT int settings_read_bool(settings_t *ctx,
+                                          const char *section,
+                                          const char *name,
+                                          bool *value);
 
 /**
  * @brief   Read value of registered setting based on index.
  * @details Call will block until read_by_idx response or internal timeout.
  *
  * @param[in] ctx           Pointer to the context to use.
- * @param[in] event         Request specific event object.
  * @param[in] idx           Index to read.
  * @param[out] section      String describing the setting section.
  * @param[in] section_len   Section str buffer size.
  * @param[out] name         String describing the setting name.
  * @param[in] name_len      Name str buffer size.
  * @param[out] value        String describing the setting value.
  * @param[in] value_len     Value str buffer size.
  * @param[out] type         String describing the setting type.
  * @param[in] type_len      Type str buffer size.
  *
  * @return                  The operation result.
- * @retval 0                The setting was read successfully. Next index is
- * ready to be read.
+ * @retval 0                The setting was read successfully. Next index is ready to be read.
  * @retval <0               Error.
- * @retval >0               Last index was read successfully. There are no more
- * indexes to read.
+ * @retval >0               Last index was read successfully. There are no more indexes to read.
  */
-LIBSETTINGS_DECLSPEC int settings_read_by_idx(settings_t *ctx, void *event,
-                                              uint16_t idx, char *section,
-                                              size_t section_len, char *name,
-                                              size_t name_len, char *value,
-                                              size_t value_len, char *type,
-                                              size_t type_len);
+LIBSETTINGS_EXPORT int settings_read_by_idx(settings_t *ctx,
+                                            uint16_t idx,
+                                            char *section,
+                                            size_t section_len,
+                                            char *name,
+                                            size_t name_len,
+                                            char *value,
+                                            size_t value_len,
+                                            char *type,
+                                            size_t type_len);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* LIBSETTINGS_SETTINGS_H */
```

### Comparing `libsettings-0.1.14/include/libsettings/settings_util.h` & `libsettings-0.1.9/include/libsettings/settings_util.h`

 * *Files 6% similar despite different names*

```diff
@@ -11,35 +11,36 @@
  */
 
 #ifndef LIBSETTINGS_SETTINGS_UTIL_H
 #define LIBSETTINGS_SETTINGS_UTIL_H
 
 #include <inttypes.h>
 
-#include <libsettings/settings_declspec.h>
-
 typedef enum settings_tokens_e {
-  SETTINGS_TOKENS_INVALID = -1, /** An error occurred */
-  SETTINGS_TOKENS_EMPTY = 0,    /** No tokens found */
-  SETTINGS_TOKENS_SECTION = 1,  /** Section token found */
-  SETTINGS_TOKENS_NAME = 2,     /** Section and name tokens found */
-  SETTINGS_TOKENS_VALUE = 3,    /** Section, name and value tokens found */
-  SETTINGS_TOKENS_TYPE = 4, /** Section, name, value and type tokens found */
-  SETTINGS_TOKENS_EXTRA_NULL = 5, /** Section, name, value and type tokens
-                                     found, this is for backwards compatibility
-                                     for FW versions 2.2 and older */
+  SETTINGS_TOKENS_INVALID = -1,   /** An error occurred */
+  SETTINGS_TOKENS_EMPTY = 0,      /** No tokens found */
+  SETTINGS_TOKENS_SECTION = 1,    /** Section token found */
+  SETTINGS_TOKENS_NAME = 2,       /** Section and name tokens found */
+  SETTINGS_TOKENS_VALUE = 3,      /** Section, name and value tokens found */
+  SETTINGS_TOKENS_TYPE = 4,       /** Section, name, value and type tokens found */
+  SETTINGS_TOKENS_EXTRA_NULL = 5, /** Section, name, value and type tokens found,
+                                      this is for backwards compatibility for FW
+                                      versions 2.2 and older */
 } settings_tokens_t;
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-LIBSETTINGS_DECLSPEC int settings_format(const char *section, const char *name,
-                                         const char *value, const char *type,
-                                         char *buf, size_t blen);
+int settings_format(const char *section,
+                    const char *name,
+                    const char *value,
+                    const char *type,
+                    char *buf,
+                    size_t blen);
 
 /**
  * @brief   Parse setting strings from SBP message buffer
  * @details Points the string pointers to corresponding message indexes.
  *          Function doesn't make copies from the strings so when the buffer
  *          is freed or out of scope the pointers shall be invalid. Each output
  *          pointer is optional and can be replaced with NULL.
@@ -51,16 +52,19 @@
  * @param[out] value        3rd string, setting value
  * @param[out] type         4th string, setting type/enum list
  *
  * @return                  Number of NULL terminated tokens found. If more than
  *                          5 is found, -1 is returned. See @ settings_tokens_t.
  * @retval -1               An error occurred.
  */
-LIBSETTINGS_DECLSPEC settings_tokens_t
-settings_parse(const char *buf, size_t blen, const char **section,
-               const char **name, const char **value, const char **type);
+settings_tokens_t settings_parse(const char *buf,
+                                 size_t blen,
+                                 const char **section,
+                                 const char **name,
+                                 const char **value,
+                                 const char **type);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* LIBSETTINGS_SETTINGS_UTIL_H */
```

### Comparing `libsettings-0.1.14/libsettings.egg-info/PKG-INFO` & `libsettings-0.1.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: libsettings
-Version: 0.1.14
+Version: 0.1.9
 Summary: Open source SwiftNav settings API library.
 Home-page: https://github.com/swift-nav/libsettings
 Author: Swift Navigation
 Author-email: dev@swift-nav.com
+License: UNKNOWN
+Description: UNKNOWN
 Platform: linux
 Platform: osx
 Platform: win32
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE
```

### Comparing `libsettings-0.1.14/python/libsettings.c` & `libsettings-0.1.9/python/libsettings.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,18 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.5 */
 
-/* BEGIN: Cython Metadata
-{
-    "distutils": {
-        "depends": [
-            "include/libsettings/settings.h"
-        ],
-        "include_dirs": [
-            "python"
-        ],
-        "name": "libsettings",
-        "sources": [
-            "/home/runner/work/libsettings/libsettings/python/libsettings.pyx"
-        ]
-    },
-    "module_name": "libsettings"
-}
-END: Cython Metadata */
-
-#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
-#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_5"
+#define CYTHON_HEX_VERSION 0x001D05F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -63,15 +43,14 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -92,34 +71,26 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -149,67 +120,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
-#elif defined(PY_NOGIL)
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
-  #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 1
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYTYPE_LOOKUP
-  #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #ifndef CYTHON_USE_ASYNC_SLOTS
-    #define CYTHON_USE_ASYNC_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYLIST_INTERNALS
-  #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
-  #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
-  #ifndef CYTHON_AVOID_BORROWED_REFS
-    #define CYTHON_AVOID_BORROWED_REFS 0
-  #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
-  #undef CYTHON_FAST_THREAD_STATE
-  #define CYTHON_FAST_THREAD_STATE 0
-  #undef CYTHON_FAST_PYCALL
-  #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
-  #endif
-  #undef CYTHON_USE_DICT_VERSIONS
-  #define CYTHON_USE_DICT_VERSIONS 0
-  #undef CYTHON_USE_EXC_INFO_STACK
-  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -221,72 +143,61 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
+    #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
+  #if PY_VERSION_HEX < 0x030300F0
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL 1
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
+    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK 0
-  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+  #ifndef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
-  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #if PY_MAJOR_VERSION < 3
-    #include "longintrepr.h"
-  #endif
+  #include "longintrepr.h"
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -395,80 +306,16 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-  #define __Pyx_DefaultClassType PyType_Type
-#if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
-                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
-                                                    PyObject *fv, PyObject *cell, PyObject* fn,
-                                                    PyObject *name, int fline, PyObject *lnos) {
-        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
-        const char *fn_cstr=NULL;
-        const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
-        PyObject *type, *value, *traceback;
-        PyErr_Fetch(&type, &value, &traceback);
-        if (!(kwds=PyDict_New())) goto end;
-        if (!(argcount=PyLong_FromLong(a))) goto end;
-        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
-        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
-        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
-        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
-        if (!(nlocals=PyLong_FromLong(l))) goto end;
-        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
-        if (!(stacksize=PyLong_FromLong(s))) goto end;
-        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
-        if (!(flags=PyLong_FromLong(f))) goto end;
-        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
-        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
-        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
-        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
-        Py_XDECREF(kwds);
-        Py_XDECREF(argcount);
-        Py_XDECREF(posonlyargcount);
-        Py_XDECREF(kwonlyargcount);
-        Py_XDECREF(nlocals);
-        Py_XDECREF(stacksize);
-        Py_XDECREF(replace);
-        Py_XDECREF(call_result);
-        Py_XDECREF(empty);
-        if (type) {
-            PyErr_Restore(type, value, traceback);
-        }
-        return co;
-    }
-#else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
-#endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
@@ -570,36 +417,24 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if PY_VERSION_HEX >= 0x030C0000
-    #define __Pyx_PyUnicode_READY(op)       (0)
-  #else
-    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                                0 : _PyUnicode_Ready((PyObject *)(op)))
-  #endif
+  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                              0 : _PyUnicode_Ready((PyObject *)(op)))
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if PY_VERSION_HEX >= 0x030C0000
-    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
-  #else
-    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-    #else
-    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-    #endif
-  #endif
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
@@ -640,35 +475,26 @@
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBaseString_Type            PyUnicode_Type
   #define PyStringObject               PyUnicodeObject
   #define PyString_Type                PyUnicode_Type
   #define PyString_Check               PyUnicode_Check
   #define PyString_CheckExact          PyUnicode_CheckExact
-#ifndef PyObject_Unicode
   #define PyObject_Unicode             PyObject_Str
 #endif
-#endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
-#if PY_VERSION_HEX >= 0x030900A4
-  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
-  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
-#else
-  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
-  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
-#endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
@@ -694,21 +520,21 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
@@ -722,18 +548,16 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
-  #if !defined(_USE_MATH_DEFINES)
-    #define _USE_MATH_DEFINES
-  #endif
+#if defined(WIN32) || defined(MS_WINDOWS)
+  #define _USE_MATH_DEFINES
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -743,18 +567,19 @@
 #endif
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
-#define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+
 #define __PYX_ERR(f_index, lineno, Ln_error) \
-    { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
+{ \
+  __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
+}
 
 #ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
@@ -773,16 +598,15 @@
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
 
 typedef struct {PyObject **p; const char *s; const Py_ssize_t n; const char* encoding;
                 const char is_unicode; const char is_str; const char intern; } __Pyx_StringTabEntry;
 
 #define __PYX_DEFAULT_STRING_ENCODING_IS_ASCII 0
-#define __PYX_DEFAULT_STRING_ENCODING_IS_UTF8 0
-#define __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT (PY_MAJOR_VERSION >= 3 && __PYX_DEFAULT_STRING_ENCODING_IS_UTF8)
+#define __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT 0
 #define __PYX_DEFAULT_STRING_ENCODING ""
 #define __Pyx_PyObject_FromString __Pyx_PyBytes_FromString
 #define __Pyx_PyObject_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
 #define __Pyx_uchar_cast(c) ((unsigned char)c)
 #define __Pyx_long_cast(x) ((long)x)
 #define __Pyx_fits_Py_ssize_t(v, type, is_signed)  (\
     (sizeof(type) < sizeof(Py_ssize_t))  ||\
@@ -857,15 +681,14 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -970,30 +793,30 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "python/libsettings.pyx",
   "stringsource",
+  "python/libsettings.pyx",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_11libsettings_Settings;
 struct __pyx_obj_11libsettings___pyx_scope_struct___callback_broker;
 struct __pyx_obj_11libsettings___pyx_scope_struct_1_genexpr;
 struct __pyx_obj_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper;
 struct __pyx_obj_11libsettings___pyx_scope_struct_3_genexpr;
 struct __pyx_obj_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper;
 struct __pyx_obj_11libsettings___pyx_scope_struct_5_genexpr;
 struct __pyx_obj___Pyx_EnumMeta;
 
-/* "libsettings.pyx":23
- * from multiprocessing.pool import ThreadPool
+/* "libsettings.pyx":21
+ * from threading import Event
  * 
  * cpdef enum SettingsWriteResponseCodes:             # <<<<<<<<<<<<<<
  *     SETTINGS_WR_OK = 0
  *     SETTINGS_WR_VALUE_REJECTED = 1
  */
 enum __pyx_t_11libsettings_SettingsWriteResponseCodes {
   __pyx_e_11libsettings_SETTINGS_WR_OK = 0,
@@ -1002,47 +825,46 @@
   __pyx_e_11libsettings_SETTINGS_WR_PARSE_FAILED = 3,
   __pyx_e_11libsettings_SETTINGS_WR_READ_ONLY = 4,
   __pyx_e_11libsettings_SETTINGS_WR_MODIFY_DISABLED = 5,
   __pyx_e_11libsettings_SETTINGS_WR_SERVICE_FAILED = 6,
   __pyx_e_11libsettings_SETTINGS_WR_TIMEOUT = 7
 };
 
-/* "libsettings.pyx":126
+/* "libsettings.pyx":119
  * 
  * 
  * cdef class Settings:             # <<<<<<<<<<<<<<
  *     cdef settings_t *ctx
  *     cdef settings_api_t c_api
  */
 struct __pyx_obj_11libsettings_Settings {
   PyObject_HEAD
   settings_t *ctx;
   settings_api_t c_api;
   PyObject *_callbacks;
   PyObject *_event;
   PyObject *_link;
   PyObject *_debug;
-  PyObject *_lock;
 };
 
 
-/* "libsettings.pyx":282
- *         return ret
+/* "libsettings.pyx":206
+ *         return settings
  * 
  *     def _callback_broker(self, sbp_msg, **metadata):             # <<<<<<<<<<<<<<
  *         if self._debug:
  *             print '_callback_broker', sbp_msg.msg_type
  */
 struct __pyx_obj_11libsettings___pyx_scope_struct___callback_broker {
   PyObject_HEAD
   PyObject *__pyx_v_sbp_msg;
 };
 
 
-/* "libsettings.pyx":285
+/* "libsettings.pyx":209
  *         if self._debug:
  *             print '_callback_broker', sbp_msg.msg_type
  *             print ":".join("{:02x}".format(ord(c)) for c in sbp_msg.payload)             # <<<<<<<<<<<<<<
  * 
  *         msg_type = sbp_msg.msg_type
  */
 struct __pyx_obj_11libsettings___pyx_scope_struct_1_genexpr {
@@ -1051,29 +873,29 @@
   PyObject *__pyx_v_c;
   PyObject *__pyx_t_0;
   Py_ssize_t __pyx_t_1;
   PyObject *(*__pyx_t_2)(PyObject *);
 };
 
 
-/* "libsettings.pyx":303
+/* "libsettings.pyx":227
  *         cb(sbp_msg.sender, sbp_msg.length, bytes(sbp_msg.payload), <void*><uintptr_t>cb_data[2])
  * 
  * cdef int send_wrapper(void *ctx, uint16_t msg_type, uint8_t length, uint8_t *payload):             # <<<<<<<<<<<<<<
  *     settings = <object>ctx
  * 
  */
 struct __pyx_obj_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper {
   PyObject_HEAD
   uint8_t __pyx_v_length;
   uint8_t *__pyx_v_payload;
 };
 
 
-/* "libsettings.pyx":308
+/* "libsettings.pyx":232
  *     if settings._debug:
  *         print 'send_wrapper', msg_type
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])             # <<<<<<<<<<<<<<
  * 
  *     # https://cython.readthedocs.io/en/latest/src/tutorial/strings.html
  */
 struct __pyx_obj_11libsettings___pyx_scope_struct_3_genexpr {
@@ -1081,29 +903,29 @@
   struct __pyx_obj_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper *__pyx_outer_scope;
   PyObject *__pyx_v_c;
   PyObject *__pyx_t_0;
   PyObject *(*__pyx_t_1)(PyObject *);
 };
 
 
-/* "libsettings.pyx":318
+/* "libsettings.pyx":242
  *     return 0
  * 
  * cdef int send_from_wrapper(void *ctx, uint16_t msg_type, uint8_t length, uint8_t *payload, uint16_t sbp_sender_id):             # <<<<<<<<<<<<<<
  *     settings = <object>ctx
  * 
  */
 struct __pyx_obj_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper {
   PyObject_HEAD
   uint8_t __pyx_v_length;
   uint8_t *__pyx_v_payload;
 };
 
 
-/* "libsettings.pyx":323
+/* "libsettings.pyx":247
  *     if settings._debug:
  *         print 'send_from_wrapper', msg_type
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])             # <<<<<<<<<<<<<<
  * 
  *     settings._link(SBP(msg_type=msg_type,
  */
 struct __pyx_obj_11libsettings___pyx_scope_struct_5_genexpr {
@@ -1209,254 +1031,76 @@
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
-/* PyDictVersioning.proto */
-#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
-#define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
-#define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
-#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
-    (version_var) = __PYX_GET_DICT_VERSION(dict);\
-    (cache_var) = (value);
-#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP) {\
-    static PY_UINT64_T __pyx_dict_version = 0;\
-    static PyObject *__pyx_dict_cached_value = NULL;\
-    if (likely(__PYX_GET_DICT_VERSION(DICT) == __pyx_dict_version)) {\
-        (VAR) = __pyx_dict_cached_value;\
-    } else {\
-        (VAR) = __pyx_dict_cached_value = (LOOKUP);\
-        __pyx_dict_version = __PYX_GET_DICT_VERSION(DICT);\
-    }\
-}
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj);
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj);
-static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version);
-#else
-#define __PYX_GET_DICT_VERSION(dict)  (0)
-#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
-#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
-#endif
-
-/* GetModuleGlobalName.proto */
-#if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  do {\
-    static PY_UINT64_T __pyx_dict_version = 0;\
-    static PyObject *__pyx_dict_cached_value = NULL;\
-    (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
-        (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
-        __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-} while(0)
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
-    PY_UINT64_T __pyx_dict_version;\
-    PyObject *__pyx_dict_cached_value;\
-    (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-} while(0)
-static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
+/* PyCFunctionFastCall.proto */
+#if CYTHON_FAST_PYCCALL
+static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
-#define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
-static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
+#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
 #endif
 
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
 #if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, int nargs, PyObject *kwargs);
 #else
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
-#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
-#endif
-
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
-
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
-#endif
-
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
-#endif
-
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
-
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
-#endif
-
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
-#endif
-
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
-
-/* ListCompAppend.proto */
-#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
-static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
-    PyListObject* L = (PyListObject*) list;
-    Py_ssize_t len = Py_SIZE(list);
-    if (likely(L->allocated > len)) {
-        Py_INCREF(x);
-        PyList_SET_ITEM(list, len, x);
-        __Pyx_SET_SIZE(list, len + 1);
-        return 0;
-    }
-    return PyList_Append(list, x);
-}
-#else
-#define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
-#endif
-
-/* DictGetItem.proto */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
-#define __Pyx_PyObject_Dict_GetItem(obj, name)\
-    (likely(PyDict_CheckExact(obj)) ?\
-     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
-#else
-#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
-#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
-#endif
-
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        __Pyx_SET_SIZE(list, len + 1);
+        Py_SIZE(list) = len+1;
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
-/* GetItemInt.proto */
-#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
-    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
-               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
-#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
-                                                     int is_list, int wraparound, int boundscheck);
-
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname);
 
 /* UnicodeAsUCS4.proto */
 static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject*);
 
 /* object_ord.proto */
@@ -1464,14 +1108,17 @@
 #define __Pyx_PyObject_Ord(c)\
     (likely(PyUnicode_Check(c)) ? (long)__Pyx_PyUnicode_AsPy_UCS4(c) : __Pyx__PyObject_Ord(c))
 #else
 #define __Pyx_PyObject_Ord(c) __Pyx__PyObject_Ord(c)
 #endif
 static long __Pyx__PyObject_Ord(PyObject* c);
 
+/* PyObjectCall2Args.proto */
+static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+
 /* StringJoin.proto */
 #if PY_MAJOR_VERSION < 3
 #define __Pyx_PyString_Join __Pyx_PyBytes_Join
 #define __Pyx_PyBaseString_Join(s, v) (PyUnicode_CheckExact(s) ? PyUnicode_Join(s, v) : __Pyx_PyBytes_Join(s, v))
 #else
 #define __Pyx_PyString_Join PyUnicode_Join
 #define __Pyx_PyBaseString_Join PyUnicode_Join
@@ -1482,33 +1129,148 @@
     #else
     #define __Pyx_PyBytes_Join _PyBytes_Join
     #endif
 #else
 static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values);
 #endif
 
+/* PyObjectCallNoArg.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+#else
+#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
+#endif
+
 /* RaiseTooManyValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
 
 /* RaiseNeedMoreValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
 
 /* IterFinish.proto */
 static CYTHON_INLINE int __Pyx_IterFinish(void);
 
 /* UnpackItemEndCheck.proto */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected);
 
+/* GetItemInt.proto */
+#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
+    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
+               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
+#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
+                                                     int is_list, int wraparound, int boundscheck);
+
 /* ObjectGetItem.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
+/* PyDictVersioning.proto */
+#if CYTHON_USE_DICT_VERSIONS
+#define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
+#define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
+#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
+    (version_var) = __PYX_GET_DICT_VERSION(dict);\
+    (cache_var) = (value);
+#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP) {\
+    static PY_UINT64_T __pyx_dict_version = 0;\
+    static PyObject *__pyx_dict_cached_value = NULL;\
+    if (likely(__PYX_GET_DICT_VERSION(DICT) == __pyx_dict_version)) {\
+        (VAR) = __pyx_dict_cached_value;\
+    } else {\
+        (VAR) = __pyx_dict_cached_value = (LOOKUP);\
+        __pyx_dict_version = __PYX_GET_DICT_VERSION(DICT);\
+    }\
+}
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj);
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj);
+static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version);
+#else
+#define __PYX_GET_DICT_VERSION(dict)  (0)
+#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
+#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
+#endif
+
+/* GetModuleGlobalName.proto */
+#if CYTHON_USE_DICT_VERSIONS
+#define __Pyx_GetModuleGlobalName(var, name)  {\
+    static PY_UINT64_T __pyx_dict_version = 0;\
+    static PyObject *__pyx_dict_cached_value = NULL;\
+    (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
+        (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
+        __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
+}
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+    PY_UINT64_T __pyx_dict_version;\
+    PyObject *__pyx_dict_cached_value;\
+    (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
+}
+static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
+#else
+#define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
+static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
+#endif
+
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
 /* PyObjectSetAttrStr.proto */
 #if CYTHON_USE_TYPE_SLOTS
@@ -1525,14 +1287,38 @@
     __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
                __Pyx_SetItemInt_Generic(o, to_py_func(i), v)))
 static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v);
 static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v,
                                                int is_list, int wraparound, int boundscheck);
 
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
 /* DelItemInt.proto */
 #define __Pyx_DelItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_DelItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
                __Pyx_DelItem_Generic(o, to_py_func(i))))
 static int __Pyx_DelItem_Generic(PyObject *o, PyObject *j);
@@ -1549,20 +1335,14 @@
 
 /* GetAttr.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
-/* PySequenceContains.proto */
-static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
-    int result = PySequence_Contains(seq, item);
-    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
-}
-
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
@@ -1581,17 +1361,14 @@
 /* PyObject_GenericGetAttr.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
-/* PyObjectGetAttrStrNoError.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
-
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
 
 /* SetNameInClass.proto */
@@ -1604,15 +1381,15 @@
 #else
 #define __Pyx_SetNameInClass(ns, name, value)  PyObject_SetItem(ns, name, value)
 #endif
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
-/* CythonFunctionShared.proto */
+/* CythonFunction.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
 #define __Pyx_CYFUNCTION_CCLASS        0x04
 #define __Pyx_CyFunction_GetClosure(f)\
     (((__pyx_CyFunctionObject *) (f))->func_closure)
 #define __Pyx_CyFunction_GetClassObj(f)\
@@ -1632,24 +1409,25 @@
     PyObject *func_doc;
     PyObject *func_globals;
     PyObject *func_code;
     PyObject *func_closure;
     PyObject *func_classobj;
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
 } __pyx_CyFunctionObject;
 static PyTypeObject *__pyx_CyFunctionType = 0;
 #define __Pyx_CyFunction_Check(obj)  (__Pyx_TypeCheck(obj, __pyx_CyFunctionType))
-static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+#define __Pyx_CyFunction_NewEx(ml, flags, qualname, self, module, globals, code)\
+    __Pyx_CyFunction_New(__pyx_CyFunctionType, ml, flags, qualname, self, module, globals, code)
+static PyObject *__Pyx_CyFunction_New(PyTypeObject *, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *self,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
                                                          size_t size,
                                                          int pyobjects);
@@ -1657,21 +1435,14 @@
                                                             PyObject *tuple);
 static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
                                                              PyObject *dict);
 static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
                                                               PyObject *dict);
 static int __pyx_CyFunction_init(void);
 
-/* CythonFunction.proto */
-static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
-                                      int flags, PyObject* qualname,
-                                      PyObject *closure,
-                                      PyObject *module, PyObject *globals,
-                                      PyObject* code);
-
 /* Py3ClassCreate.proto */
 static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name, PyObject *qualname,
                                            PyObject *mkw, PyObject *modname, PyObject *doc);
 static PyObject *__Pyx_Py3ClassCreate(PyObject *metaclass, PyObject *name, PyObject *bases, PyObject *dict,
                                       PyObject *mkw, int calculate_metaclass, int allow_py2_metaclass);
 
 /* Globals.proto */
@@ -1699,50 +1470,45 @@
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
-/* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define __Pyx_HAS_GCC_DIAGNOSTIC
-#endif
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* Print.proto */
 static int __Pyx_Print(PyObject*, PyObject *, int);
 #if CYTHON_COMPILING_IN_PYPY || PY_MAJOR_VERSION >= 3
 static PyObject* __pyx_print = 0;
 static PyObject* __pyx_print_kwargs = 0;
 #endif
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE uint16_t __Pyx_PyInt_As_uint16_t(PyObject *);
-
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint16_t(uint16_t value);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint8_t(uint8_t value);
+
+/* CIntFromPy.proto */
+static CYTHON_INLINE uint16_t __Pyx_PyInt_As_uint16_t(PyObject *);
+
+/* PrintOne.proto */
+static int __Pyx_PrintOne(PyObject* stream, PyObject *o);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE uint8_t __Pyx_PyInt_As_uint8_t(PyObject *);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint8_t(uint8_t value);
-
-/* PrintOne.proto */
-static int __Pyx_PrintOne(PyObject* stream, PyObject *o);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(enum __pyx_t_11libsettings_SettingsWriteResponseCodes value);
 
 /* CIntFromPy.proto */
@@ -1794,15 +1560,14 @@
     PyObject *gi_weakreflist;
     PyObject *classobj;
     PyObject *yieldfrom;
     PyObject *gi_name;
     PyObject *gi_qualname;
     PyObject *gi_modulename;
     PyObject *gi_code;
-    PyObject *gi_frame;
     int resume_label;
     char is_running;
 } __pyx_CoroutineObject;
 static __pyx_CoroutineObject *__Pyx__Coroutine_New(
     PyTypeObject *type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
     PyObject *name, PyObject *qualname, PyObject *module_name);
 static __pyx_CoroutineObject *__Pyx__Coroutine_NewInit(
@@ -1872,173 +1637,147 @@
 static PyTypeObject *__pyx_ptype_11libsettings___pyx_scope_struct_5_genexpr = 0;
 static PyTypeObject *__pyx_ptype___Pyx_EnumMeta = 0;
 static PyObject *__Pyx_OrderedDict = 0;
 static PyObject *__Pyx_EnumBase = 0;
 static PyObject *__Pyx_globals = 0;
 static int __pyx_f_11libsettings_send_wrapper(void *, uint16_t, uint8_t, uint8_t *); /*proto*/
 static int __pyx_f_11libsettings_send_from_wrapper(void *, uint16_t, uint8_t, uint8_t *, uint16_t); /*proto*/
-static int __pyx_f_11libsettings_wait_init_wrapper(void *); /*proto*/
 static int __pyx_f_11libsettings_wait_wrapper(void *, int); /*proto*/
 static void __pyx_f_11libsettings_signal_wrapper(void *); /*proto*/
-static int __pyx_f_11libsettings_wait_thd_wrapper(void *, int); /*proto*/
-static void __pyx_f_11libsettings_signal_thd_wrapper(void *); /*proto*/
-static void __pyx_f_11libsettings_lock_wrapper(void *); /*proto*/
-static void __pyx_f_11libsettings_unlock_wrapper(void *); /*proto*/
 static int __pyx_f_11libsettings_register_cb_wrapper(void *, uint16_t, sbp_msg_callback_t, void *, sbp_msg_callbacks_node_t **); /*proto*/
 static int __pyx_f_11libsettings_unregister_cb_wrapper(void *, sbp_msg_callbacks_node_t **); /*proto*/
-static void __pyx_f_11libsettings_log_wrapper(int, char const *); /*proto*/
+static void __pyx_f_11libsettings_log_wrapper(int, char const *, ...); /*proto*/
 static PyObject *__pyx_unpickle___Pyx_EnumMeta__set_state(struct __pyx_obj___Pyx_EnumMeta *, PyObject *); /*proto*/
 #define __Pyx_MODULE_NAME "libsettings"
 extern int __pyx_module_is_main_libsettings;
 int __pyx_module_is_main_libsettings = 0;
 
 /* Implementation of 'libsettings' */
 static PyObject *__pyx_builtin_TypeError;
-static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_ValueError;
 static const char __pyx_k_v[] = "v";
 static const char __pyx_k__2[] = ":";
 static const char __pyx_k_02x[] = "{:02x}";
 static const char __pyx_k_SBP[] = "SBP";
 static const char __pyx_k_cls[] = "cls";
 static const char __pyx_k_dct[] = "dct";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_end[] = "end";
-static const char __pyx_k_get[] = "get";
-static const char __pyx_k_idx[] = "idx";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_res[] = "res";
 static const char __pyx_k_s_s[] = "%s.%s";
 static const char __pyx_k_set[] = "set";
 static const char __pyx_k_str[] = "__str__";
-static const char __pyx_k_Lock[] = "Lock";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_enum[] = "enum";
 static const char __pyx_k_file[] = "file";
 static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_join[] = "join";
 static const char __pyx_k_link[] = "link";
-static const char __pyx_k_lock[] = "_lock";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_repr[] = "__repr__";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_send[] = "send";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_wait[] = "wait";
 static const char __pyx_k_Event[] = "Event";
-static const char __pyx_k_ascii[] = "ascii";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_debug[] = "debug";
 static const char __pyx_k_event[] = "_event";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_print[] = "print";
-static const char __pyx_k_range[] = "range";
 static const char __pyx_k_s_s_d[] = "<%s.%s: %d>";
 static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_value[] = "value";
-static const char __pyx_k_write[] = "write";
-static const char __pyx_k_decode[] = "decode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_length[] = "length";
 static const char __pyx_k_link_2[] = "_link";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_sender[] = "sender";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_values[] = "values";
 static const char __pyx_k_IntEnum[] = "IntEnum";
-static const char __pyx_k_acquire[] = "acquire";
 static const char __pyx_k_debug_2[] = "_debug";
 static const char __pyx_k_genexpr[] = "genexpr";
 static const char __pyx_k_members[] = "__members__";
 static const char __pyx_k_parents[] = "parents";
 static const char __pyx_k_payload[] = "payload";
 static const char __pyx_k_prepare[] = "__prepare__";
-static const char __pyx_k_release[] = "release";
 static const char __pyx_k_sbp_msg[] = "sbp_msg";
 static const char __pyx_k_section[] = "section";
-static const char __pyx_k_workers[] = "workers";
 static const char __pyx_k_EnumBase[] = "EnumBase";
 static const char __pyx_k_EnumType[] = "EnumType";
 static const char __pyx_k_Settings[] = "Settings";
-static const char __pyx_k_encoding[] = "encoding";
 static const char __pyx_k_fmt_type[] = "fmt_type";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_msg_type[] = "msg_type";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_qualname[] = "__qualname__";
 static const char __pyx_k_setstate[] = "__setstate__";
-static const char __pyx_k_settings[] = "settings";
 static const char __pyx_k_SENDER_ID[] = "SENDER_ID";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_callbacks[] = "_callbacks";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_sbp_msg_2[] = "sbp.msg";
 static const char __pyx_k_sender_id[] = "sender_id";
 static const char __pyx_k_threading[] = "threading";
-static const char __pyx_k_ThreadPool[] = "ThreadPool";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_OrderedDict[] = "OrderedDict";
 static const char __pyx_k_PickleError[] = "PickleError";
-static const char __pyx_k_apply_async[] = "apply_async";
 static const char __pyx_k_collections[] = "collections";
 static const char __pyx_k_libsettings[] = "libsettings";
-static const char __pyx_k_multithread[] = "multithread";
 static const char __pyx_k_Pyx_EnumBase[] = "__Pyx_EnumBase";
 static const char __pyx_k_add_callback[] = "add_callback";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_send_wrapper[] = "send_wrapper";
 static const char __pyx_k_stringsource[] = "stringsource";
-static const char __pyx_k_read_by_index[] = "_read_by_index";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_SETTINGS_WR_OK[] = "SETTINGS_WR_OK";
 static const char __pyx_k_callback_broker[] = "_callback_broker";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_remove_callback[] = "remove_callback";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_send_from_wrapper[] = "send_from_wrapper";
 static const char __pyx_k_Pyx_EnumBase___new[] = "__Pyx_EnumBase.__new__";
 static const char __pyx_k_Pyx_EnumBase___str[] = "__Pyx_EnumBase.__str__";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_Pyx_EnumBase___repr[] = "__Pyx_EnumBase.__repr__";
 static const char __pyx_k_SETTINGS_WR_TIMEOUT[] = "SETTINGS_WR_TIMEOUT";
 static const char __pyx_k_Unknown_enum_value_s[] = "Unknown enum value: '%s'";
-static const char __pyx_k_Unsupported_type_for[] = "Unsupported type {} for {}";
-static const char __pyx_k_multiprocessing_pool[] = "multiprocessing.pool";
 static const char __pyx_k_SETTINGS_WR_READ_ONLY[] = "SETTINGS_WR_READ_ONLY";
 static const char __pyx_k_SETTINGS_WR_PARSE_FAILED[] = "SETTINGS_WR_PARSE_FAILED";
 static const char __pyx_k_SETTINGS_WR_SERVICE_FAILED[] = "SETTINGS_WR_SERVICE_FAILED";
 static const char __pyx_k_SETTINGS_WR_VALUE_REJECTED[] = "SETTINGS_WR_VALUE_REJECTED";
 static const char __pyx_k_SettingsWriteResponseCodes[] = "SettingsWriteResponseCodes";
 static const char __pyx_k_SETTINGS_WR_MODIFY_DISABLED[] = "SETTINGS_WR_MODIFY_DISABLED";
 static const char __pyx_k_pyx_unpickle___Pyx_EnumMeta[] = "__pyx_unpickle___Pyx_EnumMeta";
 static const char __pyx_k_send_wrapper_locals_genexpr[] = "send_wrapper.<locals>.genexpr";
 static const char __pyx_k_SETTINGS_WR_SETTING_REJECTED[] = "SETTINGS_WR_SETTING_REJECTED";
 static const char __pyx_k_callback_broker_locals_genexpr[] = "_callback_broker.<locals>.genexpr";
 static const char __pyx_k_Callback_not_registered_for_mess[] = "Callback not registered for message type {}";
-static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())";
+static const char __pyx_k_Incompatible_checksums_s_vs_0xd4[] = "Incompatible checksums (%s vs 0xd41d8cd = ())";
 static const char __pyx_k_self_c_api_self_ctx_cannot_be_co[] = "self.c_api,self.ctx cannot be converted to a Python object for pickling";
 static const char __pyx_k_send_from_wrapper_locals_genexpr[] = "send_from_wrapper.<locals>.genexpr";
 static PyObject *__pyx_kp_s_02x;
 static PyObject *__pyx_kp_s_Callback_not_registered_for_mess;
 static PyObject *__pyx_n_s_EnumBase;
 static PyObject *__pyx_n_s_EnumType;
 static PyObject *__pyx_n_s_Event;
-static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xd4;
 static PyObject *__pyx_n_s_IntEnum;
-static PyObject *__pyx_n_s_Lock;
 static PyObject *__pyx_n_s_OrderedDict;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_Pyx_EnumBase;
 static PyObject *__pyx_n_s_Pyx_EnumBase___new;
 static PyObject *__pyx_n_s_Pyx_EnumBase___repr;
 static PyObject *__pyx_n_s_Pyx_EnumBase___str;
 static PyObject *__pyx_n_s_SBP;
@@ -2049,66 +1788,54 @@
 static PyObject *__pyx_n_s_SETTINGS_WR_READ_ONLY;
 static PyObject *__pyx_n_s_SETTINGS_WR_SERVICE_FAILED;
 static PyObject *__pyx_n_s_SETTINGS_WR_SETTING_REJECTED;
 static PyObject *__pyx_n_s_SETTINGS_WR_TIMEOUT;
 static PyObject *__pyx_n_s_SETTINGS_WR_VALUE_REJECTED;
 static PyObject *__pyx_n_s_Settings;
 static PyObject *__pyx_n_s_SettingsWriteResponseCodes;
-static PyObject *__pyx_n_s_ThreadPool;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unknown_enum_value_s;
-static PyObject *__pyx_kp_s_Unsupported_type_for;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_kp_s__2;
-static PyObject *__pyx_n_s_acquire;
 static PyObject *__pyx_n_s_add_callback;
-static PyObject *__pyx_n_s_apply_async;
 static PyObject *__pyx_n_s_args;
-static PyObject *__pyx_n_s_ascii;
 static PyObject *__pyx_n_s_callback_broker;
 static PyObject *__pyx_n_s_callback_broker_locals_genexpr;
 static PyObject *__pyx_n_s_callbacks;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
 static PyObject *__pyx_n_s_cls;
 static PyObject *__pyx_n_s_collections;
 static PyObject *__pyx_n_s_dct;
 static PyObject *__pyx_n_s_debug;
 static PyObject *__pyx_n_s_debug_2;
-static PyObject *__pyx_n_s_decode;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_doc;
-static PyObject *__pyx_n_s_encoding;
 static PyObject *__pyx_n_s_end;
 static PyObject *__pyx_n_s_enum;
 static PyObject *__pyx_n_s_event;
 static PyObject *__pyx_n_s_file;
 static PyObject *__pyx_n_s_fmt_type;
 static PyObject *__pyx_n_s_format;
 static PyObject *__pyx_n_s_genexpr;
-static PyObject *__pyx_n_s_get;
 static PyObject *__pyx_n_s_getstate;
-static PyObject *__pyx_n_s_idx;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_s_items;
 static PyObject *__pyx_n_s_join;
 static PyObject *__pyx_n_s_length;
 static PyObject *__pyx_n_s_libsettings;
 static PyObject *__pyx_n_s_link;
 static PyObject *__pyx_n_s_link_2;
-static PyObject *__pyx_n_s_lock;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_members;
 static PyObject *__pyx_n_s_metaclass;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_msg_type;
-static PyObject *__pyx_n_s_multiprocessing_pool;
-static PyObject *__pyx_n_s_multithread;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_n_s_parents;
 static PyObject *__pyx_n_s_payload;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_prepare;
@@ -2116,20 +1843,17 @@
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle___Pyx_EnumMeta;
 static PyObject *__pyx_n_s_qualname;
-static PyObject *__pyx_n_s_range;
-static PyObject *__pyx_n_s_read_by_index;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
-static PyObject *__pyx_n_s_release;
 static PyObject *__pyx_n_s_remove_callback;
 static PyObject *__pyx_n_s_repr;
 static PyObject *__pyx_n_s_res;
 static PyObject *__pyx_kp_s_s_s;
 static PyObject *__pyx_kp_s_s_s_d;
 static PyObject *__pyx_n_s_sbp_msg;
 static PyObject *__pyx_n_s_sbp_msg_2;
@@ -2142,45 +1866,39 @@
 static PyObject *__pyx_n_s_send_wrapper;
 static PyObject *__pyx_n_s_send_wrapper_locals_genexpr;
 static PyObject *__pyx_n_s_sender;
 static PyObject *__pyx_n_s_sender_id;
 static PyObject *__pyx_n_s_set;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
-static PyObject *__pyx_n_s_settings;
 static PyObject *__pyx_n_s_str;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_threading;
 static PyObject *__pyx_n_s_throw;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_v;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_n_s_values;
 static PyObject *__pyx_n_s_wait;
-static PyObject *__pyx_n_s_workers;
-static PyObject *__pyx_n_s_write;
 static int __pyx_pf_11libsettings_8Settings___init__(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_link, PyObject *__pyx_v_sender_id, PyObject *__pyx_v_debug); /* proto */
 static PyObject *__pyx_pf_11libsettings_8Settings_2destroy(struct __pyx_obj_11libsettings_Settings *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_11libsettings_8Settings_4write(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_section, PyObject *__pyx_v_name, PyObject *__pyx_v_value, PyObject *__pyx_v_encoding, PyObject *__pyx_v_multithread); /* proto */
-static PyObject *__pyx_pf_11libsettings_8Settings_6write_all(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_settings, PyObject *__pyx_v_encoding, PyObject *__pyx_v_workers); /* proto */
-static PyObject *__pyx_pf_11libsettings_8Settings_8read(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_section, PyObject *__pyx_v_name, PyObject *__pyx_v_encoding); /* proto */
-static PyObject *__pyx_pf_11libsettings_8Settings_10_read_by_index(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_idx, PyObject *__pyx_v_encoding); /* proto */
-static PyObject *__pyx_pf_11libsettings_8Settings_12read_all(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_encoding, PyObject *__pyx_v_workers); /* proto */
+static PyObject *__pyx_pf_11libsettings_8Settings_4write(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_section, PyObject *__pyx_v_name, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_11libsettings_8Settings_6read(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_section, PyObject *__pyx_v_name); /* proto */
+static PyObject *__pyx_pf_11libsettings_8Settings_8read_all(struct __pyx_obj_11libsettings_Settings *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_11libsettings_8Settings_16_callback_broker_genexpr(PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_11libsettings_8Settings_14_callback_broker(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_sbp_msg, CYTHON_UNUSED PyObject *__pyx_v_metadata); /* proto */
+static PyObject *__pyx_pf_11libsettings_8Settings_10_callback_broker(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_sbp_msg, CYTHON_UNUSED PyObject *__pyx_v_metadata); /* proto */
 static PyObject *__pyx_pf_11libsettings_8Settings_10_callbacks___get__(struct __pyx_obj_11libsettings_Settings *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_11libsettings_8Settings_6_event___get__(struct __pyx_obj_11libsettings_Settings *__pyx_v_self); /* proto */
 static int __pyx_pf_11libsettings_8Settings_6_event_2__set__(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_11libsettings_8Settings_6_event_4__del__(struct __pyx_obj_11libsettings_Settings *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_11libsettings_8Settings_5_link___get__(struct __pyx_obj_11libsettings_Settings *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_11libsettings_8Settings_6_debug___get__(struct __pyx_obj_11libsettings_Settings *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_11libsettings_8Settings_5_lock___get__(struct __pyx_obj_11libsettings_Settings *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_11libsettings_8Settings_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_11libsettings_Settings *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_11libsettings_8Settings_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_11libsettings_Settings *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_11libsettings_8Settings_12__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_11libsettings_Settings *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_11libsettings_8Settings_14__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_11libsettings_Settings *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_11libsettings_12send_wrapper_genexpr(PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_11libsettings_17send_from_wrapper_genexpr(PyObject *__pyx_self); /* proto */
 static int __pyx_pf_8EnumBase_14__Pyx_EnumMeta___init__(struct __pyx_obj___Pyx_EnumMeta *__pyx_v_cls, PyObject *__pyx_v_name, PyObject *__pyx_v_parents, PyObject *__pyx_v_dct); /* proto */
 static PyObject *__pyx_pf_8EnumBase_14__Pyx_EnumMeta_2__iter__(struct __pyx_obj___Pyx_EnumMeta *__pyx_v_cls); /* proto */
 static PyObject *__pyx_pf_8EnumBase_14__Pyx_EnumMeta_4__getitem__(struct __pyx_obj___Pyx_EnumMeta *__pyx_v_cls, PyObject *__pyx_v_name); /* proto */
 static PyObject *__pyx_pf_8EnumBase_14__Pyx_EnumMeta_6__reduce_cython__(struct __pyx_obj___Pyx_EnumMeta *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8EnumBase_14__Pyx_EnumMeta_8__setstate_cython__(struct __pyx_obj___Pyx_EnumMeta *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
@@ -2192,51 +1910,43 @@
 static PyObject *__pyx_tp_new_11libsettings___pyx_scope_struct___callback_broker(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_11libsettings___pyx_scope_struct_1_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_11libsettings___pyx_scope_struct_3_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_11libsettings___pyx_scope_struct_5_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new___Pyx_EnumMeta(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_int_0;
-static PyObject *__pyx_int_10;
 static PyObject *__pyx_int_222419149;
-static PyObject *__pyx_int_228825662;
-static PyObject *__pyx_int_238750788;
 static PyObject *__pyx_k_;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__6;
+static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_tuple__11;
-static PyObject *__pyx_tuple__13;
-static PyObject *__pyx_codeobj__7;
-static PyObject *__pyx_codeobj__10;
-static PyObject *__pyx_codeobj__12;
-static PyObject *__pyx_codeobj__14;
+static PyObject *__pyx_tuple__10;
+static PyObject *__pyx_tuple__12;
+static PyObject *__pyx_codeobj__6;
+static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_codeobj__11;
+static PyObject *__pyx_codeobj__13;
 /* Late includes */
 
-/* "libsettings.pyx":136
- *     cdef readonly object _lock
+/* "libsettings.pyx":128
+ *     cdef readonly object _debug
  * 
  *     def __init__(self, link, sender_id=SENDER_ID, debug=False):             # <<<<<<<<<<<<<<
  *         self.c_api.ctx = <void *>self
  *         self.c_api.send = &send_wrapper
  */
 
 /* Python wrapper */
 static int __pyx_pw_11libsettings_8Settings_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_11libsettings_8Settings_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_link = 0;
   PyObject *__pyx_v_sender_id = 0;
   PyObject *__pyx_v_debug = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_link,&__pyx_n_s_sender_id,&__pyx_n_s_debug,0};
     PyObject* values[3] = {0,0,0};
     values[1] = __pyx_k_;
@@ -2269,15 +1979,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_debug);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 136, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(1, 128, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -2288,15 +1998,15 @@
     }
     __pyx_v_link = values[0];
     __pyx_v_sender_id = values[1];
     __pyx_v_debug = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 136, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 128, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("libsettings.Settings.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_11libsettings_8Settings___init__(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self), __pyx_v_link, __pyx_v_sender_id, __pyx_v_debug);
 
@@ -2306,242 +2016,169 @@
 }
 
 static int __pyx_pf_11libsettings_8Settings___init__(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_link, PyObject *__pyx_v_sender_id, PyObject *__pyx_v_debug) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   uint16_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "libsettings.pyx":137
+  /* "libsettings.pyx":129
  * 
  *     def __init__(self, link, sender_id=SENDER_ID, debug=False):
  *         self.c_api.ctx = <void *>self             # <<<<<<<<<<<<<<
  *         self.c_api.send = &send_wrapper
  *         self.c_api.send_from = &send_from_wrapper
  */
   __pyx_v_self->c_api.ctx = ((void *)__pyx_v_self);
 
-  /* "libsettings.pyx":138
+  /* "libsettings.pyx":130
  *     def __init__(self, link, sender_id=SENDER_ID, debug=False):
  *         self.c_api.ctx = <void *>self
  *         self.c_api.send = &send_wrapper             # <<<<<<<<<<<<<<
  *         self.c_api.send_from = &send_from_wrapper
- *         self.c_api.wait_init = &wait_init_wrapper
+ *         self.c_api.wait = &wait_wrapper
  */
   __pyx_v_self->c_api.send = (&__pyx_f_11libsettings_send_wrapper);
 
-  /* "libsettings.pyx":139
+  /* "libsettings.pyx":131
  *         self.c_api.ctx = <void *>self
  *         self.c_api.send = &send_wrapper
  *         self.c_api.send_from = &send_from_wrapper             # <<<<<<<<<<<<<<
- *         self.c_api.wait_init = &wait_init_wrapper
  *         self.c_api.wait = &wait_wrapper
+ *         self.c_api.signal = &signal_wrapper
  */
   __pyx_v_self->c_api.send_from = (&__pyx_f_11libsettings_send_from_wrapper);
 
-  /* "libsettings.pyx":140
+  /* "libsettings.pyx":132
  *         self.c_api.send = &send_wrapper
  *         self.c_api.send_from = &send_from_wrapper
- *         self.c_api.wait_init = &wait_init_wrapper             # <<<<<<<<<<<<<<
- *         self.c_api.wait = &wait_wrapper
- *         self.c_api.signal = &signal_wrapper
- */
-  __pyx_v_self->c_api.wait_init = (&__pyx_f_11libsettings_wait_init_wrapper);
-
-  /* "libsettings.pyx":141
- *         self.c_api.send_from = &send_from_wrapper
- *         self.c_api.wait_init = &wait_init_wrapper
  *         self.c_api.wait = &wait_wrapper             # <<<<<<<<<<<<<<
  *         self.c_api.signal = &signal_wrapper
- *         self.c_api.wait_thd = &wait_thd_wrapper
+ *         self.c_api.register_cb = &register_cb_wrapper
  */
   __pyx_v_self->c_api.wait = (&__pyx_f_11libsettings_wait_wrapper);
 
-  /* "libsettings.pyx":142
- *         self.c_api.wait_init = &wait_init_wrapper
+  /* "libsettings.pyx":133
+ *         self.c_api.send_from = &send_from_wrapper
  *         self.c_api.wait = &wait_wrapper
  *         self.c_api.signal = &signal_wrapper             # <<<<<<<<<<<<<<
- *         self.c_api.wait_thd = &wait_thd_wrapper
- *         self.c_api.signal_thd = &signal_thd_wrapper
+ *         self.c_api.register_cb = &register_cb_wrapper
+ *         self.c_api.unregister_cb = &unregister_cb_wrapper
  */
   __pyx_v_self->c_api.signal = (&__pyx_f_11libsettings_signal_wrapper);
 
-  /* "libsettings.pyx":143
+  /* "libsettings.pyx":134
  *         self.c_api.wait = &wait_wrapper
  *         self.c_api.signal = &signal_wrapper
- *         self.c_api.wait_thd = &wait_thd_wrapper             # <<<<<<<<<<<<<<
- *         self.c_api.signal_thd = &signal_thd_wrapper
- *         self.c_api.lock = &lock_wrapper
- */
-  __pyx_v_self->c_api.wait_thd = (&__pyx_f_11libsettings_wait_thd_wrapper);
-
-  /* "libsettings.pyx":144
- *         self.c_api.signal = &signal_wrapper
- *         self.c_api.wait_thd = &wait_thd_wrapper
- *         self.c_api.signal_thd = &signal_thd_wrapper             # <<<<<<<<<<<<<<
- *         self.c_api.lock = &lock_wrapper
- *         self.c_api.unlock = &unlock_wrapper
- */
-  __pyx_v_self->c_api.signal_thd = (&__pyx_f_11libsettings_signal_thd_wrapper);
-
-  /* "libsettings.pyx":145
- *         self.c_api.wait_thd = &wait_thd_wrapper
- *         self.c_api.signal_thd = &signal_thd_wrapper
- *         self.c_api.lock = &lock_wrapper             # <<<<<<<<<<<<<<
- *         self.c_api.unlock = &unlock_wrapper
- *         self.c_api.register_cb = &register_cb_wrapper
- */
-  __pyx_v_self->c_api.lock = (&__pyx_f_11libsettings_lock_wrapper);
-
-  /* "libsettings.pyx":146
- *         self.c_api.signal_thd = &signal_thd_wrapper
- *         self.c_api.lock = &lock_wrapper
- *         self.c_api.unlock = &unlock_wrapper             # <<<<<<<<<<<<<<
- *         self.c_api.register_cb = &register_cb_wrapper
- *         self.c_api.unregister_cb = &unregister_cb_wrapper
- */
-  __pyx_v_self->c_api.unlock = (&__pyx_f_11libsettings_unlock_wrapper);
-
-  /* "libsettings.pyx":147
- *         self.c_api.lock = &lock_wrapper
- *         self.c_api.unlock = &unlock_wrapper
  *         self.c_api.register_cb = &register_cb_wrapper             # <<<<<<<<<<<<<<
  *         self.c_api.unregister_cb = &unregister_cb_wrapper
- *         self.c_api.log_preformatted = log_wrapper
+ *         self.c_api.log = log_wrapper
  */
   __pyx_v_self->c_api.register_cb = (&__pyx_f_11libsettings_register_cb_wrapper);
 
-  /* "libsettings.pyx":148
- *         self.c_api.unlock = &unlock_wrapper
+  /* "libsettings.pyx":135
+ *         self.c_api.signal = &signal_wrapper
  *         self.c_api.register_cb = &register_cb_wrapper
  *         self.c_api.unregister_cb = &unregister_cb_wrapper             # <<<<<<<<<<<<<<
- *         self.c_api.log_preformatted = log_wrapper
- * 
+ *         self.c_api.log = log_wrapper
+ *         self.c_api.log_preformat = True
  */
   __pyx_v_self->c_api.unregister_cb = (&__pyx_f_11libsettings_unregister_cb_wrapper);
 
-  /* "libsettings.pyx":149
+  /* "libsettings.pyx":136
  *         self.c_api.register_cb = &register_cb_wrapper
  *         self.c_api.unregister_cb = &unregister_cb_wrapper
- *         self.c_api.log_preformatted = log_wrapper             # <<<<<<<<<<<<<<
+ *         self.c_api.log = log_wrapper             # <<<<<<<<<<<<<<
+ *         self.c_api.log_preformat = True
+ * 
+ */
+  __pyx_v_self->c_api.log = __pyx_f_11libsettings_log_wrapper;
+
+  /* "libsettings.pyx":137
+ *         self.c_api.unregister_cb = &unregister_cb_wrapper
+ *         self.c_api.log = log_wrapper
+ *         self.c_api.log_preformat = True             # <<<<<<<<<<<<<<
  * 
  *         self.ctx = settings_create(sender_id, &self.c_api)
  */
-  __pyx_v_self->c_api.log_preformatted = __pyx_f_11libsettings_log_wrapper;
+  __pyx_v_self->c_api.log_preformat = 1;
 
-  /* "libsettings.pyx":151
- *         self.c_api.log_preformatted = log_wrapper
+  /* "libsettings.pyx":139
+ *         self.c_api.log_preformat = True
  * 
  *         self.ctx = settings_create(sender_id, &self.c_api)             # <<<<<<<<<<<<<<
  * 
  *         self._link = link
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_sender_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_sender_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 139, __pyx_L1_error)
   __pyx_v_self->ctx = settings_create(__pyx_t_1, (&__pyx_v_self->c_api));
 
-  /* "libsettings.pyx":153
+  /* "libsettings.pyx":141
  *         self.ctx = settings_create(sender_id, &self.c_api)
  * 
  *         self._link = link             # <<<<<<<<<<<<<<
  * 
  *         self._debug = debug
  */
   __Pyx_INCREF(__pyx_v_link);
   __Pyx_GIVEREF(__pyx_v_link);
   __Pyx_GOTREF(__pyx_v_self->_link);
   __Pyx_DECREF(__pyx_v_self->_link);
   __pyx_v_self->_link = __pyx_v_link;
 
-  /* "libsettings.pyx":155
+  /* "libsettings.pyx":143
  *         self._link = link
  * 
  *         self._debug = debug             # <<<<<<<<<<<<<<
  * 
- *         self._lock = Lock()
+ *         self._callbacks = {}
  */
   __Pyx_INCREF(__pyx_v_debug);
   __Pyx_GIVEREF(__pyx_v_debug);
   __Pyx_GOTREF(__pyx_v_self->_debug);
   __Pyx_DECREF(__pyx_v_self->_debug);
   __pyx_v_self->_debug = __pyx_v_debug;
 
-  /* "libsettings.pyx":157
+  /* "libsettings.pyx":145
  *         self._debug = debug
  * 
- *         self._lock = Lock()             # <<<<<<<<<<<<<<
- * 
- *         self._callbacks = {}
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Lock); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GIVEREF(__pyx_t_2);
-  __Pyx_GOTREF(__pyx_v_self->_lock);
-  __Pyx_DECREF(__pyx_v_self->_lock);
-  __pyx_v_self->_lock = __pyx_t_2;
-  __pyx_t_2 = 0;
-
-  /* "libsettings.pyx":159
- *         self._lock = Lock()
- * 
  *         self._callbacks = {}             # <<<<<<<<<<<<<<
  * 
  *     def destroy(self):
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->_callbacks);
   __Pyx_DECREF(__pyx_v_self->_callbacks);
   __pyx_v_self->_callbacks = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "libsettings.pyx":136
- *     cdef readonly object _lock
+  /* "libsettings.pyx":128
+ *     cdef readonly object _debug
  * 
  *     def __init__(self, link, sender_id=SENDER_ID, debug=False):             # <<<<<<<<<<<<<<
  *         self.c_api.ctx = <void *>self
  *         self.c_api.send = &send_wrapper
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("libsettings.Settings.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":161
+/* "libsettings.pyx":147
  *         self._callbacks = {}
  * 
  *     def destroy(self):             # <<<<<<<<<<<<<<
  *         settings_destroy(&self.ctx)
  * 
  */
 
@@ -2559,73 +2196,62 @@
 }
 
 static PyObject *__pyx_pf_11libsettings_8Settings_2destroy(struct __pyx_obj_11libsettings_Settings *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("destroy", 0);
 
-  /* "libsettings.pyx":162
+  /* "libsettings.pyx":148
  * 
  *     def destroy(self):
  *         settings_destroy(&self.ctx)             # <<<<<<<<<<<<<<
  * 
- *     def write(self, section, name, value, encoding='ascii', multithread=False):
+ *     def write(self, section, name, value):
  */
   settings_destroy((&__pyx_v_self->ctx));
 
-  /* "libsettings.pyx":161
+  /* "libsettings.pyx":147
  *         self._callbacks = {}
  * 
  *     def destroy(self):             # <<<<<<<<<<<<<<
  *         settings_destroy(&self.ctx)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":164
+/* "libsettings.pyx":150
  *         settings_destroy(&self.ctx)
  * 
- *     def write(self, section, name, value, encoding='ascii', multithread=False):             # <<<<<<<<<<<<<<
- *         try:
- *             if isinstance(value, str):
+ *     def write(self, section, name, value):             # <<<<<<<<<<<<<<
+ *         return settings_write_str(self.ctx,
+ *                                   bytes(section),
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_11libsettings_8Settings_5write(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_11libsettings_8Settings_5write(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_section = 0;
   PyObject *__pyx_v_name = 0;
   PyObject *__pyx_v_value = 0;
-  PyObject *__pyx_v_encoding = 0;
-  PyObject *__pyx_v_multithread = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("write (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_section,&__pyx_n_s_name,&__pyx_n_s_value,&__pyx_n_s_encoding,&__pyx_n_s_multithread,0};
-    PyObject* values[5] = {0,0,0,0,0};
-    values[3] = ((PyObject *)__pyx_n_s_ascii);
-    values[4] = ((PyObject *)Py_False);
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_section,&__pyx_n_s_name,&__pyx_n_s_value,0};
+    PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
@@ -2636,1121 +2262,170 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_section)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("write", 0, 3, 5, 1); __PYX_ERR(0, 164, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("write", 1, 3, 3, 1); __PYX_ERR(1, 150, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("write", 0, 3, 5, 2); __PYX_ERR(0, 164, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  3:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoding);
-          if (value) { values[3] = value; kw_args--; }
-        }
-        CYTHON_FALLTHROUGH;
-        case  4:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_multithread);
-          if (value) { values[4] = value; kw_args--; }
+          __Pyx_RaiseArgtupleInvalid("write", 1, 3, 3, 2); __PYX_ERR(1, 150, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "write") < 0)) __PYX_ERR(0, 164, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "write") < 0)) __PYX_ERR(1, 150, __pyx_L3_error)
       }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+      goto __pyx_L5_argtuple_error;
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_section = values[0];
     __pyx_v_name = values[1];
     __pyx_v_value = values[2];
-    __pyx_v_encoding = values[3];
-    __pyx_v_multithread = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("write", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 164, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("write", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 150, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("libsettings.Settings.write", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_11libsettings_8Settings_4write(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self), __pyx_v_section, __pyx_v_name, __pyx_v_value, __pyx_v_encoding, __pyx_v_multithread);
+  __pyx_r = __pyx_pf_11libsettings_8Settings_4write(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self), __pyx_v_section, __pyx_v_name, __pyx_v_value);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_11libsettings_8Settings_4write(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_section, PyObject *__pyx_v_name, PyObject *__pyx_v_value, PyObject *__pyx_v_encoding, PyObject *__pyx_v_multithread) {
-  PyObject *__pyx_v_e = NULL;
-  int __pyx_v_ret;
+static PyObject *__pyx_pf_11libsettings_8Settings_4write(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_section, PyObject *__pyx_v_name, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
+  char const *__pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  int __pyx_t_5;
+  char const *__pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  PyObject *__pyx_t_9 = NULL;
-  PyObject *__pyx_t_10 = NULL;
-  PyObject *__pyx_t_11 = NULL;
-  PyObject *__pyx_t_12 = NULL;
-  int __pyx_t_13;
-  PyObject *__pyx_t_14 = NULL;
-  char const *__pyx_t_15;
-  char const *__pyx_t_16;
-  char const *__pyx_t_17;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+  char const *__pyx_t_7;
   __Pyx_RefNannySetupContext("write", 0);
-  __Pyx_INCREF(__pyx_v_value);
-
-  /* "libsettings.pyx":165
- * 
- *     def write(self, section, name, value, encoding='ascii', multithread=False):
- *         try:             # <<<<<<<<<<<<<<
- *             if isinstance(value, str):
- *                 value = bytearray(value, encoding)
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "libsettings.pyx":166
- *     def write(self, section, name, value, encoding='ascii', multithread=False):
- *         try:
- *             if isinstance(value, str):             # <<<<<<<<<<<<<<
- *                 value = bytearray(value, encoding)
- *             elif isinstance(value, int) or isinstance(value, float):
- */
-      __pyx_t_4 = PyString_Check(__pyx_v_value); 
-      __pyx_t_5 = (__pyx_t_4 != 0);
-      if (__pyx_t_5) {
-
-        /* "libsettings.pyx":167
- *         try:
- *             if isinstance(value, str):
- *                 value = bytearray(value, encoding)             # <<<<<<<<<<<<<<
- *             elif isinstance(value, int) or isinstance(value, float):
- *                 # 'ascii' will always be good enough for numeric characters
- */
-        __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 167, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_INCREF(__pyx_v_value);
-        __Pyx_GIVEREF(__pyx_v_value);
-        PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_value);
-        __Pyx_INCREF(__pyx_v_encoding);
-        __Pyx_GIVEREF(__pyx_v_encoding);
-        PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_encoding);
-        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)(&PyByteArray_Type)), __pyx_t_6, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 167, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_7);
-        __pyx_t_7 = 0;
-
-        /* "libsettings.pyx":166
- *     def write(self, section, name, value, encoding='ascii', multithread=False):
- *         try:
- *             if isinstance(value, str):             # <<<<<<<<<<<<<<
- *                 value = bytearray(value, encoding)
- *             elif isinstance(value, int) or isinstance(value, float):
- */
-        goto __pyx_L9;
-      }
-
-      /* "libsettings.pyx":168
- *             if isinstance(value, str):
- *                 value = bytearray(value, encoding)
- *             elif isinstance(value, int) or isinstance(value, float):             # <<<<<<<<<<<<<<
- *                 # 'ascii' will always be good enough for numeric characters
- *                 value = bytearray(str(value), 'ascii')
- */
-      __pyx_t_4 = PyInt_Check(__pyx_v_value); 
-      __pyx_t_8 = (__pyx_t_4 != 0);
-      if (!__pyx_t_8) {
-      } else {
-        __pyx_t_5 = __pyx_t_8;
-        goto __pyx_L10_bool_binop_done;
-      }
-      __pyx_t_8 = PyFloat_Check(__pyx_v_value); 
-      __pyx_t_4 = (__pyx_t_8 != 0);
-      __pyx_t_5 = __pyx_t_4;
-      __pyx_L10_bool_binop_done:;
-      if (__pyx_t_5) {
-
-        /* "libsettings.pyx":170
- *             elif isinstance(value, int) or isinstance(value, float):
- *                 # 'ascii' will always be good enough for numeric characters
- *                 value = bytearray(str(value), 'ascii')             # <<<<<<<<<<<<<<
- *             elif isinstance(value, unicode):
- *                 # python2 string can be 'str' or 'unicode'
- */
-        __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_v_value); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 170, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 170, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_GIVEREF(__pyx_t_7);
-        PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7);
-        __Pyx_INCREF(__pyx_n_s_ascii);
-        __Pyx_GIVEREF(__pyx_n_s_ascii);
-        PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_n_s_ascii);
-        __pyx_t_7 = 0;
-        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)(&PyByteArray_Type)), __pyx_t_6, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 170, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_7);
-        __pyx_t_7 = 0;
-
-        /* "libsettings.pyx":168
- *             if isinstance(value, str):
- *                 value = bytearray(value, encoding)
- *             elif isinstance(value, int) or isinstance(value, float):             # <<<<<<<<<<<<<<
- *                 # 'ascii' will always be good enough for numeric characters
- *                 value = bytearray(str(value), 'ascii')
- */
-        goto __pyx_L9;
-      }
 
-      /* "libsettings.pyx":171
- *                 # 'ascii' will always be good enough for numeric characters
- *                 value = bytearray(str(value), 'ascii')
- *             elif isinstance(value, unicode):             # <<<<<<<<<<<<<<
- *                 # python2 string can be 'str' or 'unicode'
- *                 value = bytearray(value, encoding)
- */
-      __pyx_t_5 = PyUnicode_Check(__pyx_v_value); 
-      __pyx_t_4 = (__pyx_t_5 != 0);
-      if (__pyx_t_4) {
-
-        /* "libsettings.pyx":173
- *             elif isinstance(value, unicode):
- *                 # python2 string can be 'str' or 'unicode'
- *                 value = bytearray(value, encoding)             # <<<<<<<<<<<<<<
- *         except:
- *             raise TypeError("Unsupported type {} for {}".format(type(value),
- */
-        __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 173, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        __Pyx_INCREF(__pyx_v_value);
-        __Pyx_GIVEREF(__pyx_v_value);
-        PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_value);
-        __Pyx_INCREF(__pyx_v_encoding);
-        __Pyx_GIVEREF(__pyx_v_encoding);
-        PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_v_encoding);
-        __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)(&PyByteArray_Type)), __pyx_t_7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 173, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_6);
-        __pyx_t_6 = 0;
-
-        /* "libsettings.pyx":171
- *                 # 'ascii' will always be good enough for numeric characters
- *                 value = bytearray(str(value), 'ascii')
- *             elif isinstance(value, unicode):             # <<<<<<<<<<<<<<
- *                 # python2 string can be 'str' or 'unicode'
- *                 value = bytearray(value, encoding)
- */
-      }
-      __pyx_L9:;
-
-      /* "libsettings.pyx":165
- * 
- *     def write(self, section, name, value, encoding='ascii', multithread=False):
- *         try:             # <<<<<<<<<<<<<<
- *             if isinstance(value, str):
- *                 value = bytearray(value, encoding)
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-
-    /* "libsettings.pyx":174
- *                 # python2 string can be 'str' or 'unicode'
- *                 value = bytearray(value, encoding)
- *         except:             # <<<<<<<<<<<<<<
- *             raise TypeError("Unsupported type {} for {}".format(type(value),
- *                                                                 value))
- */
-    /*except:*/ {
-      __Pyx_AddTraceback("libsettings.Settings.write", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_9) < 0) __PYX_ERR(0, 174, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_GOTREF(__pyx_t_9);
-
-      /* "libsettings.pyx":175
- *                 value = bytearray(value, encoding)
- *         except:
- *             raise TypeError("Unsupported type {} for {}".format(type(value),             # <<<<<<<<<<<<<<
- *                                                                 value))
- * 
- */
-      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Unsupported_type_for, __pyx_n_s_format); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 175, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_11);
-
-      /* "libsettings.pyx":176
- *         except:
- *             raise TypeError("Unsupported type {} for {}".format(type(value),
- *                                                                 value))             # <<<<<<<<<<<<<<
- * 
- *         if multithread:
- */
-      __pyx_t_12 = NULL;
-      __pyx_t_13 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
-        __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
-        if (likely(__pyx_t_12)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
-          __Pyx_INCREF(__pyx_t_12);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_11, function);
-          __pyx_t_13 = 1;
-        }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_11)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_12, ((PyObject *)Py_TYPE(__pyx_v_value)), __pyx_v_value};
-        __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_13, 2+__pyx_t_13); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 175, __pyx_L5_except_error)
-        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __Pyx_GOTREF(__pyx_t_10);
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_11)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_12, ((PyObject *)Py_TYPE(__pyx_v_value)), __pyx_v_value};
-        __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_13, 2+__pyx_t_13); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 175, __pyx_L5_except_error)
-        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __Pyx_GOTREF(__pyx_t_10);
-      } else
-      #endif
-      {
-        __pyx_t_14 = PyTuple_New(2+__pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 175, __pyx_L5_except_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        if (__pyx_t_12) {
-          __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_12); __pyx_t_12 = NULL;
-        }
-        __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_value)));
-        __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_value)));
-        PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_13, ((PyObject *)Py_TYPE(__pyx_v_value)));
-        __Pyx_INCREF(__pyx_v_value);
-        __Pyx_GIVEREF(__pyx_v_value);
-        PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_13, __pyx_v_value);
-        __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_14, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 175, __pyx_L5_except_error)
-        __Pyx_GOTREF(__pyx_t_10);
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-
-      /* "libsettings.pyx":175
- *                 value = bytearray(value, encoding)
- *         except:
- *             raise TypeError("Unsupported type {} for {}".format(type(value),             # <<<<<<<<<<<<<<
- *                                                                 value))
- * 
- */
-      __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 175, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_11);
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_Raise(__pyx_t_11, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __PYX_ERR(0, 175, __pyx_L5_except_error)
-    }
-    __pyx_L5_except_error:;
-
-    /* "libsettings.pyx":165
- * 
- *     def write(self, section, name, value, encoding='ascii', multithread=False):
- *         try:             # <<<<<<<<<<<<<<
- *             if isinstance(value, str):
- *                 value = bytearray(value, encoding)
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "libsettings.pyx":178
- *                                                                 value))
- * 
- *         if multithread:             # <<<<<<<<<<<<<<
- *             e = Event()
- *             ret = settings_write_str(self.ctx,
- */
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_multithread); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 178, __pyx_L1_error)
-  if (__pyx_t_4) {
-
-    /* "libsettings.pyx":179
- * 
- *         if multithread:
- *             e = Event()             # <<<<<<<<<<<<<<
- *             ret = settings_write_str(self.ctx,
- *                                      <void*>e,
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Event); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 179, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-        __Pyx_INCREF(__pyx_t_6);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_7, function);
-      }
-    }
-    __pyx_t_9 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 179, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_v_e = __pyx_t_9;
-    __pyx_t_9 = 0;
-
-    /* "libsettings.pyx":182
- *             ret = settings_write_str(self.ctx,
- *                                      <void*>e,
- *                                      bytearray(section, encoding),             # <<<<<<<<<<<<<<
- *                                      bytearray(name, encoding),
- *                                      value)
- */
-    __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 182, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_INCREF(__pyx_v_section);
-    __Pyx_GIVEREF(__pyx_v_section);
-    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_section);
-    __Pyx_INCREF(__pyx_v_encoding);
-    __Pyx_GIVEREF(__pyx_v_encoding);
-    PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_encoding);
-    __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)(&PyByteArray_Type)), __pyx_t_9, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 182, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_15 = __Pyx_PyObject_AsString(__pyx_t_7); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L1_error)
-
-    /* "libsettings.pyx":183
- *                                      <void*>e,
- *                                      bytearray(section, encoding),
- *                                      bytearray(name, encoding),             # <<<<<<<<<<<<<<
- *                                      value)
- *         else:
- */
-    __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 183, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_INCREF(__pyx_v_name);
-    __Pyx_GIVEREF(__pyx_v_name);
-    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_name);
-    __Pyx_INCREF(__pyx_v_encoding);
-    __Pyx_GIVEREF(__pyx_v_encoding);
-    PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_encoding);
-    __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)(&PyByteArray_Type)), __pyx_t_9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 183, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_16 = __Pyx_PyObject_AsString(__pyx_t_6); if (unlikely((!__pyx_t_16) && PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L1_error)
-
-    /* "libsettings.pyx":184
- *                                      bytearray(section, encoding),
- *                                      bytearray(name, encoding),
- *                                      value)             # <<<<<<<<<<<<<<
- *         else:
- *             ret = settings_write_str(self.ctx,
- */
-    __pyx_t_17 = __Pyx_PyObject_AsString(__pyx_v_value); if (unlikely((!__pyx_t_17) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
-
-    /* "libsettings.pyx":180
- *         if multithread:
- *             e = Event()
- *             ret = settings_write_str(self.ctx,             # <<<<<<<<<<<<<<
- *                                      <void*>e,
- *                                      bytearray(section, encoding),
- */
-    __pyx_v_ret = settings_write_str(__pyx_v_self->ctx, ((void *)__pyx_v_e), __pyx_t_15, __pyx_t_16, __pyx_t_17);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-
-    /* "libsettings.pyx":178
- *                                                                 value))
- * 
- *         if multithread:             # <<<<<<<<<<<<<<
- *             e = Event()
- *             ret = settings_write_str(self.ctx,
- */
-    goto __pyx_L14;
-  }
-
-  /* "libsettings.pyx":186
- *                                      value)
- *         else:
- *             ret = settings_write_str(self.ctx,             # <<<<<<<<<<<<<<
- *                                      NULL,
- *                                      bytearray(section, encoding),
- */
-  /*else*/ {
-
-    /* "libsettings.pyx":188
- *             ret = settings_write_str(self.ctx,
- *                                      NULL,
- *                                      bytearray(section, encoding),             # <<<<<<<<<<<<<<
- *                                      bytearray(name, encoding),
- *                                      value)
- */
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_INCREF(__pyx_v_section);
-    __Pyx_GIVEREF(__pyx_v_section);
-    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_section);
-    __Pyx_INCREF(__pyx_v_encoding);
-    __Pyx_GIVEREF(__pyx_v_encoding);
-    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_encoding);
-    __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)(&PyByteArray_Type)), __pyx_t_6, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 188, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_15 = __Pyx_PyObject_AsString(__pyx_t_7); if (unlikely((!__pyx_t_15) && PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L1_error)
-
-    /* "libsettings.pyx":189
- *                                      NULL,
- *                                      bytearray(section, encoding),
- *                                      bytearray(name, encoding),             # <<<<<<<<<<<<<<
- *                                      value)
- * 
- */
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 189, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_INCREF(__pyx_v_name);
-    __Pyx_GIVEREF(__pyx_v_name);
-    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_name);
-    __Pyx_INCREF(__pyx_v_encoding);
-    __Pyx_GIVEREF(__pyx_v_encoding);
-    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_encoding);
-    __pyx_t_9 = __Pyx_PyObject_Call(((PyObject *)(&PyByteArray_Type)), __pyx_t_6, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 189, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_16 = __Pyx_PyObject_AsString(__pyx_t_9); if (unlikely((!__pyx_t_16) && PyErr_Occurred())) __PYX_ERR(0, 189, __pyx_L1_error)
-
-    /* "libsettings.pyx":190
- *                                      bytearray(section, encoding),
- *                                      bytearray(name, encoding),
- *                                      value)             # <<<<<<<<<<<<<<
- * 
- *         return (ret, section, name, value.decode(encoding))
- */
-    __pyx_t_17 = __Pyx_PyObject_AsString(__pyx_v_value); if (unlikely((!__pyx_t_17) && PyErr_Occurred())) __PYX_ERR(0, 190, __pyx_L1_error)
-
-    /* "libsettings.pyx":186
- *                                      value)
- *         else:
- *             ret = settings_write_str(self.ctx,             # <<<<<<<<<<<<<<
- *                                      NULL,
- *                                      bytearray(section, encoding),
- */
-    __pyx_v_ret = settings_write_str(__pyx_v_self->ctx, NULL, __pyx_t_15, __pyx_t_16, __pyx_t_17);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  }
-  __pyx_L14:;
-
-  /* "libsettings.pyx":192
- *                                      value)
- * 
- *         return (ret, section, name, value.decode(encoding))             # <<<<<<<<<<<<<<
+  /* "libsettings.pyx":151
  * 
- *     def write_all(self, settings, encoding='ascii', workers=10):
+ *     def write(self, section, name, value):
+ *         return settings_write_str(self.ctx,             # <<<<<<<<<<<<<<
+ *                                   bytes(section),
+ *                                   bytes(name),
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_9 = __Pyx_PyInt_From_int(__pyx_v_ret); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 192, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_decode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_11 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_11)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_11);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
-    }
-  }
-  __pyx_t_7 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_11, __pyx_v_encoding) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_encoding);
-  __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 192, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GIVEREF(__pyx_t_9);
-  PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_9);
-  __Pyx_INCREF(__pyx_v_section);
-  __Pyx_GIVEREF(__pyx_v_section);
-  PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_section);
-  __Pyx_INCREF(__pyx_v_name);
-  __Pyx_GIVEREF(__pyx_v_name);
-  PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_v_name);
-  __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_6, 3, __pyx_t_7);
-  __pyx_t_9 = 0;
-  __pyx_t_7 = 0;
-  __pyx_r = __pyx_t_6;
-  __pyx_t_6 = 0;
-  goto __pyx_L0;
-
-  /* "libsettings.pyx":164
- *         settings_destroy(&self.ctx)
- * 
- *     def write(self, section, name, value, encoding='ascii', multithread=False):             # <<<<<<<<<<<<<<
- *         try:
- *             if isinstance(value, str):
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_XDECREF(__pyx_t_14);
-  __Pyx_AddTraceback("libsettings.Settings.write", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_e);
-  __Pyx_XDECREF(__pyx_v_value);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "libsettings.pyx":194
- *         return (ret, section, name, value.decode(encoding))
- * 
- *     def write_all(self, settings, encoding='ascii', workers=10):             # <<<<<<<<<<<<<<
- *         pool = ThreadPool(workers)
- * 
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_11libsettings_8Settings_7write_all(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_11libsettings_8Settings_7write_all(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_settings = 0;
-  PyObject *__pyx_v_encoding = 0;
-  PyObject *__pyx_v_workers = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("write_all (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_settings,&__pyx_n_s_encoding,&__pyx_n_s_workers,0};
-    PyObject* values[3] = {0,0,0};
-    values[1] = ((PyObject *)__pyx_n_s_ascii);
-    values[2] = ((PyObject *)__pyx_int_10);
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_settings)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoding);
-          if (value) { values[1] = value; kw_args--; }
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_workers);
-          if (value) { values[2] = value; kw_args--; }
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "write_all") < 0)) __PYX_ERR(0, 194, __pyx_L3_error)
-      }
-    } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_settings = values[0];
-    __pyx_v_encoding = values[1];
-    __pyx_v_workers = values[2];
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("write_all", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 194, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("libsettings.Settings.write_all", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_11libsettings_8Settings_6write_all(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self), __pyx_v_settings, __pyx_v_encoding, __pyx_v_workers);
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_11libsettings_8Settings_6write_all(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_settings, PyObject *__pyx_v_encoding, PyObject *__pyx_v_workers) {
-  PyObject *__pyx_v_pool = NULL;
-  PyObject *__pyx_v_tasks = NULL;
-  PyObject *__pyx_v_results = NULL;
-  PyObject *__pyx_v_ret = NULL;
-  PyObject *__pyx_v_result = NULL;
-  PyObject *__pyx_v_s = NULL;
-  PyObject *__pyx_v_t = NULL;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  Py_ssize_t __pyx_t_4;
-  PyObject *(*__pyx_t_5)(PyObject *);
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_t_9;
-  PyObject *__pyx_t_10 = NULL;
-  int __pyx_t_11;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("write_all", 0);
-
-  /* "libsettings.pyx":195
- * 
- *     def write_all(self, settings, encoding='ascii', workers=10):
- *         pool = ThreadPool(workers)             # <<<<<<<<<<<<<<
- * 
- *         tasks = [(s['section'], s['name'], s['value'], encoding, True) for s in settings]
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ThreadPool); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_workers) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_workers);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_pool = __pyx_t_1;
-  __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":197
- *         pool = ThreadPool(workers)
- * 
- *         tasks = [(s['section'], s['name'], s['value'], encoding, True) for s in settings]             # <<<<<<<<<<<<<<
- *         results = [pool.apply_async(self.write, t) for t in tasks]
- * 
+  /* "libsettings.pyx":152
+ *     def write(self, section, name, value):
+ *         return settings_write_str(self.ctx,
+ *                                   bytes(section),             # <<<<<<<<<<<<<<
+ *                                   bytes(name),
+ *                                   bytes(str(value)))
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_section); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (likely(PyList_CheckExact(__pyx_v_settings)) || PyTuple_CheckExact(__pyx_v_settings)) {
-    __pyx_t_2 = __pyx_v_settings; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
-    __pyx_t_5 = NULL;
-  } else {
-    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_settings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 197, __pyx_L1_error)
-  }
-  for (;;) {
-    if (likely(!__pyx_t_5)) {
-      if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
-        #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        #endif
-      } else {
-        if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
-        #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        #endif
-      }
-    } else {
-      __pyx_t_3 = __pyx_t_5(__pyx_t_2);
-      if (unlikely(!__pyx_t_3)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 197, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_3);
-    }
-    __Pyx_XDECREF_SET(__pyx_v_s, __pyx_t_3);
-    __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_s, __pyx_n_s_section); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_s, __pyx_n_s_name); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_s, __pyx_n_s_value); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 197, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = PyTuple_New(5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 197, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7);
-    __Pyx_INCREF(__pyx_v_encoding);
-    __Pyx_GIVEREF(__pyx_v_encoding);
-    PyTuple_SET_ITEM(__pyx_t_8, 3, __pyx_v_encoding);
-    __Pyx_INCREF(Py_True);
-    __Pyx_GIVEREF(Py_True);
-    PyTuple_SET_ITEM(__pyx_t_8, 4, Py_True);
-    __pyx_t_3 = 0;
-    __pyx_t_6 = 0;
-    __pyx_t_7 = 0;
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 197, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_tasks = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_t_1); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(1, 152, __pyx_L1_error)
 
-  /* "libsettings.pyx":198
- * 
- *         tasks = [(s['section'], s['name'], s['value'], encoding, True) for s in settings]
- *         results = [pool.apply_async(self.write, t) for t in tasks]             # <<<<<<<<<<<<<<
- * 
- *         ret = []
- */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_v_tasks; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
-  for (;;) {
-    if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
-    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_8 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_8); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
-    #else
-    __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 198, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    #endif
-    __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_8);
-    __pyx_t_8 = 0;
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_pool, __pyx_n_s_apply_async); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 198, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_write); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = NULL;
-    __pyx_t_9 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_7, function);
-        __pyx_t_9 = 1;
-      }
-    }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_7)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_6, __pyx_v_t};
-      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 198, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_6, __pyx_v_t};
-      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 198, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    } else
-    #endif
-    {
-      __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 198, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      if (__pyx_t_3) {
-        __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_3); __pyx_t_3 = NULL;
-      }
-      __Pyx_GIVEREF(__pyx_t_6);
-      PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_6);
-      __Pyx_INCREF(__pyx_v_t);
-      __Pyx_GIVEREF(__pyx_v_t);
-      PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_v_t);
-      __pyx_t_6 = 0;
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 198, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 198, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_results = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":200
- *         results = [pool.apply_async(self.write, t) for t in tasks]
- * 
- *         ret = []             # <<<<<<<<<<<<<<
- * 
- *         for result in results:
- */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_ret = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":202
- *         ret = []
- * 
- *         for result in results:             # <<<<<<<<<<<<<<
- *             ret.append(result.get())
- * 
- */
-  __pyx_t_1 = __pyx_v_results; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
-  for (;;) {
-    if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
-    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 202, __pyx_L1_error)
-    #else
-    __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 202, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    #endif
-    __Pyx_XDECREF_SET(__pyx_v_result, __pyx_t_2);
-    __pyx_t_2 = 0;
-
-    /* "libsettings.pyx":203
- * 
- *         for result in results:
- *             ret.append(result.get())             # <<<<<<<<<<<<<<
- * 
- *         pool.close()
- */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_result, __pyx_n_s_get); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 203, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
-      if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_7);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_ret, __pyx_t_2); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 203, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-    /* "libsettings.pyx":202
- *         ret = []
- * 
- *         for result in results:             # <<<<<<<<<<<<<<
- *             ret.append(result.get())
+  /* "libsettings.pyx":153
+ *         return settings_write_str(self.ctx,
+ *                                   bytes(section),
+ *                                   bytes(name),             # <<<<<<<<<<<<<<
+ *                                   bytes(str(value)))
  * 
  */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 153, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_t_3); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(1, 153, __pyx_L1_error)
 
-  /* "libsettings.pyx":205
- *             ret.append(result.get())
- * 
- *         pool.close()             # <<<<<<<<<<<<<<
- *         pool.join()
+  /* "libsettings.pyx":154
+ *                                   bytes(section),
+ *                                   bytes(name),
+ *                                   bytes(str(value)))             # <<<<<<<<<<<<<<
  * 
+ *     def read(self, section, name):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pool, __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 205, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_8 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_8);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 205, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_v_value); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_7 = __Pyx_PyBytes_AsString(__pyx_t_6); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 154, __pyx_L1_error)
 
-  /* "libsettings.pyx":206
- * 
- *         pool.close()
- *         pool.join()             # <<<<<<<<<<<<<<
+  /* "libsettings.pyx":151
  * 
- *         return ret
+ *     def write(self, section, name, value):
+ *         return settings_write_str(self.ctx,             # <<<<<<<<<<<<<<
+ *                                   bytes(section),
+ *                                   bytes(name),
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pool, __pyx_n_s_join); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_8 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_8);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_5 = __Pyx_PyInt_From_int(settings_write_str(__pyx_v_self->ctx, __pyx_t_2, __pyx_t_4, __pyx_t_7)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 151, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":208
- *         pool.join()
- * 
- *         return ret             # <<<<<<<<<<<<<<
- * 
- *     def read(self, section, name, encoding='ascii'):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_ret);
-  __pyx_r = __pyx_v_ret;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_r = __pyx_t_5;
+  __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "libsettings.pyx":194
- *         return (ret, section, name, value.decode(encoding))
- * 
- *     def write_all(self, settings, encoding='ascii', workers=10):             # <<<<<<<<<<<<<<
- *         pool = ThreadPool(workers)
+  /* "libsettings.pyx":150
+ *         settings_destroy(&self.ctx)
  * 
+ *     def write(self, section, name, value):             # <<<<<<<<<<<<<<
+ *         return settings_write_str(self.ctx,
+ *                                   bytes(section),
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_AddTraceback("libsettings.Settings.write_all", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("libsettings.Settings.write", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_pool);
-  __Pyx_XDECREF(__pyx_v_tasks);
-  __Pyx_XDECREF(__pyx_v_results);
-  __Pyx_XDECREF(__pyx_v_ret);
-  __Pyx_XDECREF(__pyx_v_result);
-  __Pyx_XDECREF(__pyx_v_s);
-  __Pyx_XDECREF(__pyx_v_t);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":210
- *         return ret
+/* "libsettings.pyx":156
+ *                                   bytes(str(value)))
  * 
- *     def read(self, section, name, encoding='ascii'):             # <<<<<<<<<<<<<<
+ *     def read(self, section, name):             # <<<<<<<<<<<<<<
  *         cdef char value[SETTINGS_BUFLEN]
  *         ret = settings_read_str(self.ctx,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_11libsettings_8Settings_9read(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_11libsettings_8Settings_9read(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_11libsettings_8Settings_7read(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_11libsettings_8Settings_7read(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_section = 0;
   PyObject *__pyx_v_name = 0;
-  PyObject *__pyx_v_encoding = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_section,&__pyx_n_s_name,&__pyx_n_s_encoding,0};
-    PyObject* values[3] = {0,0,0};
-    values[2] = ((PyObject *)__pyx_n_s_ascii);
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_section,&__pyx_n_s_name,0};
+    PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
@@ -3759,1210 +2434,429 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_section)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read", 0, 2, 3, 1); __PYX_ERR(0, 210, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoding);
-          if (value) { values[2] = value; kw_args--; }
+          __Pyx_RaiseArgtupleInvalid("read", 1, 2, 2, 1); __PYX_ERR(1, 156, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read") < 0)) __PYX_ERR(0, 210, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read") < 0)) __PYX_ERR(1, 156, __pyx_L3_error)
       }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_section = values[0];
     __pyx_v_name = values[1];
-    __pyx_v_encoding = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 210, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 156, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("libsettings.Settings.read", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_11libsettings_8Settings_8read(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self), __pyx_v_section, __pyx_v_name, __pyx_v_encoding);
+  __pyx_r = __pyx_pf_11libsettings_8Settings_6read(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self), __pyx_v_section, __pyx_v_name);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_11libsettings_8Settings_8read(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_section, PyObject *__pyx_v_name, PyObject *__pyx_v_encoding) {
+static PyObject *__pyx_pf_11libsettings_8Settings_6read(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_section, PyObject *__pyx_v_name) {
   char __pyx_v_value[SETTINGS_BUFLEN];
   int __pyx_v_ret;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  char const *__pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
-  char const *__pyx_t_5;
-  int __pyx_t_6;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+  char const *__pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  char const *__pyx_t_4;
+  int __pyx_t_5;
   __Pyx_RefNannySetupContext("read", 0);
 
-  /* "libsettings.pyx":213
+  /* "libsettings.pyx":159
  *         cdef char value[SETTINGS_BUFLEN]
  *         ret = settings_read_str(self.ctx,
- *                                 bytearray(section, encoding),             # <<<<<<<<<<<<<<
- *                                 bytearray(name, encoding),
+ *                                 bytes(section),             # <<<<<<<<<<<<<<
+ *                                 bytes(name),
  *                                 value,
  */
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_section); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__pyx_v_section);
-  __Pyx_GIVEREF(__pyx_v_section);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_section);
-  __Pyx_INCREF(__pyx_v_encoding);
-  __Pyx_GIVEREF(__pyx_v_encoding);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_encoding);
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)(&PyByteArray_Type)), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_t_1); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(1, 159, __pyx_L1_error)
 
-  /* "libsettings.pyx":214
+  /* "libsettings.pyx":160
  *         ret = settings_read_str(self.ctx,
- *                                 bytearray(section, encoding),
- *                                 bytearray(name, encoding),             # <<<<<<<<<<<<<<
+ *                                 bytes(section),
+ *                                 bytes(name),             # <<<<<<<<<<<<<<
  *                                 value,
  *                                 sizeof(value))
  */
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__pyx_v_name);
-  __Pyx_GIVEREF(__pyx_v_name);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_name);
-  __Pyx_INCREF(__pyx_v_encoding);
-  __Pyx_GIVEREF(__pyx_v_encoding);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_encoding);
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)(&PyByteArray_Type)), __pyx_t_1, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 214, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_t_4); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 214, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 160, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_t_3); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(1, 160, __pyx_L1_error)
 
-  /* "libsettings.pyx":212
- *     def read(self, section, name, encoding='ascii'):
+  /* "libsettings.pyx":158
+ *     def read(self, section, name):
  *         cdef char value[SETTINGS_BUFLEN]
  *         ret = settings_read_str(self.ctx,             # <<<<<<<<<<<<<<
- *                                 bytearray(section, encoding),
- *                                 bytearray(name, encoding),
+ *                                 bytes(section),
+ *                                 bytes(name),
  */
-  __pyx_v_ret = settings_read_str(__pyx_v_self->ctx, __pyx_t_3, __pyx_t_5, __pyx_v_value, (sizeof(__pyx_v_value)));
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_v_ret = settings_read_str(__pyx_v_self->ctx, __pyx_t_2, __pyx_t_4, __pyx_v_value, (sizeof(__pyx_v_value)));
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "libsettings.pyx":217
+  /* "libsettings.pyx":163
  *                                 value,
  *                                 sizeof(value))
  *         if (ret == 0):             # <<<<<<<<<<<<<<
- *             return value.decode(encoding)
+ *             return str(value)
  *         else:
  */
-  __pyx_t_6 = ((__pyx_v_ret == 0) != 0);
-  if (__pyx_t_6) {
+  __pyx_t_5 = ((__pyx_v_ret == 0) != 0);
+  if (__pyx_t_5) {
 
-    /* "libsettings.pyx":218
+    /* "libsettings.pyx":164
  *                                 sizeof(value))
  *         if (ret == 0):
- *             return value.decode(encoding)             # <<<<<<<<<<<<<<
+ *             return str(value)             # <<<<<<<<<<<<<<
  *         else:
  *             return None
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyObject_FromString(__pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_FromString(__pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 164, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_2);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
-      }
-    }
-    __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_v_encoding) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_encoding);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_r = __pyx_t_4;
-    __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "libsettings.pyx":217
+    /* "libsettings.pyx":163
  *                                 value,
  *                                 sizeof(value))
  *         if (ret == 0):             # <<<<<<<<<<<<<<
- *             return value.decode(encoding)
+ *             return str(value)
  *         else:
  */
   }
 
-  /* "libsettings.pyx":220
- *             return value.decode(encoding)
+  /* "libsettings.pyx":166
+ *             return str(value)
  *         else:
  *             return None             # <<<<<<<<<<<<<<
  * 
- *     def _read_by_index(self, idx, encoding='ascii'):
+ *     def read_all(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
   }
 
-  /* "libsettings.pyx":210
- *         return ret
+  /* "libsettings.pyx":156
+ *                                   bytes(str(value)))
  * 
- *     def read(self, section, name, encoding='ascii'):             # <<<<<<<<<<<<<<
+ *     def read(self, section, name):             # <<<<<<<<<<<<<<
  *         cdef char value[SETTINGS_BUFLEN]
  *         ret = settings_read_str(self.ctx,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("libsettings.Settings.read", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":222
+/* "libsettings.pyx":168
  *             return None
  * 
- *     def _read_by_index(self, idx, encoding='ascii'):             # <<<<<<<<<<<<<<
+ *     def read_all(self):             # <<<<<<<<<<<<<<
  *         cdef char section[SETTINGS_BUFLEN]
  *         cdef char name[SETTINGS_BUFLEN]
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_11libsettings_8Settings_11_read_by_index(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_11libsettings_8Settings_11_read_by_index(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_idx = 0;
-  PyObject *__pyx_v_encoding = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+static PyObject *__pyx_pw_11libsettings_8Settings_9read_all(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_11libsettings_8Settings_9read_all(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_read_by_index (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_idx,&__pyx_n_s_encoding,0};
-    PyObject* values[2] = {0,0};
-    values[1] = ((PyObject *)__pyx_n_s_ascii);
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_idx)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoding);
-          if (value) { values[1] = value; kw_args--; }
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_read_by_index") < 0)) __PYX_ERR(0, 222, __pyx_L3_error)
-      }
-    } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_idx = values[0];
-    __pyx_v_encoding = values[1];
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_read_by_index", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 222, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("libsettings.Settings._read_by_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_11libsettings_8Settings_10_read_by_index(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self), __pyx_v_idx, __pyx_v_encoding);
+  __Pyx_RefNannySetupContext("read_all (wrapper)", 0);
+  __pyx_r = __pyx_pf_11libsettings_8Settings_8read_all(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_11libsettings_8Settings_10_read_by_index(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_idx, PyObject *__pyx_v_encoding) {
+static PyObject *__pyx_pf_11libsettings_8Settings_8read_all(struct __pyx_obj_11libsettings_Settings *__pyx_v_self) {
   char __pyx_v_section[SETTINGS_BUFLEN];
   char __pyx_v_name[SETTINGS_BUFLEN];
   char __pyx_v_value[SETTINGS_BUFLEN];
   char __pyx_v_fmt_type[SETTINGS_BUFLEN];
-  PyObject *__pyx_v_e = NULL;
+  uint16_t __pyx_v_idx;
+  PyObject *__pyx_v_settings = NULL;
   int __pyx_v_ret;
   PyObject *__pyx_v_setting = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
-  uint16_t __pyx_t_4;
+  PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_read_by_index", 0);
+  __Pyx_RefNannySetupContext("read_all", 0);
 
-  /* "libsettings.pyx":227
+  /* "libsettings.pyx":173
  *         cdef char value[SETTINGS_BUFLEN]
  *         cdef char fmt_type[SETTINGS_BUFLEN]
- *         e = Event()             # <<<<<<<<<<<<<<
- * 
- *         ret = settings_read_by_idx(self.ctx,
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Event); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_e = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":231
- *         ret = settings_read_by_idx(self.ctx,
- *                                    <void*>e,
- *                                    idx,             # <<<<<<<<<<<<<<
- *                                    section,
- *                                    sizeof(section),
- */
-  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_idx); if (unlikely((__pyx_t_4 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 231, __pyx_L1_error)
-
-  /* "libsettings.pyx":229
- *         e = Event()
- * 
- *         ret = settings_read_by_idx(self.ctx,             # <<<<<<<<<<<<<<
- *                                    <void*>e,
- *                                    idx,
- */
-  __pyx_v_ret = settings_read_by_idx(__pyx_v_self->ctx, ((void *)__pyx_v_e), __pyx_t_4, __pyx_v_section, (sizeof(__pyx_v_section)), __pyx_v_name, (sizeof(__pyx_v_name)), __pyx_v_value, (sizeof(__pyx_v_value)), __pyx_v_fmt_type, (sizeof(__pyx_v_fmt_type)));
-
-  /* "libsettings.pyx":241
- *                                    sizeof(fmt_type))
- * 
- *         setting = None             # <<<<<<<<<<<<<<
- *         if (0 == ret):
- *             setting = {
- */
-  __Pyx_INCREF(Py_None);
-  __pyx_v_setting = ((PyObject*)Py_None);
-
-  /* "libsettings.pyx":242
- * 
- *         setting = None
- *         if (0 == ret):             # <<<<<<<<<<<<<<
- *             setting = {
- *                           'section': section.decode(encoding),
- */
-  __pyx_t_5 = ((0 == __pyx_v_ret) != 0);
-  if (__pyx_t_5) {
-
-    /* "libsettings.pyx":244
- *         if (0 == ret):
- *             setting = {
- *                           'section': section.decode(encoding),             # <<<<<<<<<<<<<<
- *                           'name': name.decode(encoding),
- *                           'value': value.decode(encoding),
- */
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_FromString(__pyx_v_section); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 244, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_decode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 244, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_v_encoding) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_encoding);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 244, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_section, __pyx_t_2) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-    /* "libsettings.pyx":245
- *             setting = {
- *                           'section': section.decode(encoding),
- *                           'name': name.decode(encoding),             # <<<<<<<<<<<<<<
- *                           'value': value.decode(encoding),
- *                           'fmt_type': fmt_type.decode(encoding),
- */
-    __pyx_t_6 = __Pyx_PyObject_FromString(__pyx_v_name); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 245, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 245, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_6);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_v_encoding) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_encoding);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_name, __pyx_t_2) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-    /* "libsettings.pyx":246
- *                           'section': section.decode(encoding),
- *                           'name': name.decode(encoding),
- *                           'value': value.decode(encoding),             # <<<<<<<<<<<<<<
- *                           'fmt_type': fmt_type.decode(encoding),
- *                       }
- */
-    __pyx_t_3 = __Pyx_PyObject_FromString(__pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_decode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 246, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_v_encoding) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_encoding);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_value, __pyx_t_2) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-    /* "libsettings.pyx":247
- *                           'name': name.decode(encoding),
- *                           'value': value.decode(encoding),
- *                           'fmt_type': fmt_type.decode(encoding),             # <<<<<<<<<<<<<<
- *                       }
- * 
- */
-    __pyx_t_6 = __Pyx_PyObject_FromString(__pyx_v_fmt_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 247, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_6);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_v_encoding) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_encoding);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_fmt_type, __pyx_t_2) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF_SET(__pyx_v_setting, ((PyObject*)__pyx_t_1));
-    __pyx_t_1 = 0;
-
-    /* "libsettings.pyx":242
- * 
- *         setting = None
- *         if (0 == ret):             # <<<<<<<<<<<<<<
- *             setting = {
- *                           'section': section.decode(encoding),
- */
-  }
-
-  /* "libsettings.pyx":250
- *                       }
- * 
- *         return (ret, setting)             # <<<<<<<<<<<<<<
- * 
- *     def read_all(self, encoding='ascii', workers=10):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
-  __Pyx_INCREF(__pyx_v_setting);
-  __Pyx_GIVEREF(__pyx_v_setting);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_setting);
-  __pyx_t_1 = 0;
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
-  goto __pyx_L0;
-
-  /* "libsettings.pyx":222
- *             return None
- * 
- *     def _read_by_index(self, idx, encoding='ascii'):             # <<<<<<<<<<<<<<
- *         cdef char section[SETTINGS_BUFLEN]
- *         cdef char name[SETTINGS_BUFLEN]
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("libsettings.Settings._read_by_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_e);
-  __Pyx_XDECREF(__pyx_v_setting);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "libsettings.pyx":252
- *         return (ret, setting)
+ *         cdef uint16_t idx = 0             # <<<<<<<<<<<<<<
  * 
- *     def read_all(self, encoding='ascii', workers=10):             # <<<<<<<<<<<<<<
  *         settings = []
- *         cdef uint16_t idx = 0
  */
+  __pyx_v_idx = 0;
 
-/* Python wrapper */
-static PyObject *__pyx_pw_11libsettings_8Settings_13read_all(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_11libsettings_8Settings_13read_all(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_encoding = 0;
-  PyObject *__pyx_v_workers = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("read_all (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_encoding,&__pyx_n_s_workers,0};
-    PyObject* values[2] = {0,0};
-    values[0] = ((PyObject *)__pyx_n_s_ascii);
-    values[1] = ((PyObject *)__pyx_int_10);
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoding);
-          if (value) { values[0] = value; kw_args--; }
-        }
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_workers);
-          if (value) { values[1] = value; kw_args--; }
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_all") < 0)) __PYX_ERR(0, 252, __pyx_L3_error)
-      }
-    } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_encoding = values[0];
-    __pyx_v_workers = values[1];
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_all", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 252, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("libsettings.Settings.read_all", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_11libsettings_8Settings_12read_all(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self), __pyx_v_encoding, __pyx_v_workers);
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_11libsettings_8Settings_12read_all(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_encoding, PyObject *__pyx_v_workers) {
-  PyObject *__pyx_v_settings = NULL;
-  uint16_t __pyx_v_idx;
-  PyObject *__pyx_v_pool = NULL;
-  PyObject *__pyx_v_ret = NULL;
-  PyObject *__pyx_v_tasks = NULL;
-  PyObject *__pyx_v_results = NULL;
-  PyObject *__pyx_v_result = NULL;
-  PyObject *__pyx_v_res = NULL;
-  PyObject *__pyx_v_i = NULL;
-  PyObject *__pyx_v_t = NULL;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  int __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  Py_ssize_t __pyx_t_7;
-  PyObject *(*__pyx_t_8)(PyObject *);
-  PyObject *__pyx_t_9 = NULL;
-  PyObject *__pyx_t_10 = NULL;
-  int __pyx_t_11;
-  PyObject *__pyx_t_12 = NULL;
-  int __pyx_t_13;
-  uint16_t __pyx_t_14;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("read_all", 0);
-
-  /* "libsettings.pyx":253
+  /* "libsettings.pyx":175
+ *         cdef uint16_t idx = 0
  * 
- *     def read_all(self, encoding='ascii', workers=10):
  *         settings = []             # <<<<<<<<<<<<<<
- *         cdef uint16_t idx = 0
- *         pool = ThreadPool(workers)
+ * 
+ *         while (True):
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_settings = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":254
- *     def read_all(self, encoding='ascii', workers=10):
- *         settings = []
- *         cdef uint16_t idx = 0             # <<<<<<<<<<<<<<
- *         pool = ThreadPool(workers)
- *         ret = None
- */
-  __pyx_v_idx = 0;
-
-  /* "libsettings.pyx":255
+  /* "libsettings.pyx":177
  *         settings = []
- *         cdef uint16_t idx = 0
- *         pool = ThreadPool(workers)             # <<<<<<<<<<<<<<
- *         ret = None
  * 
+ *         while (True):             # <<<<<<<<<<<<<<
+ *             ret = settings_read_by_idx(self.ctx,
+ *                                        idx,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ThreadPool); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_workers) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_workers);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_pool = __pyx_t_1;
-  __pyx_t_1 = 0;
+  while (1) {
 
-  /* "libsettings.pyx":256
- *         cdef uint16_t idx = 0
- *         pool = ThreadPool(workers)
- *         ret = None             # <<<<<<<<<<<<<<
+    /* "libsettings.pyx":178
  * 
- *         while (ret is None):
+ *         while (True):
+ *             ret = settings_read_by_idx(self.ctx,             # <<<<<<<<<<<<<<
+ *                                        idx,
+ *                                        section,
  */
-  __Pyx_INCREF(Py_None);
-  __pyx_v_ret = ((PyObject*)Py_None);
+    __pyx_v_ret = settings_read_by_idx(__pyx_v_self->ctx, __pyx_v_idx, __pyx_v_section, (sizeof(__pyx_v_section)), __pyx_v_name, (sizeof(__pyx_v_name)), __pyx_v_value, (sizeof(__pyx_v_value)), __pyx_v_fmt_type, (sizeof(__pyx_v_fmt_type)));
 
-  /* "libsettings.pyx":258
- *         ret = None
+    /* "libsettings.pyx":189
+ *                                        sizeof(fmt_type))
  * 
- *         while (ret is None):             # <<<<<<<<<<<<<<
- *             tasks = [(i, encoding) for i in range(idx, idx + workers)]
- *             results = [pool.apply_async(self._read_by_index, t) for t in tasks]
+ *             if (ret > 0):             # <<<<<<<<<<<<<<
+ *                 break
+ *             elif (ret < 0):
  */
-  while (1) {
-    __pyx_t_4 = (__pyx_v_ret == ((PyObject*)Py_None));
-    __pyx_t_5 = (__pyx_t_4 != 0);
-    if (!__pyx_t_5) break;
+    __pyx_t_2 = ((__pyx_v_ret > 0) != 0);
+    if (__pyx_t_2) {
 
-    /* "libsettings.pyx":259
- * 
- *         while (ret is None):
- *             tasks = [(i, encoding) for i in range(idx, idx + workers)]             # <<<<<<<<<<<<<<
- *             results = [pool.apply_async(self._read_by_index, t) for t in tasks]
+      /* "libsettings.pyx":190
  * 
+ *             if (ret > 0):
+ *                 break             # <<<<<<<<<<<<<<
+ *             elif (ret < 0):
+ *                 return []
  */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_idx); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyInt_From_uint16_t(__pyx_v_idx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = PyNumber_Add(__pyx_t_3, __pyx_v_workers); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_6);
-    __pyx_t_2 = 0;
-    __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (likely(PyList_CheckExact(__pyx_t_6)) || PyTuple_CheckExact(__pyx_t_6)) {
-      __pyx_t_3 = __pyx_t_6; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
-      __pyx_t_8 = NULL;
-    } else {
-      __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 259, __pyx_L1_error)
-    }
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    for (;;) {
-      if (likely(!__pyx_t_8)) {
-        if (likely(PyList_CheckExact(__pyx_t_3))) {
-          if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_6 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_6); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 259, __pyx_L1_error)
-          #else
-          __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 259, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_6);
-          #endif
-        } else {
-          if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_6); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 259, __pyx_L1_error)
-          #else
-          __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 259, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_6);
-          #endif
-        }
-      } else {
-        __pyx_t_6 = __pyx_t_8(__pyx_t_3);
-        if (unlikely(!__pyx_t_6)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 259, __pyx_L1_error)
-          }
-          break;
-        }
-        __Pyx_GOTREF(__pyx_t_6);
-      }
-      __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_6);
-      __pyx_t_6 = 0;
-      __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 259, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_INCREF(__pyx_v_i);
-      __Pyx_GIVEREF(__pyx_v_i);
-      PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_i);
-      __Pyx_INCREF(__pyx_v_encoding);
-      __Pyx_GIVEREF(__pyx_v_encoding);
-      PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_encoding);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 259, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_tasks, ((PyObject*)__pyx_t_1));
-    __pyx_t_1 = 0;
+      goto __pyx_L4_break;
 
-    /* "libsettings.pyx":260
- *         while (ret is None):
- *             tasks = [(i, encoding) for i in range(idx, idx + workers)]
- *             results = [pool.apply_async(self._read_by_index, t) for t in tasks]             # <<<<<<<<<<<<<<
+      /* "libsettings.pyx":189
+ *                                        sizeof(fmt_type))
  * 
- *             if not results:
+ *             if (ret > 0):             # <<<<<<<<<<<<<<
+ *                 break
+ *             elif (ret < 0):
  */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __pyx_v_tasks; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
-    for (;;) {
-      if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_6 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_6); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 260, __pyx_L1_error)
-      #else
-      __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 260, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      #endif
-      __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_6);
-      __pyx_t_6 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pool, __pyx_n_s_apply_async); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 260, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_by_index); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 260, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = NULL;
-      __pyx_t_11 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-        __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
-        if (likely(__pyx_t_10)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-          __Pyx_INCREF(__pyx_t_10);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_2, function);
-          __pyx_t_11 = 1;
-        }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_2)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_t_9, __pyx_v_t};
-        __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 260, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_t_9, __pyx_v_t};
-        __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 260, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      } else
-      #endif
-      {
-        __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 260, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        if (__pyx_t_10) {
-          __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
-        }
-        __Pyx_GIVEREF(__pyx_t_9);
-        PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_t_9);
-        __Pyx_INCREF(__pyx_v_t);
-        __Pyx_GIVEREF(__pyx_v_t);
-        PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_v_t);
-        __pyx_t_9 = 0;
-        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 260, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 260, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_results, ((PyObject*)__pyx_t_1));
-    __pyx_t_1 = 0;
 
-    /* "libsettings.pyx":262
- *             results = [pool.apply_async(self._read_by_index, t) for t in tasks]
- * 
- *             if not results:             # <<<<<<<<<<<<<<
- *                 ret = settings
+    /* "libsettings.pyx":191
+ *             if (ret > 0):
+ *                 break
+ *             elif (ret < 0):             # <<<<<<<<<<<<<<
+ *                 return []
  * 
  */
-    __pyx_t_5 = (PyList_GET_SIZE(__pyx_v_results) != 0);
-    __pyx_t_4 = ((!__pyx_t_5) != 0);
-    if (__pyx_t_4) {
+    __pyx_t_2 = ((__pyx_v_ret < 0) != 0);
+    if (__pyx_t_2) {
 
-      /* "libsettings.pyx":263
- * 
- *             if not results:
- *                 ret = settings             # <<<<<<<<<<<<<<
+      /* "libsettings.pyx":192
+ *                 break
+ *             elif (ret < 0):
+ *                 return []             # <<<<<<<<<<<<<<
  * 
- *             for result in results:
+ *             setting = {
  */
-      __Pyx_INCREF(__pyx_v_settings);
-      __Pyx_DECREF_SET(__pyx_v_ret, __pyx_v_settings);
+      __Pyx_XDECREF(__pyx_r);
+      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 192, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_r = __pyx_t_1;
+      __pyx_t_1 = 0;
+      goto __pyx_L0;
 
-      /* "libsettings.pyx":262
- *             results = [pool.apply_async(self._read_by_index, t) for t in tasks]
- * 
- *             if not results:             # <<<<<<<<<<<<<<
- *                 ret = settings
+      /* "libsettings.pyx":191
+ *             if (ret > 0):
+ *                 break
+ *             elif (ret < 0):             # <<<<<<<<<<<<<<
+ *                 return []
  * 
  */
     }
 
-    /* "libsettings.pyx":265
- *                 ret = settings
- * 
- *             for result in results:             # <<<<<<<<<<<<<<
- *                 res = result.get()
- *                 if (res[0] > 0):
- */
-    __pyx_t_1 = __pyx_v_results; __Pyx_INCREF(__pyx_t_1); __pyx_t_7 = 0;
-    for (;;) {
-      if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_1)) break;
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 265, __pyx_L1_error)
-      #else
-      __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      #endif
-      __Pyx_XDECREF_SET(__pyx_v_result, __pyx_t_3);
-      __pyx_t_3 = 0;
-
-      /* "libsettings.pyx":266
+    /* "libsettings.pyx":195
  * 
- *             for result in results:
- *                 res = result.get()             # <<<<<<<<<<<<<<
- *                 if (res[0] > 0):
- *                     ret = settings
- */
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_result, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 266, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_2 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_6);
-        if (likely(__pyx_t_2)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-          __Pyx_INCREF(__pyx_t_2);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_6, function);
-        }
-      }
-      __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
-      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 266, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_res, __pyx_t_3);
-      __pyx_t_3 = 0;
-
-      /* "libsettings.pyx":267
- *             for result in results:
- *                 res = result.get()
- *                 if (res[0] > 0):             # <<<<<<<<<<<<<<
- *                     ret = settings
- *                     break
- */
-      __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_res, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 267, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_6 = PyObject_RichCompare(__pyx_t_3, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 267, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 267, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (__pyx_t_4) {
-
-        /* "libsettings.pyx":268
- *                 res = result.get()
- *                 if (res[0] > 0):
- *                     ret = settings             # <<<<<<<<<<<<<<
- *                     break
- *                 elif (res[0] < 0):
- */
-        __Pyx_INCREF(__pyx_v_settings);
-        __Pyx_DECREF_SET(__pyx_v_ret, __pyx_v_settings);
-
-        /* "libsettings.pyx":269
- *                 if (res[0] > 0):
- *                     ret = settings
- *                     break             # <<<<<<<<<<<<<<
- *                 elif (res[0] < 0):
- *                     ret = []
- */
-        goto __pyx_L11_break;
-
-        /* "libsettings.pyx":267
- *             for result in results:
- *                 res = result.get()
- *                 if (res[0] > 0):             # <<<<<<<<<<<<<<
- *                     ret = settings
- *                     break
- */
-      }
-
-      /* "libsettings.pyx":270
- *                     ret = settings
- *                     break
- *                 elif (res[0] < 0):             # <<<<<<<<<<<<<<
- *                     ret = []
- *                     break
- */
-      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_res, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 270, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_t_6, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 270, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 270, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_4) {
-
-        /* "libsettings.pyx":271
- *                     break
- *                 elif (res[0] < 0):
- *                     ret = []             # <<<<<<<<<<<<<<
- *                     break
- * 
- */
-        __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_DECREF_SET(__pyx_v_ret, ((PyObject*)__pyx_t_3));
-        __pyx_t_3 = 0;
-
-        /* "libsettings.pyx":272
- *                 elif (res[0] < 0):
- *                     ret = []
- *                     break             # <<<<<<<<<<<<<<
- * 
- *                 settings.append(res[1])
- */
-        goto __pyx_L11_break;
-
-        /* "libsettings.pyx":270
- *                     ret = settings
- *                     break
- *                 elif (res[0] < 0):             # <<<<<<<<<<<<<<
- *                     ret = []
- *                     break
+ *             setting = {
+ *                            'section': str(section),             # <<<<<<<<<<<<<<
+ *                            'name': str(name),
+ *                            'value': str(value),
  */
-      }
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 195, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_FromString(__pyx_v_section); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 195, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 195, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_section, __pyx_t_4) < 0) __PYX_ERR(1, 195, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "libsettings.pyx":274
- *                     break
- * 
- *                 settings.append(res[1])             # <<<<<<<<<<<<<<
- *             idx += workers
- * 
+    /* "libsettings.pyx":196
+ *             setting = {
+ *                            'section': str(section),
+ *                            'name': str(name),             # <<<<<<<<<<<<<<
+ *                            'value': str(value),
+ *                            'fmt_type': str(fmt_type),
  */
-      __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_res, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_settings, __pyx_t_3); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 274, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_4 = __Pyx_PyObject_FromString(__pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 196, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 196, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_name, __pyx_t_3) < 0) __PYX_ERR(1, 195, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "libsettings.pyx":265
- *                 ret = settings
- * 
- *             for result in results:             # <<<<<<<<<<<<<<
- *                 res = result.get()
- *                 if (res[0] > 0):
+    /* "libsettings.pyx":197
+ *                            'section': str(section),
+ *                            'name': str(name),
+ *                            'value': str(value),             # <<<<<<<<<<<<<<
+ *                            'fmt_type': str(fmt_type),
+ *                       }
  */
-    }
-    __pyx_L11_break:;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_3 = __Pyx_PyObject_FromString(__pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 197, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 197, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_value, __pyx_t_4) < 0) __PYX_ERR(1, 195, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "libsettings.pyx":275
- * 
- *                 settings.append(res[1])
- *             idx += workers             # <<<<<<<<<<<<<<
+    /* "libsettings.pyx":198
+ *                            'name': str(name),
+ *                            'value': str(value),
+ *                            'fmt_type': str(fmt_type),             # <<<<<<<<<<<<<<
+ *                       }
  * 
- *         pool.close()
  */
-    __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 275, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyNumber_InPlaceAdd(__pyx_t_1, __pyx_v_workers); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 275, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_FromString(__pyx_v_fmt_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 198, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 198, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_14 = __Pyx_PyInt_As_uint16_t(__pyx_t_3); if (unlikely((__pyx_t_14 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 275, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_fmt_type, __pyx_t_3) < 0) __PYX_ERR(1, 195, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_v_idx = __pyx_t_14;
-  }
+    __Pyx_XDECREF_SET(__pyx_v_setting, ((PyObject*)__pyx_t_1));
+    __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":277
- *             idx += workers
+    /* "libsettings.pyx":201
+ *                       }
  * 
- *         pool.close()             # <<<<<<<<<<<<<<
- *         pool.join()
+ *             settings.append(setting)             # <<<<<<<<<<<<<<
+ *             idx += 1
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pool, __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
-    if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_6);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
-    }
-  }
-  __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_settings, __pyx_v_setting); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(1, 201, __pyx_L1_error)
 
-  /* "libsettings.pyx":278
+    /* "libsettings.pyx":202
  * 
- *         pool.close()
- *         pool.join()             # <<<<<<<<<<<<<<
+ *             settings.append(setting)
+ *             idx += 1             # <<<<<<<<<<<<<<
  * 
- *         return ret
+ *         return settings
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pool, __pyx_n_s_join); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 278, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
-    if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_6);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
-    }
+    __pyx_v_idx = (__pyx_v_idx + 1);
   }
-  __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 278, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_L4_break:;
 
-  /* "libsettings.pyx":280
- *         pool.join()
+  /* "libsettings.pyx":204
+ *             idx += 1
  * 
- *         return ret             # <<<<<<<<<<<<<<
+ *         return settings             # <<<<<<<<<<<<<<
  * 
  *     def _callback_broker(self, sbp_msg, **metadata):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_ret);
-  __pyx_r = __pyx_v_ret;
+  __Pyx_INCREF(__pyx_v_settings);
+  __pyx_r = __pyx_v_settings;
   goto __pyx_L0;
 
-  /* "libsettings.pyx":252
- *         return (ret, setting)
+  /* "libsettings.pyx":168
+ *             return None
  * 
- *     def read_all(self, encoding='ascii', workers=10):             # <<<<<<<<<<<<<<
- *         settings = []
- *         cdef uint16_t idx = 0
+ *     def read_all(self):             # <<<<<<<<<<<<<<
+ *         cdef char section[SETTINGS_BUFLEN]
+ *         cdef char name[SETTINGS_BUFLEN]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("libsettings.Settings.read_all", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_settings);
-  __Pyx_XDECREF(__pyx_v_pool);
-  __Pyx_XDECREF(__pyx_v_ret);
-  __Pyx_XDECREF(__pyx_v_tasks);
-  __Pyx_XDECREF(__pyx_v_results);
-  __Pyx_XDECREF(__pyx_v_result);
-  __Pyx_XDECREF(__pyx_v_res);
-  __Pyx_XDECREF(__pyx_v_i);
-  __Pyx_XDECREF(__pyx_v_t);
+  __Pyx_XDECREF(__pyx_v_setting);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":282
- *         return ret
+/* "libsettings.pyx":206
+ *         return settings
  * 
  *     def _callback_broker(self, sbp_msg, **metadata):             # <<<<<<<<<<<<<<
  *         if self._debug:
  *             print '_callback_broker', sbp_msg.msg_type
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_11libsettings_8Settings_15_callback_broker(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_11libsettings_8Settings_15_callback_broker(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_11libsettings_8Settings_11_callback_broker(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_11libsettings_8Settings_11_callback_broker(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_sbp_msg = 0;
   CYTHON_UNUSED PyObject *__pyx_v_metadata = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_callback_broker (wrapper)", 0);
   __pyx_v_metadata = PyDict_New(); if (unlikely(!__pyx_v_metadata)) return NULL;
   __Pyx_GOTREF(__pyx_v_metadata);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_sbp_msg,0};
@@ -4979,70 +2873,67 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sbp_msg)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_metadata, values, pos_args, "_callback_broker") < 0)) __PYX_ERR(0, 282, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_metadata, values, pos_args, "_callback_broker") < 0)) __PYX_ERR(1, 206, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_sbp_msg = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_callback_broker", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 282, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_callback_broker", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 206, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_metadata); __pyx_v_metadata = 0;
   __Pyx_AddTraceback("libsettings.Settings._callback_broker", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_11libsettings_8Settings_14_callback_broker(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self), __pyx_v_sbp_msg, __pyx_v_metadata);
+  __pyx_r = __pyx_pf_11libsettings_8Settings_10_callback_broker(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self), __pyx_v_sbp_msg, __pyx_v_metadata);
 
   /* function exit code */
   __Pyx_XDECREF(__pyx_v_metadata);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_11libsettings_8Settings_16_callback_broker_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "libsettings.pyx":285
+/* "libsettings.pyx":209
  *         if self._debug:
  *             print '_callback_broker', sbp_msg.msg_type
  *             print ":".join("{:02x}".format(ord(c)) for c in sbp_msg.payload)             # <<<<<<<<<<<<<<
  * 
  *         msg_type = sbp_msg.msg_type
  */
 
 static PyObject *__pyx_pf_11libsettings_8Settings_16_callback_broker_genexpr(PyObject *__pyx_self) {
   struct __pyx_obj_11libsettings___pyx_scope_struct_1_genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_11libsettings___pyx_scope_struct_1_genexpr *)__pyx_tp_new_11libsettings___pyx_scope_struct_1_genexpr(__pyx_ptype_11libsettings___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_11libsettings___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 285, __pyx_L1_error)
+    __PYX_ERR(1, 209, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_11libsettings___pyx_scope_struct___callback_broker *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_11libsettings_8Settings_16_callback_broker_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_callback_broker_locals_genexpr, __pyx_n_s_libsettings); if (unlikely(!gen)) __PYX_ERR(0, 285, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_11libsettings_8Settings_16_callback_broker_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_callback_broker_locals_genexpr, __pyx_n_s_libsettings); if (unlikely(!gen)) __PYX_ERR(1, 209, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5062,94 +2953,91 @@
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   long __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("genexpr", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 285, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_sbp_msg)) { __Pyx_RaiseClosureNameError("sbp_msg"); __PYX_ERR(0, 285, __pyx_L1_error) }
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_sbp_msg, __pyx_n_s_payload); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 209, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_sbp_msg)) { __Pyx_RaiseClosureNameError("sbp_msg"); __PYX_ERR(1, 209, __pyx_L1_error) }
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_sbp_msg, __pyx_n_s_payload); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 285, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 209, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 285, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 209, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 285, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 209, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 209, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 285, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 209, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 209, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 285, __pyx_L1_error)
+          else __PYX_ERR(1, 209, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_c);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_c, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_02x, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 285, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_02x, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 209, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_Ord(__pyx_cur_scope->__pyx_v_c); if (unlikely(__pyx_t_6 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 285, __pyx_L1_error)
-    __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 285, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Ord(__pyx_cur_scope->__pyx_v_c); if (unlikely(__pyx_t_6 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(1, 209, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 209, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_8, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_7);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 209, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     __Pyx_XGIVEREF(__pyx_t_2);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_2;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_3;
@@ -5162,15 +3050,15 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_2);
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_4 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 285, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 209, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -5188,30 +3076,29 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":282
- *         return ret
+/* "libsettings.pyx":206
+ *         return settings
  * 
  *     def _callback_broker(self, sbp_msg, **metadata):             # <<<<<<<<<<<<<<
  *         if self._debug:
  *             print '_callback_broker', sbp_msg.msg_type
  */
 
-static PyObject *__pyx_pf_11libsettings_8Settings_14_callback_broker(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_sbp_msg, CYTHON_UNUSED PyObject *__pyx_v_metadata) {
+static PyObject *__pyx_pf_11libsettings_8Settings_10_callback_broker(struct __pyx_obj_11libsettings_Settings *__pyx_v_self, PyObject *__pyx_v_sbp_msg, CYTHON_UNUSED PyObject *__pyx_v_metadata) {
   struct __pyx_obj_11libsettings___pyx_scope_struct___callback_broker *__pyx_cur_scope;
   PyObject *__pyx_v_msg_type = NULL;
   PyObject *__pyx_v_cb_data = NULL;
   PyObject *__pyx_v_k = NULL;
   PyObject *__pyx_v_v = NULL;
   sbp_msg_callback_t __pyx_v_cb;
-  PyObject *__pyx_gb_11libsettings_8Settings_16_callback_broker_2generator = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
@@ -5220,371 +3107,368 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *(*__pyx_t_9)(PyObject *);
   int __pyx_t_10;
   uintptr_t __pyx_t_11;
   uint16_t __pyx_t_12;
   uint8_t __pyx_t_13;
   uint8_t *__pyx_t_14;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_callback_broker", 0);
   __pyx_cur_scope = (struct __pyx_obj_11libsettings___pyx_scope_struct___callback_broker *)__pyx_tp_new_11libsettings___pyx_scope_struct___callback_broker(__pyx_ptype_11libsettings___pyx_scope_struct___callback_broker, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_11libsettings___pyx_scope_struct___callback_broker *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 282, __pyx_L1_error)
+    __PYX_ERR(1, 206, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_sbp_msg = __pyx_v_sbp_msg;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_sbp_msg);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_sbp_msg);
 
-  /* "libsettings.pyx":283
+  /* "libsettings.pyx":207
  * 
  *     def _callback_broker(self, sbp_msg, **metadata):
  *         if self._debug:             # <<<<<<<<<<<<<<
  *             print '_callback_broker', sbp_msg.msg_type
  *             print ":".join("{:02x}".format(ord(c)) for c in sbp_msg.payload)
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->_debug); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->_debug); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 207, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "libsettings.pyx":284
+    /* "libsettings.pyx":208
  *     def _callback_broker(self, sbp_msg, **metadata):
  *         if self._debug:
  *             print '_callback_broker', sbp_msg.msg_type             # <<<<<<<<<<<<<<
  *             print ":".join("{:02x}".format(ord(c)) for c in sbp_msg.payload)
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_sbp_msg, __pyx_n_s_msg_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 284, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_sbp_msg, __pyx_n_s_msg_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 208, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 284, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 208, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_n_s_callback_broker);
     __Pyx_GIVEREF(__pyx_n_s_callback_broker);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_callback_broker);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
     __pyx_t_2 = 0;
-    if (__Pyx_Print(0, __pyx_t_3, 1) < 0) __PYX_ERR(0, 284, __pyx_L1_error)
+    if (__Pyx_Print(0, __pyx_t_3, 1) < 0) __PYX_ERR(1, 208, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "libsettings.pyx":285
+    /* "libsettings.pyx":209
  *         if self._debug:
  *             print '_callback_broker', sbp_msg.msg_type
  *             print ":".join("{:02x}".format(ord(c)) for c in sbp_msg.payload)             # <<<<<<<<<<<<<<
  * 
  *         msg_type = sbp_msg.msg_type
  */
-    __pyx_t_3 = __pyx_pf_11libsettings_8Settings_16_callback_broker_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 285, __pyx_L1_error)
+    __pyx_t_3 = __pyx_pf_11libsettings_8Settings_16_callback_broker_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 209, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyString_Join(__pyx_kp_s__2, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 285, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyString_Join(__pyx_kp_s__2, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 209, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (__Pyx_PrintOne(0, __pyx_t_2) < 0) __PYX_ERR(0, 285, __pyx_L1_error)
+    if (__Pyx_PrintOne(0, __pyx_t_2) < 0) __PYX_ERR(1, 209, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "libsettings.pyx":283
+    /* "libsettings.pyx":207
  * 
  *     def _callback_broker(self, sbp_msg, **metadata):
  *         if self._debug:             # <<<<<<<<<<<<<<
  *             print '_callback_broker', sbp_msg.msg_type
  *             print ":".join("{:02x}".format(ord(c)) for c in sbp_msg.payload)
  */
   }
 
-  /* "libsettings.pyx":287
+  /* "libsettings.pyx":211
  *             print ":".join("{:02x}".format(ord(c)) for c in sbp_msg.payload)
  * 
  *         msg_type = sbp_msg.msg_type             # <<<<<<<<<<<<<<
  * 
  *         cb_data = None
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_sbp_msg, __pyx_n_s_msg_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_sbp_msg, __pyx_n_s_msg_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_msg_type = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "libsettings.pyx":289
+  /* "libsettings.pyx":213
  *         msg_type = sbp_msg.msg_type
  * 
  *         cb_data = None             # <<<<<<<<<<<<<<
  * 
  *         for k,v in self._callbacks.items():
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_cb_data = Py_None;
 
-  /* "libsettings.pyx":291
+  /* "libsettings.pyx":215
  *         cb_data = None
  * 
  *         for k,v in self._callbacks.items():             # <<<<<<<<<<<<<<
  *             # Only one callback per msg type
  *             if v[0] == msg_type:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_callbacks, __pyx_n_s_items); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_callbacks, __pyx_n_s_items); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 291, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
     __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 291, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 291, __pyx_L1_error)
+    __pyx_t_6 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 215, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 291, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 215, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 291, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 215, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 291, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 215, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 291, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 215, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_6(__pyx_t_3);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 291, __pyx_L1_error)
+          else __PYX_ERR(1, 215, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
       PyObject* sequence = __pyx_t_2;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 291, __pyx_L1_error)
+        __PYX_ERR(1, 215, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_7);
       #else
-      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 291, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 215, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 291, __pyx_L1_error)
+      __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 215, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       #endif
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_8 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 291, __pyx_L1_error)
+      __pyx_t_8 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 215, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_9 = Py_TYPE(__pyx_t_8)->tp_iternext;
       index = 0; __pyx_t_4 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_4)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_4);
       index = 1; __pyx_t_7 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_7)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_7);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 291, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(1, 215, __pyx_L1_error)
       __pyx_t_9 = NULL;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       goto __pyx_L7_unpacking_done;
       __pyx_L6_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_9 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 291, __pyx_L1_error)
+      __PYX_ERR(1, 215, __pyx_L1_error)
       __pyx_L7_unpacking_done:;
     }
     __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "libsettings.pyx":293
+    /* "libsettings.pyx":217
  *         for k,v in self._callbacks.items():
  *             # Only one callback per msg type
  *             if v[0] == msg_type:             # <<<<<<<<<<<<<<
  *                 cb_data = self._callbacks[k]
  *                 break
  */
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_v, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 293, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_v, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 217, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = PyObject_RichCompare(__pyx_t_2, __pyx_v_msg_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 293, __pyx_L1_error)
+    __pyx_t_7 = PyObject_RichCompare(__pyx_t_2, __pyx_v_msg_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 217, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 293, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 217, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (__pyx_t_1) {
 
-      /* "libsettings.pyx":294
+      /* "libsettings.pyx":218
  *             # Only one callback per msg type
  *             if v[0] == msg_type:
  *                 cb_data = self._callbacks[k]             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
-      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_self->_callbacks, __pyx_v_k); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 294, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_self->_callbacks, __pyx_v_k); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 218, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF_SET(__pyx_v_cb_data, __pyx_t_7);
       __pyx_t_7 = 0;
 
-      /* "libsettings.pyx":295
+      /* "libsettings.pyx":219
  *             if v[0] == msg_type:
  *                 cb_data = self._callbacks[k]
  *                 break             # <<<<<<<<<<<<<<
  * 
  *         if cb_data is None:
  */
       goto __pyx_L5_break;
 
-      /* "libsettings.pyx":293
+      /* "libsettings.pyx":217
  *         for k,v in self._callbacks.items():
  *             # Only one callback per msg type
  *             if v[0] == msg_type:             # <<<<<<<<<<<<<<
  *                 cb_data = self._callbacks[k]
  *                 break
  */
     }
 
-    /* "libsettings.pyx":291
+    /* "libsettings.pyx":215
  *         cb_data = None
  * 
  *         for k,v in self._callbacks.items():             # <<<<<<<<<<<<<<
  *             # Only one callback per msg type
  *             if v[0] == msg_type:
  */
   }
   __pyx_L5_break:;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "libsettings.pyx":297
+  /* "libsettings.pyx":221
  *                 break
  * 
  *         if cb_data is None:             # <<<<<<<<<<<<<<
  *             raise Exception("Callback not registered for message type {}".format(msg_type))
  * 
  */
   __pyx_t_1 = (__pyx_v_cb_data == Py_None);
   __pyx_t_10 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_10)) {
 
-    /* "libsettings.pyx":298
+    /* "libsettings.pyx":222
  * 
  *         if cb_data is None:
  *             raise Exception("Callback not registered for message type {}".format(msg_type))             # <<<<<<<<<<<<<<
  * 
  *         cdef sbp_msg_callback_t cb = <sbp_msg_callback_t><uintptr_t>cb_data[1]
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Callback_not_registered_for_mess, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 298, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_Callback_not_registered_for_mess, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_2, __pyx_v_msg_type) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_msg_type);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 298, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 298, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_7, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __PYX_ERR(0, 298, __pyx_L1_error)
+    __PYX_ERR(1, 222, __pyx_L1_error)
 
-    /* "libsettings.pyx":297
+    /* "libsettings.pyx":221
  *                 break
  * 
  *         if cb_data is None:             # <<<<<<<<<<<<<<
  *             raise Exception("Callback not registered for message type {}".format(msg_type))
  * 
  */
   }
 
-  /* "libsettings.pyx":300
+  /* "libsettings.pyx":224
  *             raise Exception("Callback not registered for message type {}".format(msg_type))
  * 
  *         cdef sbp_msg_callback_t cb = <sbp_msg_callback_t><uintptr_t>cb_data[1]             # <<<<<<<<<<<<<<
  *         cb(sbp_msg.sender, sbp_msg.length, bytes(sbp_msg.payload), <void*><uintptr_t>cb_data[2])
  * 
  */
-  __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_cb_data, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_cb_data, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_t_7); if (unlikely((__pyx_t_11 == ((uintptr_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_t_7); if (unlikely((__pyx_t_11 == ((uintptr_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 224, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_cb = ((sbp_msg_callback_t)((uintptr_t)__pyx_t_11));
 
-  /* "libsettings.pyx":301
+  /* "libsettings.pyx":225
  * 
  *         cdef sbp_msg_callback_t cb = <sbp_msg_callback_t><uintptr_t>cb_data[1]
  *         cb(sbp_msg.sender, sbp_msg.length, bytes(sbp_msg.payload), <void*><uintptr_t>cb_data[2])             # <<<<<<<<<<<<<<
  * 
  * cdef int send_wrapper(void *ctx, uint16_t msg_type, uint8_t length, uint8_t *payload):
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_sbp_msg, __pyx_n_s_sender); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_sbp_msg, __pyx_n_s_sender); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_12 = __Pyx_PyInt_As_uint16_t(__pyx_t_7); if (unlikely((__pyx_t_12 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyInt_As_uint16_t(__pyx_t_7); if (unlikely((__pyx_t_12 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_sbp_msg, __pyx_n_s_length); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_sbp_msg, __pyx_n_s_length); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_13 = __Pyx_PyInt_As_uint8_t(__pyx_t_7); if (unlikely((__pyx_t_13 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyInt_As_uint8_t(__pyx_t_7); if (unlikely((__pyx_t_13 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_sbp_msg, __pyx_n_s_payload); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_sbp_msg, __pyx_n_s_payload); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_14 = __Pyx_PyBytes_AsWritableUString(__pyx_t_3); if (unlikely((!__pyx_t_14) && PyErr_Occurred())) __PYX_ERR(0, 301, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_cb_data, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyBytes_AsWritableUString(__pyx_t_3); if (unlikely((!__pyx_t_14) && PyErr_Occurred())) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_cb_data, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_t_7); if (unlikely((__pyx_t_11 == ((uintptr_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_t_7); if (unlikely((__pyx_t_11 == ((uintptr_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_cb(__pyx_t_12, __pyx_t_13, __pyx_t_14, ((void *)((uintptr_t)__pyx_t_11)));
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "libsettings.pyx":282
- *         return ret
+  /* "libsettings.pyx":206
+ *         return settings
  * 
  *     def _callback_broker(self, sbp_msg, **metadata):             # <<<<<<<<<<<<<<
  *         if self._debug:
  *             print '_callback_broker', sbp_msg.msg_type
  */
 
   /* function exit code */
@@ -5599,22 +3483,21 @@
   __Pyx_AddTraceback("libsettings.Settings._callback_broker", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_msg_type);
   __Pyx_XDECREF(__pyx_v_cb_data);
   __Pyx_XDECREF(__pyx_v_k);
   __Pyx_XDECREF(__pyx_v_v);
-  __Pyx_XDECREF(__pyx_gb_11libsettings_8Settings_16_callback_broker_2generator);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":130
+/* "libsettings.pyx":123
  *     cdef settings_api_t c_api
  * 
  *     cdef readonly object _callbacks             # <<<<<<<<<<<<<<
  *     cdef public object _event
  *     cdef readonly object _link
  */
 
@@ -5643,15 +3526,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":131
+/* "libsettings.pyx":124
  * 
  *     cdef readonly object _callbacks
  *     cdef public object _event             # <<<<<<<<<<<<<<
  *     cdef readonly object _link
  *     cdef readonly object _debug
  */
 
@@ -5738,20 +3621,20 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":132
+/* "libsettings.pyx":125
  *     cdef readonly object _callbacks
  *     cdef public object _event
  *     cdef readonly object _link             # <<<<<<<<<<<<<<
  *     cdef readonly object _debug
- *     cdef readonly object _lock
+ * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_11libsettings_8Settings_5_link_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_11libsettings_8Settings_5_link_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5775,20 +3658,20 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":133
+/* "libsettings.pyx":126
  *     cdef public object _event
  *     cdef readonly object _link
  *     cdef readonly object _debug             # <<<<<<<<<<<<<<
- *     cdef readonly object _lock
  * 
+ *     def __init__(self, link, sender_id=SENDER_ID, debug=False):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_11libsettings_8Settings_6_debug_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_11libsettings_8Settings_6_debug_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5812,90 +3695,50 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":134
- *     cdef readonly object _link
- *     cdef readonly object _debug
- *     cdef readonly object _lock             # <<<<<<<<<<<<<<
- * 
- *     def __init__(self, link, sender_id=SENDER_ID, debug=False):
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_11libsettings_8Settings_5_lock_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_11libsettings_8Settings_5_lock_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_11libsettings_8Settings_5_lock___get__(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_11libsettings_8Settings_5_lock___get__(struct __pyx_obj_11libsettings_Settings *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_self->_lock);
-  __pyx_r = __pyx_v_self->_lock;
-  goto __pyx_L0;
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_11libsettings_8Settings_17__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_11libsettings_8Settings_17__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_11libsettings_8Settings_13__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_11libsettings_8Settings_13__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_11libsettings_8Settings_16__reduce_cython__(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self));
+  __pyx_r = __pyx_pf_11libsettings_8Settings_12__reduce_cython__(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_11libsettings_8Settings_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_11libsettings_Settings *__pyx_v_self) {
+static PyObject *__pyx_pf_11libsettings_8Settings_12__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_11libsettings_Settings *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 2, __pyx_L1_error)
+  __PYX_ERR(0, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  */
 
@@ -5913,45 +3756,42 @@
  * def __reduce_cython__(self):
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_11libsettings_8Settings_19__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_11libsettings_8Settings_19__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_11libsettings_8Settings_15__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_11libsettings_8Settings_15__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_11libsettings_8Settings_18__setstate_cython__(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_11libsettings_8Settings_14__setstate_cython__(((struct __pyx_obj_11libsettings_Settings *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_11libsettings_8Settings_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_11libsettings_Settings *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_11libsettings_8Settings_14__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_11libsettings_Settings *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 4, __pyx_L1_error)
+  __PYX_ERR(0, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")
  */
@@ -5963,43 +3803,40 @@
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_11libsettings_12send_wrapper_2generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "libsettings.pyx":308
+/* "libsettings.pyx":232
  *     if settings._debug:
  *         print 'send_wrapper', msg_type
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])             # <<<<<<<<<<<<<<
  * 
  *     # https://cython.readthedocs.io/en/latest/src/tutorial/strings.html
  */
 
 static PyObject *__pyx_pf_11libsettings_12send_wrapper_genexpr(PyObject *__pyx_self) {
   struct __pyx_obj_11libsettings___pyx_scope_struct_3_genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_11libsettings___pyx_scope_struct_3_genexpr *)__pyx_tp_new_11libsettings___pyx_scope_struct_3_genexpr(__pyx_ptype_11libsettings___pyx_scope_struct_3_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_11libsettings___pyx_scope_struct_3_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 308, __pyx_L1_error)
+    __PYX_ERR(1, 232, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_11libsettings_12send_wrapper_2generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_send_wrapper_locals_genexpr, __pyx_n_s_libsettings); if (unlikely(!gen)) __PYX_ERR(0, 308, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_11libsettings_12send_wrapper_2generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_send_wrapper_locals_genexpr, __pyx_n_s_libsettings); if (unlikely(!gen)) __PYX_ERR(1, 232, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6018,70 +3855,67 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *(*__pyx_t_3)(PyObject *);
   PyObject *__pyx_t_4 = NULL;
   long __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("genexpr", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 308, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_cur_scope->__pyx_outer_scope->__pyx_v_payload) + 0, __pyx_cur_scope->__pyx_outer_scope->__pyx_v_length - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 308, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 232, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_cur_scope->__pyx_outer_scope->__pyx_v_payload) + 0, __pyx_cur_scope->__pyx_outer_scope->__pyx_v_length - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 232, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 308, __pyx_L1_error)
+  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 232, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 308, __pyx_L1_error)
+  __pyx_t_3 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 232, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     {
       __pyx_t_1 = __pyx_t_3(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 308, __pyx_L1_error)
+          else __PYX_ERR(1, 232, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_c);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_c, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_02x, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 308, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_02x, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_Ord(__pyx_cur_scope->__pyx_v_c); if (unlikely(__pyx_t_5 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 308, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyInt_From_long(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 308, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Ord(__pyx_cur_scope->__pyx_v_c); if (unlikely(__pyx_t_5 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(1, 232, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_long(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 308, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     __Pyx_XGIVEREF(__pyx_t_2);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_2;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_3;
@@ -6092,15 +3926,15 @@
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_2);
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_1;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 308, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 232, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -6118,168 +3952,164 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":303
+/* "libsettings.pyx":227
  *         cb(sbp_msg.sender, sbp_msg.length, bytes(sbp_msg.payload), <void*><uintptr_t>cb_data[2])
  * 
  * cdef int send_wrapper(void *ctx, uint16_t msg_type, uint8_t length, uint8_t *payload):             # <<<<<<<<<<<<<<
  *     settings = <object>ctx
  * 
  */
 
 static int __pyx_f_11libsettings_send_wrapper(void *__pyx_v_ctx, uint16_t __pyx_v_msg_type, uint8_t __pyx_v_length, uint8_t *__pyx_v_payload) {
   struct __pyx_obj_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper *__pyx_cur_scope;
   PyObject *__pyx_v_settings = NULL;
-  PyObject *__pyx_gb_11libsettings_12send_wrapper_2generator1 = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("send_wrapper", 0);
   __pyx_cur_scope = (struct __pyx_obj_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper *)__pyx_tp_new_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper(__pyx_ptype_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 303, __pyx_L1_error)
+    __PYX_ERR(1, 227, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_length = __pyx_v_length;
   __pyx_cur_scope->__pyx_v_payload = __pyx_v_payload;
 
-  /* "libsettings.pyx":304
+  /* "libsettings.pyx":228
  * 
  * cdef int send_wrapper(void *ctx, uint16_t msg_type, uint8_t length, uint8_t *payload):
  *     settings = <object>ctx             # <<<<<<<<<<<<<<
  * 
  *     if settings._debug:
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_settings = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":306
+  /* "libsettings.pyx":230
  *     settings = <object>ctx
  * 
  *     if settings._debug:             # <<<<<<<<<<<<<<
  *         print 'send_wrapper', msg_type
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_debug_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_debug_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 230, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "libsettings.pyx":307
+    /* "libsettings.pyx":231
  * 
  *     if settings._debug:
  *         print 'send_wrapper', msg_type             # <<<<<<<<<<<<<<
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])
  * 
  */
-    __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_v_msg_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 307, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_v_msg_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 307, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_n_s_send_wrapper);
     __Pyx_GIVEREF(__pyx_n_s_send_wrapper);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_send_wrapper);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
     __pyx_t_1 = 0;
-    if (__Pyx_Print(0, __pyx_t_3, 1) < 0) __PYX_ERR(0, 307, __pyx_L1_error)
+    if (__Pyx_Print(0, __pyx_t_3, 1) < 0) __PYX_ERR(1, 231, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "libsettings.pyx":308
+    /* "libsettings.pyx":232
  *     if settings._debug:
  *         print 'send_wrapper', msg_type
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])             # <<<<<<<<<<<<<<
  * 
  *     # https://cython.readthedocs.io/en/latest/src/tutorial/strings.html
  */
-    __pyx_t_3 = __pyx_pf_11libsettings_12send_wrapper_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 308, __pyx_L1_error)
+    __pyx_t_3 = __pyx_pf_11libsettings_12send_wrapper_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyString_Join(__pyx_kp_s__2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 308, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyString_Join(__pyx_kp_s__2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (__Pyx_PrintOne(0, __pyx_t_1) < 0) __PYX_ERR(0, 308, __pyx_L1_error)
+    if (__Pyx_PrintOne(0, __pyx_t_1) < 0) __PYX_ERR(1, 232, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "libsettings.pyx":306
+    /* "libsettings.pyx":230
  *     settings = <object>ctx
  * 
  *     if settings._debug:             # <<<<<<<<<<<<<<
  *         print 'send_wrapper', msg_type
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])
  */
   }
 
-  /* "libsettings.pyx":313
+  /* "libsettings.pyx":237
  *     # See section "Passing byte strings".
  *     # Copying is needed to work around NULL bytes in settings.
  *     settings._link(SBP(msg_type=msg_type,             # <<<<<<<<<<<<<<
  *                        length=length,
  *                        payload=payload[:length])) # Performs a copy of the data
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_link_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_link_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_SBP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_SBP); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyInt_From_uint16_t(__pyx_v_msg_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_uint16_t(__pyx_v_msg_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_msg_type, __pyx_t_6) < 0) __PYX_ERR(0, 313, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_msg_type, __pyx_t_6) < 0) __PYX_ERR(1, 237, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "libsettings.pyx":314
+  /* "libsettings.pyx":238
  *     # Copying is needed to work around NULL bytes in settings.
  *     settings._link(SBP(msg_type=msg_type,
  *                        length=length,             # <<<<<<<<<<<<<<
  *                        payload=payload[:length])) # Performs a copy of the data
  *     return 0
  */
-  __pyx_t_6 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 314, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_length, __pyx_t_6) < 0) __PYX_ERR(0, 313, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_length, __pyx_t_6) < 0) __PYX_ERR(1, 237, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "libsettings.pyx":315
+  /* "libsettings.pyx":239
  *     settings._link(SBP(msg_type=msg_type,
  *                        length=length,
  *                        payload=payload[:length])) # Performs a copy of the data             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
-  __pyx_t_6 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_cur_scope->__pyx_v_payload) + 0, __pyx_cur_scope->__pyx_v_length - 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_cur_scope->__pyx_v_payload) + 0, __pyx_cur_scope->__pyx_v_length - 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_payload, __pyx_t_6) < 0) __PYX_ERR(0, 313, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_payload, __pyx_t_6) < 0) __PYX_ERR(1, 237, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "libsettings.pyx":313
+  /* "libsettings.pyx":237
  *     # See section "Passing byte strings".
  *     # Copying is needed to work around NULL bytes in settings.
  *     settings._link(SBP(msg_type=msg_type,             # <<<<<<<<<<<<<<
  *                        length=length,
  *                        payload=payload[:length])) # Performs a copy of the data
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
@@ -6288,30 +4118,30 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":316
+  /* "libsettings.pyx":240
  *                        length=length,
  *                        payload=payload[:length])) # Performs a copy of the data
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * cdef int send_from_wrapper(void *ctx, uint16_t msg_type, uint8_t length, uint8_t *payload, uint16_t sbp_sender_id):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "libsettings.pyx":303
+  /* "libsettings.pyx":227
  *         cb(sbp_msg.sender, sbp_msg.length, bytes(sbp_msg.payload), <void*><uintptr_t>cb_data[2])
  * 
  * cdef int send_wrapper(void *ctx, uint16_t msg_type, uint8_t length, uint8_t *payload):             # <<<<<<<<<<<<<<
  *     settings = <object>ctx
  * 
  */
 
@@ -6322,50 +4152,46 @@
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_WriteUnraisable("libsettings.send_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_settings);
-  __Pyx_XDECREF(__pyx_gb_11libsettings_12send_wrapper_2generator1);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_11libsettings_17send_from_wrapper_2generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "libsettings.pyx":323
+/* "libsettings.pyx":247
  *     if settings._debug:
  *         print 'send_from_wrapper', msg_type
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])             # <<<<<<<<<<<<<<
  * 
  *     settings._link(SBP(msg_type=msg_type,
  */
 
 static PyObject *__pyx_pf_11libsettings_17send_from_wrapper_genexpr(PyObject *__pyx_self) {
   struct __pyx_obj_11libsettings___pyx_scope_struct_5_genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_11libsettings___pyx_scope_struct_5_genexpr *)__pyx_tp_new_11libsettings___pyx_scope_struct_5_genexpr(__pyx_ptype_11libsettings___pyx_scope_struct_5_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_11libsettings___pyx_scope_struct_5_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 323, __pyx_L1_error)
+    __PYX_ERR(1, 247, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_11libsettings_17send_from_wrapper_2generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_send_from_wrapper_locals_genexpr, __pyx_n_s_libsettings); if (unlikely(!gen)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_11libsettings_17send_from_wrapper_2generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_send_from_wrapper_locals_genexpr, __pyx_n_s_libsettings); if (unlikely(!gen)) __PYX_ERR(1, 247, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6384,70 +4210,67 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *(*__pyx_t_3)(PyObject *);
   PyObject *__pyx_t_4 = NULL;
   long __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("genexpr", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 323, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_cur_scope->__pyx_outer_scope->__pyx_v_payload) + 0, __pyx_cur_scope->__pyx_outer_scope->__pyx_v_length - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 247, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_cur_scope->__pyx_outer_scope->__pyx_v_payload) + 0, __pyx_cur_scope->__pyx_outer_scope->__pyx_v_length - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_3 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     {
       __pyx_t_1 = __pyx_t_3(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 323, __pyx_L1_error)
+          else __PYX_ERR(1, 247, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_c);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_c, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_02x, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_02x, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_Ord(__pyx_cur_scope->__pyx_v_c); if (unlikely(__pyx_t_5 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 323, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyInt_From_long(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Ord(__pyx_cur_scope->__pyx_v_c); if (unlikely(__pyx_t_5 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(1, 247, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_long(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     __Pyx_XGIVEREF(__pyx_t_2);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_2;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_3;
@@ -6458,15 +4281,15 @@
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_2);
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_1;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 323, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 247, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -6484,180 +4307,176 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":318
+/* "libsettings.pyx":242
  *     return 0
  * 
  * cdef int send_from_wrapper(void *ctx, uint16_t msg_type, uint8_t length, uint8_t *payload, uint16_t sbp_sender_id):             # <<<<<<<<<<<<<<
  *     settings = <object>ctx
  * 
  */
 
 static int __pyx_f_11libsettings_send_from_wrapper(void *__pyx_v_ctx, uint16_t __pyx_v_msg_type, uint8_t __pyx_v_length, uint8_t *__pyx_v_payload, uint16_t __pyx_v_sbp_sender_id) {
   struct __pyx_obj_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper *__pyx_cur_scope;
   PyObject *__pyx_v_settings = NULL;
-  PyObject *__pyx_gb_11libsettings_17send_from_wrapper_2generator2 = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("send_from_wrapper", 0);
   __pyx_cur_scope = (struct __pyx_obj_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper *)__pyx_tp_new_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper(__pyx_ptype_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 318, __pyx_L1_error)
+    __PYX_ERR(1, 242, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_length = __pyx_v_length;
   __pyx_cur_scope->__pyx_v_payload = __pyx_v_payload;
 
-  /* "libsettings.pyx":319
+  /* "libsettings.pyx":243
  * 
  * cdef int send_from_wrapper(void *ctx, uint16_t msg_type, uint8_t length, uint8_t *payload, uint16_t sbp_sender_id):
  *     settings = <object>ctx             # <<<<<<<<<<<<<<
  * 
  *     if settings._debug:
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_settings = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":321
+  /* "libsettings.pyx":245
  *     settings = <object>ctx
  * 
  *     if settings._debug:             # <<<<<<<<<<<<<<
  *         print 'send_from_wrapper', msg_type
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_debug_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_debug_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 321, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 245, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "libsettings.pyx":322
+    /* "libsettings.pyx":246
  * 
  *     if settings._debug:
  *         print 'send_from_wrapper', msg_type             # <<<<<<<<<<<<<<
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])
  * 
  */
-    __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_v_msg_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_v_msg_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 322, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_n_s_send_from_wrapper);
     __Pyx_GIVEREF(__pyx_n_s_send_from_wrapper);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_send_from_wrapper);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
     __pyx_t_1 = 0;
-    if (__Pyx_Print(0, __pyx_t_3, 1) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
+    if (__Pyx_Print(0, __pyx_t_3, 1) < 0) __PYX_ERR(1, 246, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "libsettings.pyx":323
+    /* "libsettings.pyx":247
  *     if settings._debug:
  *         print 'send_from_wrapper', msg_type
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])             # <<<<<<<<<<<<<<
  * 
  *     settings._link(SBP(msg_type=msg_type,
  */
-    __pyx_t_3 = __pyx_pf_11libsettings_17send_from_wrapper_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __pyx_t_3 = __pyx_pf_11libsettings_17send_from_wrapper_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyString_Join(__pyx_kp_s__2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyString_Join(__pyx_kp_s__2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (__Pyx_PrintOne(0, __pyx_t_1) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
+    if (__Pyx_PrintOne(0, __pyx_t_1) < 0) __PYX_ERR(1, 247, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "libsettings.pyx":321
+    /* "libsettings.pyx":245
  *     settings = <object>ctx
  * 
  *     if settings._debug:             # <<<<<<<<<<<<<<
  *         print 'send_from_wrapper', msg_type
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])
  */
   }
 
-  /* "libsettings.pyx":325
+  /* "libsettings.pyx":249
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])
  * 
  *     settings._link(SBP(msg_type=msg_type,             # <<<<<<<<<<<<<<
  *                        sender=sbp_sender_id,
  *                        length=length,
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_link_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_link_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_SBP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_SBP); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyInt_From_uint16_t(__pyx_v_msg_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_uint16_t(__pyx_v_msg_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_msg_type, __pyx_t_6) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_msg_type, __pyx_t_6) < 0) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "libsettings.pyx":326
+  /* "libsettings.pyx":250
  * 
  *     settings._link(SBP(msg_type=msg_type,
  *                        sender=sbp_sender_id,             # <<<<<<<<<<<<<<
  *                        length=length,
  *                        payload=payload[:length]))
  */
-  __pyx_t_6 = __Pyx_PyInt_From_uint16_t(__pyx_v_sbp_sender_id); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_uint16_t(__pyx_v_sbp_sender_id); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_sender, __pyx_t_6) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_sender, __pyx_t_6) < 0) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "libsettings.pyx":327
+  /* "libsettings.pyx":251
  *     settings._link(SBP(msg_type=msg_type,
  *                        sender=sbp_sender_id,
  *                        length=length,             # <<<<<<<<<<<<<<
  *                        payload=payload[:length]))
  *     return 0
  */
-  __pyx_t_6 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_length, __pyx_t_6) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_length, __pyx_t_6) < 0) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "libsettings.pyx":328
+  /* "libsettings.pyx":252
  *                        sender=sbp_sender_id,
  *                        length=length,
  *                        payload=payload[:length]))             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
-  __pyx_t_6 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_cur_scope->__pyx_v_payload) + 0, __pyx_cur_scope->__pyx_v_length - 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_cur_scope->__pyx_v_payload) + 0, __pyx_cur_scope->__pyx_v_length - 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_payload, __pyx_t_6) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_payload, __pyx_t_6) < 0) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "libsettings.pyx":325
+  /* "libsettings.pyx":249
  *         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])
  * 
  *     settings._link(SBP(msg_type=msg_type,             # <<<<<<<<<<<<<<
  *                        sender=sbp_sender_id,
  *                        length=length,
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
@@ -6666,30 +4485,30 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":329
+  /* "libsettings.pyx":253
  *                        length=length,
  *                        payload=payload[:length]))
  *     return 0             # <<<<<<<<<<<<<<
  * 
- * cdef int wait_init_wrapper(void *ctx):
+ * cdef int wait_wrapper(void *ctx, int timeout_ms):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "libsettings.pyx":318
+  /* "libsettings.pyx":242
  *     return 0
  * 
  * cdef int send_from_wrapper(void *ctx, uint16_t msg_type, uint8_t length, uint8_t *payload, uint16_t sbp_sender_id):             # <<<<<<<<<<<<<<
  *     settings = <object>ctx
  * 
  */
 
@@ -6700,217 +4519,158 @@
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_WriteUnraisable("libsettings.send_from_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_settings);
-  __Pyx_XDECREF(__pyx_gb_11libsettings_17send_from_wrapper_2generator2);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":331
+/* "libsettings.pyx":255
  *     return 0
  * 
- * cdef int wait_init_wrapper(void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int wait_wrapper(void *ctx, int timeout_ms):             # <<<<<<<<<<<<<<
  *     settings = <object>ctx
  *     settings._event = Event()
  */
 
-static int __pyx_f_11libsettings_wait_init_wrapper(void *__pyx_v_ctx) {
+static int __pyx_f_11libsettings_wait_wrapper(void *__pyx_v_ctx, int __pyx_v_timeout_ms) {
   PyObject *__pyx_v_settings = NULL;
+  PyObject *__pyx_v_res = NULL;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("wait_init_wrapper", 0);
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
+  __Pyx_RefNannySetupContext("wait_wrapper", 0);
 
-  /* "libsettings.pyx":332
+  /* "libsettings.pyx":256
  * 
- * cdef int wait_init_wrapper(void *ctx):
+ * cdef int wait_wrapper(void *ctx, int timeout_ms):
  *     settings = <object>ctx             # <<<<<<<<<<<<<<
  *     settings._event = Event()
- * 
+ *     res = settings._event.wait(timeout_ms / 1000.0)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_settings = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":333
- * cdef int wait_init_wrapper(void *ctx):
+  /* "libsettings.pyx":257
+ * cdef int wait_wrapper(void *ctx, int timeout_ms):
  *     settings = <object>ctx
  *     settings._event = Event()             # <<<<<<<<<<<<<<
+ *     res = settings._event.wait(timeout_ms / 1000.0)
  * 
- * cdef int wait_wrapper(void *ctx, int timeout_ms):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Event); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Event); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_settings, __pyx_n_s_event, __pyx_t_1) < 0) __PYX_ERR(0, 333, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_settings, __pyx_n_s_event, __pyx_t_1) < 0) __PYX_ERR(1, 257, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":331
- *     return 0
- * 
- * cdef int wait_init_wrapper(void *ctx):             # <<<<<<<<<<<<<<
+  /* "libsettings.pyx":258
  *     settings = <object>ctx
  *     settings._event = Event()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_WriteUnraisable("libsettings.wait_init_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_settings);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "libsettings.pyx":335
- *     settings._event = Event()
- * 
- * cdef int wait_wrapper(void *ctx, int timeout_ms):             # <<<<<<<<<<<<<<
- *     settings = <object>ctx
- *     res = settings._event.wait(timeout_ms / 1000.0)
- */
-
-static int __pyx_f_11libsettings_wait_wrapper(void *__pyx_v_ctx, int __pyx_v_timeout_ms) {
-  PyObject *__pyx_v_settings = NULL;
-  PyObject *__pyx_v_res = NULL;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("wait_wrapper", 0);
-
-  /* "libsettings.pyx":336
- * 
- * cdef int wait_wrapper(void *ctx, int timeout_ms):
- *     settings = <object>ctx             # <<<<<<<<<<<<<<
- *     res = settings._event.wait(timeout_ms / 1000.0)
- * 
- */
-  __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
-  __Pyx_INCREF(__pyx_t_1);
-  __pyx_v_settings = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":337
- * cdef int wait_wrapper(void *ctx, int timeout_ms):
- *     settings = <object>ctx
  *     res = settings._event.wait(timeout_ms / 1000.0)             # <<<<<<<<<<<<<<
  * 
  *     if res:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_event); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_event); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_wait); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_wait); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_timeout_ms / 1000.0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_timeout_ms / 1000.0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_res = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":339
+  /* "libsettings.pyx":260
  *     res = settings._event.wait(timeout_ms / 1000.0)
  * 
  *     if res:             # <<<<<<<<<<<<<<
  *         return 0
  *     else:
  */
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_res); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 339, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_res); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 260, __pyx_L1_error)
   if (__pyx_t_5) {
 
-    /* "libsettings.pyx":340
+    /* "libsettings.pyx":261
  * 
  *     if res:
  *         return 0             # <<<<<<<<<<<<<<
  *     else:
  *         return -1
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "libsettings.pyx":339
+    /* "libsettings.pyx":260
  *     res = settings._event.wait(timeout_ms / 1000.0)
  * 
  *     if res:             # <<<<<<<<<<<<<<
  *         return 0
  *     else:
  */
   }
 
-  /* "libsettings.pyx":342
+  /* "libsettings.pyx":263
  *         return 0
  *     else:
  *         return -1             # <<<<<<<<<<<<<<
  * 
  * cdef void signal_wrapper(void *ctx):
  */
   /*else*/ {
     __pyx_r = -1;
     goto __pyx_L0;
   }
 
-  /* "libsettings.pyx":335
- *     settings._event = Event()
+  /* "libsettings.pyx":255
+ *     return 0
  * 
  * cdef int wait_wrapper(void *ctx, int timeout_ms):             # <<<<<<<<<<<<<<
  *     settings = <object>ctx
- *     res = settings._event.wait(timeout_ms / 1000.0)
+ *     settings._event = Event()
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -6920,75 +4680,72 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_settings);
   __Pyx_XDECREF(__pyx_v_res);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":344
+/* "libsettings.pyx":265
  *         return -1
  * 
  * cdef void signal_wrapper(void *ctx):             # <<<<<<<<<<<<<<
  *     settings = <object>ctx
  *     settings._event.set()
  */
 
 static void __pyx_f_11libsettings_signal_wrapper(void *__pyx_v_ctx) {
   PyObject *__pyx_v_settings = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("signal_wrapper", 0);
 
-  /* "libsettings.pyx":345
+  /* "libsettings.pyx":266
  * 
  * cdef void signal_wrapper(void *ctx):
  *     settings = <object>ctx             # <<<<<<<<<<<<<<
  *     settings._event.set()
  * 
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_settings = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":346
+  /* "libsettings.pyx":267
  * cdef void signal_wrapper(void *ctx):
  *     settings = <object>ctx
  *     settings._event.set()             # <<<<<<<<<<<<<<
  * 
- * cdef int wait_thd_wrapper(void *event, int timeout_ms):
+ * cdef int register_cb_wrapper(void *ctx,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_event); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_event); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":344
+  /* "libsettings.pyx":265
  *         return -1
  * 
  * cdef void signal_wrapper(void *ctx):             # <<<<<<<<<<<<<<
  *     settings = <object>ctx
  *     settings._event.set()
  */
 
@@ -7000,383 +4757,17 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_WriteUnraisable("libsettings.signal_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_settings);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "libsettings.pyx":348
+/* "libsettings.pyx":269
  *     settings._event.set()
  * 
- * cdef int wait_thd_wrapper(void *event, int timeout_ms):             # <<<<<<<<<<<<<<
- *     e = <object>event
- *     res = e.wait(timeout_ms / 1000.0)
- */
-
-static int __pyx_f_11libsettings_wait_thd_wrapper(void *__pyx_v_event, int __pyx_v_timeout_ms) {
-  PyObject *__pyx_v_e = NULL;
-  PyObject *__pyx_v_res = NULL;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("wait_thd_wrapper", 0);
-
-  /* "libsettings.pyx":349
- * 
- * cdef int wait_thd_wrapper(void *event, int timeout_ms):
- *     e = <object>event             # <<<<<<<<<<<<<<
- *     res = e.wait(timeout_ms / 1000.0)
- * 
- */
-  __pyx_t_1 = ((PyObject *)__pyx_v_event);
-  __Pyx_INCREF(__pyx_t_1);
-  __pyx_v_e = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":350
- * cdef int wait_thd_wrapper(void *event, int timeout_ms):
- *     e = <object>event
- *     res = e.wait(timeout_ms / 1000.0)             # <<<<<<<<<<<<<<
- * 
- *     if res:
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_e, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyFloat_FromDouble((__pyx_v_timeout_ms / 1000.0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 350, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_res = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":352
- *     res = e.wait(timeout_ms / 1000.0)
- * 
- *     if res:             # <<<<<<<<<<<<<<
- *         return 0
- *     else:
- */
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_res); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 352, __pyx_L1_error)
-  if (__pyx_t_5) {
-
-    /* "libsettings.pyx":353
- * 
- *     if res:
- *         return 0             # <<<<<<<<<<<<<<
- *     else:
- *         return -1
- */
-    __pyx_r = 0;
-    goto __pyx_L0;
-
-    /* "libsettings.pyx":352
- *     res = e.wait(timeout_ms / 1000.0)
- * 
- *     if res:             # <<<<<<<<<<<<<<
- *         return 0
- *     else:
- */
-  }
-
-  /* "libsettings.pyx":355
- *         return 0
- *     else:
- *         return -1             # <<<<<<<<<<<<<<
- * 
- * cdef void signal_thd_wrapper(void *event):
- */
-  /*else*/ {
-    __pyx_r = -1;
-    goto __pyx_L0;
-  }
-
-  /* "libsettings.pyx":348
- *     settings._event.set()
- * 
- * cdef int wait_thd_wrapper(void *event, int timeout_ms):             # <<<<<<<<<<<<<<
- *     e = <object>event
- *     res = e.wait(timeout_ms / 1000.0)
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_WriteUnraisable("libsettings.wait_thd_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_e);
-  __Pyx_XDECREF(__pyx_v_res);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "libsettings.pyx":357
- *         return -1
- * 
- * cdef void signal_thd_wrapper(void *event):             # <<<<<<<<<<<<<<
- *     e = <object>event
- *     e.set()
- */
-
-static void __pyx_f_11libsettings_signal_thd_wrapper(void *__pyx_v_event) {
-  PyObject *__pyx_v_e = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("signal_thd_wrapper", 0);
-
-  /* "libsettings.pyx":358
- * 
- * cdef void signal_thd_wrapper(void *event):
- *     e = <object>event             # <<<<<<<<<<<<<<
- *     e.set()
- * 
- */
-  __pyx_t_1 = ((PyObject *)__pyx_v_event);
-  __Pyx_INCREF(__pyx_t_1);
-  __pyx_v_e = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":359
- * cdef void signal_thd_wrapper(void *event):
- *     e = <object>event
- *     e.set()             # <<<<<<<<<<<<<<
- * 
- * cdef void lock_wrapper(void *ctx):
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_e, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 359, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 359, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":357
- *         return -1
- * 
- * cdef void signal_thd_wrapper(void *event):             # <<<<<<<<<<<<<<
- *     e = <object>event
- *     e.set()
- */
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_WriteUnraisable("libsettings.signal_thd_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_e);
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "libsettings.pyx":361
- *     e.set()
- * 
- * cdef void lock_wrapper(void *ctx):             # <<<<<<<<<<<<<<
- *     settings = <object>ctx
- *     settings._lock.acquire()
- */
-
-static void __pyx_f_11libsettings_lock_wrapper(void *__pyx_v_ctx) {
-  PyObject *__pyx_v_settings = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("lock_wrapper", 0);
-
-  /* "libsettings.pyx":362
- * 
- * cdef void lock_wrapper(void *ctx):
- *     settings = <object>ctx             # <<<<<<<<<<<<<<
- *     settings._lock.acquire()
- * 
- */
-  __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
-  __Pyx_INCREF(__pyx_t_1);
-  __pyx_v_settings = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":363
- * cdef void lock_wrapper(void *ctx):
- *     settings = <object>ctx
- *     settings._lock.acquire()             # <<<<<<<<<<<<<<
- * 
- * cdef void unlock_wrapper(void *ctx):
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_acquire); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 363, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 363, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":361
- *     e.set()
- * 
- * cdef void lock_wrapper(void *ctx):             # <<<<<<<<<<<<<<
- *     settings = <object>ctx
- *     settings._lock.acquire()
- */
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_WriteUnraisable("libsettings.lock_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_settings);
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "libsettings.pyx":365
- *     settings._lock.acquire()
- * 
- * cdef void unlock_wrapper(void *ctx):             # <<<<<<<<<<<<<<
- *     settings = <object>ctx
- *     settings._lock.release()
- */
-
-static void __pyx_f_11libsettings_unlock_wrapper(void *__pyx_v_ctx) {
-  PyObject *__pyx_v_settings = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("unlock_wrapper", 0);
-
-  /* "libsettings.pyx":366
- * 
- * cdef void unlock_wrapper(void *ctx):
- *     settings = <object>ctx             # <<<<<<<<<<<<<<
- *     settings._lock.release()
- * 
- */
-  __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
-  __Pyx_INCREF(__pyx_t_1);
-  __pyx_v_settings = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":367
- * cdef void unlock_wrapper(void *ctx):
- *     settings = <object>ctx
- *     settings._lock.release()             # <<<<<<<<<<<<<<
- * 
- * cdef int register_cb_wrapper(void *ctx,
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 367, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_release); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 367, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "libsettings.pyx":365
- *     settings._lock.acquire()
- * 
- * cdef void unlock_wrapper(void *ctx):             # <<<<<<<<<<<<<<
- *     settings = <object>ctx
- *     settings._lock.release()
- */
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_WriteUnraisable("libsettings.unlock_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_settings);
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "libsettings.pyx":369
- *     settings._lock.release()
- * 
  * cdef int register_cb_wrapper(void *ctx,             # <<<<<<<<<<<<<<
  *                              uint16_t msg_type,
  *                              sbp_msg_callback_t cb,
  */
 
 static int __pyx_f_11libsettings_register_cb_wrapper(void *__pyx_v_ctx, uint16_t __pyx_v_msg_type, sbp_msg_callback_t __pyx_v_cb, void *__pyx_v_cb_context, sbp_msg_callbacks_node_t **__pyx_v_node) {
   PyObject *__pyx_v_settings = NULL;
@@ -7388,20 +4779,17 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("register_cb_wrapper", 0);
 
-  /* "libsettings.pyx":374
+  /* "libsettings.pyx":274
  *                              void *cb_context,
  *                              sbp_msg_callbacks_node_t **node):
  *     try:             # <<<<<<<<<<<<<<
  *         settings = <object>ctx
  *         settings._callbacks[<uintptr_t>node] = (msg_type, <uintptr_t>cb, <uintptr_t>cb_context)
  */
   {
@@ -7409,71 +4797,71 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "libsettings.pyx":375
+      /* "libsettings.pyx":275
  *                              sbp_msg_callbacks_node_t **node):
  *     try:
  *         settings = <object>ctx             # <<<<<<<<<<<<<<
  *         settings._callbacks[<uintptr_t>node] = (msg_type, <uintptr_t>cb, <uintptr_t>cb_context)
  *         settings._link.add_callback(settings._callback_broker, msg_type)
  */
       __pyx_t_4 = ((PyObject *)__pyx_v_ctx);
       __Pyx_INCREF(__pyx_t_4);
       __pyx_v_settings = __pyx_t_4;
       __pyx_t_4 = 0;
 
-      /* "libsettings.pyx":376
+      /* "libsettings.pyx":276
  *     try:
  *         settings = <object>ctx
  *         settings._callbacks[<uintptr_t>node] = (msg_type, <uintptr_t>cb, <uintptr_t>cb_context)             # <<<<<<<<<<<<<<
  *         settings._link.add_callback(settings._callback_broker, msg_type)
  *     except:
  */
-      __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_msg_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 376, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_msg_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 276, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyInt_FromSize_t(((uintptr_t)__pyx_v_cb)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 376, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyInt_FromSize_t(((uintptr_t)__pyx_v_cb)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 276, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyInt_FromSize_t(((uintptr_t)__pyx_v_cb_context)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 376, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyInt_FromSize_t(((uintptr_t)__pyx_v_cb_context)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 276, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 376, __pyx_L3_error)
+      __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 276, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_5 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_callbacks); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 376, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_callbacks); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 276, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_6, ((uintptr_t)__pyx_v_node), __pyx_t_7, uintptr_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1) < 0)) __PYX_ERR(0, 376, __pyx_L3_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_t_6, ((uintptr_t)__pyx_v_node), __pyx_t_7, uintptr_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1) < 0)) __PYX_ERR(1, 276, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "libsettings.pyx":377
+      /* "libsettings.pyx":277
  *         settings = <object>ctx
  *         settings._callbacks[<uintptr_t>node] = (msg_type, <uintptr_t>cb, <uintptr_t>cb_context)
  *         settings._link.add_callback(settings._callback_broker, msg_type)             # <<<<<<<<<<<<<<
  *     except:
  *         return -1
  */
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_link_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 377, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_link_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 277, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_add_callback); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 377, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_add_callback); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 277, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_callback_broker); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 377, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_callback_broker); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 277, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_msg_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_msg_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 277, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_8 = NULL;
       __pyx_t_9 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -7482,51 +4870,51 @@
           __Pyx_DECREF_SET(__pyx_t_5, function);
           __pyx_t_9 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_6, __pyx_t_4};
-        __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 377, __pyx_L3_error)
+        __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 277, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_6, __pyx_t_4};
-        __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 377, __pyx_L3_error)
+        __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 277, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else
       #endif
       {
-        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 377, __pyx_L3_error)
+        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 277, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_10);
         if (__pyx_t_8) {
           __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_6);
         __Pyx_GIVEREF(__pyx_t_4);
         PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_t_4);
         __pyx_t_6 = 0;
         __pyx_t_4 = 0;
-        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_10, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 377, __pyx_L3_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_10, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 277, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "libsettings.pyx":374
+      /* "libsettings.pyx":274
  *                              void *cb_context,
  *                              sbp_msg_callbacks_node_t **node):
  *     try:             # <<<<<<<<<<<<<<
  *         settings = <object>ctx
  *         settings._callbacks[<uintptr_t>node] = (msg_type, <uintptr_t>cb, <uintptr_t>cb_context)
  */
     }
@@ -7538,44 +4926,44 @@
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "libsettings.pyx":378
+    /* "libsettings.pyx":278
  *         settings._callbacks[<uintptr_t>node] = (msg_type, <uintptr_t>cb, <uintptr_t>cb_context)
  *         settings._link.add_callback(settings._callback_broker, msg_type)
  *     except:             # <<<<<<<<<<<<<<
  *         return -1
  * 
  */
     /*except:*/ {
       __Pyx_AddTraceback("libsettings.register_cb_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_5, &__pyx_t_10) < 0) __PYX_ERR(0, 378, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_5, &__pyx_t_10) < 0) __PYX_ERR(1, 278, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_10);
 
-      /* "libsettings.pyx":379
+      /* "libsettings.pyx":279
  *         settings._link.add_callback(settings._callback_broker, msg_type)
  *     except:
  *         return -1             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
       __pyx_r = -1;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       goto __pyx_L6_except_return;
     }
     __pyx_L5_except_error:;
 
-    /* "libsettings.pyx":374
+    /* "libsettings.pyx":274
  *                              void *cb_context,
  *                              sbp_msg_callbacks_node_t **node):
  *     try:             # <<<<<<<<<<<<<<
  *         settings = <object>ctx
  *         settings._callbacks[<uintptr_t>node] = (msg_type, <uintptr_t>cb, <uintptr_t>cb_context)
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -7588,26 +4976,26 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
     __pyx_L8_try_end:;
   }
 
-  /* "libsettings.pyx":381
+  /* "libsettings.pyx":281
  *         return -1
  * 
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * cdef int unregister_cb_wrapper(void *ctx, sbp_msg_callbacks_node_t **node):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "libsettings.pyx":369
- *     settings._lock.release()
+  /* "libsettings.pyx":269
+ *     settings._event.set()
  * 
  * cdef int register_cb_wrapper(void *ctx,             # <<<<<<<<<<<<<<
  *                              uint16_t msg_type,
  *                              sbp_msg_callback_t cb,
  */
 
   /* function exit code */
@@ -7622,15 +5010,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_settings);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":383
+/* "libsettings.pyx":283
  *     return 0
  * 
  * cdef int unregister_cb_wrapper(void *ctx, sbp_msg_callbacks_node_t **node):             # <<<<<<<<<<<<<<
  *     try:
  *         settings = <object>ctx
  */
 
@@ -7645,20 +5033,17 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unregister_cb_wrapper", 0);
 
-  /* "libsettings.pyx":384
+  /* "libsettings.pyx":284
  * 
  * cdef int unregister_cb_wrapper(void *ctx, sbp_msg_callbacks_node_t **node):
  *     try:             # <<<<<<<<<<<<<<
  *         settings = <object>ctx
  *         cb_data = settings._callbacks[<uintptr_t>node]
  */
   {
@@ -7666,56 +5051,56 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "libsettings.pyx":385
+      /* "libsettings.pyx":285
  * cdef int unregister_cb_wrapper(void *ctx, sbp_msg_callbacks_node_t **node):
  *     try:
  *         settings = <object>ctx             # <<<<<<<<<<<<<<
  *         cb_data = settings._callbacks[<uintptr_t>node]
  *         settings._link.remove_callback(settings._callback_broker, cb_data[0])
  */
       __pyx_t_4 = ((PyObject *)__pyx_v_ctx);
       __Pyx_INCREF(__pyx_t_4);
       __pyx_v_settings = __pyx_t_4;
       __pyx_t_4 = 0;
 
-      /* "libsettings.pyx":386
+      /* "libsettings.pyx":286
  *     try:
  *         settings = <object>ctx
  *         cb_data = settings._callbacks[<uintptr_t>node]             # <<<<<<<<<<<<<<
  *         settings._link.remove_callback(settings._callback_broker, cb_data[0])
  *         del settings._callbacks[<uintptr_t>node]
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_callbacks); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 386, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_callbacks); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 286, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_4, ((uintptr_t)__pyx_v_node), uintptr_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 386, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_4, ((uintptr_t)__pyx_v_node), uintptr_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 286, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v_cb_data = __pyx_t_5;
       __pyx_t_5 = 0;
 
-      /* "libsettings.pyx":387
+      /* "libsettings.pyx":287
  *         settings = <object>ctx
  *         cb_data = settings._callbacks[<uintptr_t>node]
  *         settings._link.remove_callback(settings._callback_broker, cb_data[0])             # <<<<<<<<<<<<<<
  *         del settings._callbacks[<uintptr_t>node]
  *     except:
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_link_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_link_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 287, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_remove_callback); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_remove_callback); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 287, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_callback_broker); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_callback_broker); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 287, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_cb_data, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 387, __pyx_L3_error)
+      __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_cb_data, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 287, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       __pyx_t_9 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -7724,63 +5109,63 @@
           __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_9 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_6)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_7};
-        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 287, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_7};
-        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 287, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       {
-        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 387, __pyx_L3_error)
+        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 287, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_10);
         if (__pyx_t_8) {
           __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_4);
         PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_4);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_t_7);
         __pyx_t_4 = 0;
         __pyx_t_7 = 0;
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 287, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "libsettings.pyx":388
+      /* "libsettings.pyx":288
  *         cb_data = settings._callbacks[<uintptr_t>node]
  *         settings._link.remove_callback(settings._callback_broker, cb_data[0])
  *         del settings._callbacks[<uintptr_t>node]             # <<<<<<<<<<<<<<
  *     except:
  *         return -1
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_callbacks); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 388, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_settings, __pyx_n_s_callbacks); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 288, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(__Pyx_DelItemInt(__pyx_t_5, ((uintptr_t)__pyx_v_node), uintptr_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1) < 0)) __PYX_ERR(0, 388, __pyx_L3_error)
+      if (unlikely(__Pyx_DelItemInt(__pyx_t_5, ((uintptr_t)__pyx_v_node), uintptr_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1) < 0)) __PYX_ERR(1, 288, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "libsettings.pyx":384
+      /* "libsettings.pyx":284
  * 
  * cdef int unregister_cb_wrapper(void *ctx, sbp_msg_callbacks_node_t **node):
  *     try:             # <<<<<<<<<<<<<<
  *         settings = <object>ctx
  *         cb_data = settings._callbacks[<uintptr_t>node]
  */
     }
@@ -7792,44 +5177,44 @@
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "libsettings.pyx":389
+    /* "libsettings.pyx":289
  *         settings._link.remove_callback(settings._callback_broker, cb_data[0])
  *         del settings._callbacks[<uintptr_t>node]
  *     except:             # <<<<<<<<<<<<<<
  *         return -1
  * 
  */
     /*except:*/ {
       __Pyx_AddTraceback("libsettings.unregister_cb_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_10) < 0) __PYX_ERR(0, 389, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_10) < 0) __PYX_ERR(1, 289, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_10);
 
-      /* "libsettings.pyx":390
+      /* "libsettings.pyx":290
  *         del settings._callbacks[<uintptr_t>node]
  *     except:
  *         return -1             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
       __pyx_r = -1;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       goto __pyx_L6_except_return;
     }
     __pyx_L5_except_error:;
 
-    /* "libsettings.pyx":384
+    /* "libsettings.pyx":284
  * 
  * cdef int unregister_cb_wrapper(void *ctx, sbp_msg_callbacks_node_t **node):
  *     try:             # <<<<<<<<<<<<<<
  *         settings = <object>ctx
  *         cb_data = settings._callbacks[<uintptr_t>node]
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -7842,25 +5227,25 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
     __pyx_L8_try_end:;
   }
 
-  /* "libsettings.pyx":392
+  /* "libsettings.pyx":292
  *         return -1
  * 
  *     return 0             # <<<<<<<<<<<<<<
  * 
- * cdef void log_wrapper(int priority, const char *fmt):
+ * cdef void log_wrapper(int priority, const char *fmt, ...):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "libsettings.pyx":383
+  /* "libsettings.pyx":283
  *     return 0
  * 
  * cdef int unregister_cb_wrapper(void *ctx, sbp_msg_callbacks_node_t **node):             # <<<<<<<<<<<<<<
  *     try:
  *         settings = <object>ctx
  */
 
@@ -7877,44 +5262,41 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_settings);
   __Pyx_XDECREF(__pyx_v_cb_data);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libsettings.pyx":394
+/* "libsettings.pyx":294
  *     return 0
  * 
- * cdef void log_wrapper(int priority, const char *fmt):             # <<<<<<<<<<<<<<
+ * cdef void log_wrapper(int priority, const char *fmt, ...):             # <<<<<<<<<<<<<<
  *     # Currently no proper way to cythonize the variadic arguments..
  *     # https://github.com/cython/cython/wiki/FAQ#how-do-i-use-variable-args
  */
 
-static void __pyx_f_11libsettings_log_wrapper(CYTHON_UNUSED int __pyx_v_priority, char const *__pyx_v_fmt) {
+static void __pyx_f_11libsettings_log_wrapper(CYTHON_UNUSED int __pyx_v_priority, char const *__pyx_v_fmt, ...) {
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("log_wrapper", 0);
 
-  /* "libsettings.pyx":397
+  /* "libsettings.pyx":297
  *     # Currently no proper way to cythonize the variadic arguments..
  *     # https://github.com/cython/cython/wiki/FAQ#how-do-i-use-variable-args
  *     print fmt             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_fmt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_fmt); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PrintOne(0, __pyx_t_1) < 0) __PYX_ERR(0, 397, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_t_1) < 0) __PYX_ERR(1, 297, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":394
+  /* "libsettings.pyx":294
  *     return 0
  * 
- * cdef void log_wrapper(int priority, const char *fmt):             # <<<<<<<<<<<<<<
+ * cdef void log_wrapper(int priority, const char *fmt, ...):             # <<<<<<<<<<<<<<
  *     # Currently no proper way to cythonize the variadic arguments..
  *     # https://github.com/cython/cython/wiki/FAQ#how-do-i-use-variable-args
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -7934,17 +5316,14 @@
 
 /* Python wrapper */
 static int __pyx_pw_8EnumBase_14__Pyx_EnumMeta_1__init__(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_8EnumBase_14__Pyx_EnumMeta_1__init__(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_name = 0;
   PyObject *__pyx_v_parents = 0;
   PyObject *__pyx_v_dct = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_parents,&__pyx_n_s_dct,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -7965,40 +5344,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parents)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(1, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 16, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dct)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(1, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 16, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(1, 16, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 16, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_name = values[0];
     __pyx_v_parents = values[1];
     __pyx_v_dct = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 16, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 16, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("EnumBase.__Pyx_EnumMeta.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8EnumBase_14__Pyx_EnumMeta___init__(((struct __pyx_obj___Pyx_EnumMeta *)__pyx_v_cls), __pyx_v_name, __pyx_v_parents, __pyx_v_dct);
 
@@ -8011,27 +5390,24 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "EnumBase":17
  * cdef class __Pyx_EnumMeta(type):
  *     def __init__(cls, name, parents, dct):
  *         type.__init__(cls, name, parents, dct)             # <<<<<<<<<<<<<<
  *         cls.__members__ = __Pyx_OrderedDict()
  *     def __iter__(cls):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyType_Type)), __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyType_Type)), __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8040,29 +5416,29 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[5] = {__pyx_t_3, ((PyObject *)__pyx_v_cls), __pyx_v_name, __pyx_v_parents, __pyx_v_dct};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 4+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 4+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[5] = {__pyx_t_3, ((PyObject *)__pyx_v_cls), __pyx_v_name, __pyx_v_parents, __pyx_v_dct};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 4+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 4+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(4+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 17, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(4+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 17, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(((PyObject *)__pyx_v_cls));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_cls));
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, ((PyObject *)__pyx_v_cls));
@@ -8071,15 +5447,15 @@
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_name);
     __Pyx_INCREF(__pyx_v_parents);
     __Pyx_GIVEREF(__pyx_v_parents);
     PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_4, __pyx_v_parents);
     __Pyx_INCREF(__pyx_v_dct);
     __Pyx_GIVEREF(__pyx_v_dct);
     PyTuple_SET_ITEM(__pyx_t_5, 3+__pyx_t_4, __pyx_v_dct);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "EnumBase":18
@@ -8098,18 +5474,18 @@
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 18, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_cls), __pyx_n_s_members, __pyx_t_1) < 0) __PYX_ERR(1, 18, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_cls), __pyx_n_s_members, __pyx_t_1) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "EnumBase":16
  * @cython.internal
  * cdef class __Pyx_EnumMeta(type):
  *     def __init__(cls, name, parents, dct):             # <<<<<<<<<<<<<<
  *         type.__init__(cls, name, parents, dct)
@@ -8154,48 +5530,45 @@
 
 static PyObject *__pyx_pf_8EnumBase_14__Pyx_EnumMeta_2__iter__(struct __pyx_obj___Pyx_EnumMeta *__pyx_v_cls) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
 
   /* "EnumBase":20
  *         cls.__members__ = __Pyx_OrderedDict()
  *     def __iter__(cls):
  *         return iter(cls.__members__.values())             # <<<<<<<<<<<<<<
  *     def __getitem__(cls, name):
  *         return cls.__members__[name]
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cls), __pyx_n_s_members); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 20, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cls), __pyx_n_s_members); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 20, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 20, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 20, __pyx_L1_error)
+  __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* "EnumBase":19
@@ -8241,30 +5614,27 @@
 }
 
 static PyObject *__pyx_pf_8EnumBase_14__Pyx_EnumMeta_4__getitem__(struct __pyx_obj___Pyx_EnumMeta *__pyx_v_cls, PyObject *__pyx_v_name) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
   /* "EnumBase":22
  *         return iter(cls.__members__.values())
  *     def __getitem__(cls, name):
  *         return cls.__members__[name]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cls), __pyx_n_s_members); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 22, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cls), __pyx_n_s_members); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 22, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "EnumBase":21
@@ -8313,17 +5683,14 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = ()             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
@@ -8335,15 +5702,15 @@
   /* "(tree fragment)":6
  *     cdef bint use_setstate
  *     state = ()
  *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
  *     if _dict is not None:
  *         state += (_dict,)
  */
-  __pyx_t_1 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v__dict = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "(tree fragment)":7
  *     state = ()
  *     _dict = getattr(self, '__dict__', None)
@@ -8358,20 +5725,20 @@
     /* "(tree fragment)":8
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  *         state += (_dict,)             # <<<<<<<<<<<<<<
  *         use_setstate = True
  *     else:
  */
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v__dict);
     __Pyx_GIVEREF(__pyx_v__dict);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v__dict);
-    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 8, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_4));
     __pyx_t_4 = 0;
 
     /* "(tree fragment)":9
  *     if _dict is not None:
@@ -8418,28 +5785,28 @@
  *         use_setstate = False
  *     if use_setstate:
  *         return __pyx_unpickle___Pyx_EnumMeta, (type(self), 0xd41d8cd, None), state             # <<<<<<<<<<<<<<
  *     else:
  *         return __pyx_unpickle___Pyx_EnumMeta, (type(self), 0xd41d8cd, state)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle___Pyx_EnumMeta); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle___Pyx_EnumMeta); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_INCREF(__pyx_int_222419149);
     __Pyx_GIVEREF(__pyx_int_222419149);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_222419149);
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     PyTuple_SET_ITEM(__pyx_t_1, 2, Py_None);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
@@ -8464,28 +5831,28 @@
  *     else:
  *         return __pyx_unpickle___Pyx_EnumMeta, (type(self), 0xd41d8cd, state)             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle___Pyx_EnumMeta__set_state(self, __pyx_state)
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle___Pyx_EnumMeta); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle___Pyx_EnumMeta); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_INCREF(__pyx_int_222419149);
     __Pyx_GIVEREF(__pyx_int_222419149);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_222419149);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_state);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
     __pyx_t_5 = 0;
     __pyx_t_1 = 0;
@@ -8535,26 +5902,23 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8EnumBase_14__Pyx_EnumMeta_8__setstate_cython__(struct __pyx_obj___Pyx_EnumMeta *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle___Pyx_EnumMeta, (type(self), 0xd41d8cd, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle___Pyx_EnumMeta__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
-  __pyx_t_1 = __pyx_unpickle___Pyx_EnumMeta__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_unpickle___Pyx_EnumMeta__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle___Pyx_EnumMeta, (type(self), 0xd41d8cd, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
@@ -8585,17 +5949,14 @@
 /* Python wrapper */
 static PyObject *__pyx_pw_8EnumBase_14__Pyx_EnumBase_1__new__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_8EnumBase_14__Pyx_EnumBase_1__new__ = {"__new__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8EnumBase_14__Pyx_EnumBase_1__new__, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_8EnumBase_14__Pyx_EnumBase_1__new__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_cls = 0;
   PyObject *__pyx_v_value = 0;
   PyObject *__pyx_v_name = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__new__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_cls,&__pyx_n_s_value,&__pyx_n_s_name,0};
     PyObject* values[3] = {0,0,0};
     values[2] = ((PyObject *)((PyObject *)Py_None));
@@ -8617,25 +5978,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cls)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__new__", 0, 2, 3, 1); __PYX_ERR(1, 28, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__new__", 0, 2, 3, 1); __PYX_ERR(0, 28, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__new__") < 0)) __PYX_ERR(1, 28, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__new__") < 0)) __PYX_ERR(0, 28, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -8645,15 +6006,15 @@
     }
     __pyx_v_cls = values[0];
     __pyx_v_value = values[1];
     __pyx_v_name = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__new__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 28, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__new__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 28, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("EnumBase.__Pyx_EnumBase.__new__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8EnumBase_14__Pyx_EnumBase___new__(__pyx_self, __pyx_v_cls, __pyx_v_value, __pyx_v_name);
 
@@ -8673,60 +6034,57 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__new__", 0);
 
   /* "EnumBase":29
  *     __metaclass__ = __Pyx_EnumMeta
  *     def __new__(cls, value, name=None):
  *         for v in cls:             # <<<<<<<<<<<<<<
  *             if v == value:
  *                 return v
  */
   if (likely(PyList_CheckExact(__pyx_v_cls)) || PyTuple_CheckExact(__pyx_v_cls)) {
     __pyx_t_1 = __pyx_v_cls; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_cls); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 29, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_cls); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 29, __pyx_L1_error)
+    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 29, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 29, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 29, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 29, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 29, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 29, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 29, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 29, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 29, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 29, __pyx_L1_error)
+          else __PYX_ERR(0, 29, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_4);
     __pyx_t_4 = 0;
@@ -8734,16 +6092,16 @@
     /* "EnumBase":30
  *     def __new__(cls, value, name=None):
  *         for v in cls:
  *             if v == value:             # <<<<<<<<<<<<<<
  *                 return v
  *         if name is None:
  */
-    __pyx_t_4 = PyObject_RichCompare(__pyx_v_v, __pyx_v_value, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 30, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 30, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_v_v, __pyx_v_value, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_5) {
 
       /* "EnumBase":31
  *         for v in cls:
  *             if v == value:
  *                 return v             # <<<<<<<<<<<<<<
@@ -8789,22 +6147,22 @@
     /* "EnumBase":33
  *                 return v
  *         if name is None:
  *             raise ValueError("Unknown enum value: '%s'" % value)             # <<<<<<<<<<<<<<
  *         res = int.__new__(cls, value)
  *         res.name = name
  */
-    __pyx_t_1 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Unknown_enum_value_s, __pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 33, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Unknown_enum_value_s, __pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 33, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 33, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(1, 33, __pyx_L1_error)
+    __PYX_ERR(0, 33, __pyx_L1_error)
 
     /* "EnumBase":32
  *             if v == value:
  *                 return v
  *         if name is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("Unknown enum value: '%s'" % value)
  *         res = int.__new__(cls, value)
@@ -8814,15 +6172,15 @@
   /* "EnumBase":34
  *         if name is None:
  *             raise ValueError("Unknown enum value: '%s'" % value)
  *         res = int.__new__(cls, value)             # <<<<<<<<<<<<<<
  *         res.name = name
  *         setattr(cls, name, res)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyInt_Type)), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyInt_Type)), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -8831,75 +6189,75 @@
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_v_cls, __pyx_v_value};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 34, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_4);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_v_cls, __pyx_v_value};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 34, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_4);
   } else
   #endif
   {
-    __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 34, __pyx_L1_error)
+    __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 34, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_v_cls);
     __Pyx_GIVEREF(__pyx_v_cls);
     PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_v_cls);
     __Pyx_INCREF(__pyx_v_value);
     __Pyx_GIVEREF(__pyx_v_value);
     PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_value);
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_9, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 34, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_9, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_res = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "EnumBase":35
  *             raise ValueError("Unknown enum value: '%s'" % value)
  *         res = int.__new__(cls, value)
  *         res.name = name             # <<<<<<<<<<<<<<
  *         setattr(cls, name, res)
  *         cls.__members__[name] = res
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_res, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(1, 35, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_res, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
 
   /* "EnumBase":36
  *         res = int.__new__(cls, value)
  *         res.name = name
  *         setattr(cls, name, res)             # <<<<<<<<<<<<<<
  *         cls.__members__[name] = res
  *         return res
  */
-  __pyx_t_10 = PyObject_SetAttr(__pyx_v_cls, __pyx_v_name, __pyx_v_res); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(1, 36, __pyx_L1_error)
+  __pyx_t_10 = PyObject_SetAttr(__pyx_v_cls, __pyx_v_name, __pyx_v_res); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 36, __pyx_L1_error)
 
   /* "EnumBase":37
  *         res.name = name
  *         setattr(cls, name, res)
  *         cls.__members__[name] = res             # <<<<<<<<<<<<<<
  *         return res
  *     def __repr__(self):
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_cls, __pyx_n_s_members); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 37, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_cls, __pyx_n_s_members); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_v_name, __pyx_v_res) < 0)) __PYX_ERR(1, 37, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_v_name, __pyx_v_res) < 0)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "EnumBase":38
  *         setattr(cls, name, res)
  *         cls.__members__[name] = res
  *         return res             # <<<<<<<<<<<<<<
  *     def __repr__(self):
@@ -8958,46 +6316,43 @@
 
 static PyObject *__pyx_pf_8EnumBase_14__Pyx_EnumBase_2__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
   /* "EnumBase":40
  *         return res
  *     def __repr__(self):
  *         return "<%s.%s: %d>" % (self.__class__.__name__, self.name, self)             # <<<<<<<<<<<<<<
  *     def __str__(self):
  *         return "%s.%s" % (self.__class__.__name__, self.name)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 40, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 40, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 40, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 40, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __Pyx_INCREF(__pyx_v_self);
   __Pyx_GIVEREF(__pyx_v_self);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_self);
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_s_s_d, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 40, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_s_s_d, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "EnumBase":39
@@ -9045,43 +6400,40 @@
 
 static PyObject *__pyx_pf_8EnumBase_14__Pyx_EnumBase_4__str__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
   /* "EnumBase":42
  *         return "<%s.%s: %d>" % (self.__class__.__name__, self.name, self)
  *     def __str__(self):
  *         return "%s.%s" % (self.__class__.__name__, self.name)             # <<<<<<<<<<<<<<
  * 
  * if PY_VERSION_HEX >= 0x03040000:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 42, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 42, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 42, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 42, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_s_s, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 42, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_s_s, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "EnumBase":41
@@ -9114,17 +6466,14 @@
 /* Python wrapper */
 static PyObject *__pyx_pw_8EnumBase_1__pyx_unpickle___Pyx_EnumMeta(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_8EnumBase_1__pyx_unpickle___Pyx_EnumMeta = {"__pyx_unpickle___Pyx_EnumMeta", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8EnumBase_1__pyx_unpickle___Pyx_EnumMeta, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_8EnumBase_1__pyx_unpickle___Pyx_EnumMeta(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_unpickle___Pyx_EnumMeta (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -9145,40 +6494,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_checksum)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle___Pyx_EnumMeta", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle___Pyx_EnumMeta", 1, 3, 3, 1); __PYX_ERR(0, 1, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_state)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle___Pyx_EnumMeta", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle___Pyx_EnumMeta", 1, 3, 3, 2); __PYX_ERR(0, 1, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle___Pyx_EnumMeta") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle___Pyx_EnumMeta") < 0)) __PYX_ERR(0, 1, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v___pyx_type = values[0];
-    __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
+    __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L3_error)
     __pyx_v___pyx_state = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle___Pyx_EnumMeta", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle___Pyx_EnumMeta", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("EnumBase.__pyx_unpickle___Pyx_EnumMeta", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8EnumBase___pyx_unpickle___Pyx_EnumMeta(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
@@ -9188,155 +6537,148 @@
 }
 
 static PyObject *__pyx_pf_8EnumBase___pyx_unpickle___Pyx_EnumMeta(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
-  int __pyx_t_3;
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+  int __pyx_t_6;
   __Pyx_RefNannySetupContext("__pyx_unpickle___Pyx_EnumMeta", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
  */
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__5, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = (__pyx_t_2 != 0);
-  if (__pyx_t_3) {
+  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xd41d8cd) != 0);
+  if (__pyx_t_1) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
+ *     if __pyx_checksum != 0xd41d8cd:
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
  *     __pyx_result = __Pyx_EnumMeta.__new__(__pyx_type)
  */
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
-    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_INCREF(__pyx_t_1);
-    __pyx_v___pyx_PickleError = __pyx_t_1;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
+    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, -1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_INCREF(__pyx_t_2);
+    __pyx_v___pyx_PickleError = __pyx_t_2;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
+ *     if __pyx_checksum != 0xd41d8cd:
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = __Pyx_EnumMeta.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xd4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_6);
+    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(1, 6, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __PYX_ERR(0, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
  *     __pyx_result = __Pyx_EnumMeta.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle___Pyx_EnumMeta__set_state(<__Pyx_EnumMeta> __pyx_result, __pyx_state)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype___Pyx_EnumMeta), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_5);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype___Pyx_EnumMeta), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result = __pyx_t_4;
-  __pyx_t_4 = 0;
+  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v___pyx_result = __pyx_t_3;
+  __pyx_t_3 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
  *     __pyx_result = __Pyx_EnumMeta.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle___Pyx_EnumMeta__set_state(<__Pyx_EnumMeta> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_2 = (__pyx_t_3 != 0);
-  if (__pyx_t_2) {
+  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_6 = (__pyx_t_1 != 0);
+  if (__pyx_t_6) {
 
     /* "(tree fragment)":9
  *     __pyx_result = __Pyx_EnumMeta.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle___Pyx_EnumMeta__set_state(<__Pyx_EnumMeta> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle___Pyx_EnumMeta__set_state(__Pyx_EnumMeta __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_4 = __pyx_unpickle___Pyx_EnumMeta__set_state(((struct __pyx_obj___Pyx_EnumMeta *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(0, 9, __pyx_L1_error)
+    __pyx_t_3 = __pyx_unpickle___Pyx_EnumMeta__set_state(((struct __pyx_obj___Pyx_EnumMeta *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
  *     __pyx_result = __Pyx_EnumMeta.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle___Pyx_EnumMeta__set_state(<__Pyx_EnumMeta> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -9356,18 +6698,18 @@
  * def __pyx_unpickle___Pyx_EnumMeta(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("EnumBase.__pyx_unpickle___Pyx_EnumMeta", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -9389,72 +6731,69 @@
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle___Pyx_EnumMeta__set_state", 0);
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle___Pyx_EnumMeta__set_state(__Pyx_EnumMeta __pyx_result, tuple __pyx_state):
  *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
  *         __pyx_result.__dict__.update(__pyx_state[0])
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(1, 12, __pyx_L1_error)
+    __PYX_ERR(0, 12, __pyx_L1_error)
   }
-  __pyx_t_2 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 12, __pyx_L1_error)
   __pyx_t_3 = ((__pyx_t_2 > 0) != 0);
   if (__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 12, __pyx_L1_error)
   __pyx_t_4 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_4;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
     /* "(tree fragment)":13
  * cdef __pyx_unpickle___Pyx_EnumMeta__set_state(__Pyx_EnumMeta __pyx_result, tuple __pyx_state):
  *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[0])             # <<<<<<<<<<<<<<
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_v___pyx_state == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 13, __pyx_L1_error)
+      __PYX_ERR(0, 13, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
     /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle___Pyx_EnumMeta__set_state(__Pyx_EnumMeta __pyx_result, tuple __pyx_state):
@@ -9497,15 +6836,14 @@
   }
   if (unlikely(!o)) return 0;
   p = ((struct __pyx_obj_11libsettings_Settings *)o);
   p->_callbacks = Py_None; Py_INCREF(Py_None);
   p->_event = Py_None; Py_INCREF(Py_None);
   p->_link = Py_None; Py_INCREF(Py_None);
   p->_debug = Py_None; Py_INCREF(Py_None);
-  p->_lock = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_11libsettings_Settings(PyObject *o) {
   struct __pyx_obj_11libsettings_Settings *p = (struct __pyx_obj_11libsettings_Settings *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
@@ -9513,15 +6851,14 @@
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_callbacks);
   Py_CLEAR(p->_event);
   Py_CLEAR(p->_link);
   Py_CLEAR(p->_debug);
-  Py_CLEAR(p->_lock);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static int __pyx_tp_traverse_11libsettings_Settings(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_11libsettings_Settings *p = (struct __pyx_obj_11libsettings_Settings *)o;
   if (p->_callbacks) {
@@ -9532,17 +6869,14 @@
   }
   if (p->_link) {
     e = (*v)(p->_link, a); if (e) return e;
   }
   if (p->_debug) {
     e = (*v)(p->_debug, a); if (e) return e;
   }
-  if (p->_lock) {
-    e = (*v)(p->_lock, a); if (e) return e;
-  }
   return 0;
 }
 
 static int __pyx_tp_clear_11libsettings_Settings(PyObject *o) {
   PyObject* tmp;
   struct __pyx_obj_11libsettings_Settings *p = (struct __pyx_obj_11libsettings_Settings *)o;
   tmp = ((PyObject*)p->_callbacks);
@@ -9553,17 +6887,14 @@
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->_link);
   p->_link = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->_debug);
   p->_debug = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
-  tmp = ((PyObject*)p->_lock);
-  p->_lock = Py_None; Py_INCREF(Py_None);
-  Py_XDECREF(tmp);
   return 0;
 }
 
 static PyObject *__pyx_getprop_11libsettings_8Settings__callbacks(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_11libsettings_8Settings_10_callbacks_1__get__(o);
 }
 
@@ -9584,52 +6915,40 @@
   return __pyx_pw_11libsettings_8Settings_5_link_1__get__(o);
 }
 
 static PyObject *__pyx_getprop_11libsettings_8Settings__debug(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_11libsettings_8Settings_6_debug_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_11libsettings_8Settings__lock(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_11libsettings_8Settings_5_lock_1__get__(o);
-}
-
 static PyMethodDef __pyx_methods_11libsettings_Settings[] = {
   {"destroy", (PyCFunction)__pyx_pw_11libsettings_8Settings_3destroy, METH_NOARGS, 0},
   {"write", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11libsettings_8Settings_5write, METH_VARARGS|METH_KEYWORDS, 0},
-  {"write_all", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11libsettings_8Settings_7write_all, METH_VARARGS|METH_KEYWORDS, 0},
-  {"read", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11libsettings_8Settings_9read, METH_VARARGS|METH_KEYWORDS, 0},
-  {"_read_by_index", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11libsettings_8Settings_11_read_by_index, METH_VARARGS|METH_KEYWORDS, 0},
-  {"read_all", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11libsettings_8Settings_13read_all, METH_VARARGS|METH_KEYWORDS, 0},
-  {"_callback_broker", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11libsettings_8Settings_15_callback_broker, METH_VARARGS|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_11libsettings_8Settings_17__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_11libsettings_8Settings_19__setstate_cython__, METH_O, 0},
+  {"read", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11libsettings_8Settings_7read, METH_VARARGS|METH_KEYWORDS, 0},
+  {"read_all", (PyCFunction)__pyx_pw_11libsettings_8Settings_9read_all, METH_NOARGS, 0},
+  {"_callback_broker", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11libsettings_8Settings_11_callback_broker, METH_VARARGS|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_11libsettings_8Settings_13__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_11libsettings_8Settings_15__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_11libsettings_Settings[] = {
   {(char *)"_callbacks", __pyx_getprop_11libsettings_8Settings__callbacks, 0, (char *)0, 0},
   {(char *)"_event", __pyx_getprop_11libsettings_8Settings__event, __pyx_setprop_11libsettings_8Settings__event, (char *)0, 0},
   {(char *)"_link", __pyx_getprop_11libsettings_8Settings__link, 0, (char *)0, 0},
   {(char *)"_debug", __pyx_getprop_11libsettings_8Settings__debug, 0, (char *)0, 0},
-  {(char *)"_lock", __pyx_getprop_11libsettings_8Settings__lock, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_11libsettings_Settings = {
   PyVarObject_HEAD_INIT(0, 0)
   "libsettings.Settings", /*tp_name*/
   sizeof(struct __pyx_obj_11libsettings_Settings), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_11libsettings_Settings, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -9671,23 +6990,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-  0, /*tp_vectorcall*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 
 static struct __pyx_obj_11libsettings___pyx_scope_struct___callback_broker *__pyx_freelist_11libsettings___pyx_scope_struct___callback_broker[8];
 static int __pyx_freecount_11libsettings___pyx_scope_struct___callback_broker = 0;
 
 static PyObject *__pyx_tp_new_11libsettings___pyx_scope_struct___callback_broker(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -9734,20 +7044,15 @@
 
 static PyTypeObject __pyx_type_11libsettings___pyx_scope_struct___callback_broker = {
   PyVarObject_HEAD_INIT(0, 0)
   "libsettings.__pyx_scope_struct___callback_broker", /*tp_name*/
   sizeof(struct __pyx_obj_11libsettings___pyx_scope_struct___callback_broker), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_11libsettings___pyx_scope_struct___callback_broker, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -9789,23 +7094,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-  0, /*tp_vectorcall*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 
 static struct __pyx_obj_11libsettings___pyx_scope_struct_1_genexpr *__pyx_freelist_11libsettings___pyx_scope_struct_1_genexpr[8];
 static int __pyx_freecount_11libsettings___pyx_scope_struct_1_genexpr = 0;
 
 static PyObject *__pyx_tp_new_11libsettings___pyx_scope_struct_1_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -9851,20 +7147,15 @@
 
 static PyTypeObject __pyx_type_11libsettings___pyx_scope_struct_1_genexpr = {
   PyVarObject_HEAD_INIT(0, 0)
   "libsettings.__pyx_scope_struct_1_genexpr", /*tp_name*/
   sizeof(struct __pyx_obj_11libsettings___pyx_scope_struct_1_genexpr), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_11libsettings___pyx_scope_struct_1_genexpr, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -9906,23 +7197,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-  0, /*tp_vectorcall*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 
 static struct __pyx_obj_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper *__pyx_freelist_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper[8];
 static int __pyx_freecount_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper = 0;
 
 static PyObject *__pyx_tp_new_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -9947,20 +7229,15 @@
 
 static PyTypeObject __pyx_type_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper = {
   PyVarObject_HEAD_INIT(0, 0)
   "libsettings.__pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper", /*tp_name*/
   sizeof(struct __pyx_obj_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -10002,23 +7279,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-  0, /*tp_vectorcall*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 
 static struct __pyx_obj_11libsettings___pyx_scope_struct_3_genexpr *__pyx_freelist_11libsettings___pyx_scope_struct_3_genexpr[8];
 static int __pyx_freecount_11libsettings___pyx_scope_struct_3_genexpr = 0;
 
 static PyObject *__pyx_tp_new_11libsettings___pyx_scope_struct_3_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -10064,20 +7332,15 @@
 
 static PyTypeObject __pyx_type_11libsettings___pyx_scope_struct_3_genexpr = {
   PyVarObject_HEAD_INIT(0, 0)
   "libsettings.__pyx_scope_struct_3_genexpr", /*tp_name*/
   sizeof(struct __pyx_obj_11libsettings___pyx_scope_struct_3_genexpr), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_11libsettings___pyx_scope_struct_3_genexpr, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -10119,23 +7382,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-  0, /*tp_vectorcall*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 
 static struct __pyx_obj_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper *__pyx_freelist_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper[8];
 static int __pyx_freecount_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper = 0;
 
 static PyObject *__pyx_tp_new_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -10160,20 +7414,15 @@
 
 static PyTypeObject __pyx_type_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper = {
   PyVarObject_HEAD_INIT(0, 0)
   "libsettings.__pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper", /*tp_name*/
   sizeof(struct __pyx_obj_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -10215,23 +7464,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-  0, /*tp_vectorcall*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 
 static struct __pyx_obj_11libsettings___pyx_scope_struct_5_genexpr *__pyx_freelist_11libsettings___pyx_scope_struct_5_genexpr[8];
 static int __pyx_freecount_11libsettings___pyx_scope_struct_5_genexpr = 0;
 
 static PyObject *__pyx_tp_new_11libsettings___pyx_scope_struct_5_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -10277,20 +7517,15 @@
 
 static PyTypeObject __pyx_type_11libsettings___pyx_scope_struct_5_genexpr = {
   PyVarObject_HEAD_INIT(0, 0)
   "libsettings.__pyx_scope_struct_5_genexpr", /*tp_name*/
   sizeof(struct __pyx_obj_11libsettings___pyx_scope_struct_5_genexpr), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_11libsettings___pyx_scope_struct_5_genexpr, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -10332,23 +7567,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-  0, /*tp_vectorcall*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 
 static PyObject *__pyx_tp_new___Pyx_EnumMeta(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = (&PyType_Type)->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
   return o;
 }
@@ -10409,20 +7635,15 @@
 
 static PyTypeObject __Pyx_EnumMeta = {
   PyVarObject_HEAD_INIT(0, 0)
   "libsettings.__Pyx_EnumMeta", /*tp_name*/
   sizeof(struct __pyx_obj___Pyx_EnumMeta), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc___Pyx_EnumMeta, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
   0, /*tp_getattr*/
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
@@ -10464,23 +7685,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-  0, /*tp_vectorcall*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-  0, /*tp_print*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -10526,17 +7738,16 @@
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_s_02x, __pyx_k_02x, sizeof(__pyx_k_02x), 0, 0, 1, 0},
   {&__pyx_kp_s_Callback_not_registered_for_mess, __pyx_k_Callback_not_registered_for_mess, sizeof(__pyx_k_Callback_not_registered_for_mess), 0, 0, 1, 0},
   {&__pyx_n_s_EnumBase, __pyx_k_EnumBase, sizeof(__pyx_k_EnumBase), 0, 0, 1, 1},
   {&__pyx_n_s_EnumType, __pyx_k_EnumType, sizeof(__pyx_k_EnumType), 0, 0, 1, 1},
   {&__pyx_n_s_Event, __pyx_k_Event, sizeof(__pyx_k_Event), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xd4, __pyx_k_Incompatible_checksums_s_vs_0xd4, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xd4), 0, 0, 1, 0},
   {&__pyx_n_s_IntEnum, __pyx_k_IntEnum, sizeof(__pyx_k_IntEnum), 0, 0, 1, 1},
-  {&__pyx_n_s_Lock, __pyx_k_Lock, sizeof(__pyx_k_Lock), 0, 0, 1, 1},
   {&__pyx_n_s_OrderedDict, __pyx_k_OrderedDict, sizeof(__pyx_k_OrderedDict), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_Pyx_EnumBase, __pyx_k_Pyx_EnumBase, sizeof(__pyx_k_Pyx_EnumBase), 0, 0, 1, 1},
   {&__pyx_n_s_Pyx_EnumBase___new, __pyx_k_Pyx_EnumBase___new, sizeof(__pyx_k_Pyx_EnumBase___new), 0, 0, 1, 1},
   {&__pyx_n_s_Pyx_EnumBase___repr, __pyx_k_Pyx_EnumBase___repr, sizeof(__pyx_k_Pyx_EnumBase___repr), 0, 0, 1, 1},
   {&__pyx_n_s_Pyx_EnumBase___str, __pyx_k_Pyx_EnumBase___str, sizeof(__pyx_k_Pyx_EnumBase___str), 0, 0, 1, 1},
   {&__pyx_n_s_SBP, __pyx_k_SBP, sizeof(__pyx_k_SBP), 0, 0, 1, 1},
@@ -10547,66 +7758,54 @@
   {&__pyx_n_s_SETTINGS_WR_READ_ONLY, __pyx_k_SETTINGS_WR_READ_ONLY, sizeof(__pyx_k_SETTINGS_WR_READ_ONLY), 0, 0, 1, 1},
   {&__pyx_n_s_SETTINGS_WR_SERVICE_FAILED, __pyx_k_SETTINGS_WR_SERVICE_FAILED, sizeof(__pyx_k_SETTINGS_WR_SERVICE_FAILED), 0, 0, 1, 1},
   {&__pyx_n_s_SETTINGS_WR_SETTING_REJECTED, __pyx_k_SETTINGS_WR_SETTING_REJECTED, sizeof(__pyx_k_SETTINGS_WR_SETTING_REJECTED), 0, 0, 1, 1},
   {&__pyx_n_s_SETTINGS_WR_TIMEOUT, __pyx_k_SETTINGS_WR_TIMEOUT, sizeof(__pyx_k_SETTINGS_WR_TIMEOUT), 0, 0, 1, 1},
   {&__pyx_n_s_SETTINGS_WR_VALUE_REJECTED, __pyx_k_SETTINGS_WR_VALUE_REJECTED, sizeof(__pyx_k_SETTINGS_WR_VALUE_REJECTED), 0, 0, 1, 1},
   {&__pyx_n_s_Settings, __pyx_k_Settings, sizeof(__pyx_k_Settings), 0, 0, 1, 1},
   {&__pyx_n_s_SettingsWriteResponseCodes, __pyx_k_SettingsWriteResponseCodes, sizeof(__pyx_k_SettingsWriteResponseCodes), 0, 0, 1, 1},
-  {&__pyx_n_s_ThreadPool, __pyx_k_ThreadPool, sizeof(__pyx_k_ThreadPool), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unknown_enum_value_s, __pyx_k_Unknown_enum_value_s, sizeof(__pyx_k_Unknown_enum_value_s), 0, 0, 1, 0},
-  {&__pyx_kp_s_Unsupported_type_for, __pyx_k_Unsupported_type_for, sizeof(__pyx_k_Unsupported_type_for), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_kp_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 0},
-  {&__pyx_n_s_acquire, __pyx_k_acquire, sizeof(__pyx_k_acquire), 0, 0, 1, 1},
   {&__pyx_n_s_add_callback, __pyx_k_add_callback, sizeof(__pyx_k_add_callback), 0, 0, 1, 1},
-  {&__pyx_n_s_apply_async, __pyx_k_apply_async, sizeof(__pyx_k_apply_async), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
-  {&__pyx_n_s_ascii, __pyx_k_ascii, sizeof(__pyx_k_ascii), 0, 0, 1, 1},
   {&__pyx_n_s_callback_broker, __pyx_k_callback_broker, sizeof(__pyx_k_callback_broker), 0, 0, 1, 1},
   {&__pyx_n_s_callback_broker_locals_genexpr, __pyx_k_callback_broker_locals_genexpr, sizeof(__pyx_k_callback_broker_locals_genexpr), 0, 0, 1, 1},
   {&__pyx_n_s_callbacks, __pyx_k_callbacks, sizeof(__pyx_k_callbacks), 0, 0, 1, 1},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
   {&__pyx_n_s_cls, __pyx_k_cls, sizeof(__pyx_k_cls), 0, 0, 1, 1},
   {&__pyx_n_s_collections, __pyx_k_collections, sizeof(__pyx_k_collections), 0, 0, 1, 1},
   {&__pyx_n_s_dct, __pyx_k_dct, sizeof(__pyx_k_dct), 0, 0, 1, 1},
   {&__pyx_n_s_debug, __pyx_k_debug, sizeof(__pyx_k_debug), 0, 0, 1, 1},
   {&__pyx_n_s_debug_2, __pyx_k_debug_2, sizeof(__pyx_k_debug_2), 0, 0, 1, 1},
-  {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
-  {&__pyx_n_s_encoding, __pyx_k_encoding, sizeof(__pyx_k_encoding), 0, 0, 1, 1},
   {&__pyx_n_s_end, __pyx_k_end, sizeof(__pyx_k_end), 0, 0, 1, 1},
   {&__pyx_n_s_enum, __pyx_k_enum, sizeof(__pyx_k_enum), 0, 0, 1, 1},
   {&__pyx_n_s_event, __pyx_k_event, sizeof(__pyx_k_event), 0, 0, 1, 1},
   {&__pyx_n_s_file, __pyx_k_file, sizeof(__pyx_k_file), 0, 0, 1, 1},
   {&__pyx_n_s_fmt_type, __pyx_k_fmt_type, sizeof(__pyx_k_fmt_type), 0, 0, 1, 1},
   {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
   {&__pyx_n_s_genexpr, __pyx_k_genexpr, sizeof(__pyx_k_genexpr), 0, 0, 1, 1},
-  {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
-  {&__pyx_n_s_idx, __pyx_k_idx, sizeof(__pyx_k_idx), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {&__pyx_n_s_join, __pyx_k_join, sizeof(__pyx_k_join), 0, 0, 1, 1},
   {&__pyx_n_s_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 0, 1, 1},
   {&__pyx_n_s_libsettings, __pyx_k_libsettings, sizeof(__pyx_k_libsettings), 0, 0, 1, 1},
   {&__pyx_n_s_link, __pyx_k_link, sizeof(__pyx_k_link), 0, 0, 1, 1},
   {&__pyx_n_s_link_2, __pyx_k_link_2, sizeof(__pyx_k_link_2), 0, 0, 1, 1},
-  {&__pyx_n_s_lock, __pyx_k_lock, sizeof(__pyx_k_lock), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_members, __pyx_k_members, sizeof(__pyx_k_members), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_msg_type, __pyx_k_msg_type, sizeof(__pyx_k_msg_type), 0, 0, 1, 1},
-  {&__pyx_n_s_multiprocessing_pool, __pyx_k_multiprocessing_pool, sizeof(__pyx_k_multiprocessing_pool), 0, 0, 1, 1},
-  {&__pyx_n_s_multithread, __pyx_k_multithread, sizeof(__pyx_k_multithread), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_n_s_parents, __pyx_k_parents, sizeof(__pyx_k_parents), 0, 0, 1, 1},
   {&__pyx_n_s_payload, __pyx_k_payload, sizeof(__pyx_k_payload), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
@@ -10614,20 +7813,17 @@
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle___Pyx_EnumMeta, __pyx_k_pyx_unpickle___Pyx_EnumMeta, sizeof(__pyx_k_pyx_unpickle___Pyx_EnumMeta), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
-  {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
-  {&__pyx_n_s_read_by_index, __pyx_k_read_by_index, sizeof(__pyx_k_read_by_index), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-  {&__pyx_n_s_release, __pyx_k_release, sizeof(__pyx_k_release), 0, 0, 1, 1},
   {&__pyx_n_s_remove_callback, __pyx_k_remove_callback, sizeof(__pyx_k_remove_callback), 0, 0, 1, 1},
   {&__pyx_n_s_repr, __pyx_k_repr, sizeof(__pyx_k_repr), 0, 0, 1, 1},
   {&__pyx_n_s_res, __pyx_k_res, sizeof(__pyx_k_res), 0, 0, 1, 1},
   {&__pyx_kp_s_s_s, __pyx_k_s_s, sizeof(__pyx_k_s_s), 0, 0, 1, 0},
   {&__pyx_kp_s_s_s_d, __pyx_k_s_s_d, sizeof(__pyx_k_s_s_d), 0, 0, 1, 0},
   {&__pyx_n_s_sbp_msg, __pyx_k_sbp_msg, sizeof(__pyx_k_sbp_msg), 0, 0, 1, 1},
   {&__pyx_n_s_sbp_msg_2, __pyx_k_sbp_msg_2, sizeof(__pyx_k_sbp_msg_2), 0, 0, 1, 1},
@@ -10640,33 +7836,29 @@
   {&__pyx_n_s_send_wrapper, __pyx_k_send_wrapper, sizeof(__pyx_k_send_wrapper), 0, 0, 1, 1},
   {&__pyx_n_s_send_wrapper_locals_genexpr, __pyx_k_send_wrapper_locals_genexpr, sizeof(__pyx_k_send_wrapper_locals_genexpr), 0, 0, 1, 1},
   {&__pyx_n_s_sender, __pyx_k_sender, sizeof(__pyx_k_sender), 0, 0, 1, 1},
   {&__pyx_n_s_sender_id, __pyx_k_sender_id, sizeof(__pyx_k_sender_id), 0, 0, 1, 1},
   {&__pyx_n_s_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
-  {&__pyx_n_s_settings, __pyx_k_settings, sizeof(__pyx_k_settings), 0, 0, 1, 1},
   {&__pyx_n_s_str, __pyx_k_str, sizeof(__pyx_k_str), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_threading, __pyx_k_threading, sizeof(__pyx_k_threading), 0, 0, 1, 1},
   {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_n_s_values, __pyx_k_values, sizeof(__pyx_k_values), 0, 0, 1, 1},
   {&__pyx_n_s_wait, __pyx_k_wait, sizeof(__pyx_k_wait), 0, 0, 1, 1},
-  {&__pyx_n_s_workers, __pyx_k_workers, sizeof(__pyx_k_workers), 0, 0, 1, 1},
-  {&__pyx_n_s_write, __pyx_k_write, sizeof(__pyx_k_write), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 175, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 259, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 33, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 33, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -10674,92 +7866,85 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_self_c_api_self_ctx_cannot_be_co); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_self_c_api_self_ctx_cannot_be_co); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "(tree fragment)":4
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.c_api,self.ctx cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_self_c_api_self_ctx_cannot_be_co); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_self_c_api_self_ctx_cannot_be_co); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_int_222419149, __pyx_int_238750788, __pyx_int_228825662); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "EnumBase":28
  * class __Pyx_EnumBase(int):
  *     __metaclass__ = __Pyx_EnumMeta
  *     def __new__(cls, value, name=None):             # <<<<<<<<<<<<<<
  *         for v in cls:
  *             if v == value:
  */
-  __pyx_tuple__6 = PyTuple_Pack(5, __pyx_n_s_cls, __pyx_n_s_value, __pyx_n_s_name, __pyx_n_s_v, __pyx_n_s_res); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_new, 28, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(1, 28, __pyx_L1_error)
-  __pyx_tuple__8 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__5 = PyTuple_Pack(5, __pyx_n_s_cls, __pyx_n_s_value, __pyx_n_s_name, __pyx_n_s_v, __pyx_n_s_res); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_new, 28, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "EnumBase":39
  *         cls.__members__[name] = res
  *         return res
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<%s.%s: %d>" % (self.__class__.__name__, self.name, self)
  *     def __str__(self):
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 39, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_repr, 39, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(1, 39, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_repr, 39, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 39, __pyx_L1_error)
 
   /* "EnumBase":41
  *     def __repr__(self):
  *         return "<%s.%s: %d>" % (self.__class__.__name__, self.name, self)
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "%s.%s" % (self.__class__.__name__, self.name)
  * 
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 41, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_str, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 41, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_str, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 41, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle___Pyx_EnumMeta(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__13 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle___Pyx_EnumMeta, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle___Pyx_EnumMeta, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_10 = PyInt_FromLong(10); if (unlikely(!__pyx_int_10)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_222419149 = PyInt_FromLong(222419149L); if (unlikely(!__pyx_int_222419149)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_228825662 = PyInt_FromLong(228825662L); if (unlikely(!__pyx_int_228825662)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_238750788 = PyInt_FromLong(238750788L); if (unlikely(!__pyx_int_238750788)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  __pyx_int_222419149 = PyInt_FromLong(222419149L); if (unlikely(!__pyx_int_222419149)) __PYX_ERR(1, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -10794,86 +7979,67 @@
   /*--- Function export code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_11libsettings_Settings) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
+  if (PyType_Ready(&__pyx_type_11libsettings_Settings) < 0) __PYX_ERR(1, 119, __pyx_L1_error)
   __pyx_type_11libsettings_Settings.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_11libsettings_Settings.tp_dictoffset && __pyx_type_11libsettings_Settings.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_11libsettings_Settings.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Settings, (PyObject *)&__pyx_type_11libsettings_Settings) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_11libsettings_Settings) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Settings, (PyObject *)&__pyx_type_11libsettings_Settings) < 0) __PYX_ERR(1, 119, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_11libsettings_Settings) < 0) __PYX_ERR(1, 119, __pyx_L1_error)
   __pyx_ptype_11libsettings_Settings = &__pyx_type_11libsettings_Settings;
-  if (PyType_Ready(&__pyx_type_11libsettings___pyx_scope_struct___callback_broker) < 0) __PYX_ERR(0, 282, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
+  if (PyType_Ready(&__pyx_type_11libsettings___pyx_scope_struct___callback_broker) < 0) __PYX_ERR(1, 206, __pyx_L1_error)
   __pyx_type_11libsettings___pyx_scope_struct___callback_broker.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_11libsettings___pyx_scope_struct___callback_broker.tp_dictoffset && __pyx_type_11libsettings___pyx_scope_struct___callback_broker.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_11libsettings___pyx_scope_struct___callback_broker.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_11libsettings___pyx_scope_struct___callback_broker = &__pyx_type_11libsettings___pyx_scope_struct___callback_broker;
-  if (PyType_Ready(&__pyx_type_11libsettings___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 285, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
+  if (PyType_Ready(&__pyx_type_11libsettings___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(1, 209, __pyx_L1_error)
   __pyx_type_11libsettings___pyx_scope_struct_1_genexpr.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_11libsettings___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_11libsettings___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_11libsettings___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_11libsettings___pyx_scope_struct_1_genexpr = &__pyx_type_11libsettings___pyx_scope_struct_1_genexpr;
-  if (PyType_Ready(&__pyx_type_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper) < 0) __PYX_ERR(0, 303, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
+  if (PyType_Ready(&__pyx_type_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper) < 0) __PYX_ERR(1, 227, __pyx_L1_error)
   __pyx_type_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper.tp_dictoffset && __pyx_type_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper = &__pyx_type_11libsettings___pyx_scope_struct_2___pyx_f_11libsettings_send_wrapper;
-  if (PyType_Ready(&__pyx_type_11libsettings___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 308, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
+  if (PyType_Ready(&__pyx_type_11libsettings___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(1, 232, __pyx_L1_error)
   __pyx_type_11libsettings___pyx_scope_struct_3_genexpr.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_11libsettings___pyx_scope_struct_3_genexpr.tp_dictoffset && __pyx_type_11libsettings___pyx_scope_struct_3_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_11libsettings___pyx_scope_struct_3_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_11libsettings___pyx_scope_struct_3_genexpr = &__pyx_type_11libsettings___pyx_scope_struct_3_genexpr;
-  if (PyType_Ready(&__pyx_type_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper) < 0) __PYX_ERR(0, 318, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
+  if (PyType_Ready(&__pyx_type_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper) < 0) __PYX_ERR(1, 242, __pyx_L1_error)
   __pyx_type_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper.tp_dictoffset && __pyx_type_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper = &__pyx_type_11libsettings___pyx_scope_struct_4___pyx_f_11libsettings_send_from_wrapper;
-  if (PyType_Ready(&__pyx_type_11libsettings___pyx_scope_struct_5_genexpr) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
+  if (PyType_Ready(&__pyx_type_11libsettings___pyx_scope_struct_5_genexpr) < 0) __PYX_ERR(1, 247, __pyx_L1_error)
   __pyx_type_11libsettings___pyx_scope_struct_5_genexpr.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_11libsettings___pyx_scope_struct_5_genexpr.tp_dictoffset && __pyx_type_11libsettings___pyx_scope_struct_5_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_11libsettings___pyx_scope_struct_5_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_11libsettings___pyx_scope_struct_5_genexpr = &__pyx_type_11libsettings___pyx_scope_struct_5_genexpr;
   __Pyx_EnumMeta.tp_base = (&PyType_Type);
-  if (PyType_Ready(&__Pyx_EnumMeta) < 0) __PYX_ERR(1, 15, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
+  if (PyType_Ready(&__Pyx_EnumMeta) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_EnumMeta.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__Pyx_EnumMeta.tp_dictoffset && __Pyx_EnumMeta.tp_getattro == PyObject_GenericGetAttr)) {
     __Pyx_EnumMeta.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_setup_reduce((PyObject*)&__Pyx_EnumMeta) < 0) __PYX_ERR(1, 15, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__Pyx_EnumMeta) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __pyx_ptype___Pyx_EnumMeta = &__Pyx_EnumMeta;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -10899,27 +8065,25 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#ifndef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
-#elif PY_MAJOR_VERSION < 3
-#ifdef __cplusplus
-#define __Pyx_PyMODINIT_FUNC extern "C" void
-#else
+#if PY_MAJOR_VERSION < 3
+#ifdef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC void
-#endif
 #else
-#ifdef __cplusplus
-#define __Pyx_PyMODINIT_FUNC extern "C" PyObject *
+#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#endif
 #else
+#ifdef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyObject *
+#else
+#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
 __Pyx_PyMODINIT_FUNC initlibsettings(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC initlibsettings(void)
@@ -11002,17 +8166,14 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'libsettings' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
@@ -11025,195 +8186,170 @@
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_libsettings(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
-  __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(1, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #ifdef WITH_THREAD /* Python build with threading support? */
   PyEval_InitThreads();
   #endif
+  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("libsettings", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely(!__pyx_m)) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(1, 1, __pyx_L1_error)
+  #if CYTHON_COMPILING_IN_PYPY
   Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
-  if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_InitGlobals() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
-  if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_libsettings) {
-    if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
-    PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
+    PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(1, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "libsettings")) {
-      if (unlikely(PyDict_SetItemString(modules, "libsettings", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+      if (unlikely(PyDict_SetItemString(modules, "libsettings", __pyx_m) < 0)) __PYX_ERR(1, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely(__Pyx_modinit_type_init_code() != 0)) goto __pyx_L1_error;
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
-  if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_patch_abc() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
 
   /* "libsettings.pyx":17
  * from libc.stdint cimport uintptr_t
  * 
  * from sbp.msg import SBP, SENDER_ID             # <<<<<<<<<<<<<<
  * 
- * from threading import Event, Lock
+ * from threading import Event
  */
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_SBP);
   __Pyx_GIVEREF(__pyx_n_s_SBP);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_SBP);
   __Pyx_INCREF(__pyx_n_s_SENDER_ID);
   __Pyx_GIVEREF(__pyx_n_s_SENDER_ID);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_SENDER_ID);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_sbp_msg_2, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_sbp_msg_2, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_SBP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_SBP); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SBP, __pyx_t_1) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SBP, __pyx_t_1) < 0) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_SENDER_ID); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_SENDER_ID); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SENDER_ID, __pyx_t_1) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SENDER_ID, __pyx_t_1) < 0) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "libsettings.pyx":19
  * from sbp.msg import SBP, SENDER_ID
  * 
- * from threading import Event, Lock             # <<<<<<<<<<<<<<
+ * from threading import Event             # <<<<<<<<<<<<<<
  * 
- * from multiprocessing.pool import ThreadPool
+ * cpdef enum SettingsWriteResponseCodes:
  */
-  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Event);
   __Pyx_GIVEREF(__pyx_n_s_Event);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Event);
-  __Pyx_INCREF(__pyx_n_s_Lock);
-  __Pyx_GIVEREF(__pyx_n_s_Lock);
-  PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_Lock);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_threading, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_threading, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Event); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Event, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Event); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Lock, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Event, __pyx_t_2) < 0) __PYX_ERR(1, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "libsettings.pyx":21
- * from threading import Event, Lock
- * 
- * from multiprocessing.pool import ThreadPool             # <<<<<<<<<<<<<<
- * 
- * cpdef enum SettingsWriteResponseCodes:
- */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__pyx_n_s_ThreadPool);
-  __Pyx_GIVEREF(__pyx_n_s_ThreadPool);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_ThreadPool);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_multiprocessing_pool, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_ThreadPool); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ThreadPool, __pyx_t_1) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "libsettings.pyx":136
- *     cdef readonly object _lock
+  /* "libsettings.pyx":128
+ *     cdef readonly object _debug
  * 
  *     def __init__(self, link, sender_id=SENDER_ID, debug=False):             # <<<<<<<<<<<<<<
  *         self.c_api.ctx = <void *>self
  *         self.c_api.send = &send_wrapper
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SENDER_ID); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_k_ = __pyx_t_2;
-  __Pyx_GIVEREF(__pyx_t_2);
-  __pyx_t_2 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SENDER_ID); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 128, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k_ = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "libsettings.pyx":1
  * # cython: language_level=2             # <<<<<<<<<<<<<<
  * # Copyright (C) 2018 Swift Navigation Inc.
  * # Contact: <dev@swift-nav.com>
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "EnumBase":9
  * 
  * cdef object __Pyx_OrderedDict
  * if PY_VERSION_HEX >= 0x02070000:             # <<<<<<<<<<<<<<
  *     from collections import OrderedDict as __Pyx_OrderedDict
  * else:
@@ -11224,30 +8360,30 @@
     /* "EnumBase":10
  * cdef object __Pyx_OrderedDict
  * if PY_VERSION_HEX >= 0x02070000:
  *     from collections import OrderedDict as __Pyx_OrderedDict             # <<<<<<<<<<<<<<
  * else:
  *     __Pyx_OrderedDict = dict
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 10, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_OrderedDict);
     __Pyx_GIVEREF(__pyx_n_s_OrderedDict);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_OrderedDict);
-    __pyx_t_1 = __Pyx_Import(__pyx_n_s_collections, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 10, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_OrderedDict); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 10, __pyx_L1_error)
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_OrderedDict);
+    __pyx_t_2 = __Pyx_Import(__pyx_n_s_collections, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_OrderedDict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
     __Pyx_XGOTREF(__Pyx_OrderedDict);
-    __Pyx_DECREF_SET(__Pyx_OrderedDict, __pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF_SET(__Pyx_OrderedDict, __pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
     /* "EnumBase":9
  * 
  * cdef object __Pyx_OrderedDict
  * if PY_VERSION_HEX >= 0x02070000:             # <<<<<<<<<<<<<<
  *     from collections import OrderedDict as __Pyx_OrderedDict
  * else:
@@ -11273,86 +8409,86 @@
   /* "EnumBase":26
  * 
  * cdef object __Pyx_EnumBase
  * class __Pyx_EnumBase(int):             # <<<<<<<<<<<<<<
  *     __metaclass__ = __Pyx_EnumMeta
  *     def __new__(cls, value, name=None):
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
-  PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&PyInt_Type)));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_Pyx_EnumBase, __pyx_n_s_Pyx_EnumBase, (PyObject *) NULL, __pyx_n_s_EnumBase, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 26, __pyx_L1_error)
+  PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)(&PyInt_Type)));
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_Pyx_EnumBase, __pyx_n_s_Pyx_EnumBase, (PyObject *) NULL, __pyx_n_s_EnumBase, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
   /* "EnumBase":27
  * cdef object __Pyx_EnumBase
  * class __Pyx_EnumBase(int):
  *     __metaclass__ = __Pyx_EnumMeta             # <<<<<<<<<<<<<<
  *     def __new__(cls, value, name=None):
  *         for v in cls:
  */
-  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_metaclass, ((PyObject *)__pyx_ptype___Pyx_EnumMeta)) < 0) __PYX_ERR(1, 27, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_metaclass, ((PyObject *)__pyx_ptype___Pyx_EnumMeta)) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
 
   /* "EnumBase":28
  * class __Pyx_EnumBase(int):
  *     __metaclass__ = __Pyx_EnumMeta
  *     def __new__(cls, value, name=None):             # <<<<<<<<<<<<<<
  *         for v in cls:
  *             if v == value:
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8EnumBase_14__Pyx_EnumBase_1__new__, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_Pyx_EnumBase___new, NULL, __pyx_n_s_EnumBase, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 28, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_NewEx(&__pyx_mdef_8EnumBase_14__Pyx_EnumBase_1__new__, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_Pyx_EnumBase___new, NULL, __pyx_n_s_EnumBase, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__8);
-  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_new, __pyx_t_5) < 0) __PYX_ERR(1, 28, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__7);
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_new, __pyx_t_5) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "EnumBase":39
  *         cls.__members__[name] = res
  *         return res
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<%s.%s: %d>" % (self.__class__.__name__, self.name, self)
  *     def __str__(self):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8EnumBase_14__Pyx_EnumBase_3__repr__, 0, __pyx_n_s_Pyx_EnumBase___repr, NULL, __pyx_n_s_EnumBase, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 39, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_NewEx(&__pyx_mdef_8EnumBase_14__Pyx_EnumBase_3__repr__, 0, __pyx_n_s_Pyx_EnumBase___repr, NULL, __pyx_n_s_EnumBase, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_repr, __pyx_t_5) < 0) __PYX_ERR(1, 39, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_repr, __pyx_t_5) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "EnumBase":41
  *     def __repr__(self):
  *         return "<%s.%s: %d>" % (self.__class__.__name__, self.name, self)
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "%s.%s" % (self.__class__.__name__, self.name)
  * 
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8EnumBase_14__Pyx_EnumBase_5__str__, 0, __pyx_n_s_Pyx_EnumBase___str, NULL, __pyx_n_s_EnumBase, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 41, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_NewEx(&__pyx_mdef_8EnumBase_14__Pyx_EnumBase_5__str__, 0, __pyx_n_s_Pyx_EnumBase___str, NULL, __pyx_n_s_EnumBase, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_str, __pyx_t_5) < 0) __PYX_ERR(1, 41, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_str, __pyx_t_5) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "EnumBase":26
  * 
  * cdef object __Pyx_EnumBase
  * class __Pyx_EnumBase(int):             # <<<<<<<<<<<<<<
  *     __metaclass__ = __Pyx_EnumMeta
  *     def __new__(cls, value, name=None):
  */
-  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_Pyx_EnumBase, __pyx_t_1, __pyx_t_4, NULL, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 26, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_Pyx_EnumBase, __pyx_t_2, __pyx_t_4, NULL, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XGOTREF(__Pyx_EnumBase);
   __Pyx_DECREF_SET(__Pyx_EnumBase, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "EnumBase":44
  *         return "%s.%s" % (self.__class__.__name__, self.name)
  * 
  * if PY_VERSION_HEX >= 0x03040000:             # <<<<<<<<<<<<<<
  *     from enum import IntEnum as __Pyx_EnumBase
  * 
@@ -11362,30 +8498,30 @@
 
     /* "EnumBase":45
  * 
  * if PY_VERSION_HEX >= 0x03040000:
  *     from enum import IntEnum as __Pyx_EnumBase             # <<<<<<<<<<<<<<
  * 
  */
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 45, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_n_s_IntEnum);
     __Pyx_GIVEREF(__pyx_n_s_IntEnum);
-    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_IntEnum);
-    __pyx_t_2 = __Pyx_Import(__pyx_n_s_enum, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 45, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_IntEnum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 45, __pyx_L1_error)
+    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_IntEnum);
+    __pyx_t_1 = __Pyx_Import(__pyx_n_s_enum, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_INCREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_IntEnum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_INCREF(__pyx_t_2);
     __Pyx_XGOTREF(__Pyx_EnumBase);
-    __Pyx_DECREF_SET(__Pyx_EnumBase, __pyx_t_1);
-    __Pyx_GIVEREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF_SET(__Pyx_EnumBase, __pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "EnumBase":44
  *         return "%s.%s" % (self.__class__.__name__, self.name)
  * 
  * if PY_VERSION_HEX >= 0x03040000:             # <<<<<<<<<<<<<<
  *     from enum import IntEnum as __Pyx_EnumBase
  * 
@@ -11393,33 +8529,33 @@
   }
 
   /* "(tree fragment)":1
  * def __pyx_unpickle___Pyx_EnumMeta(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_8EnumBase_1__pyx_unpickle___Pyx_EnumMeta, NULL, __pyx_n_s_EnumBase); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle___Pyx_EnumMeta, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8EnumBase_1__pyx_unpickle___Pyx_EnumMeta, NULL, __pyx_n_s_EnumBase); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle___Pyx_EnumMeta, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "EnumType":50
  * 
  * 
  * cdef dict __Pyx_globals = globals()             # <<<<<<<<<<<<<<
  * if PY_VERSION_HEX >= 0x03040000:
  * 
  */
-  __pyx_t_2 = __Pyx_Globals(); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 50, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (!(likely(PyDict_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(1, 50, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Globals(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (!(likely(PyDict_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_XGOTREF(__Pyx_globals);
-  __Pyx_DECREF_SET(__Pyx_globals, ((PyObject*)__pyx_t_2));
-  __Pyx_GIVEREF(__pyx_t_2);
-  __pyx_t_2 = 0;
+  __Pyx_DECREF_SET(__Pyx_globals, ((PyObject*)__pyx_t_1));
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "EnumType":51
  * 
  * cdef dict __Pyx_globals = globals()
  * if PY_VERSION_HEX >= 0x03040000:             # <<<<<<<<<<<<<<
  * 
  *     SettingsWriteResponseCodes = __Pyx_EnumBase('SettingsWriteResponseCodes', __Pyx_OrderedDict([
@@ -11430,351 +8566,351 @@
     /* "EnumType":54
  * 
  *     SettingsWriteResponseCodes = __Pyx_EnumBase('SettingsWriteResponseCodes', __Pyx_OrderedDict([
  *         ('SETTINGS_WR_OK', SETTINGS_WR_OK),             # <<<<<<<<<<<<<<
  *         ('SETTINGS_WR_VALUE_REJECTED', SETTINGS_WR_VALUE_REJECTED),
  *         ('SETTINGS_WR_SETTING_REJECTED', SETTINGS_WR_SETTING_REJECTED),
  */
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_OK); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 54, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 54, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_OK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_OK);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_OK);
-    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_SETTINGS_WR_OK);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
-    __pyx_t_2 = 0;
+    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_SETTINGS_WR_OK);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
 
     /* "EnumType":55
  *     SettingsWriteResponseCodes = __Pyx_EnumBase('SettingsWriteResponseCodes', __Pyx_OrderedDict([
  *         ('SETTINGS_WR_OK', SETTINGS_WR_OK),
  *         ('SETTINGS_WR_VALUE_REJECTED', SETTINGS_WR_VALUE_REJECTED),             # <<<<<<<<<<<<<<
  *         ('SETTINGS_WR_SETTING_REJECTED', SETTINGS_WR_SETTING_REJECTED),
  *         ('SETTINGS_WR_PARSE_FAILED', SETTINGS_WR_PARSE_FAILED),
  */
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_VALUE_REJECTED); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 55, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 55, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_VALUE_REJECTED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_VALUE_REJECTED);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_VALUE_REJECTED);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_SETTINGS_WR_VALUE_REJECTED);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
-    __pyx_t_2 = 0;
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
 
     /* "EnumType":56
  *         ('SETTINGS_WR_OK', SETTINGS_WR_OK),
  *         ('SETTINGS_WR_VALUE_REJECTED', SETTINGS_WR_VALUE_REJECTED),
  *         ('SETTINGS_WR_SETTING_REJECTED', SETTINGS_WR_SETTING_REJECTED),             # <<<<<<<<<<<<<<
  *         ('SETTINGS_WR_PARSE_FAILED', SETTINGS_WR_PARSE_FAILED),
  *         ('SETTINGS_WR_READ_ONLY', SETTINGS_WR_READ_ONLY),
  */
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_SETTING_REJECTED); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 56, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_SETTING_REJECTED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_SETTING_REJECTED);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_SETTING_REJECTED);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_SETTINGS_WR_SETTING_REJECTED);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
-    __pyx_t_2 = 0;
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
 
     /* "EnumType":57
  *         ('SETTINGS_WR_VALUE_REJECTED', SETTINGS_WR_VALUE_REJECTED),
  *         ('SETTINGS_WR_SETTING_REJECTED', SETTINGS_WR_SETTING_REJECTED),
  *         ('SETTINGS_WR_PARSE_FAILED', SETTINGS_WR_PARSE_FAILED),             # <<<<<<<<<<<<<<
  *         ('SETTINGS_WR_READ_ONLY', SETTINGS_WR_READ_ONLY),
  *         ('SETTINGS_WR_MODIFY_DISABLED', SETTINGS_WR_MODIFY_DISABLED),
  */
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_PARSE_FAILED); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 57, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 57, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_PARSE_FAILED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_PARSE_FAILED);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_PARSE_FAILED);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_n_s_SETTINGS_WR_PARSE_FAILED);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_2);
-    __pyx_t_2 = 0;
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
 
     /* "EnumType":58
  *         ('SETTINGS_WR_SETTING_REJECTED', SETTINGS_WR_SETTING_REJECTED),
  *         ('SETTINGS_WR_PARSE_FAILED', SETTINGS_WR_PARSE_FAILED),
  *         ('SETTINGS_WR_READ_ONLY', SETTINGS_WR_READ_ONLY),             # <<<<<<<<<<<<<<
  *         ('SETTINGS_WR_MODIFY_DISABLED', SETTINGS_WR_MODIFY_DISABLED),
  *         ('SETTINGS_WR_SERVICE_FAILED', SETTINGS_WR_SERVICE_FAILED),
  */
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_READ_ONLY); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 58, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 58, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_READ_ONLY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_READ_ONLY);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_READ_ONLY);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_n_s_SETTINGS_WR_READ_ONLY);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_2);
-    __pyx_t_2 = 0;
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
 
     /* "EnumType":59
  *         ('SETTINGS_WR_PARSE_FAILED', SETTINGS_WR_PARSE_FAILED),
  *         ('SETTINGS_WR_READ_ONLY', SETTINGS_WR_READ_ONLY),
  *         ('SETTINGS_WR_MODIFY_DISABLED', SETTINGS_WR_MODIFY_DISABLED),             # <<<<<<<<<<<<<<
  *         ('SETTINGS_WR_SERVICE_FAILED', SETTINGS_WR_SERVICE_FAILED),
  *         ('SETTINGS_WR_TIMEOUT', SETTINGS_WR_TIMEOUT),
  */
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_MODIFY_DISABLED); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 59, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 59, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_MODIFY_DISABLED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 59, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_MODIFY_DISABLED);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_MODIFY_DISABLED);
     PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_n_s_SETTINGS_WR_MODIFY_DISABLED);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_2);
-    __pyx_t_2 = 0;
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
 
     /* "EnumType":60
  *         ('SETTINGS_WR_READ_ONLY', SETTINGS_WR_READ_ONLY),
  *         ('SETTINGS_WR_MODIFY_DISABLED', SETTINGS_WR_MODIFY_DISABLED),
  *         ('SETTINGS_WR_SERVICE_FAILED', SETTINGS_WR_SERVICE_FAILED),             # <<<<<<<<<<<<<<
  *         ('SETTINGS_WR_TIMEOUT', SETTINGS_WR_TIMEOUT),
  *     ]))
  */
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_SERVICE_FAILED); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 60, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 60, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_SERVICE_FAILED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_SERVICE_FAILED);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_SERVICE_FAILED);
     PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_n_s_SETTINGS_WR_SERVICE_FAILED);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_2);
-    __pyx_t_2 = 0;
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
 
     /* "EnumType":61
  *         ('SETTINGS_WR_MODIFY_DISABLED', SETTINGS_WR_MODIFY_DISABLED),
  *         ('SETTINGS_WR_SERVICE_FAILED', SETTINGS_WR_SERVICE_FAILED),
  *         ('SETTINGS_WR_TIMEOUT', SETTINGS_WR_TIMEOUT),             # <<<<<<<<<<<<<<
  *     ]))
  *     __Pyx_globals['SETTINGS_WR_OK'] = SettingsWriteResponseCodes.SETTINGS_WR_OK
  */
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_TIMEOUT); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 61, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_TIMEOUT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_TIMEOUT);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_TIMEOUT);
     PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_n_s_SETTINGS_WR_TIMEOUT);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_2);
-    __pyx_t_2 = 0;
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
 
     /* "EnumType":53
  * if PY_VERSION_HEX >= 0x03040000:
  * 
  *     SettingsWriteResponseCodes = __Pyx_EnumBase('SettingsWriteResponseCodes', __Pyx_OrderedDict([             # <<<<<<<<<<<<<<
  *         ('SETTINGS_WR_OK', SETTINGS_WR_OK),
  *         ('SETTINGS_WR_VALUE_REJECTED', SETTINGS_WR_VALUE_REJECTED),
  */
-    __pyx_t_2 = PyList_New(8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 53, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_1);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+    __pyx_t_1 = PyList_New(8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_4);
-    PyList_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
+    PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
-    PyList_SET_ITEM(__pyx_t_2, 2, __pyx_t_5);
+    PyList_SET_ITEM(__pyx_t_1, 2, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_6);
-    PyList_SET_ITEM(__pyx_t_2, 3, __pyx_t_6);
+    PyList_SET_ITEM(__pyx_t_1, 3, __pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_7);
-    PyList_SET_ITEM(__pyx_t_2, 4, __pyx_t_7);
+    PyList_SET_ITEM(__pyx_t_1, 4, __pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_8);
-    PyList_SET_ITEM(__pyx_t_2, 5, __pyx_t_8);
+    PyList_SET_ITEM(__pyx_t_1, 5, __pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_9);
-    PyList_SET_ITEM(__pyx_t_2, 6, __pyx_t_9);
+    PyList_SET_ITEM(__pyx_t_1, 6, __pyx_t_9);
     __Pyx_GIVEREF(__pyx_t_10);
-    PyList_SET_ITEM(__pyx_t_2, 7, __pyx_t_10);
-    __pyx_t_1 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 7, __pyx_t_10);
+    __pyx_t_2 = 0;
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
     __pyx_t_6 = 0;
     __pyx_t_7 = 0;
     __pyx_t_8 = 0;
     __pyx_t_9 = 0;
     __pyx_t_10 = 0;
-    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__Pyx_OrderedDict, __pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 53, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__Pyx_OrderedDict, __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 53, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_SettingsWriteResponseCodes);
     __Pyx_GIVEREF(__pyx_n_s_SettingsWriteResponseCodes);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_SettingsWriteResponseCodes);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_SettingsWriteResponseCodes);
     __Pyx_GIVEREF(__pyx_t_10);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_10);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_10);
     __pyx_t_10 = 0;
-    __pyx_t_10 = __Pyx_PyObject_Call(__Pyx_EnumBase, __pyx_t_2, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 53, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Call(__Pyx_EnumBase, __pyx_t_1, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_d, __pyx_n_s_SettingsWriteResponseCodes, __pyx_t_10) < 0) __PYX_ERR(1, 53, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    if (PyDict_SetItem(__pyx_d, __pyx_n_s_SettingsWriteResponseCodes, __pyx_t_10) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
     /* "EnumType":63
  *         ('SETTINGS_WR_TIMEOUT', SETTINGS_WR_TIMEOUT),
  *     ]))
  *     __Pyx_globals['SETTINGS_WR_OK'] = SettingsWriteResponseCodes.SETTINGS_WR_OK             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_VALUE_REJECTED'] = SettingsWriteResponseCodes.SETTINGS_WR_VALUE_REJECTED
  *     __Pyx_globals['SETTINGS_WR_SETTING_REJECTED'] = SettingsWriteResponseCodes.SETTINGS_WR_SETTING_REJECTED
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 63, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_SETTINGS_WR_OK); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 63, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_SETTINGS_WR_OK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 63, __pyx_L1_error)
+      __PYX_ERR(0, 63, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_OK, __pyx_t_2) < 0)) __PYX_ERR(1, 63, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_OK, __pyx_t_1) < 0)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "EnumType":64
  *     ]))
  *     __Pyx_globals['SETTINGS_WR_OK'] = SettingsWriteResponseCodes.SETTINGS_WR_OK
  *     __Pyx_globals['SETTINGS_WR_VALUE_REJECTED'] = SettingsWriteResponseCodes.SETTINGS_WR_VALUE_REJECTED             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_SETTING_REJECTED'] = SettingsWriteResponseCodes.SETTINGS_WR_SETTING_REJECTED
  *     __Pyx_globals['SETTINGS_WR_PARSE_FAILED'] = SettingsWriteResponseCodes.SETTINGS_WR_PARSE_FAILED
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 64, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_SETTINGS_WR_VALUE_REJECTED); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 64, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_SETTINGS_WR_VALUE_REJECTED); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 64, __pyx_L1_error)
+      __PYX_ERR(0, 64, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_VALUE_REJECTED, __pyx_t_10) < 0)) __PYX_ERR(1, 64, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_VALUE_REJECTED, __pyx_t_10) < 0)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
     /* "EnumType":65
  *     __Pyx_globals['SETTINGS_WR_OK'] = SettingsWriteResponseCodes.SETTINGS_WR_OK
  *     __Pyx_globals['SETTINGS_WR_VALUE_REJECTED'] = SettingsWriteResponseCodes.SETTINGS_WR_VALUE_REJECTED
  *     __Pyx_globals['SETTINGS_WR_SETTING_REJECTED'] = SettingsWriteResponseCodes.SETTINGS_WR_SETTING_REJECTED             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_PARSE_FAILED'] = SettingsWriteResponseCodes.SETTINGS_WR_PARSE_FAILED
  *     __Pyx_globals['SETTINGS_WR_READ_ONLY'] = SettingsWriteResponseCodes.SETTINGS_WR_READ_ONLY
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 65, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_SETTINGS_WR_SETTING_REJECTED); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 65, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_SETTINGS_WR_SETTING_REJECTED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 65, __pyx_L1_error)
+      __PYX_ERR(0, 65, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_SETTING_REJECTED, __pyx_t_2) < 0)) __PYX_ERR(1, 65, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_SETTING_REJECTED, __pyx_t_1) < 0)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "EnumType":66
  *     __Pyx_globals['SETTINGS_WR_VALUE_REJECTED'] = SettingsWriteResponseCodes.SETTINGS_WR_VALUE_REJECTED
  *     __Pyx_globals['SETTINGS_WR_SETTING_REJECTED'] = SettingsWriteResponseCodes.SETTINGS_WR_SETTING_REJECTED
  *     __Pyx_globals['SETTINGS_WR_PARSE_FAILED'] = SettingsWriteResponseCodes.SETTINGS_WR_PARSE_FAILED             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_READ_ONLY'] = SettingsWriteResponseCodes.SETTINGS_WR_READ_ONLY
  *     __Pyx_globals['SETTINGS_WR_MODIFY_DISABLED'] = SettingsWriteResponseCodes.SETTINGS_WR_MODIFY_DISABLED
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 66, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_SETTINGS_WR_PARSE_FAILED); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 66, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_SETTINGS_WR_PARSE_FAILED); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 66, __pyx_L1_error)
+      __PYX_ERR(0, 66, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_PARSE_FAILED, __pyx_t_10) < 0)) __PYX_ERR(1, 66, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_PARSE_FAILED, __pyx_t_10) < 0)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
     /* "EnumType":67
  *     __Pyx_globals['SETTINGS_WR_SETTING_REJECTED'] = SettingsWriteResponseCodes.SETTINGS_WR_SETTING_REJECTED
  *     __Pyx_globals['SETTINGS_WR_PARSE_FAILED'] = SettingsWriteResponseCodes.SETTINGS_WR_PARSE_FAILED
  *     __Pyx_globals['SETTINGS_WR_READ_ONLY'] = SettingsWriteResponseCodes.SETTINGS_WR_READ_ONLY             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_MODIFY_DISABLED'] = SettingsWriteResponseCodes.SETTINGS_WR_MODIFY_DISABLED
  *     __Pyx_globals['SETTINGS_WR_SERVICE_FAILED'] = SettingsWriteResponseCodes.SETTINGS_WR_SERVICE_FAILED
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 67, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 67, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_SETTINGS_WR_READ_ONLY); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 67, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_SETTINGS_WR_READ_ONLY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 67, __pyx_L1_error)
+      __PYX_ERR(0, 67, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_READ_ONLY, __pyx_t_2) < 0)) __PYX_ERR(1, 67, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_READ_ONLY, __pyx_t_1) < 0)) __PYX_ERR(0, 67, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "EnumType":68
  *     __Pyx_globals['SETTINGS_WR_PARSE_FAILED'] = SettingsWriteResponseCodes.SETTINGS_WR_PARSE_FAILED
  *     __Pyx_globals['SETTINGS_WR_READ_ONLY'] = SettingsWriteResponseCodes.SETTINGS_WR_READ_ONLY
  *     __Pyx_globals['SETTINGS_WR_MODIFY_DISABLED'] = SettingsWriteResponseCodes.SETTINGS_WR_MODIFY_DISABLED             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_SERVICE_FAILED'] = SettingsWriteResponseCodes.SETTINGS_WR_SERVICE_FAILED
  *     __Pyx_globals['SETTINGS_WR_TIMEOUT'] = SettingsWriteResponseCodes.SETTINGS_WR_TIMEOUT
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 68, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_SETTINGS_WR_MODIFY_DISABLED); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 68, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_SETTINGS_WR_MODIFY_DISABLED); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 68, __pyx_L1_error)
+      __PYX_ERR(0, 68, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_MODIFY_DISABLED, __pyx_t_10) < 0)) __PYX_ERR(1, 68, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_MODIFY_DISABLED, __pyx_t_10) < 0)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
     /* "EnumType":69
  *     __Pyx_globals['SETTINGS_WR_READ_ONLY'] = SettingsWriteResponseCodes.SETTINGS_WR_READ_ONLY
  *     __Pyx_globals['SETTINGS_WR_MODIFY_DISABLED'] = SettingsWriteResponseCodes.SETTINGS_WR_MODIFY_DISABLED
  *     __Pyx_globals['SETTINGS_WR_SERVICE_FAILED'] = SettingsWriteResponseCodes.SETTINGS_WR_SERVICE_FAILED             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_TIMEOUT'] = SettingsWriteResponseCodes.SETTINGS_WR_TIMEOUT
  * else:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 69, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_SETTINGS_WR_SERVICE_FAILED); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 69, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_SETTINGS_WR_SERVICE_FAILED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 69, __pyx_L1_error)
+      __PYX_ERR(0, 69, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_SERVICE_FAILED, __pyx_t_2) < 0)) __PYX_ERR(1, 69, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_SERVICE_FAILED, __pyx_t_1) < 0)) __PYX_ERR(0, 69, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "EnumType":70
  *     __Pyx_globals['SETTINGS_WR_MODIFY_DISABLED'] = SettingsWriteResponseCodes.SETTINGS_WR_MODIFY_DISABLED
  *     __Pyx_globals['SETTINGS_WR_SERVICE_FAILED'] = SettingsWriteResponseCodes.SETTINGS_WR_SERVICE_FAILED
  *     __Pyx_globals['SETTINGS_WR_TIMEOUT'] = SettingsWriteResponseCodes.SETTINGS_WR_TIMEOUT             # <<<<<<<<<<<<<<
  * else:
  *     class SettingsWriteResponseCodes(__Pyx_EnumBase):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 70, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_SETTINGS_WR_TIMEOUT); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 70, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_SETTINGS_WR_TIMEOUT); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 70, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 70, __pyx_L1_error)
+      __PYX_ERR(0, 70, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_TIMEOUT, __pyx_t_10) < 0)) __PYX_ERR(1, 70, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_TIMEOUT, __pyx_t_10) < 0)) __PYX_ERR(0, 70, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
     /* "EnumType":51
  * 
  * cdef dict __Pyx_globals = globals()
  * if PY_VERSION_HEX >= 0x03040000:             # <<<<<<<<<<<<<<
  * 
@@ -11787,268 +8923,268 @@
  *     __Pyx_globals['SETTINGS_WR_TIMEOUT'] = SettingsWriteResponseCodes.SETTINGS_WR_TIMEOUT
  * else:
  *     class SettingsWriteResponseCodes(__Pyx_EnumBase):             # <<<<<<<<<<<<<<
  *         pass
  *     __Pyx_globals['SETTINGS_WR_OK'] = SettingsWriteResponseCodes(SETTINGS_WR_OK, 'SETTINGS_WR_OK')
  */
   /*else*/ {
-    __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 72, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_INCREF(__Pyx_EnumBase);
     __Pyx_GIVEREF(__Pyx_EnumBase);
     PyTuple_SET_ITEM(__pyx_t_10, 0, __Pyx_EnumBase);
-    __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 72, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes, __pyx_n_s_SettingsWriteResponseCodes, (PyObject *) NULL, __pyx_n_s_EnumType, (PyObject *) NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 72, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_9 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes, __pyx_n_s_SettingsWriteResponseCodes, (PyObject *) NULL, __pyx_n_s_EnumType, (PyObject *) NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_8 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_SettingsWriteResponseCodes, __pyx_t_10, __pyx_t_9, NULL, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 72, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_SettingsWriteResponseCodes, __pyx_t_10, __pyx_t_9, NULL, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_d, __pyx_n_s_SettingsWriteResponseCodes, __pyx_t_8) < 0) __PYX_ERR(1, 72, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_d, __pyx_n_s_SettingsWriteResponseCodes, __pyx_t_8) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
     /* "EnumType":74
  *     class SettingsWriteResponseCodes(__Pyx_EnumBase):
  *         pass
  *     __Pyx_globals['SETTINGS_WR_OK'] = SettingsWriteResponseCodes(SETTINGS_WR_OK, 'SETTINGS_WR_OK')             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_VALUE_REJECTED'] = SettingsWriteResponseCodes(SETTINGS_WR_VALUE_REJECTED, 'SETTINGS_WR_VALUE_REJECTED')
  *     __Pyx_globals['SETTINGS_WR_SETTING_REJECTED'] = SettingsWriteResponseCodes(SETTINGS_WR_SETTING_REJECTED, 'SETTINGS_WR_SETTING_REJECTED')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 74, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 74, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_OK); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 74, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 74, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_OK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 74, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_OK);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_OK);
     PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_n_s_SETTINGS_WR_OK);
-    __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_9, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 74, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 74, __pyx_L1_error)
+      __PYX_ERR(0, 74, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_OK, __pyx_t_2) < 0)) __PYX_ERR(1, 74, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_OK, __pyx_t_1) < 0)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "EnumType":75
  *         pass
  *     __Pyx_globals['SETTINGS_WR_OK'] = SettingsWriteResponseCodes(SETTINGS_WR_OK, 'SETTINGS_WR_OK')
  *     __Pyx_globals['SETTINGS_WR_VALUE_REJECTED'] = SettingsWriteResponseCodes(SETTINGS_WR_VALUE_REJECTED, 'SETTINGS_WR_VALUE_REJECTED')             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_SETTING_REJECTED'] = SettingsWriteResponseCodes(SETTINGS_WR_SETTING_REJECTED, 'SETTINGS_WR_SETTING_REJECTED')
  *     __Pyx_globals['SETTINGS_WR_PARSE_FAILED'] = SettingsWriteResponseCodes(SETTINGS_WR_PARSE_FAILED, 'SETTINGS_WR_PARSE_FAILED')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 75, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_VALUE_REJECTED); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 75, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_9 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_VALUE_REJECTED); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 75, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_9);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_VALUE_REJECTED);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_VALUE_REJECTED);
     PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_n_s_SETTINGS_WR_VALUE_REJECTED);
     __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_10, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 75, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_10, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 75, __pyx_L1_error)
+      __PYX_ERR(0, 75, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_VALUE_REJECTED, __pyx_t_9) < 0)) __PYX_ERR(1, 75, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_VALUE_REJECTED, __pyx_t_9) < 0)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     /* "EnumType":76
  *     __Pyx_globals['SETTINGS_WR_OK'] = SettingsWriteResponseCodes(SETTINGS_WR_OK, 'SETTINGS_WR_OK')
  *     __Pyx_globals['SETTINGS_WR_VALUE_REJECTED'] = SettingsWriteResponseCodes(SETTINGS_WR_VALUE_REJECTED, 'SETTINGS_WR_VALUE_REJECTED')
  *     __Pyx_globals['SETTINGS_WR_SETTING_REJECTED'] = SettingsWriteResponseCodes(SETTINGS_WR_SETTING_REJECTED, 'SETTINGS_WR_SETTING_REJECTED')             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_PARSE_FAILED'] = SettingsWriteResponseCodes(SETTINGS_WR_PARSE_FAILED, 'SETTINGS_WR_PARSE_FAILED')
  *     __Pyx_globals['SETTINGS_WR_READ_ONLY'] = SettingsWriteResponseCodes(SETTINGS_WR_READ_ONLY, 'SETTINGS_WR_READ_ONLY')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 76, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_SETTING_REJECTED); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 76, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_SETTING_REJECTED); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 76, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_10);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_10);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_10);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_SETTING_REJECTED);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_SETTING_REJECTED);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_SETTINGS_WR_SETTING_REJECTED);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_SETTINGS_WR_SETTING_REJECTED);
     __pyx_t_10 = 0;
-    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_2, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 76, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_1, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 76, __pyx_L1_error)
+      __PYX_ERR(0, 76, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_SETTING_REJECTED, __pyx_t_10) < 0)) __PYX_ERR(1, 76, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_SETTING_REJECTED, __pyx_t_10) < 0)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
     /* "EnumType":77
  *     __Pyx_globals['SETTINGS_WR_VALUE_REJECTED'] = SettingsWriteResponseCodes(SETTINGS_WR_VALUE_REJECTED, 'SETTINGS_WR_VALUE_REJECTED')
  *     __Pyx_globals['SETTINGS_WR_SETTING_REJECTED'] = SettingsWriteResponseCodes(SETTINGS_WR_SETTING_REJECTED, 'SETTINGS_WR_SETTING_REJECTED')
  *     __Pyx_globals['SETTINGS_WR_PARSE_FAILED'] = SettingsWriteResponseCodes(SETTINGS_WR_PARSE_FAILED, 'SETTINGS_WR_PARSE_FAILED')             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_READ_ONLY'] = SettingsWriteResponseCodes(SETTINGS_WR_READ_ONLY, 'SETTINGS_WR_READ_ONLY')
  *     __Pyx_globals['SETTINGS_WR_MODIFY_DISABLED'] = SettingsWriteResponseCodes(SETTINGS_WR_MODIFY_DISABLED, 'SETTINGS_WR_MODIFY_DISABLED')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 77, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 77, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_PARSE_FAILED); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 77, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 77, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_PARSE_FAILED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 77, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_PARSE_FAILED);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_PARSE_FAILED);
     PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_n_s_SETTINGS_WR_PARSE_FAILED);
-    __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_9, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 77, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 77, __pyx_L1_error)
+      __PYX_ERR(0, 77, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_PARSE_FAILED, __pyx_t_2) < 0)) __PYX_ERR(1, 77, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_PARSE_FAILED, __pyx_t_1) < 0)) __PYX_ERR(0, 77, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "EnumType":78
  *     __Pyx_globals['SETTINGS_WR_SETTING_REJECTED'] = SettingsWriteResponseCodes(SETTINGS_WR_SETTING_REJECTED, 'SETTINGS_WR_SETTING_REJECTED')
  *     __Pyx_globals['SETTINGS_WR_PARSE_FAILED'] = SettingsWriteResponseCodes(SETTINGS_WR_PARSE_FAILED, 'SETTINGS_WR_PARSE_FAILED')
  *     __Pyx_globals['SETTINGS_WR_READ_ONLY'] = SettingsWriteResponseCodes(SETTINGS_WR_READ_ONLY, 'SETTINGS_WR_READ_ONLY')             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_MODIFY_DISABLED'] = SettingsWriteResponseCodes(SETTINGS_WR_MODIFY_DISABLED, 'SETTINGS_WR_MODIFY_DISABLED')
  *     __Pyx_globals['SETTINGS_WR_SERVICE_FAILED'] = SettingsWriteResponseCodes(SETTINGS_WR_SERVICE_FAILED, 'SETTINGS_WR_SERVICE_FAILED')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 78, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_READ_ONLY); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 78, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_9 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_READ_ONLY); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 78, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_9);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_READ_ONLY);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_READ_ONLY);
     PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_n_s_SETTINGS_WR_READ_ONLY);
     __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_10, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 78, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_10, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 78, __pyx_L1_error)
+      __PYX_ERR(0, 78, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_READ_ONLY, __pyx_t_9) < 0)) __PYX_ERR(1, 78, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_READ_ONLY, __pyx_t_9) < 0)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     /* "EnumType":79
  *     __Pyx_globals['SETTINGS_WR_PARSE_FAILED'] = SettingsWriteResponseCodes(SETTINGS_WR_PARSE_FAILED, 'SETTINGS_WR_PARSE_FAILED')
  *     __Pyx_globals['SETTINGS_WR_READ_ONLY'] = SettingsWriteResponseCodes(SETTINGS_WR_READ_ONLY, 'SETTINGS_WR_READ_ONLY')
  *     __Pyx_globals['SETTINGS_WR_MODIFY_DISABLED'] = SettingsWriteResponseCodes(SETTINGS_WR_MODIFY_DISABLED, 'SETTINGS_WR_MODIFY_DISABLED')             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_SERVICE_FAILED'] = SettingsWriteResponseCodes(SETTINGS_WR_SERVICE_FAILED, 'SETTINGS_WR_SERVICE_FAILED')
  *     __Pyx_globals['SETTINGS_WR_TIMEOUT'] = SettingsWriteResponseCodes(SETTINGS_WR_TIMEOUT, 'SETTINGS_WR_TIMEOUT')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 79, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 79, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_MODIFY_DISABLED); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 79, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_MODIFY_DISABLED); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 79, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 79, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_10);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_10);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_10);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_MODIFY_DISABLED);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_MODIFY_DISABLED);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_SETTINGS_WR_MODIFY_DISABLED);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_SETTINGS_WR_MODIFY_DISABLED);
     __pyx_t_10 = 0;
-    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_2, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 79, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_1, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 79, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 79, __pyx_L1_error)
+      __PYX_ERR(0, 79, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_MODIFY_DISABLED, __pyx_t_10) < 0)) __PYX_ERR(1, 79, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_MODIFY_DISABLED, __pyx_t_10) < 0)) __PYX_ERR(0, 79, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
     /* "EnumType":80
  *     __Pyx_globals['SETTINGS_WR_READ_ONLY'] = SettingsWriteResponseCodes(SETTINGS_WR_READ_ONLY, 'SETTINGS_WR_READ_ONLY')
  *     __Pyx_globals['SETTINGS_WR_MODIFY_DISABLED'] = SettingsWriteResponseCodes(SETTINGS_WR_MODIFY_DISABLED, 'SETTINGS_WR_MODIFY_DISABLED')
  *     __Pyx_globals['SETTINGS_WR_SERVICE_FAILED'] = SettingsWriteResponseCodes(SETTINGS_WR_SERVICE_FAILED, 'SETTINGS_WR_SERVICE_FAILED')             # <<<<<<<<<<<<<<
  *     __Pyx_globals['SETTINGS_WR_TIMEOUT'] = SettingsWriteResponseCodes(SETTINGS_WR_TIMEOUT, 'SETTINGS_WR_TIMEOUT')
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 80, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 80, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_SERVICE_FAILED); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 80, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 80, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_SERVICE_FAILED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 80, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_SERVICE_FAILED);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_SERVICE_FAILED);
     PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_n_s_SETTINGS_WR_SERVICE_FAILED);
-    __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_9, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 80, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 80, __pyx_L1_error)
+      __PYX_ERR(0, 80, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_SERVICE_FAILED, __pyx_t_2) < 0)) __PYX_ERR(1, 80, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_SERVICE_FAILED, __pyx_t_1) < 0)) __PYX_ERR(0, 80, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "EnumType":81
  *     __Pyx_globals['SETTINGS_WR_MODIFY_DISABLED'] = SettingsWriteResponseCodes(SETTINGS_WR_MODIFY_DISABLED, 'SETTINGS_WR_MODIFY_DISABLED')
  *     __Pyx_globals['SETTINGS_WR_SERVICE_FAILED'] = SettingsWriteResponseCodes(SETTINGS_WR_SERVICE_FAILED, 'SETTINGS_WR_SERVICE_FAILED')
  *     __Pyx_globals['SETTINGS_WR_TIMEOUT'] = SettingsWriteResponseCodes(SETTINGS_WR_TIMEOUT, 'SETTINGS_WR_TIMEOUT')             # <<<<<<<<<<<<<<
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 81, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_TIMEOUT); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 81, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SettingsWriteResponseCodes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_9 = __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(__pyx_e_11libsettings_SETTINGS_WR_TIMEOUT); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 81, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 81, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 81, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_9);
     __Pyx_INCREF(__pyx_n_s_SETTINGS_WR_TIMEOUT);
     __Pyx_GIVEREF(__pyx_n_s_SETTINGS_WR_TIMEOUT);
     PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_n_s_SETTINGS_WR_TIMEOUT);
     __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_10, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 81, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_10, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 81, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (unlikely(__Pyx_globals == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 81, __pyx_L1_error)
+      __PYX_ERR(0, 81, __pyx_L1_error)
     }
-    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_TIMEOUT, __pyx_t_9) < 0)) __PYX_ERR(1, 81, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__Pyx_globals, __pyx_n_s_SETTINGS_WR_TIMEOUT, __pyx_t_9) < 0)) __PYX_ERR(0, 81, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __pyx_L4:;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
@@ -12159,15 +9295,15 @@
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_Check(key))) {
+        if (likely(PyString_CheckExact(key)) || likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
@@ -12186,15 +9322,15 @@
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
                 int cmp = (**name == key) ? 0 :
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
+                    (PyUnicode_GET_SIZE(**name) != PyUnicode_GET_SIZE(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key);
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
@@ -12202,15 +9338,15 @@
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
                 while (argname != first_kw_arg) {
                     int cmp = (**argname == key) ? 0 :
                     #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
+                        (PyUnicode_GET_SIZE(**argname) != PyUnicode_GET_SIZE(key)) ? 1 :
                     #endif
                         PyUnicode_Compare(**argname, key);
                     if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                     if (cmp == 0) goto arg_passed_twice;
                     argname++;
                 }
             }
@@ -12265,74 +9401,36 @@
     }
     PyErr_Format(PyExc_TypeError,
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
-/* PyDictVersioning */
-#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
-    PyObject *dict = Py_TYPE(obj)->tp_dict;
-    return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
-}
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
-    PyObject **dictptr = NULL;
-    Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
-    if (offset) {
-#if CYTHON_COMPILING_IN_CPYTHON
-        dictptr = (likely(offset > 0)) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
-#else
-        dictptr = _PyObject_GetDictPtr(obj);
-#endif
+/* PyCFunctionFastCall */
+#if CYTHON_FAST_PYCCALL
+static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
+    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
+    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
+    PyObject *self = PyCFunction_GET_SELF(func);
+    int flags = PyCFunction_GET_FLAGS(func);
+    assert(PyCFunction_Check(func));
+    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
+    assert(nargs >= 0);
+    assert(nargs == 0 || args != NULL);
+    /* _PyCFunction_FastCallDict() must not be called with an exception set,
+       because it may clear it (directly or indirectly) and so the
+       caller loses its exception */
+    assert(!PyErr_Occurred());
+    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
+        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
+    } else {
+        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
     }
-    return (dictptr && *dictptr) ? __PYX_GET_DICT_VERSION(*dictptr) : 0;
 }
-static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version) {
-    PyObject *dict = Py_TYPE(obj)->tp_dict;
-    if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
-        return 0;
-    return obj_dict_version == __Pyx_get_object_dict_version(obj);
-}
-#endif
-
-/* GetModuleGlobalName */
-#if CYTHON_USE_DICT_VERSIONS
-static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
-#else
-static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
-#endif
-{
-    PyObject *result;
-#if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
-    result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
-    } else if (unlikely(PyErr_Occurred())) {
-        return NULL;
-    }
-#else
-    result = PyDict_GetItem(__pyx_d, name);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
-    }
-#endif
-#else
-    result = PyObject_GetItem(__pyx_d, name);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
-    }
-    PyErr_Clear();
 #endif
-    return __Pyx_GetBuiltinName(name);
-}
 
 /* PyFunctionFastCall */
 #if CYTHON_FAST_PYCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
@@ -12357,15 +9455,15 @@
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
 #if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, int nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
 #endif
@@ -12428,20 +9526,20 @@
     }
     else {
         d = NULL;
         nd = 0;
     }
 #if PY_MAJOR_VERSION >= 3
     result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
+                               args, nargs,
                                k, (int)nk,
                                d, (int)nd, kwdefs, closure);
 #else
     result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
+                               args, nargs,
                                k, (int)nk,
                                d, (int)nd, closure);
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
@@ -12449,15 +9547,15 @@
 #endif
 #endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
+    ternaryfunc call = func->ob_type->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -12485,59 +9583,14 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCallNoArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
-    }
-#endif
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
-#else
-    if (likely(PyCFunction_Check(func)))
-#endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
-        }
-    }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
-}
-#endif
-
-/* PyCFunctionFastCall */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
-    }
-}
-#endif
-
 /* PyObjectCallOneArg */
 #if CYTHON_COMPILING_IN_CPYTHON
 static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
     PyObject *result;
     PyObject *args = PyTuple_New(1);
     if (unlikely(!args)) return NULL;
     Py_INCREF(arg);
@@ -12552,15 +9605,15 @@
         return __Pyx_PyFunction_FastCall(func, &arg, 1);
     }
 #endif
     if (likely(PyCFunction_Check(func))) {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
             return __Pyx_PyObject_CallMethO(func, arg);
 #if CYTHON_FAST_PYCCALL
-        } else if (__Pyx_PyFastCFunction_Check(func)) {
+        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
             return __Pyx_PyCFunction_FastCall(func, &arg, 1);
 #endif
         }
     }
     return __Pyx__PyObject_CallOneArg(func, arg);
 }
 #else
@@ -12570,144 +9623,313 @@
     if (unlikely(!args)) return NULL;
     result = __Pyx_PyObject_Call(func, args, NULL);
     Py_DECREF(args);
     return result;
 }
 #endif
 
-/* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
-    }
-    return exc_info;
+/* None */
+static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname) {
+    PyErr_Format(PyExc_NameError, "free variable '%s' referenced before assignment in enclosing scope", varname);
 }
+
+/* UnicodeAsUCS4 */
+static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject* x) {
+   Py_ssize_t length;
+   #if CYTHON_PEP393_ENABLED
+   length = PyUnicode_GET_LENGTH(x);
+   if (likely(length == 1)) {
+       return PyUnicode_READ_CHAR(x, 0);
+   }
+   #else
+   length = PyUnicode_GET_SIZE(x);
+   if (likely(length == 1)) {
+       return PyUnicode_AS_UNICODE(x)[0];
+   }
+   #if Py_UNICODE_SIZE == 2
+   else if (PyUnicode_GET_SIZE(x) == 2) {
+       Py_UCS4 high_val = PyUnicode_AS_UNICODE(x)[0];
+       if (high_val >= 0xD800 && high_val <= 0xDBFF) {
+           Py_UCS4 low_val = PyUnicode_AS_UNICODE(x)[1];
+           if (low_val >= 0xDC00 && low_val <= 0xDFFF) {
+               return 0x10000 + (((high_val & ((1<<10)-1)) << 10) | (low_val & ((1<<10)-1)));
+           }
+       }
+   }
+   #endif
+   #endif
+   PyErr_Format(PyExc_ValueError,
+                "only single character unicode strings can be converted to Py_UCS4, "
+                "got length %" CYTHON_FORMAT_SSIZE_T "d", length);
+   return (Py_UCS4)-1;
+}
+
+/* object_ord */
+static long __Pyx__PyObject_Ord(PyObject* c) {
+    Py_ssize_t size;
+    if (PyBytes_Check(c)) {
+        size = PyBytes_GET_SIZE(c);
+        if (likely(size == 1)) {
+            return (unsigned char) PyBytes_AS_STRING(c)[0];
+        }
+#if PY_MAJOR_VERSION < 3
+    } else if (PyUnicode_Check(c)) {
+        return (long)__Pyx_PyUnicode_AsPy_UCS4(c);
+#endif
+#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+    } else if (PyByteArray_Check(c)) {
+        size = PyByteArray_GET_SIZE(c);
+        if (likely(size == 1)) {
+            return (unsigned char) PyByteArray_AS_STRING(c)[0];
+        }
 #endif
+    } else {
+        PyErr_Format(PyExc_TypeError,
+            "ord() expected string of length 1, but %.200s found", c->ob_type->tp_name);
+        return (long)(Py_UCS4)-1;
+    }
+    PyErr_Format(PyExc_TypeError,
+        "ord() expected a character, but string of length %zd found", size);
+    return (long)(Py_UCS4)-1;
+}
 
-/* SaveResetException */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
+/* PyObjectCall2Args */
+static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
+    PyObject *args, *result = NULL;
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(function)) {
+        PyObject *args[2] = {arg1, arg2};
+        return __Pyx_PyFunction_FastCall(function, args, 2);
+    }
     #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(function)) {
+        PyObject *args[2] = {arg1, arg2};
+        return __Pyx_PyCFunction_FastCall(function, args, 2);
+    }
     #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
+    args = PyTuple_New(2);
+    if (unlikely(!args)) goto done;
+    Py_INCREF(arg1);
+    PyTuple_SET_ITEM(args, 0, arg1);
+    Py_INCREF(arg2);
+    PyTuple_SET_ITEM(args, 1, arg2);
+    Py_INCREF(function);
+    result = __Pyx_PyObject_Call(function, args, NULL);
+    Py_DECREF(args);
+    Py_DECREF(function);
+done:
+    return result;
+}
+
+/* StringJoin */
+#if !CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values) {
+    return PyObject_CallMethodObjArgs(sep, __pyx_n_s_join, values, NULL);
 }
 #endif
 
-/* GetException */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+/* PyObjectCallNoArg */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+#if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCall(func, NULL, 0);
+    }
+#endif
+#ifdef __Pyx_CyFunction_USED
+    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+    if (likely(PyCFunction_Check(func)))
 #endif
-{
-    PyObject *local_type, *local_value, *local_tb;
+    {
+        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+            return __Pyx_PyObject_CallMethO(func, NULL);
+        }
+    }
+    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
+}
+#endif
+
+/* RaiseTooManyValuesToUnpack */
+static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
+    PyErr_Format(PyExc_ValueError,
+                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
+}
+
+/* RaiseNeedMoreValuesToUnpack */
+static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
+    PyErr_Format(PyExc_ValueError,
+                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
+                 index, (index == 1) ? "" : "s");
+}
+
+/* IterFinish */
+static CYTHON_INLINE int __Pyx_IterFinish(void) {
 #if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
+    PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject* exc_type = tstate->curexc_type;
+    if (unlikely(exc_type)) {
+        if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) {
+            PyObject *exc_value, *exc_tb;
+            exc_value = tstate->curexc_value;
+            exc_tb = tstate->curexc_traceback;
+            tstate->curexc_type = 0;
+            tstate->curexc_value = 0;
+            tstate->curexc_traceback = 0;
+            Py_DECREF(exc_type);
+            Py_XDECREF(exc_value);
+            Py_XDECREF(exc_tb);
+            return 0;
+        } else {
+            return -1;
+        }
+    }
+    return 0;
 #else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
+    if (unlikely(PyErr_Occurred())) {
+        if (likely(PyErr_ExceptionMatches(PyExc_StopIteration))) {
+            PyErr_Clear();
+            return 0;
+        } else {
+            return -1;
+        }
+    }
+    return 0;
 #endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
+}
+
+/* UnpackItemEndCheck */
+static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
+    if (unlikely(retval)) {
+        Py_DECREF(retval);
+        __Pyx_RaiseTooManyValuesError(expected);
+        return -1;
+    } else {
+        return __Pyx_IterFinish();
+    }
+    return 0;
+}
+
+/* GetItemInt */
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+    PyObject *r;
+    if (!j) return NULL;
+    r = PyObject_GetItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyList_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
+        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 #else
-    if (unlikely(PyErr_Occurred()))
+    return PySequence_GetItem(o, i);
 #endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyTuple_GET_SIZE(o);
     }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
-    {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
+        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
     }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 #else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
+    return PySequence_GetItem(o, i);
 #endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
+                                                     CYTHON_NCP_UNUSED int wraparound,
+                                                     CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
+        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
+            PyObject *r = PyList_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    }
+    else if (PyTuple_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
+            PyObject *r = PyTuple_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    } else {
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return NULL;
+                    PyErr_Clear();
+                }
+            }
+            return m->sq_item(o, i);
+        }
+    }
+#else
+    if (is_list || PySequence_Check(o)) {
+        return PySequence_GetItem(o, i);
+    }
+#endif
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
+/* ObjectGetItem */
+#if CYTHON_USE_TYPE_SLOTS
+static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
+    PyObject *runerr;
+    Py_ssize_t key_value;
+    PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
+    if (unlikely(!(m && m->sq_item))) {
+        PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
+        return NULL;
+    }
+    key_value = __Pyx_PyIndex_AsSsize_t(index);
+    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
+        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
+    }
+    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
+        PyErr_Clear();
+        PyErr_Format(PyExc_IndexError, "cannot fit '%.200s' into an index-sized integer", Py_TYPE(index)->tp_name);
+    }
+    return NULL;
+}
+static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key) {
+    PyMappingMethods *m = Py_TYPE(obj)->tp_as_mapping;
+    if (likely(m && m->mp_subscript)) {
+        return m->mp_subscript(obj, key);
+    }
+    return __Pyx_PyObject_GetIndex(obj, key);
+}
+#endif
+
 /* PyErrFetchRestore */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
@@ -12861,347 +10083,107 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_FAST_THREAD_STATE
+#if CYTHON_COMPILING_IN_PYPY
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#else
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
-#else
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* PyObjectCall2Args */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
-    }
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
-    }
-    #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
+/* PyDictVersioning */
+#if CYTHON_USE_DICT_VERSIONS
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
+    PyObject *dict = Py_TYPE(obj)->tp_dict;
+    return dict ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
-
-/* DictGetItem */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            if (unlikely(PyTuple_Check(key))) {
-                PyObject* args = PyTuple_Pack(1, key);
-                if (likely(args)) {
-                    PyErr_SetObject(PyExc_KeyError, args);
-                    Py_DECREF(args);
-                }
-            } else {
-                PyErr_SetObject(PyExc_KeyError, key);
-            }
-        }
-        return NULL;
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
+    PyObject **dictptr = NULL;
+    Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
+    if (offset) {
+        dictptr = (offset > 0) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
     }
-    Py_INCREF(value);
-    return value;
+    return (dictptr && *dictptr) ? __PYX_GET_DICT_VERSION(*dictptr) : 0;
 }
-#endif
-
-/* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
-    PyObject *r;
-    if (!j) return NULL;
-    r = PyObject_GetItem(o, j);
-    Py_DECREF(j);
-    return r;
+static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version) {
+    PyObject *dict = Py_TYPE(obj)->tp_dict;
+    if (!dict || tp_dict_version != __PYX_GET_DICT_VERSION(dict))
+        return 0;
+    return obj_dict_version == __Pyx_get_object_dict_version(obj);
 }
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyList_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
-        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
 #endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyTuple_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
-        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+
+/* GetModuleGlobalName */
+#if CYTHON_USE_DICT_VERSIONS
+static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
 #else
-    return PySequence_GetItem(o, i);
+static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
 #endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
-                                                     CYTHON_NCP_UNUSED int wraparound,
-                                                     CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
-        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
-            PyObject *r = PyList_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    }
-    else if (PyTuple_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
-            PyObject *r = PyTuple_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return NULL;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_item(o, i);
-        }
+{
+    PyObject *result;
+#if !CYTHON_AVOID_BORROWED_REFS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+    result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
+    } else if (unlikely(PyErr_Occurred())) {
+        return NULL;
     }
 #else
-    if (is_list || PySequence_Check(o)) {
-        return PySequence_GetItem(o, i);
-    }
-#endif
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-}
-
-/* None */
-static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname) {
-    PyErr_Format(PyExc_NameError, "free variable '%s' referenced before assignment in enclosing scope", varname);
-}
-
-/* UnicodeAsUCS4 */
-static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject* x) {
-   Py_ssize_t length;
-   #if CYTHON_PEP393_ENABLED
-   length = PyUnicode_GET_LENGTH(x);
-   if (likely(length == 1)) {
-       return PyUnicode_READ_CHAR(x, 0);
-   }
-   #else
-   length = PyUnicode_GET_SIZE(x);
-   if (likely(length == 1)) {
-       return PyUnicode_AS_UNICODE(x)[0];
-   }
-   #if Py_UNICODE_SIZE == 2
-   else if (PyUnicode_GET_SIZE(x) == 2) {
-       Py_UCS4 high_val = PyUnicode_AS_UNICODE(x)[0];
-       if (high_val >= 0xD800 && high_val <= 0xDBFF) {
-           Py_UCS4 low_val = PyUnicode_AS_UNICODE(x)[1];
-           if (low_val >= 0xDC00 && low_val <= 0xDFFF) {
-               return 0x10000 + (((high_val & ((1<<10)-1)) << 10) | (low_val & ((1<<10)-1)));
-           }
-       }
-   }
-   #endif
-   #endif
-   PyErr_Format(PyExc_ValueError,
-                "only single character unicode strings can be converted to Py_UCS4, "
-                "got length %" CYTHON_FORMAT_SSIZE_T "d", length);
-   return (Py_UCS4)-1;
-}
-
-/* object_ord */
-static long __Pyx__PyObject_Ord(PyObject* c) {
-    Py_ssize_t size;
-    if (PyBytes_Check(c)) {
-        size = PyBytes_GET_SIZE(c);
-        if (likely(size == 1)) {
-            return (unsigned char) PyBytes_AS_STRING(c)[0];
-        }
-#if PY_MAJOR_VERSION < 3
-    } else if (PyUnicode_Check(c)) {
-        return (long)__Pyx_PyUnicode_AsPy_UCS4(c);
-#endif
-#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
-    } else if (PyByteArray_Check(c)) {
-        size = PyByteArray_GET_SIZE(c);
-        if (likely(size == 1)) {
-            return (unsigned char) PyByteArray_AS_STRING(c)[0];
-        }
-#endif
-    } else {
-        PyErr_Format(PyExc_TypeError,
-            "ord() expected string of length 1, but %.200s found", Py_TYPE(c)->tp_name);
-        return (long)(Py_UCS4)-1;
+    result = PyDict_GetItem(__pyx_d, name);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
     }
-    PyErr_Format(PyExc_TypeError,
-        "ord() expected a character, but string of length %zd found", size);
-    return (long)(Py_UCS4)-1;
-}
-
-/* StringJoin */
-#if !CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values) {
-    return PyObject_CallMethodObjArgs(sep, __pyx_n_s_join, values, NULL);
-}
 #endif
-
-/* RaiseTooManyValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
-    PyErr_Format(PyExc_ValueError,
-                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
-}
-
-/* RaiseNeedMoreValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
-    PyErr_Format(PyExc_ValueError,
-                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
-                 index, (index == 1) ? "" : "s");
-}
-
-/* IterFinish */
-static CYTHON_INLINE int __Pyx_IterFinish(void) {
-#if CYTHON_FAST_THREAD_STATE
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject* exc_type = tstate->curexc_type;
-    if (unlikely(exc_type)) {
-        if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) {
-            PyObject *exc_value, *exc_tb;
-            exc_value = tstate->curexc_value;
-            exc_tb = tstate->curexc_traceback;
-            tstate->curexc_type = 0;
-            tstate->curexc_value = 0;
-            tstate->curexc_traceback = 0;
-            Py_DECREF(exc_type);
-            Py_XDECREF(exc_value);
-            Py_XDECREF(exc_tb);
-            return 0;
-        } else {
-            return -1;
-        }
-    }
-    return 0;
 #else
-    if (unlikely(PyErr_Occurred())) {
-        if (likely(PyErr_ExceptionMatches(PyExc_StopIteration))) {
-            PyErr_Clear();
-            return 0;
-        } else {
-            return -1;
-        }
+    result = PyObject_GetItem(__pyx_d, name);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
     }
-    return 0;
+    PyErr_Clear();
 #endif
+    return __Pyx_GetBuiltinName(name);
 }
 
-/* UnpackItemEndCheck */
-static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
-    if (unlikely(retval)) {
-        Py_DECREF(retval);
-        __Pyx_RaiseTooManyValuesError(expected);
-        return -1;
-    }
-    return __Pyx_IterFinish();
-}
-
-/* ObjectGetItem */
-#if CYTHON_USE_TYPE_SLOTS
-static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr = NULL;
-    Py_ssize_t key_value;
-    PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
-    if (unlikely(!(m && m->sq_item))) {
-        PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
-        return NULL;
-    }
-    key_value = __Pyx_PyIndex_AsSsize_t(index);
-    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
-        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
-    }
-    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
-        PyErr_Clear();
-        PyErr_Format(PyExc_IndexError, "cannot fit '%.200s' into an index-sized integer", Py_TYPE(index)->tp_name);
-    }
-    return NULL;
-}
-static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key) {
-    PyMappingMethods *m = Py_TYPE(obj)->tp_as_mapping;
-    if (likely(m && m->mp_subscript)) {
-        return m->mp_subscript(obj, key);
-    }
-    return __Pyx_PyObject_GetIndex(obj, key);
-}
-#endif
-
 /* WriteUnraisableException */
 static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
                                   CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
                                   int full_traceback, CYTHON_UNUSED int nogil) {
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-    else state = (PyGILState_STATE)0;
+#ifdef _MSC_VER
+    else state = (PyGILState_STATE)-1;
+#endif
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -13285,14 +10267,144 @@
     {
         return PySequence_SetItem(o, i, v);
     }
 #endif
     return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
 }
 
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    #endif
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type, *local_value, *local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
 /* DelItemInt */
 static int __Pyx_DelItem_Generic(PyObject *o, PyObject *j) {
     int r;
     if (!j) return -1;
     r = PyObject_DelItem(o, j);
     Py_DECREF(j);
     return r;
@@ -13401,15 +10513,15 @@
         goto bad;
     empty_dict = PyDict_New();
     if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+            if (strchr(__Pyx_MODULE_NAME, '.')) {
                 module = PyImport_ImportModuleLevelObject(
                     name, global_dict, empty_dict, list, 1);
                 if (!module) {
                     if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -13518,36 +10630,14 @@
     if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
-/* PyObjectGetAttrStrNoError */
-static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        __Pyx_PyErr_Clear();
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
-    PyObject *result;
-#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
-        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
-    }
-#endif
-    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
-    if (unlikely(!result)) {
-        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
-    }
-    return result;
-}
-
 /* SetupReduce */
 static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
   name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name_2);
   if (likely(name_attr)) {
       ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
@@ -13560,89 +10650,61 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
-    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
-    PyObject *getstate = NULL;
-#if CYTHON_USE_PYTYPE_LOOKUP
-    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
-#else
-    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
-    if (!getstate && PyErr_Occurred()) {
-        goto __PYX_BAD;
-    }
-#endif
-    if (getstate) {
 #if CYTHON_USE_PYTYPE_LOOKUP
-        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto GOOD;
 #else
-        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
-        if (!object_getstate && PyErr_Occurred()) {
-            goto __PYX_BAD;
-        }
+    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto GOOD;
 #endif
-        if (object_getstate != getstate) {
-            goto __PYX_GOOD;
-        }
-    }
 #if CYTHON_USE_PYTYPE_LOOKUP
-    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
+    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto BAD;
 #else
-    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
+    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto BAD;
 #endif
-    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
+    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto BAD;
     if (reduce_ex == object_reduce_ex) {
 #if CYTHON_USE_PYTYPE_LOOKUP
-        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto BAD;
 #else
-        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto BAD;
 #endif
-        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto __PYX_BAD;
+        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto BAD;
         if (reduce == object_reduce || __Pyx_setup_reduce_is_named(reduce, __pyx_n_s_reduce_cython)) {
-            reduce_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_reduce_cython);
-            if (likely(reduce_cython)) {
-                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-            } else if (reduce == object_reduce || PyErr_Occurred()) {
-                goto __PYX_BAD;
-            }
+            reduce_cython = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_cython); if (unlikely(!reduce_cython)) goto BAD;
+            ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto BAD;
+            ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto BAD;
             setstate = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate);
             if (!setstate) PyErr_Clear();
             if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
-                setstate_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate_cython);
-                if (likely(setstate_cython)) {
-                    ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                    ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                } else if (!setstate || PyErr_Occurred()) {
-                    goto __PYX_BAD;
-                }
+                setstate_cython = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate_cython); if (unlikely(!setstate_cython)) goto BAD;
+                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto BAD;
+                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto BAD;
             }
             PyType_Modified((PyTypeObject*)type_obj);
         }
     }
-    goto __PYX_GOOD;
-__PYX_BAD:
+    goto GOOD;
+BAD:
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
-__PYX_GOOD:
+GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
-    Py_XDECREF(object_getstate);
-    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -13722,15 +10784,15 @@
     return cached_type;
 bad:
     Py_XDECREF(cached_type);
     cached_type = NULL;
     goto done;
 }
 
-/* CythonFunctionShared */
+/* CythonFunction */
 #include <structmember.h>
 static PyObject *
 __Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *closure)
 {
     if (unlikely(op->func_doc == NULL)) {
         if (op->func.m_ml->ml_doc) {
 #if PY_MAJOR_VERSION >= 3
@@ -14015,32 +11077,32 @@
     {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), PY_WRITE_RESTRICTED, 0},
     {0, 0, 0,  0, 0}
 };
 static PyObject *
 __Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, CYTHON_UNUSED PyObject *args)
 {
 #if PY_MAJOR_VERSION >= 3
-    Py_INCREF(m->func_qualname);
-    return m->func_qualname;
+    return PyUnicode_FromString(m->func.m_ml->ml_name);
 #else
     return PyString_FromString(m->func.m_ml->ml_name);
 #endif
 }
 static PyMethodDef __pyx_CyFunction_methods[] = {
     {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
     {0, 0, 0, 0}
 };
 #if PY_VERSION_HEX < 0x030500A0
 #define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
 #else
 #define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func.m_weakreflist)
 #endif
-static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
-                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
-    if (unlikely(op == NULL))
+static PyObject *__Pyx_CyFunction_New(PyTypeObject *type, PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    __pyx_CyFunctionObject *op = PyObject_GC_New(__pyx_CyFunctionObject, type);
+    if (op == NULL)
         return NULL;
     op->flags = flags;
     __Pyx_CyFunction_weakreflist(op) = NULL;
     op->func.m_ml = ml;
     op->func.m_self = (PyObject *) op;
     Py_XINCREF(closure);
     op->func_closure = closure;
@@ -14053,20 +11115,20 @@
     op->func_doc = NULL;
     op->func_classobj = NULL;
     op->func_globals = globals;
     Py_INCREF(op->func_globals);
     Py_XINCREF(code);
     op->func_code = code;
     op->defaults_pyobjects = 0;
-    op->defaults_size = 0;
     op->defaults = NULL;
     op->defaults_tuple = NULL;
     op->defaults_kwdict = NULL;
     op->defaults_getter = NULL;
     op->func_annotations = NULL;
+    PyObject_GC_Track(op);
     return (PyObject *) op;
 }
 static int
 __Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
 {
     Py_CLEAR(m->func_closure);
     Py_CLEAR(m->func.m_module);
@@ -14121,28 +11183,26 @@
         for (i = 0; i < m->defaults_pyobjects; i++)
             Py_VISIT(pydefaults[i]);
     }
     return 0;
 }
 static PyObject *__Pyx_CyFunction_descr_get(PyObject *func, PyObject *obj, PyObject *type)
 {
-#if PY_MAJOR_VERSION < 3
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     if (m->flags & __Pyx_CYFUNCTION_STATICMETHOD) {
         Py_INCREF(func);
         return func;
     }
     if (m->flags & __Pyx_CYFUNCTION_CLASSMETHOD) {
         if (type == NULL)
             type = (PyObject *)(Py_TYPE(obj));
         return __Pyx_PyMethod_New(func, type, (PyObject *)(Py_TYPE(type)));
     }
     if (obj == Py_None)
         obj = NULL;
-#endif
     return __Pyx_PyMethod_New(func, obj, type);
 }
 static PyObject*
 __Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
 {
 #if PY_MAJOR_VERSION >= 3
     return PyUnicode_FromFormat("<cyfunction %U at %p>",
@@ -14219,22 +11279,14 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
-#if PY_MAJOR_VERSION > 2
-            PyErr_Format(PyExc_TypeError,
-                         "unbound method %.200S() needs an argument",
-                         cyfunc->func_qualname);
-#else
-            PyErr_SetString(PyExc_TypeError,
-                            "unbound method needs an argument");
-#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -14295,26 +11347,14 @@
     0,
     0,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-    0,
-#endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
     }
     return 0;
@@ -14322,15 +11362,14 @@
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->defaults = PyObject_Malloc(size);
     if (unlikely(!m->defaults))
         return PyErr_NoMemory();
     memset(m->defaults, 0, size);
     m->defaults_pyobjects = pyobjects;
-    m->defaults_size = size;
     return m->defaults;
 }
 static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->defaults_tuple = tuple;
     Py_INCREF(tuple);
 }
@@ -14341,27 +11380,14 @@
 }
 static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->func_annotations = dict;
     Py_INCREF(dict);
 }
 
-/* CythonFunction */
-static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
-                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
-    PyObject *op = __Pyx_CyFunction_Init(
-        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
-        ml, flags, qualname, closure, module, globals, code
-    );
-    if (likely(op)) {
-        PyObject_GC_Track(op);
-    }
-    return op;
-}
-
 /* Py3ClassCreate */
 static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name,
                                            PyObject *qualname, PyObject *mkw, PyObject *modname, PyObject *doc) {
     PyObject *ns;
     if (metaclass) {
         PyObject *prep = __Pyx_PyObject_GetAttrStr(metaclass, __pyx_n_s_prepare);
         if (prep) {
@@ -14468,15 +11494,15 @@
     Py_XDECREF(names);
     Py_XDECREF(globals);
     return NULL;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -14498,15 +11524,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -14572,15 +11598,15 @@
         entries[pos].code_object = code_object;
         Py_DECREF(tmp);
         return;
     }
     if (__pyx_code_cache.count == __pyx_code_cache.max_count) {
         int new_max = __pyx_code_cache.max_count + 64;
         entries = (__Pyx_CodeObjectCacheEntry*)PyMem_Realloc(
-            __pyx_code_cache.entries, ((size_t)new_max) * sizeof(__Pyx_CodeObjectCacheEntry));
+            __pyx_code_cache.entries, (size_t)new_max*sizeof(__Pyx_CodeObjectCacheEntry));
         if (unlikely(!entries)) {
             return;
         }
         __pyx_code_cache.entries = entries;
         __pyx_code_cache.max_count = new_max;
     }
     for (i=__pyx_code_cache.count; i>pos; i--) {
@@ -14592,48 +11618,41 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = NULL;
-    PyObject *py_funcname = NULL;
+    PyCodeObject *py_code = 0;
+    PyObject *py_srcfile = 0;
+    PyObject *py_funcname = 0;
     #if PY_MAJOR_VERSION < 3
-    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    if (!py_srcfile) goto bad;
+    #else
+    py_srcfile = PyUnicode_FromString(filename);
     #endif
+    if (!py_srcfile) goto bad;
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
-        funcname = PyUnicode_AsUTF8(py_funcname);
-        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        if (!py_funcname) goto bad;
+        #else
+        py_funcname = PyUnicode_FromString(funcname);
         #endif
     }
-    #if PY_MAJOR_VERSION < 3
+    if (!py_funcname) goto bad;
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -14644,49 +11663,34 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    #else
-    py_code = PyCode_NewEmpty(filename, funcname, py_line);
-    #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_DECREF(py_funcname);
     return py_code;
 bad:
-    Py_XDECREF(py_funcname);
-    #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
-    #endif
+    Py_XDECREF(py_funcname);
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
-        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) {
-            /* If the code object creation fails, then we should clear the
-               fetched exception references and propagate the new exception */
-            Py_XDECREF(ptype);
-            Py_XDECREF(pvalue);
-            Py_XDECREF(ptraceback);
-            goto bad;
-        }
-        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
+        if (!py_code) goto bad;
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -14717,14 +11721,45 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
 /* Print */
 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION < 3
 static PyObject *__Pyx_GetStdout(void) {
     PyObject *f = PySys_GetObject((char *)"stdout");
     if (!f) {
         PyErr_SetString(PyExc_RuntimeError, "lost sys.stdout");
     }
@@ -14823,24 +11858,110 @@
 bad:
     if (kwargs != __pyx_print_kwargs)
         Py_XDECREF(kwargs);
     return -1;
 }
 #endif
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint16_t(uint16_t value) {
+    const uint16_t neg_one = (uint16_t) ((uint16_t) 0 - (uint16_t) 1), const_zero = (uint16_t) 0;
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(uint16_t) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(uint16_t) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(uint16_t) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(uint16_t) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(uint16_t) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(uint16_t),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint8_t(uint8_t value) {
+    const uint8_t neg_one = (uint8_t) ((uint8_t) 0 - (uint8_t) 1), const_zero = (uint8_t) 0;
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(uint8_t) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(uint8_t) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(uint8_t) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(uint8_t) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(uint8_t) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(uint8_t),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
 static CYTHON_INLINE uint16_t __Pyx_PyInt_As_uint16_t(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const uint16_t neg_one = (uint16_t) -1, const_zero = (uint16_t) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const uint16_t neg_one = (uint16_t) ((uint16_t) 0 - (uint16_t) 1), const_zero = (uint16_t) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(uint16_t) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(uint16_t, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -14883,15 +12004,15 @@
                         } else if (8 * sizeof(uint16_t) >= 4 * PyLong_SHIFT) {
                             return (uint16_t) (((((((((uint16_t)digits[3]) << PyLong_SHIFT) | (uint16_t)digits[2]) << PyLong_SHIFT) | (uint16_t)digits[1]) << PyLong_SHIFT) | (uint16_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15019,138 +12140,54 @@
     return (uint16_t) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to uint16_t");
     return (uint16_t) -1;
 }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
+/* PrintOne */
+#if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION < 3
+static int __Pyx_PrintOne(PyObject* f, PyObject *o) {
+    if (!f) {
+        if (!(f = __Pyx_GetStdout()))
+            return -1;
     }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
+    Py_INCREF(f);
+    if (PyFile_SoftSpace(f, 0)) {
+        if (PyFile_WriteString(" ", f) < 0)
+            goto error;
     }
+    if (PyFile_WriteObject(o, f, Py_PRINT_RAW) < 0)
+        goto error;
+    if (PyFile_WriteString("\n", f) < 0)
+        goto error;
+    Py_DECREF(f);
+    return 0;
+error:
+    Py_DECREF(f);
+    return -1;
+    /* the line below is just to avoid C compiler
+     * warnings about unused functions */
+    return __Pyx_Print(f, NULL, 0);
 }
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint16_t(uint16_t value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const uint16_t neg_one = (uint16_t) -1, const_zero = (uint16_t) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(uint16_t) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(uint16_t) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(uint16_t) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(uint16_t) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(uint16_t) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(uint16_t),
-                                     little, !is_unsigned);
-    }
+#else
+static int __Pyx_PrintOne(PyObject* stream, PyObject *o) {
+    int res;
+    PyObject* arg_tuple = PyTuple_Pack(1, o);
+    if (unlikely(!arg_tuple))
+        return -1;
+    res = __Pyx_Print(stream, arg_tuple, 1);
+    Py_DECREF(arg_tuple);
+    return res;
 }
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
 #endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
 
 /* CIntFromPy */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const size_t neg_one = (size_t) -1, const_zero = (size_t) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const size_t neg_one = (size_t) ((size_t) 0 - (size_t) 1), const_zero = (size_t) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(size_t) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(size_t, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -15193,15 +12230,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15331,22 +12368,15 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to size_t");
     return (size_t) -1;
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE uint8_t __Pyx_PyInt_As_uint8_t(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const uint8_t neg_one = (uint8_t) -1, const_zero = (uint8_t) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const uint8_t neg_one = (uint8_t) ((uint8_t) 0 - (uint8_t) 1), const_zero = (uint8_t) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(uint8_t) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(uint8_t, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -15389,15 +12419,15 @@
                         } else if (8 * sizeof(uint8_t) >= 4 * PyLong_SHIFT) {
                             return (uint8_t) (((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15525,99 +12555,17 @@
     return (uint8_t) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to uint8_t");
     return (uint8_t) -1;
 }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint8_t(uint8_t value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const uint8_t neg_one = (uint8_t) -1, const_zero = (uint8_t) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(uint8_t) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(uint8_t) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(uint8_t) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(uint8_t) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(uint8_t) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(uint8_t),
-                                     little, !is_unsigned);
-    }
-}
-
-/* PrintOne */
-#if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION < 3
-static int __Pyx_PrintOne(PyObject* f, PyObject *o) {
-    if (!f) {
-        if (!(f = __Pyx_GetStdout()))
-            return -1;
-    }
-    Py_INCREF(f);
-    if (PyFile_SoftSpace(f, 0)) {
-        if (PyFile_WriteString(" ", f) < 0)
-            goto error;
-    }
-    if (PyFile_WriteObject(o, f, Py_PRINT_RAW) < 0)
-        goto error;
-    if (PyFile_WriteString("\n", f) < 0)
-        goto error;
-    Py_DECREF(f);
-    return 0;
-error:
-    Py_DECREF(f);
-    return -1;
-    /* the line below is just to avoid C compiler
-     * warnings about unused functions */
-    return __Pyx_Print(f, NULL, 0);
-}
-#else
-static int __Pyx_PrintOne(PyObject* stream, PyObject *o) {
-    int res;
-    PyObject* arg_tuple = PyTuple_Pack(1, o);
-    if (unlikely(!arg_tuple))
-        return -1;
-    res = __Pyx_Print(stream, arg_tuple, 1);
-    Py_DECREF(arg_tuple);
-    return res;
-}
-#endif
-
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -15660,15 +12608,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15798,22 +12746,15 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum____pyx_t_11libsettings_SettingsWriteResponseCodes(enum __pyx_t_11libsettings_SettingsWriteResponseCodes value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const enum __pyx_t_11libsettings_SettingsWriteResponseCodes neg_one = (enum __pyx_t_11libsettings_SettingsWriteResponseCodes) -1, const_zero = (enum __pyx_t_11libsettings_SettingsWriteResponseCodes) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const enum __pyx_t_11libsettings_SettingsWriteResponseCodes neg_one = (enum __pyx_t_11libsettings_SettingsWriteResponseCodes) ((enum __pyx_t_11libsettings_SettingsWriteResponseCodes) 0 - (enum __pyx_t_11libsettings_SettingsWriteResponseCodes) 1), const_zero = (enum __pyx_t_11libsettings_SettingsWriteResponseCodes) 0;
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(enum __pyx_t_11libsettings_SettingsWriteResponseCodes) < sizeof(long)) {
             return PyInt_FromLong((long) value);
         } else if (sizeof(enum __pyx_t_11libsettings_SettingsWriteResponseCodes) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
@@ -15836,22 +12777,15 @@
         return _PyLong_FromByteArray(bytes, sizeof(enum __pyx_t_11libsettings_SettingsWriteResponseCodes),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -15894,15 +12828,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16282,20 +13216,14 @@
     if (unlikely(!method)) return NULL;
     return __Pyx__PyObject_CallMethod1(method, arg);
 }
 
 /* CoroutineBase */
 #include <structmember.h>
 #include <frameobject.h>
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
 #define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
 static int __Pyx_PyGen__FetchStopIterationValue(CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject **pvalue) {
     PyObject *et, *ev, *tb;
     PyObject *value = NULL;
     __Pyx_ErrFetch(&et, &ev, &tb);
     if (!et) {
         Py_XDECREF(tb);
@@ -16459,21 +13387,17 @@
     exc_state = &self->gi_exc_state;
     if (exc_state->exc_type) {
         #if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
         #else
         if (exc_state->exc_traceback) {
             PyTracebackObject *tb = (PyTracebackObject *) exc_state->exc_traceback;
             PyFrameObject *f = tb->tb_frame;
-            assert(f->f_back == NULL);
-            #if PY_VERSION_HEX >= 0x030B00A1
-            f->f_back = PyThreadState_GetFrame(tstate);
-            #else
             Py_XINCREF(tstate->frame);
+            assert(f->f_back == NULL);
             f->f_back = tstate->frame;
-            #endif
         }
         #endif
     }
 #if CYTHON_USE_EXC_INFO_STACK
     exc_state->previous_item = tstate->exc_info;
     tstate->exc_info = exc_state;
 #else
@@ -16518,38 +13442,14 @@
                 exc = __Pyx_PyExc_StopAsyncIteration;
             #endif
             __Pyx_PyErr_SetNone(exc);
         }
     }
     return retval;
 }
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
-static CYTHON_INLINE
-PyObject *__Pyx_PyGen_Send(PyGenObject *gen, PyObject *arg) {
-#if PY_VERSION_HEX <= 0x030A00A1
-    return _PyGen_Send(gen, arg);
-#else
-    PyObject *result;
-    if (PyIter_Send((PyObject*)gen, arg ? arg : Py_None, &result) == PYGEN_RETURN) {
-        if (PyAsyncGen_CheckExact(gen)) {
-            assert(result == Py_None);
-            PyErr_SetNone(PyExc_StopAsyncIteration);
-        }
-        else if (result == Py_None) {
-            PyErr_SetNone(PyExc_StopIteration);
-        }
-        else {
-            _PyGen_SetStopIterationValue(result);
-        }
-        Py_CLEAR(result);
-    }
-    return result;
-#endif
-}
-#endif
 static CYTHON_INLINE
 PyObject *__Pyx_Coroutine_FinishDelegation(__pyx_CoroutineObject *gen) {
     PyObject *ret;
     PyObject *val = NULL;
     __Pyx_Coroutine_Undelegate(gen);
     __Pyx_PyGen__FetchStopIterationValue(__Pyx_PyThreadState_Current, &val);
     ret = __Pyx_Coroutine_SendEx(gen, val, 0);
@@ -16578,20 +13478,20 @@
         #ifdef __Pyx_AsyncGen_USED
         if (__pyx_PyAsyncGenASend_CheckExact(yf)) {
             ret = __Pyx_async_gen_asend_send(yf, value);
         } else
         #endif
         #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
         if (PyGen_CheckExact(yf)) {
-            ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
+            ret = _PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
         } else
         #endif
         #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03050000 && defined(PyCoro_CheckExact) && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
         if (PyCoro_CheckExact(yf)) {
-            ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
+            ret = _PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
         } else
         #endif
         {
             if (value == Py_None)
                 ret = Py_TYPE(yf)->tp_iternext(yf);
             else
                 ret = __Pyx_PyObject_CallMethod1(yf, __pyx_n_s_send, value);
@@ -16667,15 +13567,15 @@
         #ifdef __Pyx_Generator_USED
         if (__Pyx_Generator_CheckExact(yf)) {
             ret = __Pyx_Generator_Next(yf);
         } else
         #endif
         #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
         if (PyGen_CheckExact(yf)) {
-            ret = __Pyx_PyGen_Send((PyGenObject*)yf, NULL);
+            ret = _PyGen_Send((PyGenObject*)yf, NULL);
         } else
         #endif
         #ifdef __Pyx_Coroutine_USED
         if (__Pyx_Coroutine_Check(yf)) {
             ret = __Pyx_Coroutine_Send(yf, Py_None);
         } else
         #endif
@@ -16827,15 +13727,14 @@
     __Pyx_Coroutine_ExceptionClear(&gen->gi_exc_state);
 #ifdef __Pyx_AsyncGen_USED
     if (__Pyx_AsyncGen_CheckExact(self)) {
         Py_CLEAR(((__pyx_PyAsyncGenObject*)gen)->ag_finalizer);
     }
 #endif
     Py_CLEAR(gen->gi_code);
-    Py_CLEAR(gen->gi_frame);
     Py_CLEAR(gen->gi_name);
     Py_CLEAR(gen->gi_qualname);
     Py_CLEAR(gen->gi_modulename);
     return 0;
 }
 static void __Pyx_Coroutine_dealloc(PyObject *self) {
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
@@ -16844,15 +13743,15 @@
         PyObject_ClearWeakRefs(self);
     if (gen->resume_label >= 0) {
         PyObject_GC_Track(self);
 #if PY_VERSION_HEX >= 0x030400a1 && CYTHON_USE_TP_FINALIZE
         if (PyObject_CallFinalizerFromDealloc(self))
 #else
         Py_TYPE(gen)->tp_del(self);
-        if (Py_REFCNT(self) > 0)
+        if (self->ob_refcnt > 0)
 #endif
         {
             return;
         }
         PyObject_GC_UnTrack(self);
     }
 #ifdef __Pyx_AsyncGen_USED
@@ -16871,15 +13770,15 @@
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
     __Pyx_PyThreadState_declare
     if (gen->resume_label < 0) {
         return;
     }
 #if !CYTHON_USE_TP_FINALIZE
     assert(self->ob_refcnt == 0);
-    __Pyx_SET_REFCNT(self, 1);
+    self->ob_refcnt = 1;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&error_type, &error_value, &error_traceback);
 #ifdef __Pyx_AsyncGen_USED
     if (__Pyx_AsyncGen_CheckExact(self)) {
         __pyx_PyAsyncGenObject *agen = (__pyx_PyAsyncGenObject*)self;
         PyObject *finalizer = agen->ag_finalizer;
@@ -16938,25 +13837,25 @@
                 PyErr_WriteUnraisable(self);
         } else {
             Py_DECREF(res);
         }
     }
     __Pyx_ErrRestore(error_type, error_value, error_traceback);
 #if !CYTHON_USE_TP_FINALIZE
-    assert(Py_REFCNT(self) > 0);
+    assert(self->ob_refcnt > 0);
     if (--self->ob_refcnt == 0) {
         return;
     }
     {
-        Py_ssize_t refcnt = Py_REFCNT(self);
+        Py_ssize_t refcnt = self->ob_refcnt;
         _Py_NewReference(self);
-        __Pyx_SET_REFCNT(self, refcnt);
+        self->ob_refcnt = refcnt;
     }
 #if CYTHON_COMPILING_IN_CPYTHON
-    assert(PyType_IS_GC(Py_TYPE(self)) &&
+    assert(PyType_IS_GC(self->ob_type) &&
            _Py_AS_GC(self)->gc.gc_refs != _PyGC_REFS_UNTRACKED);
     _Py_DEC_REFTOTAL;
 #endif
 #ifdef COUNT_ALLOCS
     --Py_TYPE(self)->tp_frees;
     --Py_TYPE(self)->tp_allocs;
 #endif
@@ -17014,35 +13913,14 @@
     }
     tmp = self->gi_qualname;
     Py_INCREF(value);
     self->gi_qualname = value;
     Py_XDECREF(tmp);
     return 0;
 }
-static PyObject *
-__Pyx_Coroutine_get_frame(__pyx_CoroutineObject *self, CYTHON_UNUSED void *context)
-{
-    PyObject *frame = self->gi_frame;
-    if (!frame) {
-        if (unlikely(!self->gi_code)) {
-            Py_RETURN_NONE;
-        }
-        frame = (PyObject *) PyFrame_New(
-            PyThreadState_Get(),            /*PyThreadState *tstate,*/
-            (PyCodeObject*) self->gi_code,  /*PyCodeObject *code,*/
-            __pyx_d,                 /*PyObject *globals,*/
-            0                               /*PyObject *locals*/
-        );
-        if (unlikely(!frame))
-            return NULL;
-        self->gi_frame = frame;
-    }
-    Py_INCREF(frame);
-    return frame;
-}
 static __pyx_CoroutineObject *__Pyx__Coroutine_New(
             PyTypeObject* type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
             PyObject *name, PyObject *qualname, PyObject *module_name) {
     __pyx_CoroutineObject *gen = PyObject_GC_New(__pyx_CoroutineObject, type);
     if (unlikely(!gen))
         return NULL;
     return __Pyx__Coroutine_NewInit(gen, body, code, closure, name, qualname, module_name);
@@ -17068,15 +13946,14 @@
     gen->gi_qualname = qualname;
     Py_XINCREF(name);
     gen->gi_name = name;
     Py_XINCREF(module_name);
     gen->gi_modulename = module_name;
     Py_XINCREF(code);
     gen->gi_code = code;
-    gen->gi_frame = NULL;
     PyObject_GC_Track(gen);
     return gen;
 }
 
 /* PatchModuleWithCoroutine */
 static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code) {
 #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
@@ -17192,16 +14069,14 @@
     {0, 0, 0, 0, 0}
 };
 static PyGetSetDef __pyx_Generator_getsets[] = {
     {(char *) "__name__", (getter)__Pyx_Coroutine_get_name, (setter)__Pyx_Coroutine_set_name,
      (char*) PyDoc_STR("name of the generator"), 0},
     {(char *) "__qualname__", (getter)__Pyx_Coroutine_get_qualname, (setter)__Pyx_Coroutine_set_qualname,
      (char*) PyDoc_STR("qualified name of the generator"), 0},
-    {(char *) "gi_frame", (getter)__Pyx_Coroutine_get_frame, NULL,
-     (char*) PyDoc_STR("Frame of the generator"), 0},
     {0, 0, 0, 0, 0}
 };
 static PyTypeObject __pyx_GeneratorType_type = {
     PyVarObject_HEAD_INIT(0, 0)
     "generator",
     sizeof(__pyx_CoroutineObject),
     0,
@@ -17253,66 +14128,32 @@
 #endif
     0,
 #if CYTHON_USE_TP_FINALIZE
     __Pyx_Coroutine_del,
 #elif PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-    0,
-#endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
     if (unlikely(!__pyx_GeneratorType)) {
         return -1;
     }
     return 0;
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
-        }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
-            break;
-        }
-    }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    char ctversion[4], rtversion[4];
+    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
+    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -17562,31 +14403,14 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
-  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
-    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
-#if PY_MAJOR_VERSION < 3
-  } else if (likely(PyInt_CheckExact(o))) {
-    return PyInt_AS_LONG(o);
-#endif
-  } else {
-    Py_ssize_t ival;
-    PyObject *x;
-    x = PyNumber_Index(o);
-    if (!x) return -1;
-    ival = PyInt_AsLong(x);
-    Py_DECREF(x);
-    return ival;
-  }
-}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `libsettings-0.1.14/python/libsettings.pyx` & `libsettings-0.1.9/python/libsettings.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 cimport cython
 
 from libc.stdint cimport uint8_t, uint16_t
 from libc.stdint cimport uintptr_t
 
 from sbp.msg import SBP, SENDER_ID
 
-from threading import Event, Lock
-
-from multiprocessing.pool import ThreadPool
+from threading import Event
 
 cpdef enum SettingsWriteResponseCodes:
     SETTINGS_WR_OK = 0
     SETTINGS_WR_VALUE_REJECTED = 1
     SETTINGS_WR_SETTING_REJECTED = 2
     SETTINGS_WR_PARSE_FAILED = 3
     SETTINGS_WR_READ_ONLY = 4
@@ -53,69 +51,64 @@
                                          uint16_t sbp_sender_id)
 
     ctypedef int (*settings_wait_init_t)(void *ctx)
     ctypedef int (*settings_wait_t)(void *ctx, int timeout_ms)
     ctypedef int (*settings_wait_deinit_t)(void *ctx)
     ctypedef void (*settings_signal_t)(void *ctx)
 
-    ctypedef int (*settings_wait_thd_t)(void *event, int timeout_ms)
-    ctypedef void (*settings_signal_thd_t)(void *event)
-
-    ctypedef void (*settings_lock_t)(void *ctx)
-    ctypedef void (*settings_unlock_t)(void *ctx)
-
     ctypedef int (*settings_reg_cb_t)(void *ctx,
                                       uint16_t msg_type,
                                       sbp_msg_callback_t cb,
                                       void *cb_context,
                                       sbp_msg_callbacks_node_t **node)
     ctypedef int (*settings_unreg_cb_t)(void *ctx, sbp_msg_callbacks_node_t **node)
 
     ctypedef void (*settings_log_t)(int priority, const char *format, ...)
-    ctypedef void (*settings_log_preformatted_t)(int priority, const char *format)
 
     cdef struct settings_api_s:
         void *ctx
         settings_send_t send
         settings_send_from_t send_from
         settings_wait_init_t wait_init
         settings_wait_t wait
         settings_wait_deinit_t wait_deinit
         settings_signal_t signal
-        settings_wait_thd_t wait_thd
-        settings_signal_thd_t signal_thd
-        settings_lock_t lock
-        settings_unlock_t unlock
         settings_reg_cb_t register_cb
         settings_unreg_cb_t unregister_cb
         settings_log_t log
-        settings_log_preformatted_t log_preformatted
-
+        bint log_preformat
     ctypedef settings_api_s settings_api_t
 
     settings_t *settings_create(uint16_t sender_id, settings_api_t *api_impl)
     void settings_destroy(settings_t **ctx)
 
     ctypedef int settings_type_t
     ctypedef int (*settings_notify_fn)(void *ctx)
 
+    int settings_register_setting(settings_t *ctx,
+                                  const char *section,
+                                  const char *name,
+                                  void *var,
+                                  size_t var_len,
+                                  settings_type_t stype,
+                                  settings_notify_fn notify,
+                                  void *notify_context)
+
     int settings_write_str(settings_t *ctx,
-                           void *event,
                            const char *section,
                            const char *name,
                            const char *str)
 
     int settings_read_str(settings_t *ctx,
                           const char *section,
                           const char *name,
                           char *str,
                           size_t str_len)
 
     int settings_read_by_idx(settings_t *ctx,
-                             void *event,
                              uint16_t idx,
                              char *section,
                              size_t section_len,
                              char *name,
                              size_t name_len,
                              char *value,
                              size_t value_len,
@@ -127,161 +120,92 @@
     cdef settings_t *ctx
     cdef settings_api_t c_api
 
     cdef readonly object _callbacks
     cdef public object _event
     cdef readonly object _link
     cdef readonly object _debug
-    cdef readonly object _lock
 
     def __init__(self, link, sender_id=SENDER_ID, debug=False):
         self.c_api.ctx = <void *>self
         self.c_api.send = &send_wrapper
         self.c_api.send_from = &send_from_wrapper
-        self.c_api.wait_init = &wait_init_wrapper
         self.c_api.wait = &wait_wrapper
         self.c_api.signal = &signal_wrapper
-        self.c_api.wait_thd = &wait_thd_wrapper
-        self.c_api.signal_thd = &signal_thd_wrapper
-        self.c_api.lock = &lock_wrapper
-        self.c_api.unlock = &unlock_wrapper
         self.c_api.register_cb = &register_cb_wrapper
         self.c_api.unregister_cb = &unregister_cb_wrapper
-        self.c_api.log_preformatted = log_wrapper
+        self.c_api.log = log_wrapper
+        self.c_api.log_preformat = True
 
         self.ctx = settings_create(sender_id, &self.c_api)
 
         self._link = link
 
         self._debug = debug
 
-        self._lock = Lock()
-
         self._callbacks = {}
 
     def destroy(self):
         settings_destroy(&self.ctx)
 
-    def write(self, section, name, value, encoding='ascii', multithread=False):
-        try:
-            if isinstance(value, str):
-                value = bytearray(value, encoding)
-            elif isinstance(value, int) or isinstance(value, float):
-                # 'ascii' will always be good enough for numeric characters
-                value = bytearray(str(value), 'ascii')
-            elif isinstance(value, unicode):
-                # python2 string can be 'str' or 'unicode'
-                value = bytearray(value, encoding)
-        except:
-            raise TypeError("Unsupported type {} for {}".format(type(value),
-                                                                value))
-
-        if multithread:
-            e = Event()
-            ret = settings_write_str(self.ctx,
-                                     <void*>e,
-                                     bytearray(section, encoding),
-                                     bytearray(name, encoding),
-                                     value)
-        else:
-            ret = settings_write_str(self.ctx,
-                                     NULL,
-                                     bytearray(section, encoding),
-                                     bytearray(name, encoding),
-                                     value)
-
-        return (ret, section, name, value.decode(encoding))
-
-    def write_all(self, settings, encoding='ascii', workers=10):
-        pool = ThreadPool(workers)
-
-        tasks = [(s['section'], s['name'], s['value'], encoding, True) for s in settings]
-        results = [pool.apply_async(self.write, t) for t in tasks]
-
-        ret = []
+    def write(self, section, name, value):
+        return settings_write_str(self.ctx,
+                                  bytes(section),
+                                  bytes(name),
+                                  bytes(str(value)))
 
-        for result in results:
-            ret.append(result.get())
-
-        pool.close()
-        pool.join()
-
-        return ret
-
-    def read(self, section, name, encoding='ascii'):
+    def read(self, section, name):
         cdef char value[SETTINGS_BUFLEN]
         ret = settings_read_str(self.ctx,
-                                bytearray(section, encoding),
-                                bytearray(name, encoding),
+                                bytes(section),
+                                bytes(name),
                                 value,
                                 sizeof(value))
         if (ret == 0):
-            return value.decode(encoding)
+            return str(value)
         else:
             return None
 
-    def _read_by_index(self, idx, encoding='ascii'):
+    def read_all(self):
         cdef char section[SETTINGS_BUFLEN]
         cdef char name[SETTINGS_BUFLEN]
         cdef char value[SETTINGS_BUFLEN]
         cdef char fmt_type[SETTINGS_BUFLEN]
-        e = Event()
-
-        ret = settings_read_by_idx(self.ctx,
-                                   <void*>e,
-                                   idx,
-                                   section,
-                                   sizeof(section),
-                                   name,
-                                   sizeof(name),
-                                   value,
-                                   sizeof(value),
-                                   fmt_type,
-                                   sizeof(fmt_type))
-
-        setting = None
-        if (0 == ret):
-            setting = {
-                          'section': section.decode(encoding),
-                          'name': name.decode(encoding),
-                          'value': value.decode(encoding),
-                          'fmt_type': fmt_type.decode(encoding),
-                      }
-
-        return (ret, setting)
+        cdef uint16_t idx = 0
 
-    def read_all(self, encoding='ascii', workers=10):
         settings = []
-        cdef uint16_t idx = 0
-        pool = ThreadPool(workers)
-        ret = None
 
-        while (ret is None):
-            tasks = [(i, encoding) for i in range(idx, idx + workers)]
-            results = [pool.apply_async(self._read_by_index, t) for t in tasks]
-
-            if not results:
-                ret = settings
-
-            for result in results:
-                res = result.get()
-                if (res[0] > 0):
-                    ret = settings
-                    break
-                elif (res[0] < 0):
-                    ret = []
-                    break
+        while (True):
+            ret = settings_read_by_idx(self.ctx,
+                                       idx,
+                                       section,
+                                       sizeof(section),
+                                       name,
+                                       sizeof(name),
+                                       value,
+                                       sizeof(value),
+                                       fmt_type,
+                                       sizeof(fmt_type))
 
-                settings.append(res[1])
-            idx += workers
+            if (ret > 0):
+                break
+            elif (ret < 0):
+                return []
 
-        pool.close()
-        pool.join()
+            setting = {
+                           'section': str(section),
+                           'name': str(name),
+                           'value': str(value),
+                           'fmt_type': str(fmt_type),
+                      }
 
-        return ret
+            settings.append(setting)
+            idx += 1
+
+        return settings
 
     def _callback_broker(self, sbp_msg, **metadata):
         if self._debug:
             print '_callback_broker', sbp_msg.msg_type
             print ":".join("{:02x}".format(ord(c)) for c in sbp_msg.payload)
 
         msg_type = sbp_msg.msg_type
@@ -298,15 +222,15 @@
             raise Exception("Callback not registered for message type {}".format(msg_type))
 
         cdef sbp_msg_callback_t cb = <sbp_msg_callback_t><uintptr_t>cb_data[1]
         cb(sbp_msg.sender, sbp_msg.length, bytes(sbp_msg.payload), <void*><uintptr_t>cb_data[2])
 
 cdef int send_wrapper(void *ctx, uint16_t msg_type, uint8_t length, uint8_t *payload):
     settings = <object>ctx
-
+    
     if settings._debug:
         print 'send_wrapper', msg_type
         print ":".join("{:02x}".format(ord(c)) for c in payload[:length])
 
     # https://cython.readthedocs.io/en/latest/src/tutorial/strings.html
     # See section "Passing byte strings".
     # Copying is needed to work around NULL bytes in settings.
@@ -324,52 +248,28 @@
 
     settings._link(SBP(msg_type=msg_type,
                        sender=sbp_sender_id,
                        length=length,
                        payload=payload[:length]))
     return 0
 
-cdef int wait_init_wrapper(void *ctx):
-    settings = <object>ctx
-    settings._event = Event()
-
 cdef int wait_wrapper(void *ctx, int timeout_ms):
     settings = <object>ctx
+    settings._event = Event()
     res = settings._event.wait(timeout_ms / 1000.0)
 
     if res:
         return 0
     else:
         return -1
 
 cdef void signal_wrapper(void *ctx):
     settings = <object>ctx
     settings._event.set()
 
-cdef int wait_thd_wrapper(void *event, int timeout_ms):
-    e = <object>event
-    res = e.wait(timeout_ms / 1000.0)
-
-    if res:
-        return 0
-    else:
-        return -1
-
-cdef void signal_thd_wrapper(void *event):
-    e = <object>event
-    e.set()
-
-cdef void lock_wrapper(void *ctx):
-    settings = <object>ctx
-    settings._lock.acquire()
-
-cdef void unlock_wrapper(void *ctx):
-    settings = <object>ctx
-    settings._lock.release()
-
 cdef int register_cb_wrapper(void *ctx,
                              uint16_t msg_type,
                              sbp_msg_callback_t cb,
                              void *cb_context,
                              sbp_msg_callbacks_node_t **node):
     try:
         settings = <object>ctx
@@ -387,11 +287,11 @@
         settings._link.remove_callback(settings._callback_broker, cb_data[0])
         del settings._callbacks[<uintptr_t>node]
     except:
         return -1
 
     return 0
 
-cdef void log_wrapper(int priority, const char *fmt):
+cdef void log_wrapper(int priority, const char *fmt, ...):
     # Currently no proper way to cythonize the variadic arguments..
     # https://github.com/cython/cython/wiki/FAQ#how-do-i-use-variable-args
     print fmt
```

### Comparing `libsettings-0.1.14/setup.py` & `libsettings-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,73 @@
+#!/usr/bin/env python
 # Copyright (C) 2018 Swift Navigation Inc.
 # Contact: <dev@swift-nav.com>
 #
 # This source is subject to the license found in the file 'LICENSE' which must
 # be be distributed together with this source. All other rights reserved.
 #
 # THIS CODE AND INFORMATION IS PROVIDED "AS IS" WITHOUT WARRANTY OF ANY KIND,
 # EITHER EXPRESSED OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE IMPLIED
 # WARRANTIES OF MERCHANTABILITY AND/OR FITNESS FOR A PARTICULAR PURPOSE.
 
-import os.path
-
 from glob import glob
 from setuptools import setup, Extension
 
 import os, sys
 
 CLASSIFIERS = [
-  "Intended Audience :: Developers",
-  "Intended Audience :: Science/Research",
-  "Operating System :: POSIX :: Linux",
-  "Operating System :: MacOS :: MacOS X",
-  "Operating System :: Microsoft :: Windows",
-  "Programming Language :: Python",
-  "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator",
-  "Topic :: Software Development :: Libraries :: Python Modules",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
+  'Intended Audience :: Developers',
+  'Intended Audience :: Science/Research',
+#  'Operating System :: POSIX :: Linux',
+  'Operating System :: MacOS :: MacOS X',
+  'Operating System :: Microsoft :: Windows',
+  'Programming Language :: Python',
+  'Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator',
+  'Topic :: Software Development :: Libraries :: Python Modules',
+  'Programming Language :: Python :: 2.7',
+  'Programming Language :: Python :: 3.4',
+  'Programming Language :: Python :: 3.5',
+  'Programming Language :: Python :: 3.6',
+  'Programming Language :: Python :: 3.7',
 ]
 
 PLATFORMS = [
-  "linux",
-  "osx",
-  "win32",
+  'linux',
+  'osx',
+  'win32',
 ]
 
-HERE = os.path.dirname(__file__)
-
-if HERE:
-    os.chdir(HERE)
+include_dirs = ["include", "libsbp/c/include", "libswiftnav/include"]
+sources = glob("python/*.pyx") + glob("src/*.c") + glob("libswiftnav/src/logging*.c") 
 
-include_dirs = ["include", "third_party/libsbp/c/include", "third_party/libswiftnav/include"]
-sources = glob("python/*.pyx") + glob("src/*.c") + glob("third_party/libswiftnav/src/logging*.c")
+py_version = '{}{}'.format(sys.version_info[0], sys.version_info[1])
 
+cflags = ["-Wno-unused-label", "-std=c99"]
 ldflags = []
 libraries = []
 
-if os.name == "nt":
-    cflags = []
-else:
-    cflags = ["-Wno-unused-label", "-std=c99"]
+if os.name == 'nt':
+    if py_version == '27' or py_version == '34':
+      ldflags.append("-static-libgcc")
+      libraries.append("python{}-gen".format(py_version))
+    else:
+       cflags = []
 
 setup(
-    name="libsettings",
-    version="0.1.14",
+    name='libsettings',
+    version="0.1.9",
     author="Swift Navigation",
     author_email="dev@swift-nav.com",
     description="Open source SwiftNav settings API library.",
     url="https://github.com/swift-nav/libsettings",
     classifiers=CLASSIFIERS,
     platforms=PLATFORMS,
-    options={"bdist_wheel": {"universal": True}},
     ext_modules=[
         Extension(
-            "libsettings",
+            'libsettings',
             sources,
             libraries=libraries,
             include_dirs=include_dirs,
             extra_compile_args=cflags,
             extra_link_args=ldflags,
         )
     ],
```

### Comparing `libsettings-0.1.14/src/setting_data.c` & `libsettings-0.1.9/src/setting_data.c`

 * *Files 5% similar despite different names*

```diff
@@ -10,68 +10,69 @@
  * WARRANTIES OF MERCHANTABILITY AND/OR FITNESS FOR A PARTICULAR PURPOSE.
  */
 
 #include <assert.h>
 #include <stdlib.h>
 #include <string.h>
 
-#include <swiftnav/logging.h>
-
 #include <libsettings/settings_util.h>
 
 #include <internal/setting_data.h>
 
-setting_data_t *setting_data_create(type_data_t *type_list, const char *section,
-                                    const char *name, void *var, size_t var_len,
+setting_data_t *setting_data_create(type_data_t *type_list,
+                                    const char *section,
+                                    const char *name,
+                                    void *var,
+                                    size_t var_len,
                                     settings_type_t type,
                                     settings_notify_fn notify,
-                                    void *notify_context, bool readonly,
-                                    bool watchonly) {
+                                    void *notify_context,
+                                    bool readonly,
+                                    bool watchonly)
+{
   /* Look up type data */
   type_data_t *type_data = type_data_lookup(type_list, type);
   assert(type_data != NULL);
 
   /* Set up setting data */
-  setting_data_t *setting_data =
-      (setting_data_t *)malloc(sizeof(*setting_data));
+  setting_data_t *setting_data = (setting_data_t *)malloc(sizeof(*setting_data));
   if (setting_data == NULL) {
     return NULL;
   }
 
-  size_t section_len = strlen(section);
-  size_t name_len = strlen(name);
-
   *setting_data = (setting_data_t){
-      .section = malloc(section_len + 1),
-      .name = malloc(name_len + 1),
-      .var = var,
-      .var_len = var_len,
-      .var_copy = malloc(var_len),
-      .type_data = type_data,
-      .notify = notify,
-      .notify_context = notify_context,
-      .readonly = readonly,
-      .watchonly = watchonly,
-      .next = NULL,
+    .section = malloc(strlen(section) + 1),
+    .name = malloc(strlen(name) + 1),
+    .var = var,
+    .var_len = var_len,
+    .var_copy = malloc(var_len),
+    .type_data = type_data,
+    .notify = notify,
+    .notify_context = notify_context,
+    .readonly = readonly,
+    .watchonly = watchonly,
+    .next = NULL,
   };
 
-  if ((setting_data->section == NULL) || (setting_data->name == NULL) ||
-      (setting_data->var_copy == NULL)) {
+  if ((setting_data->section == NULL) || (setting_data->name == NULL)
+      || (setting_data->var_copy == NULL)) {
     setting_data_destroy(setting_data);
     free(setting_data);
     setting_data = NULL;
   } else {
-    memcpy(setting_data->section, section, section_len + 1);
-    memcpy(setting_data->name, name, name_len + 1);
+    /* See setting_data initialization, section and name are guaranteed to fit */
+    strcpy(setting_data->section, section);
+    strcpy(setting_data->name, name);
   }
 
   return setting_data;
 }
 
-void setting_data_destroy(setting_data_t *setting_data) {
+void setting_data_destroy(setting_data_t *setting_data)
+{
   if (setting_data->section) {
     free(setting_data->section);
     setting_data->section = NULL;
   }
 
   if (setting_data->name) {
     free(setting_data->name);
@@ -80,30 +81,28 @@
 
   if (setting_data->var_copy) {
     free(setting_data->var_copy);
     setting_data->var_copy = NULL;
   }
 }
 
-settings_write_res_t setting_data_update_value(setting_data_t *setting_data,
-                                               const char *value) {
+settings_write_res_t setting_data_update_value(setting_data_t *setting_data, const char *value)
+{
   if (setting_data->readonly) {
-    log_warn("trying to update read only setting %s.%s", setting_data->section,
-             setting_data->name);
     return SETTINGS_WR_READ_ONLY;
   }
 
   /* Store copy and update value */
   memcpy(setting_data->var_copy, setting_data->var, setting_data->var_len);
   if (!setting_data->type_data->from_string(setting_data->type_data->priv,
                                             setting_data->var,
-                                            setting_data->var_len, value)) {
+                                            setting_data->var_len,
+                                            value)) {
     /* Revert value if conversion fails */
     memcpy(setting_data->var, setting_data->var_copy, setting_data->var_len);
-    log_error("parsing failed while updating setting value");
     return SETTINGS_WR_PARSE_FAILED;
   }
 
   if (NULL == setting_data->notify) {
     return SETTINGS_WR_OK;
   }
 
@@ -113,43 +112,46 @@
   if (setting_data->watchonly) {
     /* No need for actions */
     return SETTINGS_WR_OK;
   }
 
   if (res != SETTINGS_WR_OK) {
     /* Revert value if notify returns error */
-    log_error("setting value update notify failed for %s.%s",
-              setting_data->section, setting_data->name);
     memcpy(setting_data->var, setting_data->var_copy, setting_data->var_len);
   }
 
   return res;
 }
 
-int setting_data_format(setting_data_t *setting_data, bool type, char *buf,
-                        int blen, uint8_t *msg_hdr_len) {
+int setting_data_format(setting_data_t *setting_data,
+                        bool type,
+                        char *buf,
+                        int blen,
+                        uint8_t *msg_hdr_len)
+{
   int res = 0;
   int bytes = 0;
 
-  res = settings_format(setting_data->section, setting_data->name, NULL, NULL,
-                        buf, blen);
+  res = settings_format(setting_data->section, setting_data->name, NULL, NULL, buf, blen);
 
   if (res <= 0) {
     return -1;
   }
   bytes += res;
 
   if (msg_hdr_len != NULL) {
     *msg_hdr_len = res;
   }
 
   /* Value */
-  res = setting_data->type_data->to_string(
-      setting_data->type_data->priv, &buf[bytes], blen - bytes,
-      setting_data->var, setting_data->var_len);
+  res = setting_data->type_data->to_string(setting_data->type_data->priv,
+                                           &buf[bytes],
+                                           blen - bytes,
+                                           setting_data->var,
+                                           setting_data->var_len);
   if ((res < 0) || (res >= blen - bytes)) {
     return -1;
   }
   /* Add terminating null (+ 1) */
   bytes += res + 1;
 
   if (!type) {
@@ -157,45 +159,45 @@
   }
 
   /* Type information */
   if (setting_data->type_data->format_type == NULL) {
     return bytes;
   }
 
-  res = setting_data->type_data->format_type(setting_data->type_data->priv,
-                                             &buf[bytes], blen - bytes);
+  res =
+    setting_data->type_data->format_type(setting_data->type_data->priv, &buf[bytes], blen - bytes);
   if ((res < 0) || (res >= blen - bytes)) {
     return -1;
   }
   /* Add terminating null (+ 1) */
   bytes += res + 1;
 
   return bytes;
 }
 
-void setting_data_append(setting_data_t **data_list,
-                         setting_data_t *setting_data) {
+void setting_data_append(setting_data_t **data_list, setting_data_t *setting_data)
+{
   if (*data_list == NULL) {
     *data_list = setting_data;
   } else {
     setting_data_t *s;
     /* Find last element in the same section */
     for (s = *data_list; s->next != NULL; s = s->next) {
-      if ((strcmp(s->section, setting_data->section) == 0) &&
-          (strcmp(s->next->section, setting_data->section) != 0)) {
+      if ((strcmp(s->section, setting_data->section) == 0)
+          && (strcmp(s->next->section, setting_data->section) != 0)) {
         break;
       }
     }
     setting_data->next = s->next;
     s->next = setting_data;
   }
 }
 
-void setting_data_remove(setting_data_t **data_list,
-                         setting_data_t **setting_data) {
+void setting_data_remove(setting_data_t **data_list, setting_data_t **setting_data)
+{
   assert(data_list != NULL);
   assert(setting_data != NULL);
   assert(*setting_data != NULL);
 
   setting_data_t *curr = *data_list;
   setting_data_t *prev = NULL;
   /* Find element to remove */
@@ -217,26 +219,28 @@
     free(*setting_data);
     *setting_data = NULL;
     break;
   }
 }
 
 setting_data_t *setting_data_lookup(setting_data_t *data_list,
-                                    const char *section, const char *name) {
+                                    const char *section,
+                                    const char *name)
+{
   while (data_list != NULL) {
-    if ((strcmp(data_list->section, section) == 0) &&
-        (strcmp(data_list->name, name) == 0)) {
+    if ((strcmp(data_list->section, section) == 0) && (strcmp(data_list->name, name) == 0)) {
       break;
     }
     data_list = data_list->next;
   }
   return data_list;
 }
 
-void setting_data_free(setting_data_t *data_list) {
+void setting_data_free(setting_data_t *data_list)
+{
   /* Free setting data list elements */
   while (data_list != NULL) {
     setting_data_t *s = data_list;
     data_list = data_list->next;
     setting_data_destroy(s);
     free(s);
   }
```

### Comparing `libsettings-0.1.14/src/setting_sbp_cb.c` & `libsettings-0.1.9/src/setting_sbp_cb.c`

 * *Files 20% similar despite different names*

```diff
@@ -19,391 +19,366 @@
 #include <swiftnav/logging.h>
 
 #include <libsettings/settings_util.h>
 
 #include <internal/request_state.h>
 #include <internal/setting_data.h>
 #include <internal/setting_def.h>
-#include <internal/setting_macros.h>
 #include <internal/setting_sbp_cb.h>
 
-#define UPDATE_FILTER_NONE 0x0
-#define UPDATE_FILTER_BASIC (0x1 << 3)
-#define UPDATE_FILTER_READONLY (0x1 << 1)
-#define UPDATE_FILTER_WATCHONLY (0x1 << 2)
-
-#define update_filter_check(filter_mask, filter_enum) \
-  (filter_mask & filter_enum)
-
 /**
  * @brief setting_send_write_response
  * @param write_response: pre-formatted write response sbp message
  * @param len: length of the message
  * @return zero on success, -1 if message failed to send
  */
 static int setting_send_write_response(settings_t *ctx,
-                                       setting_data_t *setting_data,
-                                       settings_write_res_t write_result) {
-  uint8_t resp[SETTINGS_BUFLEN] = {0};
-  uint8_t resp_len = 0;
-  msg_settings_write_resp_t *write_response = (msg_settings_write_resp_t *)resp;
-  write_response->status = write_result;
-  resp_len += sizeof(write_response->status);
-  int l = setting_data_format(setting_data, false, write_response->setting,
-                              sizeof(resp) - resp_len, NULL);
-  if (l < 0) {
-    log_error("formatting settings write response failed");
-    return -1;
-  }
-  resp_len += l;
-
+                                       msg_settings_write_resp_t *write_response,
+                                       uint8_t len)
+{
   settings_api_t *api = &ctx->client_iface;
-  if (api->send(api->ctx, SBP_MSG_SETTINGS_WRITE_RESP, resp_len,
-                (uint8_t *)write_response) != 0) {
+  if (api->send(api->ctx, SBP_MSG_SETTINGS_WRITE_RESP, len, (uint8_t *)write_response) != 0) {
     log_error("sending settings write response failed");
     return -1;
   }
   return 0;
 }
 
-static void setting_update_value(settings_t *ctx, const char *msg, uint8_t len,
-                                 uint32_t filter) {
+static void setting_update_value(settings_t *ctx, uint8_t *msg, uint8_t len)
+{
   /* Extract parameters from message:
    * 4 null terminated strings: section, name, value and type.
    * Expect to find at least section, name and value.
    */
   const char *section = NULL, *name = NULL, *value = NULL, *type = NULL;
-  if (settings_parse((char *)msg, len, &section, &name, &value, &type) <
-      SETTINGS_TOKENS_VALUE) {
+  if (settings_parse((char *)msg, len, &section, &name, &value, &type) < SETTINGS_TOKENS_VALUE) {
     log_warn("setting update value, error parsing setting");
     return;
   }
 
   /* Look up setting data */
-  setting_data_t *setting_data =
-      setting_data_lookup(ctx->setting_data_list, section, name);
+  setting_data_t *setting_data = setting_data_lookup(ctx->setting_data_list, section, name);
   if (setting_data == NULL) {
     return;
   }
 
-  if (update_filter_check(filter, UPDATE_FILTER_WATCHONLY) &&
-      setting_data->watchonly) {
+  if (setting_data->watchonly) {
     return;
   }
 
-  if (update_filter_check(filter, UPDATE_FILTER_READONLY) &&
-      setting_data->readonly) {
-    return;
-  }
-
-  if (update_filter_check(filter, UPDATE_FILTER_BASIC) &&
-      !setting_data->readonly && !setting_data->watchonly) {
-    return;
-  }
+  settings_write_res_t write_result = setting_data_update_value(setting_data, value);
 
-  /* Reject messages that are too large for READ_BY_INDEX_RESP*/
-  if (len > MAX_SETTING_WRITE_LEN) {
-    setting_send_write_response(ctx, setting_data, SETTINGS_WR_VALUE_REJECTED);
-    log_warn("setting message rejected, length:%u limit:%u", len,
-             MAX_SETTING_WRITE_LEN);
+  uint8_t resp[SETTINGS_BUFLEN] = {0};
+  uint8_t resp_len = 0;
+  msg_settings_write_resp_t *write_response = (msg_settings_write_resp_t *)resp;
+  write_response->status = write_result;
+  resp_len += sizeof(write_response->status);
+  int l = setting_data_format(setting_data,
+                              false,
+                              write_response->setting,
+                              sizeof(resp) - resp_len,
+                              NULL);
+  if (l < 0) {
     return;
   }
+  resp_len += l;
 
-  settings_write_res_t write_result =
-      setting_data_update_value(setting_data, value);
-
-  /* In case of watcher, do not send write response */
-  if (!setting_data->watchonly) {
-    setting_send_write_response(ctx, setting_data, write_result);
-  }
+  setting_send_write_response(ctx, write_response, resp_len);
 }
 
-static void setting_register_resp_callback(uint16_t sender_id, uint8_t len,
-                                           uint8_t *msg, void *context) {
+static void setting_register_resp_callback(uint16_t sender_id,
+                                           uint8_t len,
+                                           uint8_t *msg,
+                                           void *context)
+{
   settings_t *ctx = (settings_t *)context;
   (void)sender_id;
 
   if (sender_id != SBP_SENDER_ID) {
     log_warn("invalid sender %d != %d", sender_id, SBP_SENDER_ID);
     return;
   }
 
   msg_settings_register_resp_t *resp = (msg_settings_register_resp_t *)msg;
 
-  switch ((settings_reg_res_t)resp->status) {
-    case SETTINGS_REG_PARSE_FAILED:
-      /* In case the request was corrupted during transfer, let the timeout
-       * trigger and request be sent again, parse error is printed in
-       * sbp_settings_daemon */
-      return;
-
-    /* Use the returned value to update in all cases */
-    case SETTINGS_REG_OK:
-    case SETTINGS_REG_OK_PERM:
-    case SETTINGS_REG_REGISTERED:
-      break;
-
-    default:
-      log_error("invalid reg resp return code %d", resp->status);
-      return;
+  if (resp->status == SETTINGS_REG_PARSE_FAILED) {
+    /* In case the request was corrupted during transfer, let the timeout trigger
+     * and request be sent again, parse error is printed in sbp_settings_daemon */
+    return;
   }
 
   /* Check for a response to a pending registration request */
-  request_state_t *state =
-      request_state_check(ctx, resp->setting, len - sizeof(resp->status));
+  int state = request_state_check(&ctx->request_state,
+                                  &ctx->client_iface,
+                                  resp->setting,
+                                  len - sizeof(resp->status));
 
-  if (NULL == state) {
-    /* No pending registration request or no pending request and the response
-     * don't match, most likely this response was meant to some other client
-     * doing registration at the same time. */
+  if (state > 0) {
+    /* No pending registration request */
     return;
   }
 
-  /* In case of readonly, trust the initialized value.
-   * Watchers shall not be readonly. */
-  setting_update_value(ctx, resp->setting, len - sizeof(resp->status),
-                       UPDATE_FILTER_READONLY);
+  if (state < 0) {
+    /* Pending request and the response don't match, most likely this response
+     * was meant to some other client doing registration at the same time. */
+    return;
+  }
 
-  request_state_signal(state, &ctx->client_iface, SBP_MSG_SETTINGS_REGISTER);
+  setting_update_value(ctx, (uint8_t *)resp->setting, len - sizeof(resp->status));
 }
 
-static void setting_write_callback(uint16_t sender_id, uint8_t len,
-                                   uint8_t *msg, void *context) {
+static void setting_write_callback(uint16_t sender_id, uint8_t len, uint8_t *msg, void *context)
+{
   settings_t *ctx = (settings_t *)context;
   (void)sender_id;
 
   if (sender_id != SBP_SENDER_ID) {
     log_warn("invalid sender %d != %d", sender_id, SBP_SENDER_ID);
     return;
   }
 
-  msg_settings_write_t *request = (msg_settings_write_t *)msg;
+  setting_update_value(ctx, msg, len);
+}
+
+static int setting_update_watch_only(settings_t *ctx, const char *msg, uint8_t len)
+{
+  /* Extract parameters from message:
+   * 4 null terminated strings: section, name, value and type
+   * Expect to find at least section, name and value.
+   */
+  const char *section = NULL, *name = NULL, *value = NULL, *type = NULL;
+  if (settings_parse(msg, len, &section, &name, &value, &type) < SETTINGS_TOKENS_VALUE) {
+    log_warn("updating watched values failed, error parsing setting");
+    return -1;
+  }
+
+  /* Look up setting data */
+  setting_data_t *setting_data = setting_data_lookup(ctx->setting_data_list, section, name);
+  if (setting_data == NULL) {
+    return 0;
+  }
+
+  if (!setting_data->watchonly) {
+    return 0;
+  }
+
+  if (setting_data_update_value(setting_data, value) != SETTINGS_WR_OK) {
+    return -1;
+  }
 
-  /* Update value, ignore watchers, they are updated from
-   * setting_write_resp_callback() */
-  setting_update_value(ctx, request->setting, len, UPDATE_FILTER_WATCHONLY);
+  return 0;
 }
 
-static void setting_read_resp_callback(uint16_t sender_id, uint8_t len,
-                                       uint8_t *msg, void *context) {
+static void setting_read_resp_callback(uint16_t sender_id,
+                                       uint8_t len,
+                                       uint8_t msg[],
+                                       void *context)
+{
   (void)sender_id;
   assert(msg);
   assert(context);
 
   settings_t *ctx = (settings_t *)context;
-  const msg_settings_read_resp_t *read_response =
-      (msg_settings_read_resp_t *)msg;
+  const msg_settings_read_resp_t *read_response = (msg_settings_read_resp_t *)msg;
 
   /* Check for a response to a pending request */
-  request_state_t *state =
-      request_state_check(ctx, read_response->setting, len);
+  int res =
+    request_state_check(&ctx->request_state, &ctx->client_iface, read_response->setting, len);
 
-  if (NULL == state) {
+  if (res != 0) {
     return;
   }
 
-  state->resp_value_valid = false;
-  state->resp_value[0] = '\0';
-  state->resp_type[0] = '\0';
+  if (setting_update_watch_only(ctx, read_response->setting, len) != 0) {
+    log_warn("error in settings read response message");
+  }
 
-  const char *section = NULL, *name = NULL, *value = NULL, *type = NULL;
-  settings_tokens_t tokens = settings_parse(read_response->setting, len,
-                                            &section, &name, &value, &type);
-  if (tokens >= SETTINGS_TOKENS_VALUE) {
+  const char *value = NULL, *type = NULL;
+  if (settings_parse(read_response->setting, len, NULL, NULL, &value, &type)
+      >= SETTINGS_TOKENS_VALUE) {
     if (value) {
-      strncpy(state->resp_value, value, sizeof(state->resp_value) - 1);
-      state->resp_value[sizeof(state->resp_value) - 1] = '\0';
-      state->resp_value_valid = true;
+      strncpy(ctx->resp_value, value, sizeof(ctx->resp_value));
     }
     if (type) {
-      strncpy(state->resp_type, type, sizeof(state->resp_type) - 1);
-      state->resp_type[sizeof(state->resp_type) - 1] = '\0';
+      strncpy(ctx->resp_type, type, sizeof(ctx->resp_type));
     }
-  } else if (tokens == SETTINGS_TOKENS_NAME) {
-    log_debug("setting %s.%s not found", section, name);
   } else {
     log_warn("read response parsing failed");
+    ctx->resp_value[0] = '\0';
+    ctx->resp_type[0] = '\0';
   }
-
-  request_state_signal(state, &ctx->client_iface, SBP_MSG_SETTINGS_READ_REQ);
 }
 
-static void setting_write_resp_callback(uint16_t sender_id, uint8_t len,
-                                        uint8_t *msg, void *context) {
+static void setting_write_resp_callback(uint16_t sender_id,
+                                        uint8_t len,
+                                        uint8_t msg[],
+                                        void *context)
+{
   (void)sender_id;
   settings_t *ctx = (settings_t *)context;
   msg_settings_write_resp_t *write_response = (msg_settings_write_resp_t *)msg;
 
-  if (write_response->status == SETTINGS_WR_OK) {
-    /* Update watchers, do not update the actual setting since it's already done
-     * in setting_write_callback() */
-    setting_update_value(ctx, write_response->setting,
-                         len - sizeof(write_response->status),
-                         UPDATE_FILTER_BASIC);
-  }
+  ctx->status = write_response->status;
 
   /* Check for a response to a pending request */
-  request_state_t *state = request_state_check(
-      ctx, write_response->setting, len - sizeof(write_response->status));
+  request_state_check(&ctx->request_state,
+                      &ctx->client_iface,
+                      write_response->setting,
+                      len - sizeof(write_response->status));
 
-  if (NULL == state) {
+  if (write_response->status != SETTINGS_WR_OK) {
+    /* Enable this warning back after ESD-1022 is fixed
+     * log_warn(
+     *                       "setting write rejected (code: %d), not updating watched values",
+     *                       write_response->status);
+     */
     return;
   }
 
-  state->status = write_response->status;
-
-  request_state_signal(state, &ctx->client_iface, SBP_MSG_SETTINGS_WRITE);
+  if (setting_update_watch_only(ctx, write_response->setting, len - sizeof(write_response->status))
+      != 0) {
+    log_warn("error in settings read response message");
+  }
 }
 
-static void setting_read_by_index_resp_callback(uint16_t sender_id, uint8_t len,
-                                                uint8_t *msg, void *context) {
+static void setting_read_by_index_resp_callback(uint16_t sender_id,
+                                                uint8_t len,
+                                                uint8_t msg[],
+                                                void *context)
+{
   (void)sender_id;
   settings_t *ctx = (settings_t *)context;
-  msg_settings_read_by_index_resp_t *resp =
-      (msg_settings_read_by_index_resp_t *)msg;
+  msg_settings_read_by_index_resp_t *resp = (msg_settings_read_by_index_resp_t *)msg;
 
   /* Check for a response to a pending request */
-  request_state_t *state =
-      request_state_check(ctx, (char *)msg, sizeof(resp->index));
+  int res =
+    request_state_check(&ctx->request_state, &ctx->client_iface, (char *)msg, sizeof(resp->index));
 
-  if (NULL == state) {
+  if (res != 0) {
     return;
   }
 
-  state->resp_value_valid = false;
-  state->resp_section[0] = '\0';
-  state->resp_name[0] = '\0';
-  state->resp_value[0] = '\0';
-  state->resp_type[0] = '\0';
-
   const char *section = NULL, *name = NULL, *value = NULL, *type = NULL;
-  if (settings_parse(resp->setting, len - sizeof(resp->index), &section, &name,
-                     &value, &type) > 0) {
+
+  if (settings_parse(resp->setting, len - sizeof(resp->index), &section, &name, &value, &type)
+      > 0) {
     if (section) {
-      strncpy(state->resp_section, section, sizeof(state->resp_section) - 1);
-      state->resp_section[sizeof(state->resp_section) - 1] = '\0';
+      strncpy(ctx->resp_section, section, sizeof(ctx->resp_section));
     }
     if (name) {
-      strncpy(state->resp_name, name, sizeof(state->resp_name) - 1);
-      state->resp_name[sizeof(state->resp_name) - 1] = '\0';
+      strncpy(ctx->resp_name, name, sizeof(ctx->resp_name));
     }
     if (value) {
-      strncpy(state->resp_value, value, sizeof(state->resp_value) - 1);
-      state->resp_value[sizeof(state->resp_value) - 1] = '\0';
-      state->resp_value_valid = true;
+      strncpy(ctx->resp_value, value, sizeof(ctx->resp_value));
     }
     if (type) {
-      strncpy(state->resp_type, type, sizeof(state->resp_type) - 1);
-      state->resp_type[sizeof(state->resp_type) - 1] = '\0';
+      strncpy(ctx->resp_type, type, sizeof(ctx->resp_type));
     }
   }
-
-  request_state_signal(state, &ctx->client_iface,
-                       SBP_MSG_SETTINGS_READ_BY_INDEX_REQ);
 }
 
-static void setting_read_by_index_done_callback(uint16_t sender_id, uint8_t len,
-                                                uint8_t *msg, void *context) {
+static void setting_read_by_index_done_callback(uint16_t sender_id,
+                                                uint8_t len,
+                                                uint8_t msg[],
+                                                void *context)
+{
   (void)sender_id;
   (void)len;
   (void)msg;
 
   settings_t *ctx = (settings_t *)context;
 
-  /* Traverse the pending requests */
-  request_state_t *state = ctx->req_list;
-  while (state != NULL) {
-    state->read_by_idx_done = true;
-    request_state_signal(state, &ctx->client_iface,
-                         SBP_MSG_SETTINGS_READ_BY_INDEX_REQ);
-    state = state->next;
+  ctx->resp_section[0] = '\0';
+  ctx->resp_name[0] = '\0';
+  ctx->resp_value[0] = '\0';
+  ctx->resp_type[0] = '\0';
+  ctx->read_by_idx_done = true;
+
+  int ret = request_state_signal(&ctx->request_state,
+                                 &ctx->client_iface,
+                                 SBP_MSG_SETTINGS_READ_BY_INDEX_REQ);
+
+  if (ret != 0) {
+    log_warn("Signaling request state failed with code: %d", ret);
   }
 }
 
-static sbp_msg_callback_t setting_sbp_cb_get(uint16_t msg_id) {
+static sbp_msg_callback_t setting_sbp_cb_get(uint16_t msg_id)
+{
   switch (msg_id) {
-    case SBP_MSG_SETTINGS_REGISTER_RESP:
-      return setting_register_resp_callback;
+  case SBP_MSG_SETTINGS_REGISTER_RESP: return setting_register_resp_callback;
 
-    case SBP_MSG_SETTINGS_WRITE:
-      return setting_write_callback;
+  case SBP_MSG_SETTINGS_WRITE: return setting_write_callback;
 
-    case SBP_MSG_SETTINGS_WRITE_RESP:
-      return setting_write_resp_callback;
+  case SBP_MSG_SETTINGS_WRITE_RESP: return setting_write_resp_callback;
 
-    case SBP_MSG_SETTINGS_READ_RESP:
-      return setting_read_resp_callback;
+  case SBP_MSG_SETTINGS_READ_RESP: return setting_read_resp_callback;
 
-    case SBP_MSG_SETTINGS_READ_BY_INDEX_RESP:
-      return setting_read_by_index_resp_callback;
+  case SBP_MSG_SETTINGS_READ_BY_INDEX_RESP: return setting_read_by_index_resp_callback;
 
-    case SBP_MSG_SETTINGS_READ_BY_INDEX_DONE:
-      return setting_read_by_index_done_callback;
+  case SBP_MSG_SETTINGS_READ_BY_INDEX_DONE: return setting_read_by_index_done_callback;
 
-    default:
-      assert(!"callback not found");
+  default: assert(!"callback not found");
   }
 
   /* To make cythonizer happy.. */
   return NULL;
 }
 
-int setting_sbp_cb_register(settings_t *ctx, uint16_t msg_id) {
-  LIBSETTINGS_LOCK(ctx);
+int setting_sbp_cb_register(settings_t *ctx, uint16_t msg_id)
+{
   setting_sbp_cb_t *sbp_cb_list = ctx->sbp_cb_list;
   setting_sbp_cb_t *last = NULL;
 
   /* Traverse to list end */
   while (sbp_cb_list != NULL) {
     if (sbp_cb_list->msg_id == msg_id) {
       /* Already registered */
-      LIBSETTINGS_UNLOCK(ctx);
       return 1;
     }
     last = sbp_cb_list;
     sbp_cb_list = sbp_cb_list->next;
   }
 
   setting_sbp_cb_t *sbp_cb = malloc(sizeof(*sbp_cb));
   if (sbp_cb == NULL) {
-    LIBSETTINGS_UNLOCK(ctx);
     return -1;
   }
 
   *sbp_cb = (setting_sbp_cb_t){.msg_id = msg_id,
                                .cb = setting_sbp_cb_get(msg_id),
                                .cb_node = NULL,
                                .next = NULL};
 
-  int res = ctx->client_iface.register_cb(ctx->client_iface.ctx, sbp_cb->msg_id,
-                                          sbp_cb->cb, ctx, &sbp_cb->cb_node);
+  int res = ctx->client_iface.register_cb(ctx->client_iface.ctx,
+                                          sbp_cb->msg_id,
+                                          sbp_cb->cb,
+                                          ctx,
+                                          &sbp_cb->cb_node);
 
   if (res != 0) {
     log_error("error registering callback for msg id %d", msg_id);
     free(sbp_cb);
-    LIBSETTINGS_UNLOCK(ctx);
     return -1;
   }
 
   if (last == NULL) {
     /* List was empty, set as list head */
     ctx->sbp_cb_list = sbp_cb;
   } else {
     last->next = sbp_cb;
   }
 
-  LIBSETTINGS_UNLOCK(ctx);
   return 0;
 }
 
-int setting_sbp_cb_unregister(settings_t *ctx, uint16_t msg_id) {
-  LIBSETTINGS_LOCK(ctx);
+int setting_sbp_cb_unregister(settings_t *ctx, uint16_t msg_id)
+{
   if (ctx->sbp_cb_list == NULL) {
     /* List is empty, nothing to unregister */
-    LIBSETTINGS_UNLOCK(ctx);
     return 1;
   }
 
   setting_sbp_cb_t *sbp_cb_list = ctx->sbp_cb_list;
 
   setting_sbp_cb_t *prev = NULL;
   while (sbp_cb_list != NULL) {
@@ -413,15 +388,14 @@
     }
     prev = sbp_cb_list;
     sbp_cb_list = sbp_cb_list->next;
   }
 
   if (sbp_cb_list == NULL) {
     /* Not registered */
-    LIBSETTINGS_UNLOCK(ctx);
     return 1;
   }
 
   setting_sbp_cb_t *sbp_cb = sbp_cb_list;
 
   /* Update list linking */
   if (prev == NULL) {
@@ -429,17 +403,15 @@
     ctx->sbp_cb_list = sbp_cb->next;
   } else {
     prev->next = sbp_cb->next;
   }
 
   int ret = 0;
 
-  if (ctx->client_iface.unregister_cb(ctx->client_iface.ctx,
-                                      &sbp_cb->cb_node) != 0) {
+  if (ctx->client_iface.unregister_cb(ctx->client_iface.ctx, &sbp_cb->cb_node) != 0) {
     log_error("error unregistering callback for msg id %d", msg_id);
     ret = -1;
   }
 
   free(sbp_cb);
-  LIBSETTINGS_UNLOCK(ctx);
   return ret;
 }
```

### Comparing `libsettings-0.1.14/src/setting_type.c` & `libsettings-0.1.9/src/setting_type.c`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,29 @@
  * WARRANTIES OF MERCHANTABILITY AND/OR FITNESS FOR A PARTICULAR PURPOSE.
  */
 
 #include <stdlib.h>
 
 #include <internal/setting_type.h>
 
-type_data_t *type_data_lookup(type_data_t *data_list, settings_type_t type) {
+type_data_t *type_data_lookup(type_data_t *data_list, settings_type_t type)
+{
   for (int i = 0; i < type && data_list != NULL; i++) {
     data_list = data_list->next;
   }
   return data_list;
 }
 
-int type_register(type_data_t **data_list, to_string_fn to_string,
-                  from_string_fn from_string, format_type_fn format_type,
-                  const void *priv, settings_type_t *type) {
+int type_register(type_data_t **data_list,
+                  to_string_fn to_string,
+                  from_string_fn from_string,
+                  format_type_fn format_type,
+                  const void *priv,
+                  settings_type_t *type)
+{
   type_data_t *type_data = (type_data_t *)malloc(sizeof(*type_data));
   if (type_data == NULL) {
     return -1;
   }
 
   *type_data = (type_data_t){.to_string = to_string,
                              .from_string = from_string,
@@ -43,15 +48,16 @@
   }
 
   *data_list = type_data;
   *type = next_type;
   return 0;
 }
 
-void type_data_free(type_data_t *data_list) {
+void type_data_free(type_data_t *data_list)
+{
   /* Free type data list elements */
   while (data_list != NULL) {
     type_data_t *t = data_list;
     data_list = data_list->next;
     free(t);
   }
 }
```

### Comparing `libsettings-0.1.14/src/setting_type_enum.c` & `libsettings-0.1.9/src/setting_type_enum.c`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 #include <inttypes.h>
 #include <stdio.h>
 #include <string.h>
 
 #include <internal/setting_type_enum.h>
 
-int enum_format_type(const void *priv, char *str, int slen) {
+int enum_format_type(const void *priv, char *str, int slen)
+{
   int n = 0;
   int l;
 
   /* Print "enum:" header */
   l = snprintf(&str[n], slen - n, LIBSETTINGS_ENUM_TAG);
   if (l < 0) {
     return l;
@@ -45,24 +46,25 @@
     str[n - 1] = '\0';
     n--;
   }
 
   return n;
 }
 
-int enum_to_string(const void *priv, char *str, int slen, const void *blob,
-                   int blen) {
+int enum_to_string(const void *priv, char *str, int slen, const void *blob, int blen)
+{
   (void)blen;
 
   const char *const *enum_names = priv;
   int index = *(uint8_t *)blob;
   return snprintf(str, slen, "%s", enum_names[index]);
 }
 
-bool enum_from_string(const void *priv, void *blob, int blen, const char *str) {
+bool enum_from_string(const void *priv, void *blob, int blen, const char *str)
+{
   (void)blen;
 
   const char *const *enum_names = priv;
   int i;
 
   for (i = 0; enum_names[i] && (strcmp(str, enum_names[i]) != 0); i++) {
     ;
```

### Comparing `libsettings-0.1.14/src/setting_type_int.c` & `libsettings-0.1.9/src/setting_type_int.c`

 * *Files 12% similar despite different names*

```diff
@@ -11,47 +11,42 @@
  */
 
 #include <inttypes.h>
 #include <stdio.h>
 
 #include <internal/setting_type_int.h>
 
-int int_to_string(const void *priv, char *str, int slen, const void *blob,
-                  int blen) {
+int int_to_string(const void *priv, char *str, int slen, const void *blob, int blen)
+{
   (void)priv;
 
   switch (blen) {
-    case 1: {
-      int16_t tmp = *(int8_t *)blob;
-      /* mingw's crappy snprintf doesn't understand %hhd */
-      return snprintf(str, slen, "%hd", tmp);
-    }
-    case 2:
-      return snprintf(str, slen, "%hd", *(int16_t *)blob);
-    case 4:
-      return snprintf(str, slen, "%" PRId32, *(int32_t *)blob);
-    default:
-      return -1;
+  case 1: {
+    int16_t tmp = *(int8_t *)blob;
+    /* mingw's crappy snprintf doesn't understand %hhd */
+    return snprintf(str, slen, "%hd", tmp);
+  }
+  case 2: return snprintf(str, slen, "%hd", *(int16_t *)blob);
+  case 4: return snprintf(str, slen, "%" PRId32, *(int32_t *)blob);
+  default: return -1;
   }
 }
 
-bool int_from_string(const void *priv, void *blob, int blen, const char *str) {
+bool int_from_string(const void *priv, void *blob, int blen, const char *str)
+{
   (void)priv;
 
   switch (blen) {
-    case 1: {
-      int16_t tmp;
-      /* Newlib's crappy sscanf doesn't understand %hhd */
-      if (sscanf(str, "%hd", &tmp) == 1) {
-        *(int8_t *)blob = tmp;
-        return true;
-      }
-      return false;
+  case 1: {
+    int16_t tmp;
+    /* Newlib's crappy sscanf doesn't understand %hhd */
+    if (sscanf(str, "%hd", &tmp) == 1) {
+      *(int8_t *)blob = tmp;
+      return true;
     }
-    case 2:
-      return sscanf(str, "%hd", (int16_t *)blob) == 1;
-    case 4:
-      return sscanf(str, "%" PRId32, (int32_t *)blob) == 1;
-    default:
-      return false;
+    return false;
+  }
+  case 2: return sscanf(str, "%hd", (int16_t *)blob) == 1;
+  case 4: return sscanf(str, "%" PRId32, (int32_t *)blob) == 1;
+  default: return false;
   }
 }
```

### Comparing `libsettings-0.1.14/src/setting_type_str.c` & `libsettings-0.1.9/src/setting_type_str.c`

 * *Files 14% similar despite different names*

```diff
@@ -11,23 +11,24 @@
  */
 
 #include <inttypes.h>
 #include <stdio.h>
 
 #include <internal/setting_type_str.h>
 
-int str_to_string(const void *priv, char *str, int slen, const void *blob,
-                  int blen) {
+int str_to_string(const void *priv, char *str, int slen, const void *blob, int blen)
+{
   (void)priv;
   (void)blen;
 
   return snprintf(str, slen, "%s", (char *)blob);
 }
 
-bool str_from_string(const void *priv, void *blob, int blen, const char *str) {
+bool str_from_string(const void *priv, void *blob, int blen, const char *str)
+{
   (void)priv;
 
   int l = snprintf(blob, blen, "%s", str);
   if ((l < 0) || (l >= blen)) {
     return false;
   }
```

### Comparing `libsettings-0.1.14/src/settings.c` & `libsettings-0.1.9/src/settings.c`

 * *Files 11% similar despite different names*

```diff
@@ -89,254 +89,225 @@
 #include <internal/setting_sbp_cb.h>
 #include <internal/setting_type.h>
 #include <internal/setting_type_enum.h>
 #include <internal/setting_type_float.h>
 #include <internal/setting_type_int.h>
 #include <internal/setting_type_str.h>
 
-/* This is GCC specific so void for others */
-#ifndef __GNUC__
-#define __attribute__(x)
-#endif
-
 #define REGISTER_TIMEOUT_MS 500
 #define REGISTER_TRIES 5
 
 #define WATCH_INIT_TIMEOUT_MS 500
 #define WATCH_INIT_TRIES 5
 
 static const char *const bool_enum_names[] = {"False", "True", NULL};
 
-static settings_log_preformatted_t client_log_preformatted = NULL;
+static settings_log_t client_log = NULL;
 
 /* Workaround for Cython not properly supporting variadic arguments */
-__attribute__((format(printf, 2, 3))) static void log_preformat(int level,
-                                                                const char *fmt,
-                                                                ...) {
+__attribute__((format(printf, 2, 3))) static void log_preformat(int level, const char *fmt, ...)
+{
   char buffer[SETTINGS_BUFLEN];
   va_list args;
   va_start(args, fmt);
-  int ret = vsnprintf(buffer, sizeof(buffer), fmt, args); /* NOLINT */
+  int ret = vsnprintf(buffer, sizeof(buffer), fmt, args);
   va_end(args);
 
   if (ret < 0) {
-    client_log_preformatted(LOG_ERROR, "log_preformat encoding error");
+    client_log(LOG_ERROR, "log_preformat encoding error");
     return;
-  } else if ((size_t)ret >= sizeof(buffer))
-
-  {
-    client_log_preformatted(LOG_WARN, "log_preformat too long message");
+  } else if ((size_t)ret >= sizeof(buffer)) {
+    client_log(LOG_WARN, "log_preformat too long message");
   }
 
-  client_log_preformatted(level, buffer);
+  client_log(level, buffer);
 }
 
-static int send_single_thd(settings_t *ctx, uint16_t message_type,
-                           char *message, uint8_t message_length,
-                           uint32_t timeout_ms, uint8_t retries,
-                           uint16_t sender_id, request_state_t *req_state) {
+/**
+ * @brief setting_perform_request_reply_from
+ * Performs a synchronous req/reply transation for the provided
+ * message using the compare structure to match the header in callbacks.
+ * Uses an explicit sender_id to allow for settings interactions with manager.
+ * @param ctx: settings context
+ * @param message_type: sbp message to use when sending the message
+ * @param message: sbp message payload
+ * @param message_length: length of payload
+ * @param header_length: length of the substring to match during compare
+ * @param timeout_ms: timeout between retries
+ * @param retries: number of times to retry the transaction
+ * @param sender_id: sender_id to use for outgoing message
+ * @return zero on success, -1 the transaction failed to complete
+ */
+static int setting_perform_request_reply_from(settings_t *ctx,
+                                              uint16_t message_type,
+                                              char *message,
+                                              uint8_t message_length,
+                                              uint8_t header_length,
+                                              uint32_t timeout_ms,
+                                              uint8_t retries,
+                                              uint16_t sender_id)
+{
+  request_state_init(&ctx->request_state, message_type, message, header_length);
+
   uint8_t tries = 0;
   bool success = false;
 
   /* Prime semaphores etc if applicable */
   if (ctx->client_iface.wait_init) {
     ctx->client_iface.wait_init(ctx->client_iface.ctx);
   }
 
   do {
-    ctx->client_iface.send_from(ctx->client_iface.ctx, message_type,
-                                message_length, (uint8_t *)message, sender_id);
-
-    if (0 == ctx->client_iface.wait(ctx->client_iface.ctx, timeout_ms)) {
-      success = request_state_match(req_state);
+    ctx->client_iface.send_from(ctx->client_iface.ctx,
+                                message_type,
+                                message_length,
+                                (uint8_t *)message,
+                                sender_id);
+
+    if (ctx->client_iface.wait(ctx->client_iface.ctx, timeout_ms)) {
+      size_t len1 = strlen(message) + 1;
+      log_warn("Waiting reply for msg id %d with %s.%s timed out",
+               message_type,
+               message,
+               message + len1);
+    } else {
+      success = request_state_match(&ctx->request_state);
     }
+
   } while (!success && (++tries < retries));
 
   /* Defuse semaphores etc if applicable */
   if (ctx->client_iface.wait_deinit) {
     ctx->client_iface.wait_deinit(ctx->client_iface.ctx);
   }
 
-  return success ? 0 : -1;
-}
-
-static int send_multi_thd(settings_t *ctx, void *event, uint16_t message_type,
-                          char *message, uint8_t message_length,
-                          uint32_t timeout_ms, uint8_t retries,
-                          uint16_t sender_id, request_state_t *req_state) {
-  assert(event);
-  assert(ctx->client_iface.wait_thd);
-
-  uint8_t tries = 0;
-  bool success = false;
-
-  do {
-    ctx->client_iface.send_from(ctx->client_iface.ctx, message_type,
-                                message_length, (uint8_t *)message, sender_id);
-    if (0 == ctx->client_iface.wait_thd(event, timeout_ms)) {
-      success = request_state_match(req_state);
-    }
-  } while (!success && (++tries < retries));
-
-  return success ? 0 : -1;
-}
+  request_state_deinit(&ctx->request_state);
 
-/**
- * @brief setting_perform_request_reply_from
- * Performs a synchronous req/reply transation for the provided
- * message using the compare structure to match the header in callbacks.
- * Uses an explicit sender_id to allow for settings interactions with manager.
- * @param ctx: settings context
- * @param event: event object in case of multithreading
- * @param message_type: sbp message to use when sending the message
- * @param message: sbp message payload
- * @param message_length: length of payload
- * @param header_length: length of the substring to match during compare
- * @param timeout_ms: timeout between retries
- * @param retries: number of times to retry the transaction
- * @param sender_id: sender_id to use for outgoing message
- * @return zero on success, -1 the transaction failed to complete
- */
-static int setting_perform_request_reply_from(
-    settings_t *ctx, void *event, uint16_t message_type, char *message,
-    uint8_t message_length, uint8_t header_length, uint32_t timeout_ms,
-    uint8_t retries, uint16_t sender_id, request_state_t *req_state) {
-  request_state_t local_req_state;
-  if (NULL == req_state) {
-    req_state = &local_req_state;
-  }
-
-  request_state_init(req_state, event, message_type, message, header_length);
-  request_state_append(ctx, req_state);
-
-  int res = 0;
-
-  if (event) {
-    res = send_multi_thd(ctx, event, message_type, message, message_length,
-                         timeout_ms, retries, sender_id, req_state);
-  } else {
-    res = send_single_thd(ctx, message_type, message, message_length,
-                          timeout_ms, retries, sender_id, req_state);
+  if (!success) {
+    log_warn("setting req/reply failed after %d retries (msg id: %d)", tries, message_type);
+    return -1;
   }
 
-  request_state_remove(ctx, req_state);
-
-  return res;
+  return 0;
 }
 
 /**
  * @brief setting_perform_request_reply - same as above but with implicit
  * sender_id
  * @param ctx: settings context
- * @param event: event object in case of multithreading
  * @param message_type: sbp message to use when sending the message
  * @param message: sbp message payload
  * @param message_length: length of payload
  * @param header_length: length of the substring to match during compare
  * @param timeout_ms: timeout between retries
  * @param retries: number of times to retry the transaction
  * @return zero on success, -1 the transaction failed to complete
  */
-static int setting_perform_request_reply(settings_t *ctx, void *event,
-                                         uint16_t message_type, char *message,
+static int setting_perform_request_reply(settings_t *ctx,
+                                         uint16_t message_type,
+                                         char *message,
                                          uint8_t message_length,
                                          uint8_t header_length,
-                                         uint16_t timeout_ms, uint8_t retries,
-                                         request_state_t *req_state) {
-  return setting_perform_request_reply_from(
-      ctx, event, message_type, message, message_length, header_length,
-      timeout_ms, retries, ctx->sender_id, req_state);
+                                         uint16_t timeout_ms,
+                                         uint8_t retries)
+{
+  return setting_perform_request_reply_from(ctx,
+                                            message_type,
+                                            message,
+                                            message_length,
+                                            header_length,
+                                            timeout_ms,
+                                            retries,
+                                            ctx->sender_id);
 }
 
 /**
  * @brief setting_register - perform SBP_MSG_SETTINGS_REGISTER req/reply
  * @param ctx: settings context
  * @param setting_data: setting to register with settings daemon
  * @return zero on success, -1 the transaction failed to complete
  */
-static int setting_register(settings_t *ctx, setting_data_t *setting_data) {
+static int setting_register(settings_t *ctx, setting_data_t *setting_data)
+{
   char msg[SETTINGS_BUFLEN] = {0};
   uint8_t msg_header_len;
 
-  int msg_len = setting_data_format(setting_data, true, msg, sizeof(msg),
-                                    &msg_header_len);
+  int msg_len = setting_data_format(setting_data, true, msg, sizeof(msg), &msg_header_len);
 
   if (msg_len < 0) {
     log_error("setting register message format failed");
     return -1;
   }
 
-  return setting_perform_request_reply(
-      ctx, NULL, SBP_MSG_SETTINGS_REGISTER, msg, msg_len, msg_header_len,
-      REGISTER_TIMEOUT_MS, REGISTER_TRIES, NULL);
+  return setting_perform_request_reply(ctx,
+                                       SBP_MSG_SETTINGS_REGISTER,
+                                       msg,
+                                       msg_len,
+                                       msg_header_len,
+                                       REGISTER_TIMEOUT_MS,
+                                       REGISTER_TRIES);
 }
 
 /**
  * @brief setting_read_watched_value - perform SBP_MSG_SETTINGS_READ_REQ
  * req/reply
  * @param ctx: setting context
  * @param setting_data: setting to read from settings daemon
- *
- * @retval  0 success
- * @retval -1 transaction failed to complete
- * @retval  1 setting is not yet registered
+ * @return zero on success, -1 the transaction failed to complete
  */
-static int setting_read_watched_value(settings_t *ctx,
-                                      setting_data_t *setting_data) {
+static int setting_read_watched_value(settings_t *ctx, setting_data_t *setting_data)
+{
   int result = 0;
   /* Build message */
   char msg[SETTINGS_BUFLEN] = {0};
   uint8_t msg_len = 0;
   int l;
 
   if (!setting_data->watchonly) {
     log_error("cannot update non-watchonly setting manually");
     return -1;
   }
 
-  l = settings_format(setting_data->section, setting_data->name, NULL, NULL,
-                      msg, sizeof(msg));
+  l = settings_format(setting_data->section, setting_data->name, NULL, NULL, msg, sizeof(msg));
   if (l < 0) {
     log_error("error building settings read req message");
     return -1;
   }
   msg_len += l;
 
   if (setting_sbp_cb_register(ctx, SBP_MSG_SETTINGS_READ_RESP) < 0) {
     log_error("error registering settings read resp callback");
     return -1;
   }
 
-  request_state_t req_state;
-  result = setting_perform_request_reply_from(
-      ctx, NULL, SBP_MSG_SETTINGS_READ_REQ, msg, msg_len, msg_len,
-      WATCH_INIT_TIMEOUT_MS, WATCH_INIT_TRIES, SBP_SENDER_ID, &req_state);
+  result = setting_perform_request_reply_from(ctx,
+                                              SBP_MSG_SETTINGS_READ_REQ,
+                                              msg,
+                                              msg_len,
+                                              msg_len,
+                                              WATCH_INIT_TIMEOUT_MS,
+                                              WATCH_INIT_TRIES,
+                                              SBP_SENDER_ID);
 
   setting_sbp_cb_unregister(ctx, SBP_MSG_SETTINGS_READ_RESP);
-
-  if (0 == result) {
-    if (!req_state.resp_value_valid) {
-      /* Valid response was received but didn't contain value data, indicating
-       * that setting is not yet registered */
-      return 1;
-    }
-    setting_data_update_value(setting_data, req_state.resp_value);
-  }
-
   return result;
 }
 
-int settings_register_enum(settings_t *ctx, const char *const enum_names[],
-                           settings_type_t *type) {
+int settings_register_enum(settings_t *ctx, const char *const enum_names[], settings_type_t *type)
+{
   assert(ctx != NULL);
   assert(enum_names != NULL);
   assert(type != NULL);
 
-  return type_register(&ctx->type_data_list, enum_to_string, enum_from_string,
-                       enum_format_type, enum_names, type);
+  return type_register(&ctx->type_data_list,
+                       enum_to_string,
+                       enum_from_string,
+                       enum_format_type,
+                       enum_names,
+                       type);
 }
 
 /**
  * @brief settings_add_setting - internal subroutine for handling new settings
  * This method forwards all parameters to the setting factory to create a new
  * settings but also performs the addition of the setting to the settings
  * context internal list and performs either registration of the setting (if
@@ -349,47 +320,59 @@
  * @param type: type identifier
  * @param notify: optional notification callback
  * @param notify_context: optional data reference to pass during notification
  * @param readonly: set to true to disable value updates
  * @param watchonly: set to true to indicate a non-owned setting watch
  * @return zero on success, -1 if the addition of the setting has failed
  */
-static int settings_add_setting(settings_t *ctx, const char *section,
-                                const char *name, void *var, size_t var_len,
-                                settings_type_t type, settings_notify_fn notify,
-                                void *notify_context, bool readonly,
-                                bool watchonly) {
+static int settings_add_setting(settings_t *ctx,
+                                const char *section,
+                                const char *name,
+                                void *var,
+                                size_t var_len,
+                                settings_type_t type,
+                                settings_notify_fn notify,
+                                void *notify_context,
+                                bool readonly,
+                                bool watchonly)
+{
   assert(ctx != NULL);
   assert(section != NULL);
   assert(name != NULL);
   assert(var != NULL);
 
   if (setting_data_lookup(ctx->setting_data_list, section, name) != NULL) {
     log_error("setting add failed - duplicate setting");
     return -1;
   }
 
-  setting_data_t *setting_data =
-      setting_data_create(ctx->type_data_list, section, name, var, var_len,
-                          type, notify, notify_context, readonly, watchonly);
+  setting_data_t *setting_data = setting_data_create(ctx->type_data_list,
+                                                     section,
+                                                     name,
+                                                     var,
+                                                     var_len,
+                                                     type,
+                                                     notify,
+                                                     notify_context,
+                                                     readonly,
+                                                     watchonly);
   if (setting_data == NULL) {
     log_error("error creating setting data");
     return -1;
   }
 
   /* Add to list */
   setting_data_append(&ctx->setting_data_list, setting_data);
 
   if (watchonly) {
     if (setting_sbp_cb_register(ctx, SBP_MSG_SETTINGS_WRITE_RESP) < 0) {
       log_error("error registering settings write resp callback");
     }
-    if (setting_read_watched_value(ctx, setting_data) < 0) {
-      log_warn("Unable to read watched setting to initial value (%s.%s)",
-               section, name);
+    if (setting_read_watched_value(ctx, setting_data) != 0) {
+      log_warn("Unable to read watched setting to initial value (%s.%s)", section, name);
     }
   } else {
     if (setting_sbp_cb_register(ctx, SBP_MSG_SETTINGS_REGISTER_RESP) < 0) {
       log_error("error registering settings register resp callback");
     }
     if (setting_sbp_cb_register(ctx, SBP_MSG_SETTINGS_WRITE) < 0) {
       log_error("error registering settings write callback");
@@ -399,106 +382,169 @@
       setting_data_remove(&ctx->setting_data_list, &setting_data);
       return -1;
     }
   }
   return 0;
 }
 
-int settings_register_setting(settings_t *ctx, const char *section,
-                              const char *name, void *var, size_t var_len,
-                              settings_type_t type, settings_notify_fn notify,
-                              void *notify_context) {
-  return settings_add_setting(ctx, section, name, var, var_len, type, notify,
-                              notify_context, false, false);
-}
-
-int settings_register_readonly(settings_t *ctx, const char *section,
-                               const char *name, const void *var,
-                               size_t var_len, settings_type_t type) {
-  return settings_add_setting(ctx, section, name, (void *)var, var_len, type,
-                              NULL, NULL, true, false);
-}
-
-int settings_register_watch(settings_t *ctx, const char *section,
-                            const char *name, void *var, size_t var_len,
-                            settings_type_t type, settings_notify_fn notify,
-                            void *notify_context) {
-  return settings_add_setting(ctx, section, name, var, var_len, type, notify,
-                              notify_context, false, true);
-}
-
-settings_write_res_t settings_write(settings_t *ctx, void *event,
-                                    const char *section, const char *name,
-                                    const void *value, size_t value_len,
-                                    settings_type_t type) {
+int settings_register_setting(settings_t *ctx,
+                              const char *section,
+                              const char *name,
+                              void *var,
+                              size_t var_len,
+                              settings_type_t type,
+                              settings_notify_fn notify,
+                              void *notify_context)
+{
+  return settings_add_setting(ctx,
+                              section,
+                              name,
+                              var,
+                              var_len,
+                              type,
+                              notify,
+                              notify_context,
+                              false,
+                              false);
+}
+
+int settings_register_readonly(settings_t *ctx,
+                               const char *section,
+                               const char *name,
+                               const void *var,
+                               size_t var_len,
+                               settings_type_t type)
+{
+  return settings_add_setting(ctx,
+                              section,
+                              name,
+                              (void *)var,
+                              var_len,
+                              type,
+                              NULL,
+                              NULL,
+                              true,
+                              false);
+}
+
+int settings_register_watch(settings_t *ctx,
+                            const char *section,
+                            const char *name,
+                            void *var,
+                            size_t var_len,
+                            settings_type_t type,
+                            settings_notify_fn notify,
+                            void *notify_context)
+{
+  return settings_add_setting(ctx,
+                              section,
+                              name,
+                              var,
+                              var_len,
+                              type,
+                              notify,
+                              notify_context,
+                              false,
+                              true);
+}
+
+settings_write_res_t settings_write(settings_t *ctx,
+                                    const char *section,
+                                    const char *name,
+                                    const void *value,
+                                    size_t value_len,
+                                    settings_type_t type)
+{
   char msg[SETTINGS_BUFLEN] = {0};
   uint8_t msg_header_len;
 
   if (setting_sbp_cb_register(ctx, SBP_MSG_SETTINGS_WRITE_RESP) < 0) {
     log_error("error registering settings write response callback");
     return -1;
   }
 
-  setting_data_t *setting_data =
-      setting_data_create(ctx->type_data_list, section, name, (void *)value,
-                          value_len, type, NULL, NULL, false, false);
+  setting_data_t *setting_data = setting_data_create(ctx->type_data_list,
+                                                     section,
+                                                     name,
+                                                     (void *)value,
+                                                     value_len,
+                                                     type,
+                                                     NULL,
+                                                     NULL,
+                                                     false,
+                                                     false);
   if (setting_data == NULL) {
     log_error("settings write error while creating setting data");
     return -1;
   }
 
-  int msg_len = setting_data_format(setting_data, false, msg, sizeof(msg),
-                                    &msg_header_len);
+  int msg_len = setting_data_format(setting_data, false, msg, sizeof(msg), &msg_header_len);
 
   if (msg_len < 0) {
     log_error("setting write error format failed");
     setting_data_destroy(setting_data);
     return -1;
   }
 
-  request_state_t req_state;
-  setting_perform_request_reply_from(
-      ctx, event, SBP_MSG_SETTINGS_WRITE, msg, msg_len, msg_header_len,
-      REGISTER_TIMEOUT_MS, REGISTER_TRIES, SBP_SENDER_ID, &req_state);
+  /* This will be updated in the settings_write_resp_callback */
+  ctx->status = SETTINGS_WR_TIMEOUT;
 
-  setting_data_destroy(setting_data);
-
-  return req_state.status;
-}
-
-settings_write_res_t settings_write_int(settings_t *ctx, void *event,
-                                        const char *section, const char *name,
-                                        int value) {
-  return settings_write(ctx, event, section, name, &value, sizeof(value),
-                        SETTINGS_TYPE_INT);
-}
+  setting_perform_request_reply_from(ctx,
+                                     SBP_MSG_SETTINGS_WRITE,
+                                     msg,
+                                     msg_len,
+                                     msg_header_len,
+                                     REGISTER_TIMEOUT_MS,
+                                     REGISTER_TRIES,
+                                     SBP_SENDER_ID);
 
-settings_write_res_t settings_write_float(settings_t *ctx, void *event,
-                                          const char *section, const char *name,
-                                          float value) {
-  return settings_write(ctx, event, section, name, &value, sizeof(value),
-                        SETTINGS_TYPE_FLOAT);
-}
-
-settings_write_res_t settings_write_str(settings_t *ctx, void *event,
-                                        const char *section, const char *name,
-                                        const char *str) {
-  return settings_write(ctx, event, section, name, str, strlen(str),
-                        SETTINGS_TYPE_STRING);
-}
+  setting_data_destroy(setting_data);
 
-settings_write_res_t settings_write_bool(settings_t *ctx, void *event,
-                                         const char *section, const char *name,
-                                         bool value) {
-  return settings_write(ctx, event, section, name, &value, sizeof(value),
-                        SETTINGS_TYPE_BOOL);
+  return ctx->status;
 }
 
-int settings_read(settings_t *ctx, const char *section, const char *name,
-                  void *value, size_t value_len, settings_type_t type) {
+settings_write_res_t settings_write_int(settings_t *ctx,
+                                        const char *section,
+                                        const char *name,
+                                        int value)
+{
+  return settings_write(ctx, section, name, &value, sizeof(value), SETTINGS_TYPE_INT);
+}
+
+settings_write_res_t settings_write_float(settings_t *ctx,
+                                          const char *section,
+                                          const char *name,
+                                          float value)
+{
+  return settings_write(ctx, section, name, &value, sizeof(value), SETTINGS_TYPE_FLOAT);
+}
+
+settings_write_res_t settings_write_str(settings_t *ctx,
+                                        const char *section,
+                                        const char *name,
+                                        const char *str)
+{
+  return settings_write(ctx, section, name, str, strlen(str), SETTINGS_TYPE_STRING);
+}
+
+settings_write_res_t settings_write_bool(settings_t *ctx,
+                                         const char *section,
+                                         const char *name,
+                                         bool value)
+{
+  return settings_write(ctx, section, name, &value, sizeof(value), SETTINGS_TYPE_BOOL);
+}
+
+int settings_read(settings_t *ctx,
+                  const char *section,
+                  const char *name,
+                  void *value,
+                  size_t value_len,
+                  settings_type_t type)
+{
   assert(ctx);
   assert(section);
   assert(name);
   assert(value);
   assert(value_len);
 
   /* Build message */
@@ -511,31 +557,40 @@
   }
 
   if (setting_sbp_cb_register(ctx, SBP_MSG_SETTINGS_READ_RESP) < 0) {
     log_error("error registering settings read resp callback");
     return -1;
   }
 
-  request_state_t req_state;
-  int res = setting_perform_request_reply_from(
-      ctx, NULL, SBP_MSG_SETTINGS_READ_REQ, msg, msg_len, msg_len,
-      WATCH_INIT_TIMEOUT_MS, WATCH_INIT_TRIES, SBP_SENDER_ID, &req_state);
+  ctx->resp_section[0] = '\0';
+  ctx->resp_name[0] = '\0';
+  ctx->resp_value[0] = '\0';
+  ctx->resp_type[0] = '\0';
+
+  int res = setting_perform_request_reply_from(ctx,
+                                               SBP_MSG_SETTINGS_READ_REQ,
+                                               msg,
+                                               msg_len,
+                                               msg_len,
+                                               WATCH_INIT_TIMEOUT_MS,
+                                               WATCH_INIT_TRIES,
+                                               SBP_SENDER_ID);
 
   setting_sbp_cb_unregister(ctx, SBP_MSG_SETTINGS_READ_RESP);
 
   if (res != 0) {
     return res;
   }
 
   settings_type_t parsed_type = SETTINGS_TYPE_STRING;
 
-  if (strlen(req_state.resp_type) != 0) {
+  if (strlen(ctx->resp_type) != 0) {
     const char *cmp = "enum:";
-    if (strncmp(req_state.resp_type, cmp, strlen(cmp)) != 0) {
-      parsed_type = strtol(req_state.resp_type, NULL, 10);
+    if (strncmp(ctx->resp_type, cmp, strlen(cmp)) != 0) {
+      parsed_type = strtol(ctx->resp_type, NULL, 10);
     }
   } else {
     parsed_type = type;
   }
 
   if (type != parsed_type) {
     log_error("setting types don't match");
@@ -545,102 +600,128 @@
   const type_data_t *td = type_data_lookup(ctx->type_data_list, parsed_type);
 
   if (td == NULL) {
     log_error("unknown setting type");
     return -1;
   }
 
-  if (!td->from_string(td->priv, value, value_len, req_state.resp_value)) {
+  if (!td->from_string(td->priv, value, value_len, ctx->resp_value)) {
     log_error("value parsing failed");
     return -1;
   }
 
   return 0;
 }
 
-int settings_read_int(settings_t *ctx, const char *section, const char *name,
-                      int *value) {
-  return settings_read(ctx, section, name, value, sizeof(int),
-                       SETTINGS_TYPE_INT);
-}
-
-int settings_read_float(settings_t *ctx, const char *section, const char *name,
-                        float *value) {
-  return settings_read(ctx, section, name, value, sizeof(float),
-                       SETTINGS_TYPE_FLOAT);
-}
-
-int settings_read_str(settings_t *ctx, const char *section, const char *name,
-                      char *str, size_t str_len) {
+int settings_read_int(settings_t *ctx, const char *section, const char *name, int *value)
+{
+  return settings_read(ctx, section, name, value, sizeof(int), SETTINGS_TYPE_INT);
+}
+
+int settings_read_float(settings_t *ctx, const char *section, const char *name, float *value)
+{
+  return settings_read(ctx, section, name, value, sizeof(float), SETTINGS_TYPE_FLOAT);
+}
+
+int settings_read_str(settings_t *ctx,
+                      const char *section,
+                      const char *name,
+                      char *str,
+                      size_t str_len)
+{
   return settings_read(ctx, section, name, str, str_len, SETTINGS_TYPE_STRING);
 }
 
-int settings_read_bool(settings_t *ctx, const char *section, const char *name,
-                       bool *value) {
-  return settings_read(ctx, section, name, value, sizeof(bool),
-                       SETTINGS_TYPE_BOOL);
-}
-
-int settings_read_by_idx(settings_t *ctx, void *event, uint16_t idx,
-                         char *section, size_t section_len, char *name,
-                         size_t name_len, char *value, size_t value_len,
-                         char *type, size_t type_len) {
+int settings_read_bool(settings_t *ctx, const char *section, const char *name, bool *value)
+{
+  return settings_read(ctx, section, name, value, sizeof(bool), SETTINGS_TYPE_BOOL);
+}
+
+int settings_read_by_idx(settings_t *ctx,
+                         uint16_t idx,
+                         char *section,
+                         size_t section_len,
+                         char *name,
+                         size_t name_len,
+                         char *value,
+                         size_t value_len,
+                         char *type,
+                         size_t type_len)
+{
   assert(section_len > 0);
   assert(name_len > 0);
   assert(value_len > 0);
   assert(type_len > 0);
 
   int res = -1;
 
   if (setting_sbp_cb_register(ctx, SBP_MSG_SETTINGS_READ_BY_INDEX_RESP) < 0) {
     log_error("error registering settings read by idx resp callback");
-    return res;
+    goto read_by_idx_cleanup;
   }
 
   if (setting_sbp_cb_register(ctx, SBP_MSG_SETTINGS_READ_BY_INDEX_DONE) < 0) {
-    setting_sbp_cb_unregister(ctx, SBP_MSG_SETTINGS_READ_BY_INDEX_RESP);
     log_error("error registering settings read by idx done callback");
-    return res;
+    goto read_by_idx_cleanup;
   }
 
-  request_state_t req_state;
-  res = setting_perform_request_reply_from(
-      ctx, event, SBP_MSG_SETTINGS_READ_BY_INDEX_REQ, (char *)&idx,
-      sizeof(uint16_t), sizeof(uint16_t), WATCH_INIT_TIMEOUT_MS,
-      WATCH_INIT_TRIES, SBP_SENDER_ID, &req_state);
+  ctx->resp_section[0] = '\0';
+  ctx->resp_name[0] = '\0';
+  ctx->resp_value[0] = '\0';
+  ctx->resp_type[0] = '\0';
+  ctx->read_by_idx_done = false;
+
+  res = setting_perform_request_reply_from(ctx,
+                                           SBP_MSG_SETTINGS_READ_BY_INDEX_REQ,
+                                           (char *)&idx,
+                                           sizeof(uint16_t),
+                                           sizeof(uint16_t),
+                                           WATCH_INIT_TIMEOUT_MS,
+                                           WATCH_INIT_TRIES,
+                                           SBP_SENDER_ID);
+
+  if (res != 0) {
+    log_error("read by idx request failed");
+    goto read_by_idx_cleanup;
+  }
+
+  strncpy(section, ctx->resp_section, section_len);
+  strncpy(name, ctx->resp_name, name_len);
+  strncpy(value, ctx->resp_value, value_len);
+  strncpy(type, ctx->resp_type, type_len);
+
+read_by_idx_cleanup:
+  setting_sbp_cb_unregister(ctx, SBP_MSG_SETTINGS_READ_BY_INDEX_RESP);
+  setting_sbp_cb_unregister(ctx, SBP_MSG_SETTINGS_READ_BY_INDEX_DONE);
 
   /* Error */
-  if (res < 0) {
+  if (res != 0) {
     return res;
   }
 
   /* Last index was read */
-  if (req_state.read_by_idx_done) {
-    setting_sbp_cb_unregister(ctx, SBP_MSG_SETTINGS_READ_BY_INDEX_RESP);
-    setting_sbp_cb_unregister(ctx, SBP_MSG_SETTINGS_READ_BY_INDEX_DONE);
+  if (ctx->read_by_idx_done) {
     return 1;
   }
 
-  strncpy(section, req_state.resp_section, section_len);
-  strncpy(name, req_state.resp_name, name_len);
-  strncpy(value, req_state.resp_value, value_len);
-  strncpy(type, req_state.resp_type, type_len);
-
   /* No errors, next index to be read */
   return 0;
 }
 
-settings_t *settings_create(uint16_t sender_id, settings_api_t *client_iface) {
+settings_t *settings_create(uint16_t sender_id, settings_api_t *client_iface)
+{
   assert(client_iface != NULL);
 
-  if (client_iface->log_preformatted != NULL) {
-    client_log_preformatted = client_iface->log_preformatted;
-    logging_set_implementation(log_preformat, detailed_log_);
-  } else if (client_iface->log != NULL) {
-    logging_set_implementation(client_iface->log, detailed_log_);
+  if (client_iface->log != NULL) {
+    if (client_iface->log_preformat) {
+      client_log = client_iface->log;
+      logging_set_implementation(log_preformat, detailed_log_);
+    } else {
+      logging_set_implementation(client_iface->log, detailed_log_);
+    }
   }
 
   log_info("Building settings framework");
 
   settings_t *ctx = (settings_t *)malloc(sizeof(*ctx));
   if (ctx == NULL) {
     log_error("error allocating context");
@@ -651,56 +732,58 @@
 
   ctx->client_iface = *client_iface;
 
   ctx->type_data_list = NULL;
   ctx->setting_data_list = NULL;
   ctx->sbp_cb_list = NULL;
 
-  ctx->req_list = NULL;
+  ctx->request_state.pending = false;
 
   /* Register standard types */
   settings_type_t type;
 
-  int ret = type_register(&ctx->type_data_list, int_to_string, int_from_string,
-                          NULL, NULL, &type);
+  int ret = type_register(&ctx->type_data_list, int_to_string, int_from_string, NULL, NULL, &type);
   /* To make cythonizer happy.. */
   (void)ret;
 
   assert(ret == 0);
   assert(type == SETTINGS_TYPE_INT);
 
-  ret = type_register(&ctx->type_data_list, float_to_string, float_from_string,
-                      NULL, NULL, &type);
+  ret = type_register(&ctx->type_data_list, float_to_string, float_from_string, NULL, NULL, &type);
   assert(ret == 0);
   assert(type == SETTINGS_TYPE_FLOAT);
 
-  ret = type_register(&ctx->type_data_list, str_to_string, str_from_string,
-                      NULL, NULL, &type);
+  ret = type_register(&ctx->type_data_list, str_to_string, str_from_string, NULL, NULL, &type);
   assert(ret == 0);
   assert(type == SETTINGS_TYPE_STRING);
 
-  ret = type_register(&ctx->type_data_list, enum_to_string, enum_from_string,
-                      enum_format_type, bool_enum_names, &type);
+  ret = type_register(&ctx->type_data_list,
+                      enum_to_string,
+                      enum_from_string,
+                      enum_format_type,
+                      bool_enum_names,
+                      &type);
   assert(ret == 0);
   assert(type == SETTINGS_TYPE_BOOL);
 
   return ctx;
 }
 
 /**
  * @brief members_destroy - deinit for settings context members
  * @param ctx: settings context to deinit
  */
-static void members_destroy(settings_t *ctx) {
+static void members_destroy(settings_t *ctx)
+{
   type_data_free(ctx->type_data_list);
   setting_data_free(ctx->setting_data_list);
-  request_state_free(ctx);
 }
 
-void settings_destroy(settings_t **ctx) {
+void settings_destroy(settings_t **ctx)
+{
   assert(ctx != NULL);
   assert(*ctx != NULL);
   log_info("Releasing settings framework");
   setting_sbp_cb_unregister(*ctx, SBP_MSG_SETTINGS_REGISTER_RESP);
   setting_sbp_cb_unregister(*ctx, SBP_MSG_SETTINGS_WRITE);
   setting_sbp_cb_unregister(*ctx, SBP_MSG_SETTINGS_WRITE_RESP);
   setting_sbp_cb_unregister(*ctx, SBP_MSG_SETTINGS_READ_RESP);
```

### Comparing `libsettings-0.1.14/src/settings_util.c` & `libsettings-0.1.9/src/settings_util.c`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,21 @@
  */
 
 #include <stddef.h>
 #include <stdio.h>
 
 #include <libsettings/settings_util.h>
 
-int settings_format(const char *section, const char *name, const char *value,
-                    const char *type, char *buf, size_t blen) {
+int settings_format(const char *section,
+                    const char *name,
+                    const char *value,
+                    const char *type,
+                    char *buf,
+                    size_t blen)
+{
   int n = 0;
   int l = 0;
 
   const char *tokens[] = {section, name, value, type};
 
   for (uint8_t i = 0; i < sizeof(tokens) / sizeof(tokens[0]); ++i) {
     const char *token = tokens[i];
@@ -38,17 +43,21 @@
     n += l + 1;
   }
 
   return n;
 }
 
 /* Parse SBP message payload into setting parameters */
-settings_tokens_t settings_parse(const char *buf, size_t blen,
-                                 const char **section, const char **name,
-                                 const char **value, const char **type) {
+settings_tokens_t settings_parse(const char *buf,
+                                 size_t blen,
+                                 const char **section,
+                                 const char **name,
+                                 const char **value,
+                                 const char **type)
+{
   if (section) *section = NULL;
   if (name) *name = NULL;
   if (value) *value = NULL;
   if (type) *type = NULL;
 
   /* All strings must be NULL terminated */
   if ((blen > 0) && (buf[blen - 1] != '\0')) {
@@ -58,16 +67,15 @@
   const char **tokens[] = {section, name, value, type};
   settings_tokens_t tok = SETTINGS_TOKENS_EMPTY;
   size_t str_start = 0;
   for (size_t idx = 0; idx < blen; ++idx) {
     if (buf[idx] != '\0') {
       continue;
     }
-    if ((size_t)tok < sizeof(tokens) / sizeof(tokens[0]) &&
-        tokens[tok] != NULL) {
+    if ((size_t)tok < sizeof(tokens) / sizeof(tokens[0]) && tokens[tok] != NULL) {
       *(tokens[tok]) = &buf[str_start];
     }
     str_start = idx + 1;
     tok++;
   }
 
   return (tok <= SETTINGS_TOKENS_EXTRA_NULL) ? tok : SETTINGS_TOKENS_INVALID;
```

### Comparing `libsettings-0.1.14/third_party/libswiftnav/src/logging_common.c` & `libsettings-0.1.9/libswiftnav/src/logging_common.c`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
  * EITHER EXPRESSED OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE IMPLIED
  * WARRANTIES OF MERCHANTABILITY AND/OR FITNESS FOR A PARTICULAR PURPOSE.
  */
 
 #include <assert.h>
 #include <stdarg.h>
 #include <string.h>
+
 #include <swiftnav/logging.h>
 
 const char *level_string[] = {
     "EMERGENCY",
     "ALERT",
     "CRITICAL",
     "ERROR",
@@ -31,25 +32,19 @@
  * \param  path string of full path to file where this function was called
  * @return base file name of the path
  */
 const char *truncate_path_(char *path) {
   assert(NULL != path);
   int i;
 
-  if (path[0] == '\0') {
-    return "";
-  }
-  for (i = strlen(path) - 1; i >= 0 && path[i] == '/'; i--) {
+  if (path[0] == '\0') return "";
+  for (i = strlen(path) - 1; i >= 0 && path[i] == '/'; i--)
     ;
-  }
-  if (i == -1) {
-    return "/";
-  }
-  /* set the trailing character to null in case it was '/' e.g. /dev/null/ */
+  if (i == -1) return "/";
+  // set the trailing character to null in case it was '/'
+  // e.g. /dev/null/
   path[i + 1] = '\0';
-  /* Go backwards until the prior '/' */
-  while (i >= 0 && path[i] != '/') {
-    i--;
-  }
-  /* Return a pointer to the remainder */
+  // Go backwards until the prior '/'
+  while (i >= 0 && path[i] != '/') i--;
+  // Return a pointer to the remainder
   return &path[i + 1];
 }
```

