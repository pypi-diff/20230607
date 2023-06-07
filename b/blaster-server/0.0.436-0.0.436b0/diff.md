# Comparing `tmp/blaster-server-0.0.436.tar.gz` & `tmp/blaster-server-0.0.436b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.436.tar", last modified: Tue Jun  6 08:11:29 2023, max compression
+gzip compressed data, was "blaster-server-0.0.436b0.tar", last modified: Wed Jun  7 13:55:26 2023, max compression
```

## Comparing `blaster-server-0.0.436.tar` & `blaster-server-0.0.436b0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.436/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.436/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-06-06 08:11:29.895786 blaster-server-0.0.436/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.436/README.md
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.436/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.436/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/cloud/aws/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.436/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.436/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.436/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/connection_pool.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.436/blaster/env.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.436/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62732 2023-06-05 22:08:59.000000 blaster-server-0.0.436/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15845 2023-06-06 08:10:08.000000 blaster-server-0.0.436/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38854 2023-06-02 15:26:46.000000 blaster-server-0.0.436/blaster/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/tools/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46341 2023-06-05 22:16:59.000000 blaster-server-0.0.436/blaster/tools/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/utils/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/data/mime_types.json
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.436/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/fork.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/lat_long_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3966 2023-05-30 19:47:55.000000 blaster-server-0.0.436/blaster/utils/phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/websocket/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_app.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_core.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_exceptions.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_handshake.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_http.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_logging.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_socket.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_ssl_compat.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_url.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/_utils.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster/websocket/tests/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/tests/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.436/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/blaster_server.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-06-06 08:11:29.000000 blaster-server-0.0.436/blaster_server.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1726 2023-06-06 08:11:29.000000 blaster-server-0.0.436/blaster_server.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-06 08:11:29.000000 blaster-server-0.0.436/blaster_server.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-06-06 08:11:29.000000 blaster-server-0.0.436/blaster_server.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-06-06 08:11:29.000000 blaster-server-0.0.436/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/examples/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/fast_api_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/gevent_wsgi_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/meinheld_flask.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1743 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/simple_examples.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/test_chat_room.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/tornado_hello_world.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.436/examples/wheezy_hello.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-06-06 08:11:29.899786 blaster-server-0.0.436/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1530 2023-06-06 08:06:59.000000 blaster-server-0.0.436/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 08:11:29.895786 blaster-server-0.0.436/test/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.436/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.436/test/test_phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.436/test/test_schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5954 2023-06-05 22:21:25.000000 blaster-server-0.0.436/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.436/test/test_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.436/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.436b0/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.436b0/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/cloud/aws/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.436b0/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.436b0/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.436b0/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/connection_pool.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.436b0/blaster/env.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.436b0/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62732 2023-06-05 22:08:59.000000 blaster-server-0.0.436b0/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15679 2023-06-07 13:51:59.000000 blaster-server-0.0.436b0/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38804 2023-06-07 13:55:11.000000 blaster-server-0.0.436b0/blaster/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/tools/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46341 2023-06-05 22:16:59.000000 blaster-server-0.0.436b0/blaster/tools/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/utils/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/data/mime_types.json
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.436b0/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/fork.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/lat_long_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3953 2023-06-06 19:29:14.000000 blaster-server-0.0.436b0/blaster/utils/phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/websocket/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_app.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_core.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_exceptions.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_handshake.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_http.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_logging.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_socket.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_ssl_compat.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_url.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/_utils.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster/websocket/tests/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/tests/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/blaster_server.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-07 13:55:26.000000 blaster-server-0.0.436b0/blaster_server.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1726 2023-06-07 13:55:26.000000 blaster-server-0.0.436b0/blaster_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-07 13:55:26.000000 blaster-server-0.0.436b0/blaster_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-06-07 13:55:26.000000 blaster-server-0.0.436b0/blaster_server.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-06-07 13:55:26.000000 blaster-server-0.0.436b0/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/examples/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/fast_api_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/gevent_wsgi_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/meinheld_flask.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1743 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/simple_examples.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/test_chat_room.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/tornado_hello_world.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/examples/wheezy_hello.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1531 2023-06-07 13:52:37.000000 blaster-server-0.0.436b0/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-07 13:55:26.380857 blaster-server-0.0.436b0/test/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.436b0/test/test_phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.436b0/test/test_schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5954 2023-06-05 22:21:25.000000 blaster-server-0.0.436b0/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/test/test_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.436b0/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.436/LICENSE.txt` & `blaster-server-0.0.436b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/PKG-INFO` & `blaster-server-0.0.436b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.436
+Version: 0.0.436b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.436/README.md` & `blaster-server-0.0.436b0/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/__init__.py` & `blaster-server-0.0.436b0/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/cloud/analytics.py` & `blaster-server-0.0.436b0/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.436b0/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/cloud/push_tasks.py` & `blaster-server-0.0.436b0/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/cloud/storage.py` & `blaster-server-0.0.436b0/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/config.py` & `blaster-server-0.0.436b0/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/connection_pool.py` & `blaster-server-0.0.436b0/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/env.py` & `blaster-server-0.0.436b0/blaster/env.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/logging.py` & `blaster-server-0.0.436b0/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/mongo_orm.py` & `blaster-server-0.0.436b0/blaster/mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/schema.py` & `blaster-server-0.0.436b0/blaster/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,65 +350,50 @@
 	if(simple_types and isinstance(e, simple_types)):
 		valid = True
 	if(complex_validations):
 		for _complex_validation in complex_validations:
 			if(_complex_validation(e)):
 				valid = True
 				break
