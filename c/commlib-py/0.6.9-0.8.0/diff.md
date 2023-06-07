# Comparing `tmp/commlib-py-0.6.9.tar.gz` & `tmp/commlib-py-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commlib-py-0.6.9.tar", last modified: Wed Dec 28 13:28:45 2022, max compression
+gzip compressed data, was "commlib-py-0.8.0.tar", last modified: Wed Dec 28 13:59:21 2022, max compression
```

## Comparing `commlib-py-0.6.9.tar` & `commlib-py-0.8.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:28:45.508022 commlib-py-0.6.9/
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      178 2021-03-03 19:36:50.000000 commlib-py-0.6.9/AUTHORS.rst
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     3530 2021-03-03 19:36:46.000000 commlib-py-0.6.9/CONTRIBUTING.rst
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       89 2021-03-03 19:36:46.000000 commlib-py-0.6.9/HISTORY.rst
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1082 2021-03-03 19:36:46.000000 commlib-py-0.6.9/LICENSE
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1082 2022-08-07 13:51:37.000000 commlib-py-0.6.9/LICENSE.txt
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      262 2021-03-03 19:36:46.000000 commlib-py-0.6.9/MANIFEST.in
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    28642 2022-12-28 13:28:45.508022 commlib-py-0.6.9/PKG-INFO
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1093 2021-03-03 19:36:50.000000 commlib-py-0.6.9/README.rst
-drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:28:45.504689 commlib-py-0.6.9/commlib/
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      139 2022-12-28 13:28:25.000000 commlib-py-0.6.9/commlib/__init__.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    18947 2022-12-28 10:22:47.000000 commlib-py-0.6.9/commlib/action.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    13763 2022-08-06 17:23:33.000000 commlib-py-0.6.9/commlib/bridges.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1686 2022-08-06 17:23:33.000000 commlib-py-0.6.9/commlib/endpoints.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1819 2022-12-28 10:22:47.000000 commlib-py-0.6.9/commlib/events.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     2803 2022-08-06 17:23:33.000000 commlib-py-0.6.9/commlib/exceptions.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     3990 2022-12-28 10:22:47.000000 commlib-py-0.6.9/commlib/logger.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     3860 2022-12-28 10:22:47.000000 commlib-py-0.6.9/commlib/msg.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    15012 2022-12-28 10:22:47.000000 commlib-py-0.6.9/commlib/node.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     3917 2022-12-28 10:22:47.000000 commlib-py-0.6.9/commlib/pubsub.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     3468 2022-12-28 10:22:47.000000 commlib-py-0.6.9/commlib/rest_proxy.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     8431 2022-12-28 10:22:47.000000 commlib-py-0.6.9/commlib/rpc.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     2299 2022-12-28 10:22:47.000000 commlib-py-0.6.9/commlib/serializer.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1481 2022-08-06 17:23:33.000000 commlib-py-0.6.9/commlib/tcp_proxy.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     2261 2022-08-06 17:23:33.000000 commlib-py-0.6.9/commlib/timer.py
-drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:28:45.504689 commlib-py-0.6.9/commlib/transports/
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      115 2022-08-06 17:23:33.000000 commlib-py-0.6.9/commlib/transports/__init__.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    46635 2022-12-28 10:22:47.000000 commlib-py-0.6.9/commlib/transports/amqp.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    27175 2022-12-28 10:22:47.000000 commlib-py-0.6.9/commlib/transports/mqtt.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    20984 2022-12-28 10:22:47.000000 commlib-py-0.6.9/commlib/transports/redis.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1166 2022-08-06 17:23:33.000000 commlib-py-0.6.9/commlib/utils.py
-drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:28:45.504689 commlib-py-0.6.9/commlib_py.egg-info/
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    28642 2022-12-28 13:28:45.000000 commlib-py-0.6.9/commlib_py.egg-info/PKG-INFO
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1069 2022-12-28 13:28:45.000000 commlib-py-0.6.9/commlib_py.egg-info/SOURCES.txt
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)        1 2022-12-28 13:28:45.000000 commlib-py-0.6.9/commlib_py.egg-info/dependency_links.txt
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)        1 2022-12-28 13:28:45.000000 commlib-py-0.6.9/commlib_py.egg-info/not-zip-safe
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       29 2022-12-28 13:28:45.000000 commlib-py-0.6.9/commlib_py.egg-info/requires.txt
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       14 2022-12-28 13:28:45.000000 commlib-py-0.6.9/commlib_py.egg-info/top_level.txt
-drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:28:45.504689 commlib-py-0.6.9/docs/
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      608 2022-03-11 00:09:26.000000 commlib-py-0.6.9/docs/Makefile
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       28 2022-03-11 00:09:26.000000 commlib-py-0.6.9/docs/authors.rst
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     2082 2022-03-11 00:09:26.000000 commlib-py-0.6.9/docs/commlib.rst
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      677 2022-03-11 00:06:52.000000 commlib-py-0.6.9/docs/commlib.transports.rst
--rwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)     4823 2022-03-11 00:09:26.000000 commlib-py-0.6.9/docs/conf.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       33 2022-03-11 00:09:26.000000 commlib-py-0.6.9/docs/contributing.rst
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       28 2022-03-11 00:09:26.000000 commlib-py-0.6.9/docs/history.rst
-drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:28:45.504689 commlib-py-0.6.9/docs/images/
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)   208772 2022-03-11 00:09:26.000000 commlib-py-0.6.9/docs/images/ptopicbridge_example.png
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      307 2022-03-11 00:09:26.000000 commlib-py-0.6.9/docs/index.rst
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1123 2022-03-11 00:09:26.000000 commlib-py-0.6.9/docs/installation.rst
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      769 2022-03-11 00:09:26.000000 commlib-py-0.6.9/docs/make.bat
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       58 2022-03-11 00:06:52.000000 commlib-py-0.6.9/docs/modules.rst
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       27 2022-03-11 00:09:26.000000 commlib-py-0.6.9/docs/readme.rst
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     4405 2022-03-11 00:09:26.000000 commlib-py-0.6.9/docs/usage.rst
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1430 2022-12-28 13:28:45.508022 commlib-py-0.6.9/setup.cfg
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1209 2022-04-06 16:28:45.000000 commlib-py-0.6.9/setup.py
-drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:28:45.504689 commlib-py-0.6.9/tests/
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    12996 2022-12-27 16:08:59.000000 commlib-py-0.6.9/tests/.coverage
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      137 2021-03-03 19:36:46.000000 commlib-py-0.6.9/tests/README.md
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       37 2021-03-03 19:36:46.000000 commlib-py-0.6.9/tests/__init__.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     2678 2022-12-28 10:22:47.000000 commlib-py-0.6.9/tests/test_msgs.py
--rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      862 2022-12-28 10:22:47.000000 commlib-py-0.6.9/tests/test_timer.py
+drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:59:21.317134 commlib-py-0.8.0/
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      178 2021-03-03 19:36:50.000000 commlib-py-0.8.0/AUTHORS.rst
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     3530 2021-03-03 19:36:46.000000 commlib-py-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       89 2021-03-03 19:36:46.000000 commlib-py-0.8.0/HISTORY.rst
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1082 2021-03-03 19:36:46.000000 commlib-py-0.8.0/LICENSE
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1082 2022-08-07 13:51:37.000000 commlib-py-0.8.0/LICENSE.txt
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      262 2021-03-03 19:36:46.000000 commlib-py-0.8.0/MANIFEST.in
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    28642 2022-12-28 13:59:21.317134 commlib-py-0.8.0/PKG-INFO
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1093 2021-03-03 19:36:50.000000 commlib-py-0.8.0/README.rst
+drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:59:21.313801 commlib-py-0.8.0/commlib/
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      139 2022-12-28 13:59:06.000000 commlib-py-0.8.0/commlib/__init__.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    18699 2022-12-28 13:58:22.000000 commlib-py-0.8.0/commlib/action.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1270 2022-12-28 13:58:00.000000 commlib-py-0.8.0/commlib/async_utils.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    13763 2022-08-06 17:23:33.000000 commlib-py-0.8.0/commlib/bridges.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      717 2022-12-28 13:58:00.000000 commlib-py-0.8.0/commlib/compression.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      207 2022-12-28 13:58:00.000000 commlib-py-0.8.0/commlib/connection.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1686 2022-08-06 17:23:33.000000 commlib-py-0.8.0/commlib/endpoints.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1750 2022-12-28 13:58:22.000000 commlib-py-0.8.0/commlib/events.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     2803 2022-08-06 17:23:33.000000 commlib-py-0.8.0/commlib/exceptions.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     3063 2022-12-28 13:58:00.000000 commlib-py-0.8.0/commlib/logger.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     2059 2022-12-28 13:58:22.000000 commlib-py-0.8.0/commlib/msg.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    14428 2022-12-28 13:58:22.000000 commlib-py-0.8.0/commlib/node.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     4047 2022-12-28 13:58:22.000000 commlib-py-0.8.0/commlib/pubsub.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     3259 2022-12-28 13:58:00.000000 commlib-py-0.8.0/commlib/rest_proxy.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     8469 2022-12-28 13:58:22.000000 commlib-py-0.8.0/commlib/rpc.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     2330 2022-12-28 13:58:00.000000 commlib-py-0.8.0/commlib/serializer.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1481 2022-08-06 17:23:33.000000 commlib-py-0.8.0/commlib/tcp_proxy.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     2261 2022-08-06 17:23:33.000000 commlib-py-0.8.0/commlib/timer.py
+drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:59:21.313801 commlib-py-0.8.0/commlib/transports/
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      115 2022-08-06 17:23:33.000000 commlib-py-0.8.0/commlib/transports/__init__.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    44700 2022-12-28 13:58:22.000000 commlib-py-0.8.0/commlib/transports/amqp.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    29453 2022-12-28 13:58:22.000000 commlib-py-0.8.0/commlib/transports/mqtt.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    21105 2022-12-28 13:58:22.000000 commlib-py-0.8.0/commlib/transports/redis.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1166 2022-08-06 17:23:33.000000 commlib-py-0.8.0/commlib/utils.py
+drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:59:21.313801 commlib-py-0.8.0/commlib_py.egg-info/
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)    28642 2022-12-28 13:59:21.000000 commlib-py-0.8.0/commlib_py.egg-info/PKG-INFO
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1121 2022-12-28 13:59:21.000000 commlib-py-0.8.0/commlib_py.egg-info/SOURCES.txt
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)        1 2022-12-28 13:59:21.000000 commlib-py-0.8.0/commlib_py.egg-info/dependency_links.txt
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)        1 2022-12-28 13:59:21.000000 commlib-py-0.8.0/commlib_py.egg-info/not-zip-safe
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       29 2022-12-28 13:59:21.000000 commlib-py-0.8.0/commlib_py.egg-info/requires.txt
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       14 2022-12-28 13:59:21.000000 commlib-py-0.8.0/commlib_py.egg-info/top_level.txt
+drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:59:21.317134 commlib-py-0.8.0/docs/
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      608 2022-03-11 00:09:26.000000 commlib-py-0.8.0/docs/Makefile
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       28 2022-03-11 00:09:26.000000 commlib-py-0.8.0/docs/authors.rst
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     2082 2022-03-11 00:09:26.000000 commlib-py-0.8.0/docs/commlib.rst
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      677 2022-03-11 00:06:52.000000 commlib-py-0.8.0/docs/commlib.transports.rst
+-rwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)     4823 2022-03-11 00:09:26.000000 commlib-py-0.8.0/docs/conf.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       33 2022-03-11 00:09:26.000000 commlib-py-0.8.0/docs/contributing.rst
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       28 2022-03-11 00:09:26.000000 commlib-py-0.8.0/docs/history.rst
+drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:59:21.317134 commlib-py-0.8.0/docs/images/
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)   208772 2022-03-11 00:09:26.000000 commlib-py-0.8.0/docs/images/ptopicbridge_example.png
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      307 2022-03-11 00:09:26.000000 commlib-py-0.8.0/docs/index.rst
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1123 2022-03-11 00:09:26.000000 commlib-py-0.8.0/docs/installation.rst
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      769 2022-03-11 00:09:26.000000 commlib-py-0.8.0/docs/make.bat
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       58 2022-03-11 00:06:52.000000 commlib-py-0.8.0/docs/modules.rst
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       27 2022-03-11 00:09:26.000000 commlib-py-0.8.0/docs/readme.rst
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     4405 2022-03-11 00:09:26.000000 commlib-py-0.8.0/docs/usage.rst
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1430 2022-12-28 13:59:21.317134 commlib-py-0.8.0/setup.cfg
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     1209 2022-04-06 16:28:45.000000 commlib-py-0.8.0/setup.py
+drwxr-xr-x   0 klpanagi  (1000) klpanagi  (1000)        0 2022-12-28 13:59:21.317134 commlib-py-0.8.0/tests/
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      137 2021-03-03 19:36:46.000000 commlib-py-0.8.0/tests/README.md
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)       37 2021-03-03 19:36:46.000000 commlib-py-0.8.0/tests/__init__.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)     2678 2022-12-28 13:58:22.000000 commlib-py-0.8.0/tests/test_msgs.py
+-rw-r--r--   0 klpanagi  (1000) klpanagi  (1000)      862 2022-12-28 13:58:22.000000 commlib-py-0.8.0/tests/test_timer.py
```

### Comparing `commlib-py-0.6.9/CONTRIBUTING.rst` & `commlib-py-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/LICENSE` & `commlib-py-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/LICENSE.txt` & `commlib-py-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/PKG-INFO` & `commlib-py-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commlib-py
-Version: 0.6.9
+Version: 0.8.0
 Summary: Communication Lirary for Python implementing the most common communication patterns for CyberPhysical Systems.
 Home-page: https://github.com/robotics-4-all/commlib-py
 Author: Konstantinos Panayiotou
 Author-email: klpanagi@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `commlib-py-0.6.9/README.rst` & `commlib-py-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/commlib/action.py` & `commlib-py-0.8.0/commlib/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import concurrent.futures.thread
-import datetime
 import threading
 import time
-import uuid
 from concurrent.futures import ThreadPoolExecutor
 from enum import IntEnum
 from functools import partial
-from typing import Dict
+from typing import Dict, Any
+
+from commlib.compression import CompressionType
 
 from .logger import Logger
-from .msg import ActionMessage, DataClass, DataField, PubSubMessage, RPCMessage
+from .msg import ActionMessage, Message, PubSubMessage, RPCMessage
 from .serializer import JSONSerializer, Serializer
-from .utils import gen_random_id
+from .utils import gen_random_id, gen_timestamp
 
 
 class GoalStatus(IntEnum):
     """GoalStatus.
     """
     ACCEPTED = 1
     EXECUTING = 2
@@ -26,92 +26,79 @@
 
 
 class _ActionGoalMessage(RPCMessage):
     """_ActionGoalMessage.
     Internal Action Goal (RPC) Message
     """
 
-    @DataClass
     class Request(RPCMessage.Request):
         description: str = ''
-        goal_data: dict = DataField(default_factory=dict)
+        goal_data: Dict = {}
 
-    @DataClass
     class Response(RPCMessage.Response):
         status: int = 0
         timestamp: int = -1
         goal_id: str = ''
 
         def __post_init__(self):
             self.timestamp = int(time.time())
 
 
 class _ActionResultMessage(RPCMessage):
     """_ActionResultMessage.
     Internal Action Result (RPC) Message
     """
 
-    @DataClass
     class Request(RPCMessage.Request):
         goal_id: str = ''
 
-    @DataClass
     class Response(RPCMessage.Response):
         status: int = 0
         timestamp: int = -1
-        result: dict = DataField(default_factory=dict)
+        result: Dict = {}
 
         def __post_init__(self):
             self.timestamp = int(time.time())
 
 
 class _ActionCancelMessage(RPCMessage):
     """_ActionCancelMessage.
     Internal Action Cancel (RPC) Message
     """
 
-    @DataClass
     class Request(RPCMessage.Request):
         goal_id: str = ''
-        timestamp: int = -1  ## Timestamp of when the request was made
+        timestamp: int = gen_timestamp()
 
-        def __post_init__(self):
-            self.timestamp = int(time.time())
 
-    @DataClass
     class Response(RPCMessage.Response):
         status: int = 0
-        timestamp: int = -1  ## Timestamp of when it was canceled
-        result: dict = DataField(default_factory=dict)
-
-        def __post_init__(self):
-            self.timestamp = int(time.time())
+        timestamp: int = gen_timestamp()
+        result: Dict[str, Any]
 
 
-@DataClass
 class _ActionStatusMessage(PubSubMessage):
     """_ActionStatusMessage.
     Internal Action Status Message.
     """
 
     goal_id: str = ''
     status: int = 0
 
 
-@DataClass
 class _ActionFeedbackMessage(PubSubMessage):
     """_ActionFeedbackMessage.
     Internal Action Feedback Message
     """
 
-    feedback_data: dict = DataField(default_factory=dict)
+    feedback_data: Dict[str, Any]
     goal_id: str = ''
 
 
-class GoalHandler(object):
+class GoalHandler:
     def __init__(self, msg_type: ActionMessage,
                  status_publisher: callable,
                  feedback_publisher: callable,
                  on_goal: callable,
                  on_cancel: callable):
         """__init__.
 
@@ -213,30 +200,29 @@
             raise ValueError('Wrong status code!')
         status = int(status)
         self.status = status
         msg = _ActionStatusMessage(status=status, goal_id=self.id)
         self._pub_status.publish(msg)
 
     def send_feedback(self, feedback_msg: _ActionFeedbackMessage):
-        _fb = feedback_msg.as_dict() if self._msg_type is not None \
-            else feedback_msg
-        msg = _ActionFeedbackMessage(feedback_data=_fb,
-                                     goal_id=self.id)
+        _fb = feedback_msg.dict() if self._msg_type is not None else feedback_msg
+        msg = _ActionFeedbackMessage(feedback_data=_fb, goal_id=self.id)
         self._pub_feedback.publish(msg)
 
     def set_result(self, result):
         self.result = result
 
 
-class BaseActionService(object):
+class BaseActionService:
     def __init__(self,
                  action_name: str,
                  msg_type: ActionMessage = None,
                  logger: Logger = None,
                  debug: bool = True,
+                 compression: CompressionType = CompressionType.NO_COMPRESSION,
                  on_goal: callable = None,
                  on_cancel: callable = None,
                  on_getresult: callable = None):
         """__init__.
 
         Args:
             action_name (str): The name (uri) of the action
@@ -245,14 +231,15 @@
             debug (bool): Debug mode
             on_goal (callable): on_goal callback function
             on_cancel (callable): on_cancel callback function
             on_getresult (callable): on_getresult callback function
         """
         self._msg_type = msg_type
         self._debug = debug
+        self._compression = compression
         self._action_name = action_name
         self._on_goal = on_goal
         self._on_cancel = on_cancel
         self._on_getresult = on_getresult
 
         self._status_topic = f'{self._action_name}.status'
         self._feedback_topic = f'{self._action_name}.feedback'
@@ -370,29 +357,30 @@
         elif self._current_goal is None:
             return resp
         elif self._current_goal.id != _goal_id:
             return resp
         resp.status = self._current_goal.status
         ## Set Result data
         if self._msg_type is not None:
-            resp.result = self._current_goal.result.as_dict()
+            resp.result = self._current_goal.result.dict()
         else:
             resp.result = self._current_goal.result
         return resp
 
     def __del__(self):
         self.stop()
 
 
-class BaseActionClient(object):
+class BaseActionClient:
     def __init__(self,
                  action_name: str,
                  msg_type: ActionMessage = None,
                  logger: Logger = None,
                  debug: bool = False,
+                 compression: CompressionType = CompressionType.NO_COMPRESSION,
                  on_feedback: callable = None,
                  on_result: callable = None,
                  on_goal_reached: callable = None):
         """__init__.
 
         Args:
             action_name (str): The name (uri) of the action
@@ -402,14 +390,15 @@
             on_feedback (callable): on_feedback
             on_result (callable): on_result
             on_goal_reached (callable): on_goal_reached
         """
         self._debug = debug
         self._action_name = action_name
         self._msg_type = msg_type
+        self._compression = compression
 
         self._status_topic = f'{self._action_name}.status'
         self._feedback_topic = f'{self._action_name}.feedback'
         self._goal_rpc_uri = f'{self._action_name}.send_goal'
         self._cancel_rpc_uri = f'{self._action_name}.cancel_goal'
         self._result_rpc_uri = f'{self._action_name}.get_result'
 
@@ -466,15 +455,15 @@
         Returns:
             _ActionGoalMessage.Response:
         """
         _data = {}
         if isinstance(goal_msg, dict) or isinstance(goal_msg, Dict):
             _data = goal_msg
         elif isinstance(goal_msg, ActionMessage.Goal):
-            _data = goal_msg.as_dict()
+            _data = goal_msg.dict()
         req = _ActionGoalMessage.Request(goal_data=_data)
         self._status = _ActionStatusMessage()
         resp = self._goal_client.call(req, timeout=timeout)
         self.result = None
         self._goal_id = resp.goal_id
         return resp
```