+	# if no validations are given are we good
+	if(not simple_types and not complex_validations):
+		valid = True
 
 	if(valid):
 		return e
 
 	if(nullable):
 		return None
 
 	raise TypeError("Cannot be none")
 
 
 def array_validation(_type, arr, simple_types=None, complex_validations=None, mix=False, nullable=True):
 	# sequece
 	if(arr == None):
 		if(_type._default != _OBJ_END_):
+			# None or copy of default
 			return list(_type._default) if _type._default != None else None
 		if(nullable):
 			return None
 		raise TypeError("Cannot be none")
+
 	if(not isinstance(arr, list)):
 		arr = json.loads(arr)
 
-	filter_nones = False
 	_prev_type = _OBJ_END_
 	for i in range(len(arr)):
-		valid = False
-		e = arr[i]
-		if(simple_types and isinstance(e, simple_types)):
-			valid = True
-		if(complex_validations):
-			for _complex_validation in complex_validations:
-				if(_complex_validation(e)):
-					valid = True
+		e = item_validation(arr[i], simple_types, complex_validations, nullable)
 		# check types should not mixed
 		if(not mix):  # single type, so check type matches with previous
 			_cur_type = type(e)
 			if(_prev_type == _OBJ_END_):
 				_prev_type = _cur_type
 			elif(_prev_type != _cur_type):
-				valid = False
-
-		if(not valid):
-			arr[i] = None
-			filter_nones = True
-
-	if(filter_nones and not nullable):  # null not allowed
-		n = len(arr)
-		i = n - 1
-		while(i >= 0):
-			if(arr[i] == None):
-				arr.pop(i)
-			i -= 1
+				raise TypeError(f"Array values should not be mixed types: {_prev_type} != {_cur_type}")
 
 	return arr
 
 
 # Array(str), Array((int, str), default=None), Array(Object), Array(Pet)
 # List[str, int]-> anyOf int, str
 # List[[str, int]] -> oneOf int, str
```

### Comparing `blaster-server-0.0.436/blaster/server.py` & `blaster-server-0.0.436b0/blaster/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1012,15 +1012,14 @@
 					path=request_path, wallclockms=int(1000 * time.time()) - cur_millis
 				)
 
 				return I_AM_HANDLING_THE_SOCKET
 
 			# resp.3.2 Send finalizing headers(content related only) and body
 			else:
-				# just a variable to track api type responses
 				if(isinstance(body, (dict, list))):
 					body = json.dumps(body)
 					buffered_socket.send(b'Content-Type: application/json\r\n')
 
 				# encode body
 				if(isinstance(body, str)):
 					body = body.encode()
```

### Comparing `blaster-server-0.0.436/blaster/tools/__init__.py` & `blaster-server-0.0.436b0/blaster/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/utils/data/countries.json` & `blaster-server-0.0.436b0/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/utils/data/mime_types.json` & `blaster-server-0.0.436b0/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/utils/data_utils.py` & `blaster-server-0.0.436b0/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/utils/events.py` & `blaster-server-0.0.436b0/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/utils/fork.py` & `blaster-server-0.0.436b0/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.436b0/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.436b0/blaster/utils/phone_number_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from .data_utils import COUNTRY_DATA
-from ..tools import ltrim
+
 
 NON_DIGITS = re.compile(r"[^0-9]")
 