### Comparing `commlib-py-0.6.9/commlib/bridges.py` & `commlib-py-0.8.0/commlib/bridges.py`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/commlib/endpoints.py` & `commlib-py-0.8.0/commlib/endpoints.py`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/commlib/events.py` & `commlib-py-0.8.0/commlib/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,80 @@
-import time
-import datetime
 from typing import Text, Dict, Any
 
 from commlib.serializer import JSONSerializer, Serializer
 from commlib.logger import Logger
 from commlib.utils import gen_random_id
-from commlib.msg import Object, DataClass, DataField
+from pydantic import BaseModel, NoneIsAllowedError
 
+em_logger = None
 
-@DataClass
-class Event(Object):
+
+class Event(BaseModel):
     """Event.
     """
 
     name: Text
     uri: Text
     description: Text = ''
-    payload: Dict[str, Any] = DataField(default_factory=dict)
+    data: Dict[str, Any] = {}
 
 
 class BaseEventEmitter(object):
     """BaseEventEmitter.
     """
+    @classmethod
+    def logger(cls) -> Logger:
+        global em_logger
+        if em_logger is None:
+            em_logger = Logger('event-emitter')
+        return em_logger
 
     def __init__(self,
                  name: Text = None,
-                 logger: Logger = None,
                  debug: bool = False,
                  serializer: Serializer = None):
         """__init__.
 
         Args:
             name (Text): name
-            logger (Logger): logger
             debug (bool): debug
             serializer (Serializer): serializer
         """
         if name is None:
             name = gen_random_id()
         self._name = name
         self._debug = debug
         if serializer is not None:
             self._serializer = serializer
         else:
             self._serializer = JSONSerializer
 
-        self._logger = Logger(self.__class__.__name__, debug=debug) if \
-            logger is None else logger
-        self.logger.info(f'Initiated Event Emitter <{self._name}>')
+        self.log.info(f'Initiated Event Emitter <{self._name}>')
 
     @property
     def debug(self) -> bool:
         """debug.
 
         Args:
 
         Returns:
             bool:
         """
         return self._debug
 
     @property
-    def logger(self) -> Logger:
+    def log(self) -> Logger:
         """logger.
 
         Args:
 
         Returns:
             Logger:
         """
-        return self._logger
+        return self.logger()
 
     def send_event(self, event: Event) -> None:
         """send_event.
 
         Args:
             event (Event): event
```

### Comparing `commlib-py-0.6.9/commlib/exceptions.py` & `commlib-py-0.8.0/commlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/commlib/node.py` & `commlib-py-0.8.0/commlib/node.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from functools import wraps
-from enum import IntEnum
-from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
-import concurrent.futures.thread
-import time
 import threading
-from typing import Dict, List, Any, Optional
+import time
+from enum import IntEnum
+from functools import wraps
+from typing import Any, Dict, List, Optional
+from commlib.compression import CompressionType
 
 from commlib.endpoints import TransportType
-from commlib.utils import gen_random_id
 from commlib.logger import Logger
-from commlib.bridges import TopicBridge, RPCBridge
-from commlib.msg import HeartbeatMessage, RPCMessage, DataClass, DataField
+from commlib.msg import HeartbeatMessage, RPCMessage
+from commlib.utils import gen_random_id
+
+n_logger = None
 
 
 class NodePort:
     """NodePort.
     """
 
     def __init__(self):
@@ -74,56 +74,57 @@
     STOPPED = 4
     EXITED = 3
 
 
 class HeartbeatThread(threading.Thread):
     """HeartbeatThread.
     """
+    @classmethod
+    def logger(cls) -> Logger:
+        global n_logger
+        if n_logger is None:
+            n_logger = Logger('MQTTHeartbeatThread')
+        return n_logger
 
     def __init__(self, pub_instance=None,
                  interval: int = 10,
-                 logger: Logger = None,
                  *args, **kwargs):
         """__init__.
 
         Args:
             pub_instance:
             interval (int): interval
-            logger (Logger): logger
             args:
             kwargs:
         """
         super().__init__(*args, **kwargs)
         self._stop_event = threading.Event()
         self._rate_secs = interval
         self._heartbeat_pub = pub_instance
-        if logger is None:
-            logger = Logger(self.__class__.__name__)
-        self.logger = logger
         self.daemon = True
 
     def run(self):
         """run.
         """
         try:
             msg = HeartbeatMessage(ts=self.get_ts())
             while not self._stop_event.isSet():
-                self.logger.info(
+                self.logger().debug(
                     f'Sending heartbeat message - {self._heartbeat_pub._topic}')
                 if self._heartbeat_pub._msg_type == None:
-                    self._heartbeat_pub.publish(msg.as_dict())
+                    self._heartbeat_pub.publish(msg.dict())
                 else:
                     self._heartbeat_pub.publish(msg)
                 # Wait for n seconds or until stop event is raised
                 self._stop_event.wait(self._rate_secs)
                 msg.ts = self.get_ts()
         except Exception as exc:
-            self.logger.info(f'Exception in Heartbeat-Thread: {exc}')
+            self.logger().error(f'Exception in Heartbeat-Thread: {exc}')
         finally:
-            self.logger.info('Heartbeat Thread Ended')
+            self.logger().error('Heartbeat Thread Ended')
 
     def force_join(self, timeout: float = None):
         """force_join.
         Sudo stop the thread!
 
         Args:
             timeout (float): timeout
@@ -144,168 +145,164 @@
     def get_ts(self):
         """get_ts.
         """
         timestamp = (time.time() + 0.5) * 1000000
         return int(timestamp)
 
 
-class NodeStartMessage(RPCMessage):
-    @DataClass
+class _NodeStartMessage(RPCMessage):
     class Request(RPCMessage.Request):
         pass
 
-    @DataClass
     class Response(RPCMessage.Response):
-        status: int = DataField(default=0)
-        error: str = DataField(default='')
+        status: int = 0
+        error: str = ''
 
 
-class NodeStopMessage(RPCMessage):
-    @DataClass
+class _NodeStopMessage(RPCMessage):
     class Request(RPCMessage.Request):
         pass
 
-    @DataClass
     class Response(RPCMessage.Response):
-        status: int = DataField(default=0)
-        error: str = DataField(default='')
+        status: int = 0
+        error: str = ''
 
 
 class Node:
     """Node.
     """
+    @classmethod
+    def logger(cls) -> Logger:
+        global n_logger
+        if n_logger is None:
+            n_logger = Logger(f'node-{cls.__name__}')
+        return n_logger
 
     def __init__(self,
                  node_name: Optional[str] = '',
-                 transport_type: Optional[TransportType] = TransportType.REDIS,
                  connection_params: Optional[Any] = None,
                  transport_connection_params: Optional[Any] = None,
-                 remote_logger: Optional[bool] = False,
-                 remote_logger_uri: Optional[str] = '',
                  debug: Optional[bool] = False,
                  heartbeat_thread: Optional[bool] = True,
                  heartbeat_uri: Optional[str] = None,
+                 compression: CompressionType = CompressionType.NO_COMPRESSION,
                  ctrl_services: Optional[bool] = False):
         """__init__.
 
         Args:
             node_name (Optional[str]): node_name
             transport_type (Optional[TransportType]): transport_type
             connection_params (Optional[Any]): connection_params
             transport_connection_params (Optional[Any]): Same with connection_params.
                 Used for backward compatibility
-            remote_logger (Optional[bool]): remote_logger
-            remote_logger_uri (Optional[str]): remote_logger_uri
             debug (Optional[bool]): debug
             heartbeat_thread (Optional[bool]): heartbeat_thread
             heartbeat_uri (Optional[str]): heartbeat_uri
             ctrl_services (Optional[bool]): ctrl_services
         """
         if node_name == '' or node_name is None:
             node_name = gen_random_id()
         node_name = node_name.replace('-', '_')
         self._node_name = node_name
         self._debug = debug
         self._heartbeat_thread = heartbeat_thread
         self._heartbeat_uri = heartbeat_uri
+        self._compression = compression
         self._hb_thread = None
         self.state = NodeState.IDLE
         self._has_ctrl_services = ctrl_services
         self._namespace = f'{self._node_name}'
 
         self._publishers = []
         self._subscribers = []
         self._rpc_services = []
         self._rpc_clients = []
         self._action_services = []
         self._action_clients = []
         self._event_emitters = []
 
-        if transport_type == TransportType.REDIS:
-            import commlib.transports.redis as comm
-        elif transport_type == TransportType.AMQP:
-            import commlib.transports.amqp as comm
-        elif transport_type == TransportType.MQTT:
-            import commlib.transports.mqtt as comm
-        else:
-            raise ValueError('Transport type is not supported!')
-        self._commlib = comm
 
         ## Set default ConnectionParameters ---->
-        if transport_connection_params is not None:
-            self._conn_params = transport_connection_params
-        elif connection_params is None:
-            if transport_type == TransportType.REDIS:
-                from commlib.transports.redis import \
-                    UnixSocketConnectionParameters as ConnParams
-            elif transport_type == TransportType.AMQP:
-                from commlib.transports.amqp import \
-                    ConnectionParameters as ConnParams
-            elif transport_type == TransportType.MQTT:
-                from commlib.transports.mqtt import \
-                    ConnectionParameters as ConnParams
-            connection_params = ConnParams()
-            self._conn_params = connection_params
+        if transport_connection_params is not None and connection_params is None:
+            connection_params = transport_connection_params
+        self._conn_params = connection_params
+        type_str = str(type(self._conn_params)).split('\'')[1]
+
+        if type_str == 'commlib.transports.mqtt.ConnectionParameters':
+            import commlib.transports.mqtt as transport_module
+        elif type_str == 'commlib.transports.redis.ConnectionParameters':
+            import commlib.transports.redis as transport_module
+        elif type_str == 'commlib.transports.amqp.ConnectionParameters':
+            import commlib.transports.amqp as transport_module
         else:
-            self._conn_params = connection_params
-        ## <--------------------------------------
+            raise ValueError('Transport type is not supported!')
+        self._transport_module = transport_module
+
+        self.log.info(f'Created Node <{self._node_name}>')
+
+    @property
+    def log(self) -> Logger:
+        """logger.
 
-        self._logger = Logger(self._node_name, debug=debug)
-        self._logger.info(f'Created Node <{self._node_name}>')
+        Args:
+
+        Returns:
+            Logger:
+        """
+        return self.logger()
 
     def init_heartbeat_thread(self, topic: str = None) -> None:
         """init_heartbeat_thread.
         Starts the heartbeat thread. Heartbeat messages are sent periodically
         to inform about correct execution of the node.
 
         Args:
             topic (str): topic
         """
         if topic is None:
             topic = f'{self._namespace}.heartbeat'
         self._hb_thread = HeartbeatThread(
-            self.create_publisher(topic=topic, msg_type=HeartbeatMessage),
-            logger=self._logger
+            self.create_publisher(topic=topic, msg_type=HeartbeatMessage)
         )
         self._hb_thread.start()
-        self._logger.info(
+        self.log.info(
             f'Started Heartbeat Publisher <{topic}> in background')
 
     def init_stop_service(self, uri: str = None) -> None:
         if uri is None:
             uri = f'{self._namespace}.stop'
         stop_rpc = self.create_rpc(rpc_name=uri,
-                                   msg_type=NodeStopMessage,
+                                   msg_type=_NodeStopMessage,
                                    on_request=self._stop_rpc_callback)
         stop_rpc.run()
         self._stop_rpc = stop_rpc
 
-    def _stop_rpc_callback(self, msg: NodeStopMessage.Request) -> \
-            NodeStopMessage.Response:
-        resp = NodeStopMessage.Response()
+    def _stop_rpc_callback(self, msg: _NodeStopMessage.Request) -> \
+            _NodeStopMessage.Response:
+        resp = _NodeStopMessage.Response()
         if self.state == NodeState.RUNNING:
             self.state = NodeState.STOPPED
             self.stop()
         else:
             resp.status = 1
             resp.error = 'Cannot make the transition from current state!'
         return resp
 
     def init_start_service(self, uri: str = None) -> None:
         if uri is None:
             uri = f'{self._namespace}.start'
         start_rpc = self.create_rpc(rpc_name=uri,
-                                    msg_type=NodeStartMessage,
+                                    msg_type=_NodeStartMessage,
                                     on_request=self._start_rpc_callback)
         start_rpc.run()
         self._start_rpc = start_rpc
 
-    def _start_rpc_callback(self, msg: NodeStartMessage.Request) -> \
-            NodeStartMessage.Response:
-        resp = NodeStartMessage.Response()
+    def _start_rpc_callback(self, msg: _NodeStartMessage.Request) -> \
+            _NodeStartMessage.Response:
+        resp = _NodeStartMessage.Response()
         if self.state == NodeState.STOPPED:
             self.run()
         else:
             resp.status = 1
             resp.error = 'Cannot make the transition from current state!'
         return resp
 
@@ -329,15 +326,15 @@
     def ports(self):
         return {
             'input': self.input_ports,
             'output': self.output_ports
         }
 
     def get_logger(self):
-        return self._logger
+        return self.logger()
 
     def run(self) -> None:
         """run.
         Starts Services, Subscribers and ActionServices.
         Also starts the heartbeat thread (if enabled).
 
         Args:
@@ -381,90 +378,116 @@
             r.stop()
         for r in self._action_services:
             r.stop()
 
     def create_publisher(self, *args, **kwargs):
         """Creates a new Publisher Endpoint.
         """
-        pub = self._commlib.Publisher(conn_params=self._conn_params,
-                                      logger = self._logger,
-                                      *args, **kwargs)
+        pub = self._transport_module.Publisher(
+            conn_params=self._conn_params,
+            logger=self.logger(),
+            compression=self._compression,
+            *args, **kwargs
+        )
         self._publishers.append(pub)
         return pub
 
     def create_mpublisher(self, *args, **kwargs):
         """Creates a new Publisher Endpoint.
         """
-        pub = self._commlib.MPublisher(conn_params=self._conn_params,
-                                       logger = self._logger,
-                                       *args, **kwargs)
+        pub = self._transport_module.MPublisher(
+            conn_params=self._conn_params,
+            logger=self.logger(),
+            compression=self._compression,
+            *args, **kwargs
+        )
         self._publishers.append(pub)
         return pub
 
     def create_subscriber(self, *args, **kwargs):
         """Creates a new Publisher Endpoint.
         """
-        sub =  self._commlib.Subscriber(conn_params=self._conn_params,
-                                        logger = self._logger,
-                                        *args, **kwargs)
+        sub =  self._transport_module.Subscriber(
+            conn_params=self._conn_params,
+            logger=self.logger(),
+            compression=self._compression,
+            *args, **kwargs
+        )
         self._subscribers.append(sub)
         return sub
 
     def create_psubscriber(self, *args, **kwargs):
         """Creates a new Publisher Endpoint.
         """
-        sub =  self._commlib.PSubscriber(conn_params=self._conn_params,
-                                         logger = self._logger,
-                                         *args, **kwargs)
+        sub =  self._transport_module.PSubscriber(
+            conn_params=self._conn_params,
+            logger=self.logger(),
+            compression=self._compression,
+            *args, **kwargs
+        )
         self._subscribers.append(sub)
         return sub
 
     def subscriber_callback(self, fn):
         @wraps(fn)
         def wrapper(*args, **kwargs):
             return self.create_subscriber(*args, **kwargs)
         return wrapper
 
     def create_rpc(self, *args, **kwargs):
         """Creates a new Publisher Endpoint.
         """
-        rpc = self._commlib.RPCService(conn_params=self._conn_params,
-                                       logger = self._logger,
-                                       *args, **kwargs)
+        rpc = self._transport_module.RPCService(
+            conn_params=self._conn_params,
+            logger=self.logger(),
+            compression=self._compression,
+            *args, **kwargs
+        )
         self._rpc_services.append(rpc)
         return rpc
 
     def create_rpc_client(self, *args, **kwargs):
         """Creates a new Publisher Endpoint.
         """
-        client = self._commlib.RPCClient(conn_params=self._conn_params,
-                                         logger = self._logger,
-                                         *args, **kwargs)
+        client = self._transport_module.RPCClient(
+            conn_params=self._conn_params,
+            logger=self.logger(),
+            compression=self._compression,
+            *args, **kwargs
+        )
         self._rpc_clients.append(client)
         return client
 
     def create_action(self, *args, **kwargs):
         """Creates a new ActionService Endpoint.
         """
-        action =  self._commlib.ActionService(conn_params=self._conn_params,
-                                             logger = self._logger,
-                                             *args, **kwargs)
+        action =  self._transport_module.ActionService(
+            conn_params=self._conn_params,
+            logger=self.logger(),
+            compression=self._compression,
+            *args, **kwargs
+        )
         self._action_services.append(action)
         return action
 
     def create_action_client(self, *args, **kwargs):
         """Creates a new ActionClient Endpoint.
         """
-        aclient = self._commlib.ActionClient(conn_params=self._conn_params,
-                                             logger = self._logger,
-                                             *args, **kwargs)
+        aclient = self._transport_module.ActionClient(
+            conn_params=self._conn_params,
+            logger=self.logger(),
+            compression=self._compression,
+            *args, **kwargs
+        )
         self._action_clients.append(aclient)
         return aclient
 
     def create_event_emitter(self, *args, **kwargs):
         """Creates a new EventEmitter Endpoint.
         """
-        em = self._commlib.EventEmitter(conn_params=self._conn_params,
-                                        logger = self._logger,
-                                        *args, **kwargs)
+        em = self._transport_module.EventEmitter(
+            conn_params=self._conn_params,
+            compression=self._compression,
+            *args, **kwargs
+        )
         self._event_emitters.append(em)
         return em
```

### Comparing `commlib-py-0.6.9/commlib/pubsub.py` & `commlib-py-0.8.0/commlib/pubsub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 from concurrent.futures import ThreadPoolExecutor
 import threading
-import uuid
-from typing import Dict, Any
+from typing import Dict, Any, Callable
 
-from .serializer import JSONSerializer
+from .serializer import Serializer, JSONSerializer
 from .logger import Logger
 from .utils import gen_random_id
 from .msg import PubSubMessage
+from .compression import CompressionType
 
 
 class BasePublisher(object):
     """BasePublisher.
     """
 
     def __init__(self, topic: str = None,
                  msg_type: PubSubMessage = None,
                  logger: Logger = None,
                  debug: bool = True,
-                 serializer=None):
+                 serializer: Serializer = JSONSerializer,
+                 compression: CompressionType = CompressionType.NO_COMPRESSION):
         """__init__.
 
         Args:
             topic (str): topic
             msg_type (PubSubMessage): msg_type
             logger (Logger): logger
             debug (bool): debug
             serializer:
         """
-        self._debug = debug
-        self._topic = topic
-        self._msg_type = msg_type
-
         if topic is None:
             raise ValueError('Topic Name not defined')
 
-        if serializer is not None:
-            self._serializer = serializer
-        else:
-            self._serializer = JSONSerializer
+        self._debug = debug
+        self._topic = topic
+        self._msg_type = msg_type
+        self._serializer = serializer
+        self._compression = compression
 
         self._logger = Logger(self.__class__.__name__) if \
             logger is None else logger
 
         self._gen_random_id = gen_random_id
 
-        self.logger.debug('Created Publisher: <{}>'.format(self._topic))
+        self.logger.debug(f'Initiated Publisher <{self._topic}>')
 
     @property
     def debug(self) -> bool:
         return self._debug
 
     @property
     def logger(self) -> Logger:
@@ -68,42 +66,38 @@
 
 class BaseSubscriber(object):
     """BaseSubscriber.
     """
 
     def __init__(self, topic: str = None,
                  msg_type: PubSubMessage = None,
-                 on_message: callable = None,
+                 on_message: Callable = None,
                  logger: Logger = None,
                  debug: bool = True,
-                 serializer=None):
+                 serializer: Serializer = JSONSerializer,
+                 compression: CompressionType = CompressionType.NO_COMPRESSION):
         """__init__.
 
         Args:
             topic (str): topic
             msg_type (PubSubMessage): msg_type
             on_message (callable): on_message
             logger (Logger): logger
             debug (bool): debug
             serializer:
         """
+        if topic is None:
+            raise ValueError('Topic name cannot be None')
         self._debug = debug
         self._topic = topic
         self._msg_type = msg_type
-
-        if topic is None:
-            raise ValueError('Topic name cannot be None')
-
+        self._compression = compression
+        self._serializer = serializer
         self.onmessage = on_message
 
-        if serializer is not None:
-            self._serializer = serializer
-        else:
-            self._serializer = JSONSerializer
-
         self._logger = Logger(self.__class__.__name__) if \
             logger is None else logger
 
         self._gen_random_id = gen_random_id
 
         self._executor = ThreadPoolExecutor(max_workers=2)
```

### Comparing `commlib-py-0.6.9/commlib/rest_proxy.py` & `commlib-py-0.8.0/commlib/rest_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import time
 import json
 
 import requests
 
-from typing import Dict, List, Any, Optional
+from typing import Dict, List, Any, Optional, Union
 
 from commlib.endpoints import TransportType, EndpointType, endpoint_factory
-from commlib.msg import DataClass, DataField, Object, PubSubMessage, RPCMessage
+from commlib.msg import PubSubMessage, RPCMessage
 
 
 """
 {
     BASE_URL: 'https://example.org:9080',
     VERB: 'GET',
     PARAMS: {
@@ -20,28 +20,26 @@
     }
     HEADERS: {}
 }
 
 """
 
 class RESTProxyMessage(RPCMessage):
-    @DataClass
     class Request(RPCMessage.Request):
         base_url: str
         path: str = '/'
         verb: str = 'GET'
-        query_params: Dict = DataField(default_factory=dict)
-        path_params: Dict = DataField(default_factory=dict)
-        body_params: Dict = DataField(default_factory=dict)
-        headers: Dict = DataField(default_factory=dict)
+        query_params: Dict = {}
+        path_params: Dict = {}
+        body_params: Dict = {}
+        headers: Dict = {}
 
-    @DataClass
     class Response(RPCMessage.Response):
-        data: Any = DataField(default_factory=dict)
-        headers: Dict = DataField(default_factory=dict)
+        data: Union[str, Dict, int]
+        headers: Dict[str, Any]
         status_code: int = 200
 
 
 class RESTProxy:
     """RESTProxy.
 
     REST Proxy implementation class. Call REST Web services via commlib
```

### Comparing `commlib-py-0.6.9/commlib/rpc.py` & `commlib-py-0.8.0/commlib/rpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,70 +1,65 @@
 from concurrent.futures import ThreadPoolExecutor
 import threading
 import uuid
 from concurrent import futures
 from functools import partial
-from typing import Any, Dict, Tuple
+from typing import Any, Dict, Callable
 
-from commlib.serializer import JSONSerializer
+from commlib.serializer import JSONSerializer, Serializer
+from commlib.compression import CompressionType
 from commlib.logger import Logger
 from commlib.utils import gen_random_id, gen_timestamp
+from pydantic import BaseModel
 from commlib.msg import (
-    DataClass,
-    DataField,
-    Object,
     PubSubMessage,
     RPCMessage
 )
 
 
-@DataClass
-class CommRPCHeader(Object):
-    timestamp: int = DataField(default=gen_timestamp())
-    reply_to: str = DataField(default='')
+class CommRPCHeader(BaseModel):
+    reply_to: str = ''
+    timestamp: int = gen_timestamp()
 
 
-@DataClass
-class CommRPCObject(Object):
-    header: CommRPCHeader = DataField(default_factory=CommRPCHeader)
-    data: Dict[str, Any] = DataField(default_factory=dict)
+class CommRPCObject(BaseModel):
+    header: CommRPCHeader = CommRPCHeader()
+    data: Dict[str, Any] = {}
 
 
-class BaseRPCServer(object):
+class BaseRPCServer:
     """RPCServer Base class.
     Inherit to implement transport-specific RPCService.
 
     Args:
         - rpc_name (str)
     """
 
     def __init__(self,
                  base_uri: str = '',
                  svc_map: dict = {},
                  logger: Logger = None,
                  debug: bool = False,
                  workers: int = 2,
-                 serializer: Any = None):
+                 serializer: Serializer = JSONSerializer,
+                 compression: CompressionType = CompressionType.NO_COMPRESSION):
         """__init__.
 
         Args:
             logger (Logger): logger
             debug (bool): debug
             workers (int): workers
             serializer:
         """
         self._base_uri = base_uri
         self._svc_map = svc_map
         self._num_workers = workers
         self._debug = debug