-country_code_num_digits_map = {"93": [9], "358": [10], "355": [9], "213": [9], "1": [10], "374": [6], "297": [7], "61": [9], "672": [6], "43": [11], "994": [9], "973": [8], "880": [10], "375": [9], "32": [9], "501": [7], "229": [6, 7, 8, 9], "387": [8], "55": [11], "246": [7], "359": [9], "226": [8], "855": [9], "235": [8], "56": [9], "86": [11], "57": [10], "682": [5], "506": [8], "385": [9], "357": [8], "420": [9], "45": [8], "670": [8], "593": [9], "20": [10], "503": [7], "44": [10], "268": [8], "500": [5], "298": [5], "691": [7], "33": [9], "594": [9], "689": [6], "241": [7], "995": [9], "49": [10], "233": [9], "30": [10], "299": [6], "590": [12], "852": [8], "36": [9], "91": [10], "62": [10], "98": [10], "353": [9], "972": [9], "39": [10], "81": [11], "7": [10], "686": [5], "383": [8], "965": [8], "371": [8], "961": [8], "231": [8], "218": [10], "370": [8], "352": [9], "265": [7, 8, 9], "60": [7], "960": [7], "223": [8], "692": [7], "596": [12], "230": [8], "52": [10], "373": [8], "976": [8], "382": [8], "95": [10], "977": [10], "31": [9], "687": [6], "64": [8, 9, 10], "227": [8], "234": [8, 10], "254": [9], "255": [9], "683": [4], "90": [11], "47": [8], "968": [8], "92": [10], "680": [7], "970": [9], "507": [8], "51": [9], "63": [10], "48": [9], "351": [9], "974": [8], "262": [12], "290": [4], "966": [9], "381": [8], "65": [8], "421": [9], "677": [7], "252": [7, 8], "27": [9], "34": [9], "94": [7], "46": [7], "41": [9], "963": [9], "886": [9], "66": [9], "228": [8], "216": [8], "380": [9], "971": [9], "58": [7], "84": [9], "967": [9]}
+country_code_num_digits_map = {"93": [9], "358": [10], "355": [9], "213": [9], "1": [10], "374": [6], "297": [7], "61": [9], "672": [6], "43": [11], "994": [9], "973": [8], "880": [10], "375": [9], "32": [9], "501": [7], "229": [6, 7, 8, 9], "387": [8], "55": [11], "246": [7], "359": [9], "226": [8], "855": [9], "235": [8], "56": [9], "86": [11], "57": [10], "682": [5], "506": [8], "385": [9], "357": [8], "420": [9], "45": [8], "670": [8], "593": [9], "20": [10], "503": [7], "44": [10], "268": [8], "500": [5], "298": [5], "691": [7], "33": [9], "594": [9], "689": [6], "241": [7], "995": [9], "49": [10], "233": [9], "30": [10], "299": [6], "590": [12], "852": [8], "36": [9], "91": [10], "62": [10], "98": [10], "353": [9], "972": [9], "39": [10], "81": [11], "7": [10], "686": [5], "383": [8], "965": [8], "371": [8], "961": [8], "231": [8], "218": [10], "370": [8], "352": [9], "265": [7, 8, 9], "60": [7], "960": [7], "223": [8], "692": [7], "596": [12], "230": [8], "52": [10], "373": [8], "976": [8], "382": [8], "95": [10], "977": [10], "31": [9], "687": [6], "64": [8, 9, 10], "227": [8], "234": [8, 10], "254": [9], "255": [9], "256": [9], "683": [4], "90": [11], "47": [8], "968": [8], "92": [10], "680": [7], "970": [9], "507": [8], "51": [9], "63": [10], "48": [9], "351": [9], "974": [8], "262": [12], "290": [4], "966": [9], "381": [8], "65": [8], "421": [9], "677": [7], "252": [7, 8], "27": [9], "34": [9], "94": [7], "46": [7], "41": [9], "963": [9], "886": [9], "66": [9], "228": [8], "216": [8], "380": [9], "971": [9], "58": [7], "84": [9], "967": [9]}
 
 
 class SimpleTrie(dict):
 	end_obj = None
 
 
 country_code_num_digits_trie = SimpleTrie()
```

### Comparing `blaster-server-0.0.436/blaster/utils/xss_html.py` & `blaster-server-0.0.436b0/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/__init__.py` & `blaster-server-0.0.436b0/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/_abnf.py` & `blaster-server-0.0.436b0/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/_app.py` & `blaster-server-0.0.436b0/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/_core.py` & `blaster-server-0.0.436b0/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/_exceptions.py` & `blaster-server-0.0.436b0/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/_handshake.py` & `blaster-server-0.0.436b0/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/_http.py` & `blaster-server-0.0.436b0/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/_logging.py` & `blaster-server-0.0.436b0/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/_socket.py` & `blaster-server-0.0.436b0/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.436b0/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/_url.py` & `blaster-server-0.0.436b0/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/_utils.py` & `blaster-server-0.0.436b0/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/server.py` & `blaster-server-0.0.436b0/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.436b0/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.436b0/blaster_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.436
+Version: 0.0.436b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.436/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.436b0/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/examples/gevent_wsgi_test.py` & `blaster-server-0.0.436b0/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/examples/mongo_ormexample.py` & `blaster-server-0.0.436b0/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/examples/simple_examples.py` & `blaster-server-0.0.436b0/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/examples/test_chat_room.py` & `blaster-server-0.0.436b0/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/examples/tornado_hello_world.py` & `blaster-server-0.0.436b0/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/examples/wheezy_hello.py` & `blaster-server-0.0.436b0/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/setup.py` & `blaster-server-0.0.436b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.436',
+	version='0.0.436b',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.436/test/test_mongo_orm.py` & `blaster-server-0.0.436b0/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/test/test_phone_number_utils.py` & `blaster-server-0.0.436b0/test/test_phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/test/test_schema.py` & `blaster-server-0.0.436b0/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/test/test_tools.py` & `blaster-server-0.0.436b0/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/test/test_utils.py` & `blaster-server-0.0.436b0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.436/test/timeit_snippets.py` & `blaster-server-0.0.436b0/test/timeit_snippets.py`

 * *Files identical despite different names*