-
-        if serializer is not None:
-            self._serializer = serializer
-        else:
-            self._serializer = JSONSerializer
+        self._serializer = serializer
+        self._compression = compression
 
         self._logger = Logger(self.__class__.__name__, self._debug) if \
             logger is None else logger
 
         self._gen_random_id = gen_random_id
 
         self._executor = ThreadPoolExecutor(max_workers=self._num_workers)
@@ -102,29 +97,30 @@
         """stop.
         Stop the RPC Service.
         """
         if self._t_stop_event is not None:
             self._t_stop_event.set()
 
 
-class BaseRPCService(object):
+class BaseRPCService:
     """RPCService Base class.
     Inherit to implement transport-specific RPCService.
 
     Args:
         - rpc_name (str)
     """
 
     def __init__(self, rpc_name: str = None,
                  msg_type: RPCMessage = None,
-                 on_request: callable = None,
+                 on_request: Callable = None,
                  logger: Logger = None,
                  debug: bool = False,
                  workers: int = 2,
-                 serializer=None):
+                 serializer: Serializer = JSONSerializer,
+                 compression: CompressionType = CompressionType.NO_COMPRESSION):
         """__init__.
 
         Args:
             rpc_name (str): rpc_name
             msg_type (RPCMessage): msg_type
             on_request (callable): on_request
             logger (Logger): logger
@@ -135,19 +131,16 @@
         if rpc_name is None:
             raise ValueError('RPC Name cannot be None')
         self._rpc_name = rpc_name
         self._msg_type = msg_type
         self._num_workers = workers
         self._debug = debug
         self.on_request = on_request
-
-        if serializer is not None:
-            self._serializer = serializer
-        else:
-            self._serializer = JSONSerializer
+        self._serializer = serializer
+        self._compression = compression
 
         self._logger = Logger(self.__class__.__name__, self._debug) if \
             logger is None else logger
 
         self._gen_random_id = gen_random_id
 
         self._executor = ThreadPoolExecutor(max_workers=2)
@@ -157,16 +150,15 @@
 
         self._comm_obj = CommRPCObject()
 
     def _serialize_data(self, payload: Dict[str, Any]) -> str:
         return self._serializer.serialize(payload)
 
     def _serialize_response(self, message: RPCMessage.Response) -> str:
-        return self._serialize_data(message.as_dict())
-
+        return self._serialize_data(message.dict())
 
     @property
     def debug(self):
         return self._debug
 
     @property
     def logger(self):
@@ -192,44 +184,42 @@
         """stop.
         Stop the RPC Service.
         """
         if self._t_stop_event is not None:
             self._t_stop_event.set()
 
 
-class BaseRPCClient(object):
+class BaseRPCClient:
     """RPCClient Base class.
     Inherit to implement transport-specific RPCClient.
     """
 
     def __init__(self,
                  rpc_name: str = None,
                  msg_type: RPCMessage = None,
                  logger: Logger = None,
                  debug: bool = False,
-                 serializer=None,
-                 max_workers: int = 5):
+                 max_workers: int = 5,
+                 serializer: Serializer = JSONSerializer,
+                 compression: CompressionType = CompressionType.NO_COMPRESSION):
         """__init__.
 
         Args:
             rpc_name (str): rpc_name
             msg_type (RPCMessage): msg_type
             logger (Logger): logger
             debug (bool): debug
         """
         if rpc_name is None:
             raise ValueError('RPC name cannot be None')
         self._rpc_name = rpc_name
         self._msg_type = msg_type
         self._debug = debug
-
-        if serializer is not None:
-            self._serializer = serializer
-        else:
-            self._serializer = JSONSerializer
+        self._serializer = serializer
+        self._compression = compression
 
         self._logger = Logger(self.__class__.__name__, debug=self._debug) if \
             logger is None else logger
 
         self._gen_random_id = gen_random_id
 
         self._executor = futures.ThreadPoolExecutor(max_workers=max_workers)
@@ -293,9 +283,9 @@
                 on_response(result)
                 return result
 
     def _serialize_data(self, payload: Dict[str, Any]) -> str:
         return self._serializer.serialize(payload)
 
     def _serialize_request(self, message: RPCMessage.Request) -> str:
-        return self._serialize_data(message.as_dict())
+        return self._serialize_data(message.dict())
```

### Comparing `commlib-py-0.6.9/commlib/serializer.py` & `commlib-py-0.8.0/commlib/serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import abc
 import enum
-from typing import Any
+from typing import Any, Dict
 
 DEFAULT_JSON_SERIALIZER = 'ujson'
 
 
 if DEFAULT_JSON_SERIALIZER == 'json':
     import json as json
 elif DEFAULT_JSON_SERIALIZER == 'ujson':
@@ -65,27 +65,27 @@
 
 
 class JSONSerializer(Serializer):
     """Thin wrapper to implement json serializer.
 
     Static class.
     """
-    CONTENT_TYPE: str = 'application/json'
+    CONTENT_TYPE: str = ContentType.json
     CONTENT_ENCODING: str = 'utf8'
 
     @staticmethod
-    def serialize(data: Any) -> str:
+    def serialize(data: Dict[str, Any]) -> str:
         """serialize.
 
         Args:
             data (dict): Serialize to json string
         """
-        return json.dumps(data)
+        return str(json.dumps(data))
 
     @staticmethod
-    def deserialize(data: str) -> Any:
+    def deserialize(data: str) -> Dict[str, Any]:
         """deserialize.
 
         Args:
             data (str): json str to dict
         """
         return json.loads(data)
```

### Comparing `commlib-py-0.6.9/commlib/tcp_proxy.py` & `commlib-py-0.8.0/commlib/tcp_proxy.py`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/commlib/timer.py` & `commlib-py-0.8.0/commlib/timer.py`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/commlib/transports/amqp.py` & `commlib-py-0.8.0/commlib/transports/amqp.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 from collections import deque
 from threading import Event as ThreadEvent
 from threading import Semaphore, Thread
 from typing import Dict
 
 import pika
 
-from commlib.action import (
-    BaseActionClient, BaseActionService, _ActionCancelMessage,
-    _ActionFeedbackMessage, _ActionGoalMessage,
-    _ActionResultMessage, _ActionStatusMessage
-)
+from commlib.action import (BaseActionClient, BaseActionService,
+                            _ActionCancelMessage, _ActionFeedbackMessage,
+                            _ActionGoalMessage, _ActionResultMessage,
+                            _ActionStatusMessage)
+from commlib.compression import CompressionType, deflate, inflate_str
 from commlib.events import BaseEventEmitter, Event
 from commlib.exceptions import *
 from commlib.logger import Logger
 from commlib.msg import PubSubMessage, RPCMessage
 from commlib.pubsub import BasePublisher, BaseSubscriber
 from commlib.rpc import BaseRPCClient, BaseRPCService
 from commlib.utils import gen_timestamp
+from commlib.connection import ConnectionParametersBase
 
 # Reduce log level for pika internal logger
 logging.getLogger("pika").setLevel(logging.WARN)
 
 
 class MessageProperties(pika.BasicProperties):
     """Message Properties/Attribures used for sending and receiving messages.
@@ -67,115 +68,37 @@
             reply_to=reply_to,
             message_id=str(message_id) if message_id is not None else None,
             user_id=str(user_id) if user_id is not None else None,
             app_id=str(app_id) if app_id is not None else None
         )
 
 
-class Credentials:
-    """Connection credentials for authn/authz.
-
-    Args:
-        username (str): The username.
-        password (str): The password (Basic Authentication).
-    """
-
-    __slots__ = ['username', 'password']
-
-    def __init__(self, username: str = 'guest', password: str = 'guest'):
-        """__init__.
-
-        Args:
-            username (str): username
-            password (str): password
-        """
-        self.username = username
-        self.password = password
-
-    def make_pika(self):
-        """make_pika.
-        Create Pika Credentials instance.
-        """
-        return pika.PlainCredentials(username=self.username,
-                                     password=self.password)
-
-
-class ConnectionParameters():
+class ConnectionParameters(ConnectionParametersBase):
     """AMQP Connection parameters.
     AMQP connection parameters class
     """
-
-    __slots__ = [
-        'host', 'port', 'secure', 'vhost', 'reconnect_attempts', 'retry_delay',
-        'timeout', 'heartbeat_timeout', 'blocked_connection_timeout', 'creds',
-        'channel_max'
-    ]
-
-    def __init__(self,
-                 host: str = '127.0.0.1',
-                 port: int = 5672,
-                 vhost: str = '/',
-                 creds: Credentials = None,
-                 secure: bool = False,
-                 reconnect_attempts: int = 10,
-                 retry_delay: float = 2.0,
-                 timeout: float = 120,
-                 blocked_connection_timeout: float = None,
-                 heartbeat_timeout: int = 60,
-                 channel_max: int = 128):
-        """__init__.
-
-        Args:
-            host (str): Hostname of AMQP broker to connect to.
-            port (int): AMQP broker listening port.
-            creds (Credentials): Auth Credentials - Credentials instance.
-            secure (bool): Enable SSL/TLS (AMQPS) - Not supported!!
-            reconnect_attempts (int): The reconnection attempts to make before
-                droping and raising an Exception.
-            retry_delay (float): Time delay between reconnect attempts.
-            timeout (float): Socket Connection timeout value.
-            timeout (float): Blocked Connection timeout value.
-                Set the timeout, in seconds, that the connection may remain blocked
-                (triggered by Connection.Blocked from broker). If the timeout
-                expires before connection becomes unblocked, the connection will
-                be torn down.
-            heartbeat_timeout (int): Controls AMQP heartbeat
-                timeout negotiation during connection tuning. An integer value
-                always overrides the value proposed by broker. Use 0 to deactivate
-                heartbeats and None to always accept the broker's proposal.
-                The value passed for timeout is also used to calculate an interval
-                at which a heartbeat frame is sent to the broker. The interval is
-                equal to the timeout value divided by two.
-            channel_max (int): The max permissible number of channels per
-                connection. Defaults to 128.
-        """
-        self.host = host
-        self.port = port
-        self.secure = secure
-        self.vhost = vhost
-        self.reconnect_attempts = reconnect_attempts
-        self.retry_delay = retry_delay
-        self.timeout = timeout
-        self.blocked_connection_timeout = blocked_connection_timeout
-        self.heartbeat_timeout = heartbeat_timeout
-        self.channel_max = channel_max
-
-        if creds is None:
-            creds = Credentials()
-        self.creds = creds
-
-    @property
-    def credentials(self):
-        return self.creds
+    host: str = '127.0.0.1'
+    port: int = 5672
+    vhost: str = '/'
+    secure: bool = False
+    reconnect_attempts: int = 10
+    retry_delay: float = 2.0
+    timeout: float = 120
+    blocked_connection_timeout: float = None
+    heartbeat_timeout: int = 60
+    channel_max: int = 128
+    username: str = 'guest'
+    password: str = 'guest'
 
     def make_pika(self):
         return pika.ConnectionParameters(
             host=self.host,
             port=str(self.port),
-            credentials=self.creds.make_pika(),
+            credentials=pika.PlainCredentials(username=self.username,
+                                              password=self.password),
             connection_attempts=self.reconnect_attempts,
             retry_delay=self.retry_delay,
             blocked_connection_timeout=self.blocked_connection_timeout,
             socket_timeout=self.timeout,
             virtual_host=self.vhost,
             heartbeat=self.heartbeat_timeout,
             channel_max=self.channel_max)
@@ -310,18 +233,18 @@
     def create_channel(self):
         """Connect to the AMQP broker. Creates a new channel."""
         try:
             # Create a new communication channel
             self._channel = self._connection.channel()
             # self.add_threadsafe_callback(self._on_connect)
             self.logger.debug(
-                    'Connected to AMQP broker @ [{}:{}, vhost={}]'.format(
-                        self._conn_params.host,
-                        self._conn_params.port,
-                        self._conn_params.vhost))
+                f'Connected to AMQP broker <amqp://' + \
+                f'{self._conn_params.host}:{self._conn_params.port}, ' + \
+                f'vhost={self._conn_params.vhost}>'
+            )
         except pika.exceptions.ConnectionClosed:
             self.logger.debug('Connection timed out. Reconnecting...')
             self.connect()
         except pika.exceptions.AuthenticationError:
             self.logger.debug('Authentication Error. Reconnecting...')
         except pika.exceptions.AMQPConnectionError as e:
             self.logger.debug(f'Connection Error ({e}). Reconnecting...')
@@ -501,17 +424,14 @@
 
     def close(self):
         self._graceful_shutdown()
 
     def disconnect(self):
         self._graceful_shutdown()
 
-    # def __del__(self):
-    #     self._graceful_shutdown()
-
 
 class RPCService(BaseRPCService):
     """AMQP RPC Service class.
     Implements an AMQP RPC Service.
 
     Args:
         rpc_name (str): The name of the RPC.
@@ -580,14 +500,16 @@
             _cencoding = properties.content_encoding
             _dmode = properties.delivery_mode
             _ts_send = properties.timestamp
         except Exception:
             self.logger.error("Exception Thrown in on_request_handle",
                               exc_info=True)
         try:
+            if self._compression != CompressionType.NO_COMPRESSION:
+                body = deflate(body)
             _data = self._serializer.deserialize(body)
         except Exception:
             self.logger.error("Could not deserialize data", exc_info=True)
             # Return data as is. Let callback handle with encoding...
             _data = {}
             self._send_response(_data, ch, _corr_id, _reply_to, _delivery_tag)
             return
@@ -604,26 +526,30 @@
         else:
             try:
                 msg = self._msg_type.Request(**data)
                 resp = self.on_request(msg)
             except Exception as exc:
                 self.logger.error(str(exc), exc_info=False)
                 resp = self._msg_type.Response()
-            resp = resp.as_dict()
+            resp = resp.dict()
         return resp
 
     def _send_response(self, data: dict, channel, correlation_id: str,
                        reply_to: str, delivery_tag: str):
         _payload = None
         _encoding = None
         _type = None
         try:
             _encoding = self._serializer.CONTENT_ENCODING
             _type = self._serializer.CONTENT_TYPE
-            _payload = self._serializer.serialize(data).encode(_encoding)
+            _payload = self._serializer.serialize(data)
+            if self._compression != CompressionType.NO_COMPRESSION:
+                _payload = inflate_str(_payload)
+            else:
+                _payload = _payload.encode(_encoding)
         except Exception as e:
             self.logger.error("Could not deserialize data",
                               exc_info=True)
             _payload = {
                 'status': 501,
                 'error': f'Internal server error: {e}'
             }
@@ -744,15 +670,15 @@
         Args:
             timeout (float): Response timeout. Set this value carefully
                 based on application criteria.
         """
         if self._msg_type is None:
             data = msg
         else:
-            data = msg.as_dict()
+            data = msg.dict()
 
         self._response = None
         if self._use_corr_id:
             self._corr_id = self.gen_corr_id()
 
         start_t = time.time()
         self._transport.connection.add_callback_threadsafe(
@@ -791,29 +717,35 @@
             _dmode = properties.delivery_mode
             _ts_send = properties.timestamp
         except Exception:
             self.logger.error("Error parsing response from rpc server.",
                               exc_info=True)
 
         try:
+            if self._compression != CompressionType.NO_COMPRESSION:
+                body = deflate(body)
             _data = self._serializer.deserialize(body)
         except Exception:
             self.logger.error("Could not deserialize data",
                               exc_info=True)
             _data = {}
         self._response = _data
 
-    def _send_msg(self, data: dict) -> None:
+    def _send_msg(self, data: Dict) -> None:
         _payload = None
         _encoding = None
         _type = None
 
         _encoding = self._serializer.CONTENT_ENCODING
         _type = self._serializer.CONTENT_TYPE
-        _payload = self._serializer.serialize(data).encode(_encoding)
+        _payload = self._serializer.serialize(data)
+        if self._compression != CompressionType.NO_COMPRESSION:
+            _payload = inflate_str(_payload)
+        else:
+            _payload = _payload.encode(_encoding)
 
         # Direct reply-to implementation
         _rpc_props = MessageProperties(
             content_type=_type,
             content_encoding=_encoding,
             correlation_id=self._corr_id,
             timestamp=gen_timestamp(),
@@ -870,27 +802,31 @@
             msg (PubSubMessage): Message to publish.
         """
         if self._msg_type is not None and not isinstance(msg, PubSubMessage):
             raise ValueError('Argument "msg" must be of type PubSubMessage')
         elif isinstance(msg, dict):
             data = msg
         elif isinstance(msg, PubSubMessage):
-            data = msg.as_dict()
+            data = msg.dict()
         ## Thread Safe solution
         self._transport.add_threadsafe_callback(self._send_msg, data,
                                                 self._topic)
 
     def _send_msg(self, msg: Dict, topic: str):
         _payload = None
         _encoding = None
         _type = None
 
         _encoding = self._serializer.CONTENT_ENCODING
         _type = self._serializer.CONTENT_TYPE
-        _payload = self._serializer.serialize(msg).encode(_encoding)
+        _payload = self._serializer.serialize(msg)
+        if self._compression != CompressionType.NO_COMPRESSION:
+            _payload = inflate_str(_payload)
+        else:
+            _payload = _payload.encode(_encoding)
 
         msg_props = MessageProperties(
             content_type=_type,
             content_encoding=_encoding,
             message_id=0,
         )
 
@@ -915,15 +851,15 @@
             msg (PubSubMessage): Message to publish.
         """
         if self._msg_type is not None and not isinstance(msg, PubSubMessage):
             raise ValueError('Argument "msg" must be of type PubSubMessage')
         elif isinstance(msg, dict):
             data = msg
         elif isinstance(msg, PubSubMessage):
-            data = msg.as_dict()
+            data = msg.dict()
         ## Thread Safe solution
         self._transport.add_threadsafe_callback(self._send_msg, data, topic)
 
 
 class Subscriber(BaseSubscriber):
     """Subscriber class.
     Implements the Subscriber endpoint of the PubSub communication pattern.
@@ -1043,14 +979,16 @@
             _cencoding = properties.content_encoding
             _dmode = properties.delivery_mode
             _ts_send = properties.timestamp
         except Exception:
             self.logger.debug("Failed to read message properties",
                               exc_info=True)
         try:
+            if self._compression != CompressionType.NO_COMPRESSION:
+                body = deflate(body)
             _data = self._serializer.deserialize(body)
         except Exception:
             self.logger.error("Could not deserialize data",
                               exc_info=True)
             # Return data as is. Let callback handle with encoding...
             _data = {}
         try:
@@ -1094,16 +1032,25 @@
         self.close()
 
     def __exit__(self, exc_type, value, traceback):
         self.close()
 
 
 class PSubscriber(Subscriber):
+    """PSubscriber.
+    """
+
 
     def __init__(self, *args, **kwargs):
+        """__init__.
+
+        Args:
+            args:
+            kwargs:
+        """
         kwargs['topic'] = kwargs['topic'].replace('*', '#')
         super(PSubscriber, self).__init__(*args, **kwargs)
 
     def _on_msg_callback_wrapper(self, ch, method, properties, body):
         _data = {}
         _ctype = None
         _cencoding = None
@@ -1116,14 +1063,16 @@
             _dmode = properties.delivery_mode
             _ts_send = properties.timestamp
         except Exception:
             self.logger.debug("Error reading message properties",
                               exc_info=True)
 
         try:
+            if self._compression != CompressionType.NO_COMPRESSION:
+                body = deflate(body)
             _data = self._serializer.deserialize(body)
         except Exception:
             self.logger.error("Could not deserialize data",
                               exc_info=True)
             # Return data as is. Let callback handle with encoding...
             _data = {}
         try:
@@ -1265,15 +1214,15 @@
         if connection is None:
             self.run()
 
     def run(self) -> None:
         self._transport.detach_amqp_events_thread()
 
     def send_event(self, event: Event):
-        _data = event.as_dict()
+        _data = event.dict()
         self._logger.debug(f'Sending Event <{event.uri}>')
         self._transport.add_threadsafe_callback(
             functools.partial(self._send_data, event.uri, _data)
         )
 
     def _send_data(self, topic: str, data: dict) -> None:
         _payload = None
```

### Comparing `commlib-py-0.6.9/commlib/transports/mqtt.py` & `commlib-py-0.8.0/commlib/transports/mqtt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,204 +1,249 @@
 """
 MQTT Implementation
 """
 
 import functools
 import time
 from enum import IntEnum
-from typing import Any, Dict, Tuple
+from typing import Any, Dict, Tuple, Callable
 
 import paho.mqtt.client as mqtt
+from paho.mqtt.properties import Properties
+from paho.mqtt.packettypes import PacketTypes
 
 from commlib.action import (BaseActionClient, BaseActionService,
                             _ActionCancelMessage, _ActionFeedbackMessage,
                             _ActionGoalMessage, _ActionResultMessage,
                             _ActionStatusMessage)
 from commlib.events import BaseEventEmitter, Event
 from commlib.exceptions import RPCClientTimeoutError
 from commlib.logger import Logger
 from commlib.msg import PubSubMessage, RPCMessage
 from commlib.pubsub import BasePublisher, BaseSubscriber
 from commlib.rpc import BaseRPCClient, BaseRPCServer, BaseRPCService
-from commlib.serializer import Serializer, JSONSerializer
+from commlib.serializer import JSONSerializer, Serializer
 from commlib.utils import gen_timestamp
+from commlib.connection import ConnectionParametersBase
+
+mqtt_logger = None
+from commlib.compression import CompressionType, inflate_str, deflate
 
 
 class MQTTReturnCode(IntEnum):
     CONNECTION_SUCCESS = 0
     INCORRECT_PROTOCOL_VERSION = 1
     INVALID_CLIENT_ID = 2
     SERVER_UNAVAILABLE = 3
     AUTHENTICATION_ERROR = 4
     AUTHORIZATION_ERROR = 5
 
 
 class MQTTProtocolType(IntEnum):
-    MQTTv31 = 1
-    MQTTv311 = 2
-
-
-class Credentials:
-    def __init__(self, username: str = '', password: str = ''):
-        self.username = username
-        self.password = password
+    MQTTv31 = mqtt.MQTTv31
+    MQTTv311 = mqtt.MQTTv311
+    MQTTv5 = mqtt.MQTTv5
 
 
-class ConnectionParameters:
-    __slots__ = ['host', 'port', 'creds', 'protocol']
-    def __init__(self,
-                 host: str = 'localhost',
-                 port: int = 1883,
-                 protocol: MQTTProtocolType = MQTTProtocolType.MQTTv311,
-                 creds: Credentials = Credentials()):
-        """__init__.
+class MQTTQoS(IntEnum):
+    """
+    MQTT QoS Levels.
+    https://mntolia.com/mqtt-qos-levels-explained/
+    """
+    L0 = 0  # At Most Once
+    L1 = 1  # At Least Once
+    L2 = 2  # Exactly Once
 
-        Args:
-            host (str): host
-            port (int): port
-            protocol (MQTTProtocolType): protocol
-            creds (Credentials): creds
-        """
-        self.host = host
-        self.port = port
-        self.protocol = protocol
-        self.creds = creds
 
-    @property
-    def credentials(self):
-        return self.creds
+class ConnectionParameters(ConnectionParametersBase):
+    host: str = 'localhost'
+    port: int = 1883
+    username: str = ''
+    password: str = ''
+    protocol: MQTTProtocolType = MQTTProtocolType.MQTTv311
+    ssl: bool = False
+    transport: str = 'tcp'
 
 
 class MQTTTransport:
     """MQTTTransport.
     """
+    @classmethod
+    def logger(cls) -> Logger:
+        global mqtt_logger
+        if mqtt_logger is None:
+            mqtt_logger = Logger('mqtt')
+        return mqtt_logger
+
+    @property
+    def log(self):
+        return self.logger()
 
     def __init__(self,
                  conn_params: ConnectionParameters = ConnectionParameters(),
                  serializer: Serializer = JSONSerializer(),
-                 logger: Logger = None):
+                 compression: CompressionType = CompressionType.DEFAULT_COMPRESSION):
         """__init__.
 
         Args:
             conn_params (ConnectionParameters): conn_params
+            serializer (Serializer): serializer
+            compression (CompressionType): compression_type
             logger (Logger): logger
         """
         self._conn_params = conn_params
-        self._logger = logger
-        self._connected = False
-
         self._serializer = serializer
+        self._compression= compression
 
-        self.logger = Logger(self.__class__.__name__) if \
-            logger is None else logger
+        ## Workaround for bith v3 and v5 support
+        # http://www.steves-internet-guide.com/python-mqtt-client-changes/
+        if self._conn_params.protocol == MQTTProtocolType.MQTTv5:
+            properties = Properties(PacketTypes.CONNECT)
+            properties.MaximumPacketSize=20
+        else:
+            properties = None
+        self._mqtt_properties = properties
+
+        self._connected = False
 
         self._client = mqtt.Client(clean_session=True,
-                                   protocol=mqtt.MQTTv311,
-                                   transport='tcp')
+                                   protocol=self._conn_params.protocol,
+                                   transport=self._conn_params.transport)
 
         self._client.on_connect = self.on_connect
         self._client.on_disconnect = self.on_disconnect
         # self._client.on_log = self.on_log
         self._client.on_message = self.on_message
 
-        self._client.username_pw_set(self._conn_params.creds.username,
-                                     self._conn_params.creds.password)
-
-        self._client.connect(self._conn_params.host,
-                             int(self._conn_params.port),
-                             60)
+        self._client.username_pw_set(self._conn_params.username,
+                                     self._conn_params.password)
+        if self._conn_params.ssl:
+            import ssl
+            self._client.tls_set(cert_reqs=None, certfile=None, keyfile=None)
+
+        self._client.connect(
+            self._conn_params.host, int(self._conn_params.port),
+            keepalive=60,
+            properties=self._mqtt_properties
+        )
+        self.log.debug('MQTT Transport initiated:')
+        self.log.debug(
+            f'- Broker: mqtt://' + \
+            f'{self._conn_params.host}:{self._conn_params.port}'
+        )
+        self.log.debug(f'- Data Serialization: {self._serializer}')
+        self.log.debug(f'- Data Compression: {self._compression}')
 
     @property
     def is_connected(self):
         return self._connected
 
     def on_connect(self, client: Any, userdata: Any,
-                   flags: Dict[str, Any], rc: int):
+                   flags: Dict[str, Any], rc: int, properties=None):
         """on_connect.
 
         Callback for on-connect event.
 
         Args:
             client (Any): Internal paho-mqtt
             userdata (Any): Internal paho-mqtt userdata
             flags (Dict[str, Any]): Interla paho-mqtt flags
             rc (int): Return Code - Internal paho-mqtt
         """
         if rc == MQTTReturnCode.CONNECTION_SUCCESS:
-            self.logger.debug(
-                f"Connected to MQTT broker <{self._conn_params.host}:{self._conn_params.port}>")
-            self._connected = True
+            self.log.debug('MQTT Transport initiated:')
+            self.log.debug(
+                f'- Broker: mqtt://' + \
+                f'{self._conn_params.host}:{self._conn_params.port}'
+            )
+            self.log.debug(f'- Data Serialization: {self._serializer}')
+            self.log.debug(f'- Data Compression: {self._compression}')
 
     def on_disconnect(self, client: Any, userdata: Any,
                       rc: Dict[str, Any]):
         """on_disconnect.
 
         Callback for on-disconnect event.
 
         Args:
             client (Any): Internal paho-mqtt
             userdata (Any): Internal paho-mqtt userdata
             rc (int): Return Code - Internal paho-mqtt
         """
         if rc != 0:
-            self.logger.warn("Unexpected disconnection from MQTT Broker.")
+            self.log.warn("Unexpected disconnection from MQTT Broker.")
 
-    def on_message(self, client: Any, userdata: Any,
-                   msg: Dict[str, Any]):
+    def on_message(self, client: Any, userdata: Any, msg: Dict[str, Any]):
         """on_message.
 
         Callback for on-message event.
 
         Args:
             client (Any): Internal paho-mqtt
             userdata (Any): Internal paho-mqtt userdata
             msg (Dict[str, Any]): Received message
         """
         raise NotImplementedError()
 
     def on_log(self, client: Any, userdata: Any,
                level, buf):
         ## SPAM output
-        # self.logger.debug(f'MQTT Log: {buf}')
+        # self.log.debug(f'MQTT Log: {buf}')
         pass
 
-    def publish(self, topic: str, payload: Dict[str, Any], qos: int = 0,
-                retain: bool = False, confirm_delivery: bool = False):
+    def publish(self, topic: str, payload: Dict[str, Any],
+                qos: MQTTQoS = MQTTQoS.L0,
+                retain: bool = False):
         """publish.
 
         Args:
             topic (str): topic
             payload (Dict[str, Any]): payload
-            qos (int): qos
-            retain (bool): retain
-            confirm_delivery (bool): confirm_delivery
+            qos (int): MQTT QoS Level (see MQTTQoS class)
+            retain (bool): If set to True, then it tells the broker to store
+                that message on the topic as the “last good message”.
         """
         topic = topic.replace('.', '/')
         pl = self._serializer.serialize(payload)
-        ph = self._client.publish(topic, pl, qos=qos, retain=retain)
-        if confirm_delivery:
-            ph.wait_for_publish()
+        if self._compression != CompressionType.NO_COMPRESSION:
+            pl = inflate_str(pl)
+        ph = self._client.publish(topic, pl, qos=qos, retain=retain,
+                                  properties=self._mqtt_properties)
 
-    def subscribe(self, topic: str, callback: Any, qos: int = 0) -> str:
+    def subscribe(self, topic: str, callback: Any,
+                  qos: MQTTQoS = MQTTQoS.L0) -> str:
         """subscribe.
 
         Args:
             topic (str): topic
             callback (Any): callback
-            qos (int): qos
+            qos (int): MQTT QoS Level (see MQTTQoS class)
 
         Returns:
             str:
         """
         ## Adds subtopic specific callback handlers
         topic = topic.replace('.', '/').replace('*', '#')
-        self._client.subscribe(topic, qos)
-        self._client.message_callback_add(topic, callback)
+        self._client.subscribe(topic, qos=qos, options=None,
+                               properties=self._mqtt_properties)
+        _clb = functools.partial(self._on_msg_internal, callback)
+        self._client.message_callback_add(topic, _clb)
         return topic
 
+    def _on_msg_internal(self, callback: Callable, client: Any,
+                         userdata: Any, msg: Any):
+        _topic = msg.topic
+        _payload = msg.payload
+        _qos = msg.qos
+        _retain = msg.retain
+        if self._compression != CompressionType.NO_COMPRESSION:
+            _payload = deflate(_payload)
+        msg.payload = _payload
+        callback(client, userdata, msg)
+
     def start_loop(self):
         """start_loop.
 
         Start the event loop. Cannot create any more endpoints from here on.
         """
         self._client.loop_start()
 
@@ -233,15 +278,15 @@
             kwargs: See BasePublisher
         """
         self._msg_seq = 0
         self.conn_params = conn_params
         super().__init__(*args, **kwargs)
         self._transport = MQTTTransport(conn_params=conn_params,
                                         serializer=self._serializer,
-                                        logger=self._logger)
+                                        compression=self._compression)
         self._transport.start_loop()
 
     def publish(self, msg: PubSubMessage) -> None:
         """publish.
 
         Args:
             msg (PubSubMessage): Message to Publish
@@ -250,16 +295,16 @@
             None:
         """
         if self._msg_type is not None and not isinstance(msg, PubSubMessage):
             raise ValueError('Argument "msg" must be of type PubSubMessage')
         elif isinstance(msg, dict):
             data = msg
         elif isinstance(msg, PubSubMessage):
-            data = msg.as_dict()
-        self._transport.publish(self._topic, data)
+            data = msg.dict()
+        self._transport.publish(self._topic, data, qos=MQTTQoS.L0)
         self._msg_seq += 1
 
 
 class MPublisher(Publisher):
     """MPublisher.
     Multi-Topic Publisher
     """
@@ -278,15 +323,15 @@
             None:
         """
         if self._msg_type is not None and not isinstance(msg, PubSubMessage):
             raise ValueError('Argument "msg" must be of type PubSubMessage')
         elif isinstance(msg, dict):
             data = msg
         elif isinstance(msg, PubSubMessage):
-            data = msg.as_dict()
+            data = msg.dict()
         self._transport.publish(topic, data)
         self._msg_seq += 1
 
 
 class Subscriber(BaseSubscriber):
     """Subscriber.
     MQTT Subscriber
@@ -302,15 +347,15 @@
             args: See BaseSubscriber
             kwargs: See BaseSubscriber
         """
         self.conn_params = conn_params
         super(Subscriber, self).__init__(*args, **kwargs)
         self._transport = MQTTTransport(conn_params=conn_params,
                                         serializer=self._serializer,
-                                        logger=self._logger)
+                                        compression=self._compression)
 
     def run(self):
         self._topic = self._transport.subscribe(self._topic,
                                                 self._on_message)
         self._transport.start_loop()
         self.logger.debug(f'Started Subscriber: <{self._topic}>')
 
@@ -390,27 +435,27 @@
             args: See BaseRPCService
             kwargs: See BaseRPCService
         """
         self.conn_params = conn_params
         super(RPCService, self).__init__(*args, **kwargs)
         self._transport = MQTTTransport(conn_params=conn_params,
                                         serializer=self._serializer,
-                                        logger=self._logger)
+                                        compression=self._compression)
 
     def _send_response(self, data: dict, reply_to: str):
         """_send_response.
 
         Args:
             data (dict): data
             reply_to (str): reply_to
         """
         self._comm_obj.header.timestamp = gen_timestamp()   #pylint: disable=E0237
         self._comm_obj.data = data
-        _resp = self._comm_obj.as_dict()
-        self._transport.publish(reply_to, _resp)
+        _resp = self._comm_obj.dict()
+        self._transport.publish(reply_to, _resp, qos=MQTTQoS.L1)
 
     def _on_request_internal(self, client: Any, userdata: Any,
                              msg: Dict[str, Any]):
         """_on_request_internal.
 
         Args:
             client (Any): client
@@ -425,15 +470,15 @@
             return
         try:
             if self._msg_type is None:
                 resp = self.on_request(data)
             else:
                 resp = self.on_request(self._msg_type.Request(**data))
                 ## RPCMessage.Response object here
-                resp = resp.as_dict()
+                resp = resp.dict()
         except Exception as exc:
             self.logger.error(str(exc), exc_info=False)
             resp = {}
         reply_to = header['reply_to']
         self._send_response(resp, reply_to)
 
     def _unpack_comm_msg(self, msg: Any) -> Tuple[Any, Any, Any]:
@@ -453,15 +498,16 @@
         _header = _payload['header']
         return _data, _header, _uri
 
     def run_forever(self):
         """run_forever.
         """
         self._transport.subscribe(self._rpc_name,
-                                  self._on_request_internal)
+                                  self._on_request_internal,
+                                  qos=MQTTQoS.L1)
         self._transport.start_loop()
         while True:
             if self._t_stop_event is not None:
                 if self._t_stop_event.is_set():
                     self.logger.debug('Stop event caught in thread')
                     break
             time.sleep(0.001)
@@ -482,31 +528,31 @@
             args: See BaseRPCServer
             kwargs: See BaseRPCServer
         """
         self.conn_params = conn_params
         super(RPCServer, self).__init__(*args, **kwargs)
         self._transport = MQTTTransport(conn_params=conn_params,
                                         serializer=self._serializer,
-                                        logger=self._logger)
+                                        compression=self._compression)
         for uri in self._svc_map:
             callback = self._svc_map[uri][0]
             msg_type = self._svc_map[uri][1]
             self._register_endpoint(uri, callback, msg_type)
 
     def _send_response(self, data: dict, reply_to: str):
         """_send_response.
 
         Args:
             data (dict): data
             reply_to (str): reply_to
         """
         self._comm_obj.header.timestamp = gen_timestamp()   #pylint: disable=E0237
         self._comm_obj.data = data
-        _resp = self._comm_obj.as_dict()
-        self._transport.publish(reply_to, _resp)
+        _resp = self._comm_obj.dict()
+        self._transport.publish(reply_to, _resp, qos=MQTTQoS.L1)
 
     def _on_request_internal(self, client: Any, userdata: Any,
                              msg: Dict[str, Any]):
         """_on_request_internal.
 
         Args:
             client (Any): client
@@ -525,15 +571,15 @@
             else:
                 clb = self._svc_map[svc_uri][0]
                 msg_type = self._svc_map[svc_uri][1]
                 if msg_type is None:
                     resp = clb(data)
                 else:
                     resp = clb(msg_type.Request(**data))
-                    resp = resp.as_dict()
+                    resp = resp.dict()
         except Exception as exc:
             self.logger.error(exc, exc_info=False)
             resp = {}
             return
         self._send_response(resp, reply_to)
 
     def _unpack_comm_msg(self, msg: Any) -> Tuple[Any, Any, Any]:
@@ -555,15 +601,16 @@
                            msg_type: RPCMessage = None):
         self._svc_map[uri] = (callback, msg_type)
         if self._base_uri in (None, ''):
             full_uri = uri
         else:
             full_uri = f'{self._base_uri}.{uri}'
         self.logger.info(f'Registering endpoint <{full_uri}>')
-        self._transport.subscribe(full_uri, self._on_request_internal)
+        self._transport.subscribe(full_uri, self._on_request_internal,
+                                  qos=MQTTQoS.L1)
 
     def run_forever(self):
         """run_forever.
         """
         self._transport.start_loop()
         while True:
             if self._t_stop_event is not None:
@@ -594,15 +641,15 @@
         """
         self.conn_params = conn_params
         self._response = None
 
         super(RPCClient, self).__init__(*args, **kwargs)
         self._transport = MQTTTransport(conn_params=conn_params,
                                         serializer=self._serializer,
-                                        logger=self._logger)
+                                        compression=self._compression)
         self._transport.start_loop()
 
     def _gen_queue_name(self):
         """_gen_queue_name.
         """
         return f'rpc-{self._gen_random_id()}'
 
@@ -611,15 +658,15 @@
 
         Args:
             data:
         """
         self._comm_obj.header.timestamp = gen_timestamp()   #pylint: disable=E0237
         self._comm_obj.header.reply_to = self._gen_queue_name()
         self._comm_obj.data = data
-        return self._comm_obj.as_dict()
+        return self._comm_obj.dict()
 
     def _on_response_wrapper(self, client: Any, userdata: Any,
                              msg: Dict[str, Any]):
         """_on_response_wrapper.
 
         Args:
             client (Any): client
@@ -664,24 +711,25 @@
             timeout (float): timeout
         """
         if self._msg_type is None:
             data = msg
         else:
             if not isinstance(msg, self._msg_type.Request):
                 raise ValueError('Message type not valid')
-            data = msg.as_dict()
+            data = msg.dict()
 
         self._response = None
 
         _msg = self._prepare_request(data)
         _reply_to = _msg['header']['reply_to']
 
-        self._transport.subscribe(_reply_to, callback=self._on_response_wrapper)
+        self._transport.subscribe(_reply_to, callback=self._on_response_wrapper,
+                                  qos=MQTTQoS.L1)
         start_t = time.time()
-        self._transport.publish(self._rpc_name, _msg)
+        self._transport.publish(self._rpc_name, _msg, qos=MQTTQoS.L1)
         _resp = self._wait_for_response(timeout=timeout)
         elapsed_t = time.time() - start_t
         self._delay = elapsed_t
 
         if self._msg_type is None:
             return _resp
         else:
@@ -800,23 +848,22 @@
             conn_params (ConnectionParameters): Broker Connection Parameters
             args: See BaseEventEmitter
             kwargs: See BaseEventEmitter
         """
         super(EventEmitter, self).__init__(*args, **kwargs)
 
         self._transport = MQTTTransport(conn_params=conn_params,
-                                        serializer=self._serializer,
-                                        logger=self._logger)
+                                        serializer=self._serializer)
         self._transport.start_loop()
 
     def send_event(self, event: Event) -> None:
         """send_event.
 
         Args:
             event (Event): The Event to send.
 
         Returns:
             None:
         """
-        _msg = event.as_dict()
-        self.logger.debug(f'Firing Event: {event.name}:<{event.uri}>')
-        self._transport.publish(event.uri, _msg)
+        _msg = event.dict()
+        self.log.debug(f'Firing Event: {event.name}:<{event.uri}>')
+        self._transport.publish(event.uri, _msg, qos=MQTTQoS.L1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `commlib-py-0.6.9/commlib/transports/redis.py` & `commlib-py-0.8.0/commlib/transports/redis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,178 +1,166 @@
 import datetime
 import functools
 import sys
 import time
-from typing import Any, Dict, Tuple
+from typing import Any, Dict, Tuple, Callable
 
 import redis
 
 from commlib.action import (BaseActionClient, BaseActionService,
                             _ActionCancelMessage, _ActionFeedbackMessage,
                             _ActionGoalMessage, _ActionResultMessage,
                             _ActionStatusMessage)
 from commlib.events import BaseEventEmitter, Event
 from commlib.exceptions import RPCClientTimeoutError, SubscriberError
 from commlib.logger import Logger
-from commlib.msg import DataClass, DataField, Object, PubSubMessage, RPCMessage
+from commlib.msg import PubSubMessage, RPCMessage
 from commlib.pubsub import BasePublisher, BaseSubscriber
 from commlib.rpc import BaseRPCClient, BaseRPCService
 from commlib.serializer import Serializer, JSONSerializer
+from commlib.compression import CompressionType, inflate_str, deflate
 from commlib.utils import gen_timestamp
+from commlib.connection import ConnectionParametersBase
 
+redis_logger = None
 
-class Credentials(object):
-    def __init__(self, username: str = '', password: str = ''):
-        self.username = username
 
-        self.password = password
+class ConnectionParameters(ConnectionParametersBase):
+    host: str = 'localhost'
+    port: int = 6379
+    unix_socket: str = ''
+    db: int = 0
+    username: str = ''
+    password: str = ''
 
 
-class ConnectionParametersBase(object):
-    __slots__ = ['db', 'creds']
-
-    def __init__(self, db: int = 0, creds: Credentials = None):
-        self.db = db
-
-        if creds is None:
-            creds = Credentials()
-        self.creds = creds
-
-    @property
-    def credentials(self):
-        return self.creds
-
-
-class TCPConnectionParameters(ConnectionParametersBase):
-    """TCPConnectionParameters.
-    Redis TCP connection parameters
+class RedisConnection(redis.Redis):
+    """RedisConnection.
     """
 
-    def __init__(self,
-                 host: str = 'localhost',
-                 port: str = 6379,
-                 *args, **kwargs):
-        """__init__.
-
-        Args:
-            host (str): host
-            port (str): port
-            args: See ConnectionParametersBase class
-            kwargs: See ConnectionParametersBase class
-        """
-        super(TCPConnectionParameters, self).__init__(*args, **kwargs)
-        self.host = host
-        self.port = port
-
-
-class UnixSocketConnectionParameters(ConnectionParametersBase):
-    def __init__(self,
-                 unix_socket: str = '/tmp/redis.sock',
-                 *args, **kwargs):
+    def __init__(self, *args, **kwargs):
         """__init__.
 
         Args:
-            unix_socket (str): unix_socket
-            args: See ConnectionParametersBase class
-            kwargs: See ConnectionParametersBase class
+            args:
+            kwargs:
         """
-        super(UnixSocketConnectionParameters, self).__init__(*args, **kwargs)
-        self.unix_socket = unix_socket
-
-
-class ConnectionParameters(TCPConnectionParameters):
-    def __init__(self, *args, **kwargs):
-        super(ConnectionParameters, self).__init__(*args, **kwargs)
-
-
-class RedisConnection(redis.Redis):
-    def __init__(self, *args, **kwargs):
         super(RedisConnection, self).__init__(*args, **kwargs)
 
 
 class RedisTransport(object):
+    @classmethod
+    def logger(cls) -> Logger:
+        global redis_logger
+        if redis_logger is None:
+            redis_logger = Logger('redis')
+        return redis_logger
+
     def __init__(self,
                  conn_params: Any = None,
-                 serializer: Serializer = JSONSerializer(),
-                 logger: Any = None):
+                 compression: CompressionType = CompressionType.DEFAULT_COMPRESSION,
+                 serializer: Serializer = JSONSerializer()):
         """__init__.
 
         Args:
             conn_params (Any): conn_params
             serializer (Serializer): serializer
-            logger (Any): logger
+            compression (CompressionType): compression
         """
-        conn_params = TCPConnectionParameters() if \
+        conn_params = ConnectionParameters() if \
             conn_params is None else conn_params
         self._conn_params = conn_params
-
         self._serializer = serializer
-
-        self.logger = Logger(self.__class__.__name__) if \
-            logger is None else logger
+        self._compression = compression
 
         try:
             self.connect()
         except Exception as e:
-            self.logger.error(
-                f'Failed to connect to Redis broker <{self._conn_params.host}' +
-                f'{self._conn_params.port}>')
+            self.log.error(
+                f'Failed to connect to Redis <redis://' + \
+                f'{self._conn_params.host}:{self._conn_params.port}>')
             raise e
-        else:
-            self.logger.debug(
-                f'Connected to Redis <{self._conn_params.host}:{self._conn_params.port}>')
+        self.log.debug('Redis Transport initiated:')
+        self.log.debug(
+            f'- Broker: mqtt://' + \
+            f'{self._conn_params.host}:{self._conn_params.port}'
+        )
+        self.log.debug(f'- Data Serialization: {self._serializer}')
+        self.log.debug(f'- Data Compression: {self._compression}')
 
+    @property
+    def log(self) -> Logger:
+        """logger.
+
+        Args:
+
+        Returns:
+            Logger:
+        """
+        return self.logger()
 
     def connect(self):
-        if isinstance(self._conn_params, UnixSocketConnectionParameters):
+        if self._conn_params.unix_socket not in ('', None):
             self._redis = RedisConnection(
                 unix_socket_path=self._conn_params.unix_socket,
-                username=self._conn_params.credentials.username,
-                password=self._conn_params.credentials.password,
+                username=self._conn_params.username,
+                password=self._conn_params.password,
                 db=self._conn_params.db,
                 decode_responses=True)
-        elif isinstance(self._conn_params, TCPConnectionParameters):
+        else:
             self._redis = RedisConnection(
                 host=self._conn_params.host,
                 port=self._conn_params.port,
-                username=self._conn_params.credentials.username,
-                password=self._conn_params.credentials.password,
+                username=self._conn_params.username,
+                password=self._conn_params.password,
                 db=self._conn_params.db,
-                decode_responses=True)
+                decode_responses=False)
 
         self._rsub = self._redis.pubsub()
 
-
     def delete_queue(self, queue_name: str) -> bool:
-        # self.logger.debug('Removing message queue: <{}>'.format(queue_name))
+        # self.log.debug('Removing message queue: <{}>'.format(queue_name))
         return True if self._redis.delete(queue_name) else False
 
     def queue_exists(self, queue_name: str) -> bool:
         return True if self._redis.exists(queue_name) else False
 
     def push_msg_to_queue(self, queue_name: str, data: Dict[str, Any]):
         payload = self._serializer.serialize(data)
+        if self._compression != CompressionType.NO_COMPRESSION:
+            payload = inflate_str(payload)
         self._redis.rpush(queue_name, payload)
 
     def publish(self, queue_name: str, data: Dict[str, Any]):
         payload = self._serializer.serialize(data)
+        if self._compression != CompressionType.NO_COMPRESSION:
+            payload = inflate_str(payload)
         self._redis.publish(queue_name, payload)
 
-    def subscribe(self, topic: str, callback: callable):
+    def subscribe(self, topic: str, callback: Callable):
+        _clb = functools.partial(self._on_msg_internal, callback)
         self._sub = self._rsub.psubscribe(
-            **{topic: callback})
+            **{topic: _clb})
         self._rsub.get_message()
         t = self._rsub.run_in_thread(0.001, daemon=True)
         return t
 
+    def _on_msg_internal(self, callback: Callable, data: Any):
+        if self._compression != CompressionType.NO_COMPRESSION:
+            # _topic = data['channel']
+            data['data'] = deflate(data['data'])
+        callback(data)
+
     def wait_for_msg(self, queue_name: str, timeout=10):
         try:
             msgq, payload = self._redis.blpop(queue_name, timeout=timeout)
+            if self._compression != CompressionType.NO_COMPRESSION:
+                payload = deflate(payload)
         except Exception as exc:
-            self.logger.error(exc, exc_info=True)
+            self.log.error(exc, exc_info=True)
             msgq = ''
             payload = None
         return msgq, payload
 
 
 class RPCService(BaseRPCService):
     """RPCService.
@@ -187,30 +175,31 @@
         Args:
             conn_params (ConnectionParameters): conn_params
             args: See BaseRPCService class
             kwargs: See BaseRPCService class
         """
         super(RPCService, self).__init__(*args, **kwargs)
         self._transport = RedisTransport(conn_params=conn_params,
-                                         logger=self._logger)
+                                         serializer=self._serializer,
+                                         compression=self._compression)
 
     def _send_response(self, data, reply_to):
         self._comm_obj.header.timestamp = gen_timestamp()   #pylint: disable=E0237
         self._comm_obj.data = data
-        _resp = self._comm_obj.as_dict()
+        _resp = self._comm_obj.dict()
         self._transport.push_msg_to_queue(reply_to, _resp)
 
     def _on_request(self, data: dict, header: dict):
         try:
             if self._msg_type is None:
                 resp = self.on_request(data)
             else:
                 resp = self.on_request(self._msg_type.Request(**data))
                 ## RPCMessage.Response object here
-                resp = resp.as_dict()
+                resp = resp.dict()
         except Exception as exc:
             self.logger.error(str(exc), exc_info=False)
             resp = {}
         reply_to = header['reply_to']
         self._send_response(resp, reply_to)
 
     def run_forever(self):
@@ -247,37 +236,48 @@
 
     def __exec_in_thread(self, on_request):
         _future = self._executor.submit(on_request)
         return _future
 
 
 class RPCClient(BaseRPCClient):
+    """RPCClient.
+    """
+
     def __init__(self,
                  conn_params: ConnectionParameters = None,
                  *args, **kwargs):
+        """__init__.
+
+        Args:
+            conn_params (ConnectionParameters): conn_params
+            args:
+            kwargs:
+        """
         super(RPCClient, self).__init__(*args, **kwargs)
         self._transport = RedisTransport(conn_params=conn_params,
-                                         logger=self._logger)
+                                         serializer=self._serializer,
+                                         compression=self._compression)
 
     def _gen_queue_name(self):
         return f'rpc-{self._gen_random_id()}'
 
     def _prepare_request(self, data):
         self._comm_obj.header.timestamp = gen_timestamp()   #pylint: disable=E0237
         self._comm_obj.header.reply_to = self._gen_queue_name()
         self._comm_obj.data = data
-        return self._comm_obj.as_dict()
+        return self._comm_obj.dict()
 
     def call(self, msg: RPCMessage.Request,
              timeout: float = 30) -> RPCMessage.Response:
         ## TODO: Evaluate msg type passed here.
         if self._msg_type is None:
             data = msg
         else:
-            data = msg.as_dict()
+            data = msg.dict()
 
         _msg = self._prepare_request(data)
         _reply_to = _msg['header']['reply_to']
         self._transport.push_msg_to_queue(self._rpc_name, _msg)
         _, _msg = self._transport.wait_for_msg(_reply_to, timeout=timeout)
         self._transport.delete_queue(_reply_to)
         if _msg is None:
@@ -315,15 +315,16 @@
         """
         self._queue_size = queue_size
         self._msg_seq = 0
 
         super(Publisher, self).__init__(*args, **kwargs)
 
         self._transport = RedisTransport(conn_params=conn_params,
-                                         logger=self._logger)
+                                         serializer=self._serializer,
+                                         compression=self._compression)
 
     def publish(self, msg: PubSubMessage) -> None:
         """publish.
         Publish message
 
         Args:
             msg (PubSubMessage): msg
@@ -332,15 +333,15 @@
             None:
         """
         if self._msg_type is not None and not isinstance(msg, PubSubMessage):
             raise ValueError('Argument "msg" must be of type PubSubMessage')
         elif isinstance(msg, dict):
             data = msg
         elif isinstance(msg, PubSubMessage):
-            data = msg.as_dict()
+            data = msg.dict()
         self.logger.debug(f'Publishing Message to topic <{self._topic}>')
         self._transport.publish(self._topic, data)
         self._msg_seq += 1
 
     def _publish(self, data, topic) -> None:
         pass
 
@@ -370,15 +371,15 @@
             None:
         """
         if self._msg_type is not None and not isinstance(msg, PubSubMessage):
             raise ValueError('Argument "msg" must be of type PubSubMessage')
         elif isinstance(msg, dict):
             data = msg
         elif isinstance(msg, PubSubMessage):
-            data = msg.as_dict()
+            data = msg.dict()
         self.logger.debug(
             f'Publishing Message: <{topic}>:{data}')
         self._transport.publish(topic, data)
         self._msg_seq += 1
 
 
 class Subscriber(BaseSubscriber):
@@ -398,15 +399,16 @@
             args:
             kwargs:
         """
         self._queue_size = queue_size
         super(Subscriber, self).__init__(*args, **kwargs)
 
         self._transport = RedisTransport(conn_params=conn_params,
-                                         logger=self._logger)
+                                         serializer=self._serializer,
+                                         compression=self._compression)
 
     def run(self):
         self._subscriber_thread = self._transport.subscribe(self._topic,
                                                             self._on_message)
         self.logger.debug(f'Started Subscriber: <{self._topic}>')
 
     def stop(self):
@@ -476,15 +478,15 @@
         """__init__.
 
         Args:
             conn_params (ConnectionParameters): Broker Connection Parameters
             args: See BaseActionService class.
             kwargs:
         """
-        conn_params = UnixSocketConnectionParameters() if \
+        conn_params = ConnectionParameters() if \
             conn_params is None else conn_params
 
         super(ActionService, self).__init__(*args, **kwargs)
 
         self._goal_rpc = RPCService(msg_type=_ActionGoalMessage,
                                     rpc_name=self._goal_rpc_uri,
                                     conn_params=conn_params,
@@ -526,15 +528,15 @@
         """__init__.
 
         Args:
             conn_params (ConnectionParameters): Broker Connection Parameters
             args: See BaseActionClient class
             kwargs: See BaseActionClient class
         """
-        conn_params = UnixSocketConnectionParameters() if \
+        conn_params = gonnectionParameters() if \
             conn_params is None else conn_params
 
         super(ActionClient, self).__init__(*args, **kwargs)
 
         self._goal_client = RPCClient(msg_type=_ActionGoalMessage,
                                       rpc_name=self._goal_rpc_uri,
                                       conn_params=conn_params,
@@ -575,22 +577,21 @@
         Args:
             conn_params (ConnectionParameters): Broker Connection Parameters
             args: See BaseEventEmitter class
             kwargs: See BaseEventEmitter class
         """
         super(EventEmitter, self).__init__(*args, **kwargs)
 
-        self._transport = RedisTransport(conn_params=conn_params,
-                                         logger=self._logger)
+        self._transport = RedisTransport(conn_params=conn_params)
 
     def send_event(self, event: Event) -> None:
         """send_event.
 
         Args:
             event (Event): The Event to send.
 
         Returns:
             None:
         """
-        _msg = event.as_dict()
-        self.logger.debug(f'Firing Event: {event.name}:<{event.uri}>')
+        _msg = event.dict()
+        self.log.debug(f'Firing Event: {event.name}:<{event.uri}>')
         self._transport.publish(event.uri, _msg)
```

### Comparing `commlib-py-0.6.9/commlib/utils.py` & `commlib-py-0.8.0/commlib/utils.py`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/commlib_py.egg-info/PKG-INFO` & `commlib-py-0.8.0/commlib_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commlib-py
-Version: 0.6.9
+Version: 0.8.0
 Summary: Communication Lirary for Python implementing the most common communication patterns for CyberPhysical Systems.
 Home-page: https://github.com/robotics-4-all/commlib-py
 Author: Konstantinos Panayiotou
 Author-email: klpanagi@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `commlib-py-0.6.9/commlib_py.egg-info/SOURCES.txt` & `commlib-py-0.8.0/commlib_py.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 commlib/__init__.py
 commlib/action.py
+commlib/async_utils.py
 commlib/bridges.py
+commlib/compression.py
+commlib/connection.py
 commlib/endpoints.py
 commlib/events.py
 commlib/exceptions.py
 commlib/logger.py
 commlib/msg.py
 commlib/node.py
 commlib/pubsub.py
@@ -43,12 +46,11 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/usage.rst
 docs/images/ptopicbridge_example.png
-tests/.coverage
 tests/README.md
 tests/__init__.py
 tests/test_msgs.py
 tests/test_timer.py
```

### Comparing `commlib-py-0.6.9/docs/Makefile` & `commlib-py-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/docs/commlib.rst` & `commlib-py-0.8.0/docs/commlib.rst`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/docs/commlib.transports.rst` & `commlib-py-0.8.0/docs/commlib.transports.rst`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/docs/conf.py` & `commlib-py-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/docs/images/ptopicbridge_example.png` & `commlib-py-0.8.0/docs/images/ptopicbridge_example.png`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/docs/installation.rst` & `commlib-py-0.8.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/docs/make.bat` & `commlib-py-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/docs/usage.rst` & `commlib-py-0.8.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/setup.cfg` & `commlib-py-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/setup.py` & `commlib-py-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/tests/test_msgs.py` & `commlib-py-0.8.0/tests/test_msgs.py`

 * *Files identical despite different names*

### Comparing `commlib-py-0.6.9/tests/test_timer.py` & `commlib-py-0.8.0/tests/test_timer.py`

 * *Files identical despite different names*

