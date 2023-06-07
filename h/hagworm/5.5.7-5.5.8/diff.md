# Comparing `tmp/hagworm-5.5.7.tar.gz` & `tmp/hagworm-5.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagworm-5.5.7.tar", last modified: Tue May 23 07:13:08 2023, max compression
+gzip compressed data, was "hagworm-5.5.8.tar", last modified: Wed Jun  7 06:19:53 2023, max compression
```

## Comparing `hagworm-5.5.7.tar` & `hagworm-5.5.8.tar`

### file list

```diff
@@ -1,91 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.216977 hagworm-5.5.7/
--rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.5.7/LICENSE
--rw-rw-rw-   0        0        0     7508 2023-05-23 07:13:08.216977 hagworm-5.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.5.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.117977 hagworm-5.5.7/c_extend/
--rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.5.7/c_extend/math.c
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.120977 hagworm-5.5.7/example/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.7/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.125977 hagworm-5.5.7/example/fastapi_demo/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.7/example/fastapi_demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.128977 hagworm-5.5.7/example/fastapi_demo/controller/
--rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.5.7/example/fastapi_demo/controller/__init__.py
--rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.5.7/example/fastapi_demo/controller/home.py
--rw-rw-rw-   0        0        0      888 2023-05-11 03:07:54.000000 hagworm-5.5.7/example/fastapi_demo/gunicorn.config.py
--rw-rw-rw-   0        0        0     1431 2023-05-17 08:11:13.000000 hagworm-5.5.7/example/fastapi_demo/main.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.130978 hagworm-5.5.7/example/fastapi_demo/model/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.7/example/fastapi_demo/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.131977 hagworm-5.5.7/example/fastapi_demo/service/
--rw-rw-rw-   0        0        0     3496 2023-05-22 00:30:47.000000 hagworm-5.5.7/example/fastapi_demo/service/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.5.7/example/fastapi_demo/setting.py
--rw-rw-rw-   0        0        0      800 2023-05-11 03:07:54.000000 hagworm-5.5.7/example/main_test.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.133978 hagworm-5.5.7/hagworm/
--rw-rw-rw-   0        0        0      495 2023-05-23 07:12:03.000000 hagworm-5.5.7/hagworm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.168976 hagworm-5.5.7/hagworm/extend/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.193976 hagworm-5.5.7/hagworm/extend/asyncio/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/asyncio/__init__.py
--rw-rw-rw-   0        0        0    16802 2023-05-07 00:52:16.000000 hagworm-5.5.7/hagworm/extend/asyncio/base.py
--rw-rw-rw-   0        0        0     4988 2023-05-07 00:52:16.000000 hagworm-5.5.7/hagworm/extend/asyncio/buffer.py
--rw-rw-rw-   0        0        0     2396 2023-05-11 03:07:54.000000 hagworm-5.5.7/hagworm/extend/asyncio/command.py
--rw-rw-rw-   0        0        0     3194 2023-05-07 00:52:16.000000 hagworm-5.5.7/hagworm/extend/asyncio/event.py
--rw-rw-rw-   0        0        0     1370 2023-05-07 00:52:16.000000 hagworm-5.5.7/hagworm/extend/asyncio/file.py
--rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/asyncio/future.py
--rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/asyncio/mail.py
--rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/asyncio/mongo.py
--rw-rw-rw-   0        0        0    15022 2023-05-07 00:52:16.000000 hagworm-5.5.7/hagworm/extend/asyncio/mysql.py
--rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/asyncio/net.py
--rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/asyncio/ntp.py
--rw-rw-rw-   0        0        0     1570 2023-05-20 02:55:55.000000 hagworm-5.5.7/hagworm/extend/asyncio/pool.py
--rw-rw-rw-   0        0        0    12507 2023-05-22 03:45:54.000000 hagworm-5.5.7/hagworm/extend/asyncio/redis.py
--rw-rw-rw-   0        0        0     7279 2023-05-11 03:07:54.000000 hagworm-5.5.7/hagworm/extend/asyncio/socket.py
--rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.5.7/hagworm/extend/asyncio/task.py
--rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/asyncio/transaction.py
--rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/asyncio/zmq.py
--rw-rw-rw-   0        0        0    22623 2023-05-11 03:07:54.000000 hagworm-5.5.7/hagworm/extend/base.py
--rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/cache.py
--rw-rw-rw-   0        0        0     1839 2023-05-07 00:52:16.000000 hagworm-5.5.7/hagworm/extend/compile.py
--rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/config.py
--rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/crypto.py
--rw-rw-rw-   0        0        0     1792 2023-05-07 00:52:16.000000 hagworm-5.5.7/hagworm/extend/error.py
--rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/event.py
--rw-rw-rw-   0        0        0     4558 2023-05-07 00:52:16.000000 hagworm-5.5.7/hagworm/extend/igraph.py
--rw-rw-rw-   0        0        0     2326 2023-05-07 00:52:16.000000 hagworm-5.5.7/hagworm/extend/interface.py
--rw-rw-rw-   0        0        0    14870 2023-05-13 05:06:56.000000 hagworm-5.5.7/hagworm/extend/logging.py
--rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/media.py
--rw-rw-rw-   0        0        0     1603 2023-05-10 07:58:09.000000 hagworm-5.5.7/hagworm/extend/metaclass.py
--rw-rw-rw-   0        0        0     4500 2023-05-11 03:07:54.000000 hagworm-5.5.7/hagworm/extend/process.py
--rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/qrcode.py
--rw-rw-rw-   0        0        0     7235 2023-05-07 00:52:16.000000 hagworm-5.5.7/hagworm/extend/struct.py
--rw-rw-rw-   0        0        0     3758 2023-05-07 00:52:16.000000 hagworm-5.5.7/hagworm/extend/text.py
--rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/trace.py
--rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/transaction.py
--rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/extend/validator.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.198978 hagworm-5.5.7/hagworm/frame/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/frame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.204977 hagworm-5.5.7/hagworm/frame/fastapi/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/frame/fastapi/__init__.py
--rw-rw-rw-   0        0        0     8148 2023-05-22 01:25:41.000000 hagworm-5.5.7/hagworm/frame/fastapi/base.py
--rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/frame/fastapi/field.py
--rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/frame/fastapi/model.py
--rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/frame/fastapi/response.py
--rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/frame/gunicorn.py
--rw-rw-rw-   0        0        0     3846 2023-05-11 03:07:54.000000 hagworm-5.5.7/hagworm/frame/stress_tests.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.207977 hagworm-5.5.7/hagworm/static/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/static/__init__.py
--rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/static/cacert.pem
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.209979 hagworm-5.5.7/hagworm/third/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/third/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.214977 hagworm-5.5.7/hagworm/third/rabbitmq/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.7/hagworm/third/rabbitmq/__init__.py
--rw-rw-rw-   0        0        0     3564 2023-05-07 00:52:16.000000 hagworm-5.5.7/hagworm/third/rabbitmq/consume.py
--rw-rw-rw-   0        0        0     5183 2023-05-20 03:08:12.000000 hagworm-5.5.7/hagworm/third/rabbitmq/publish.py
--rw-rw-rw-   0        0        0     5743 2023-05-20 02:53:42.000000 hagworm-5.5.7/hagworm/third/rabbitmq/rpc.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:13:08.140977 hagworm-5.5.7/hagworm.egg-info/
--rw-rw-rw-   0        0        0     7508 2023-05-23 07:13:08.000000 hagworm-5.5.7/hagworm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2100 2023-05-23 07:13:08.000000 hagworm-5.5.7/hagworm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 07:13:08.000000 hagworm-5.5.7/hagworm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      683 2023-05-23 07:13:08.000000 hagworm-5.5.7/hagworm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-23 07:13:08.000000 hagworm-5.5.7/hagworm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 07:13:08.216977 hagworm-5.5.7/setup.cfg
--rw-rw-rw-   0        0        0     2334 2023-05-23 07:10:41.000000 hagworm-5.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.595070 hagworm-5.5.8/
+-rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.5.8/LICENSE
+-rw-rw-rw-   0        0        0     7509 2023-06-07 06:19:53.595070 hagworm-5.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6066 2023-05-25 05:12:49.000000 hagworm-5.5.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.490038 hagworm-5.5.8/c_extend/
+-rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.5.8/c_extend/math.c
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.493039 hagworm-5.5.8/example/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.8/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.499040 hagworm-5.5.8/example/fastapi_demo/
+-rw-rw-rw-   0        0        0       61 2023-05-26 07:33:49.000000 hagworm-5.5.8/example/fastapi_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.502039 hagworm-5.5.8/example/fastapi_demo/controller/
+-rw-rw-rw-   0        0        0      223 2023-05-26 07:33:49.000000 hagworm-5.5.8/example/fastapi_demo/controller/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-05-26 07:33:49.000000 hagworm-5.5.8/example/fastapi_demo/controller/home.py
+-rw-rw-rw-   0        0        0      935 2023-05-26 07:33:49.000000 hagworm-5.5.8/example/fastapi_demo/gunicorn.config.py
+-rw-rw-rw-   0        0        0     1481 2023-05-26 07:33:49.000000 hagworm-5.5.8/example/fastapi_demo/main.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.503039 hagworm-5.5.8/example/fastapi_demo/model/
+-rw-rw-rw-   0        0        0       61 2023-05-26 07:33:49.000000 hagworm-5.5.8/example/fastapi_demo/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.505039 hagworm-5.5.8/example/fastapi_demo/service/
+-rw-rw-rw-   0        0        0     3616 2023-05-26 07:33:49.000000 hagworm-5.5.8/example/fastapi_demo/service/__init__.py
+-rw-rw-rw-   0        0        0     2165 2023-05-26 07:33:49.000000 hagworm-5.5.8/example/fastapi_demo/setting.py
+-rw-rw-rw-   0        0        0      800 2023-05-11 03:07:54.000000 hagworm-5.5.8/example/main_test.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.506039 hagworm-5.5.8/hagworm/
+-rw-rw-rw-   0        0        0      495 2023-05-27 06:02:31.000000 hagworm-5.5.8/hagworm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.542039 hagworm-5.5.8/hagworm/extend/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.568040 hagworm-5.5.8/hagworm/extend/asyncio/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    16802 2023-05-07 00:52:16.000000 hagworm-5.5.8/hagworm/extend/asyncio/base.py
+-rw-rw-rw-   0        0        0     4988 2023-05-07 00:52:16.000000 hagworm-5.5.8/hagworm/extend/asyncio/buffer.py
+-rw-rw-rw-   0        0        0     2066 2023-06-01 02:52:07.000000 hagworm-5.5.8/hagworm/extend/asyncio/command.py
+-rw-rw-rw-   0        0        0     3194 2023-05-07 00:52:16.000000 hagworm-5.5.8/hagworm/extend/asyncio/event.py
+-rw-rw-rw-   0        0        0     1370 2023-05-07 00:52:16.000000 hagworm-5.5.8/hagworm/extend/asyncio/file.py
+-rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/asyncio/future.py
+-rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/asyncio/mail.py
+-rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/asyncio/mongo.py
+-rw-rw-rw-   0        0        0    15022 2023-05-07 00:52:16.000000 hagworm-5.5.8/hagworm/extend/asyncio/mysql.py
+-rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/asyncio/net.py
+-rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/asyncio/ntp.py
+-rw-rw-rw-   0        0        0     1473 2023-05-31 02:11:58.000000 hagworm-5.5.8/hagworm/extend/asyncio/pool.py
+-rw-rw-rw-   0        0        0    12507 2023-05-22 03:45:54.000000 hagworm-5.5.8/hagworm/extend/asyncio/redis.py
+-rw-rw-rw-   0        0        0     6969 2023-06-01 05:16:27.000000 hagworm-5.5.8/hagworm/extend/asyncio/socket.py
+-rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.5.8/hagworm/extend/asyncio/task.py
+-rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/asyncio/transaction.py
+-rw-rw-rw-   0        0        0    23001 2023-05-31 02:03:45.000000 hagworm-5.5.8/hagworm/extend/base.py
+-rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/cache.py
+-rw-rw-rw-   0        0        0     1839 2023-05-07 00:52:16.000000 hagworm-5.5.8/hagworm/extend/compile.py
+-rw-rw-rw-   0        0        0     3855 2023-06-07 02:09:21.000000 hagworm-5.5.8/hagworm/extend/config.py
+-rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/crypto.py
+-rw-rw-rw-   0        0        0     1792 2023-05-07 00:52:16.000000 hagworm-5.5.8/hagworm/extend/error.py
+-rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/event.py
+-rw-rw-rw-   0        0        0     4558 2023-05-07 00:52:16.000000 hagworm-5.5.8/hagworm/extend/igraph.py
+-rw-rw-rw-   0        0        0     2326 2023-05-07 00:52:16.000000 hagworm-5.5.8/hagworm/extend/interface.py
+-rw-rw-rw-   0        0        0    15160 2023-06-05 06:16:53.000000 hagworm-5.5.8/hagworm/extend/logging.py
+-rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/media.py
+-rw-rw-rw-   0        0        0     1603 2023-05-10 07:58:09.000000 hagworm-5.5.8/hagworm/extend/metaclass.py
+-rw-rw-rw-   0        0        0     4181 2023-06-01 02:29:09.000000 hagworm-5.5.8/hagworm/extend/process.py
+-rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/qrcode.py
+-rw-rw-rw-   0        0        0     7235 2023-05-07 00:52:16.000000 hagworm-5.5.8/hagworm/extend/struct.py
+-rw-rw-rw-   0        0        0     3758 2023-05-07 00:52:16.000000 hagworm-5.5.8/hagworm/extend/text.py
+-rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/trace.py
+-rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/transaction.py
+-rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/extend/validator.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.572039 hagworm-5.5.8/hagworm/frame/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/frame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.579039 hagworm-5.5.8/hagworm/frame/fastapi/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/frame/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     7804 2023-06-01 02:38:54.000000 hagworm-5.5.8/hagworm/frame/fastapi/base.py
+-rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/frame/fastapi/field.py
+-rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/frame/fastapi/model.py
+-rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/frame/fastapi/response.py
+-rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/frame/gunicorn.py
+-rw-rw-rw-   0        0        0     3846 2023-05-11 03:07:54.000000 hagworm-5.5.8/hagworm/frame/stress_tests.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.582039 hagworm-5.5.8/hagworm/static/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/static/__init__.py
+-rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/static/cacert.pem
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.583040 hagworm-5.5.8/hagworm/third/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/third/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.587039 hagworm-5.5.8/hagworm/third/grpc/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/third/grpc/__init__.py
+-rw-rw-rw-   0        0        0     4362 2023-06-07 03:01:53.000000 hagworm-5.5.8/hagworm/third/grpc/client.py
+-rw-rw-rw-   0        0        0     3825 2023-06-06 11:05:09.000000 hagworm-5.5.8/hagworm/third/grpc/server.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.593041 hagworm-5.5.8/hagworm/third/rabbitmq/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.5.8/hagworm/third/rabbitmq/__init__.py
+-rw-rw-rw-   0        0        0     3564 2023-05-07 00:52:16.000000 hagworm-5.5.8/hagworm/third/rabbitmq/consume.py
+-rw-rw-rw-   0        0        0     5364 2023-05-30 10:37:07.000000 hagworm-5.5.8/hagworm/third/rabbitmq/publish.py
+-rw-rw-rw-   0        0        0     5743 2023-05-20 02:53:42.000000 hagworm-5.5.8/hagworm/third/rabbitmq/rpc.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:19:53.513039 hagworm-5.5.8/hagworm.egg-info/
+-rw-rw-rw-   0        0        0     7509 2023-06-07 06:19:53.000000 hagworm-5.5.8/hagworm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2159 2023-06-07 06:19:53.000000 hagworm-5.5.8/hagworm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 06:19:53.000000 hagworm-5.5.8/hagworm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      684 2023-06-07 06:19:53.000000 hagworm-5.5.8/hagworm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-07 06:19:53.000000 hagworm-5.5.8/hagworm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 06:19:53.596038 hagworm-5.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     2335 2023-06-07 05:44:16.000000 hagworm-5.5.8/setup.py
```

### Comparing `hagworm-5.5.7/LICENSE` & `hagworm-5.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/PKG-INFO` & `hagworm-5.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.5.7
+Version: 5.5.8
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
         
@@ -67,15 +67,15 @@
         │    │    ├── net.py                            网络工具
         │    │    ├── ntp.py                            时间同步
         │    │    ├── pool.py                           对象池抽象
         │    │    ├── redis.py                          Redis工具
         │    │    ├── socket.py                         Socket封装
         │    │    ├── task.py                           任务相关
         │    │    ├── transaction.py                    事务抽象
-        │    │    └── zmq.py                            ZMQ扩展
+        │    │    └── grpc.py                           grpc扩展
         │    ├── base.py                                基础工具
         │    ├── cache.py                               缓存相关
         │    ├── compile.py                             pyc编译
         │    ├── config.py                              配置相关
         │    ├── crypto.py                              加解密相关
         │    ├── error.py                               错误定义
         │    ├── event.py                               事件总线
```

### Comparing `hagworm-5.5.7/README.md` & `hagworm-5.5.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 │    │    ├── net.py                            网络工具
 │    │    ├── ntp.py                            时间同步
 │    │    ├── pool.py                           对象池抽象
 │    │    ├── redis.py                          Redis工具
 │    │    ├── socket.py                         Socket封装
 │    │    ├── task.py                           任务相关
 │    │    ├── transaction.py                    事务抽象
-│    │    └── zmq.py                            ZMQ扩展
+│    │    └── grpc.py                           grpc扩展
 │    ├── base.py                                基础工具
 │    ├── cache.py                               缓存相关
 │    ├── compile.py                             pyc编译
 │    ├── config.py                              配置相关
 │    ├── crypto.py                              加解密相关
 │    ├── error.py                               错误定义
 │    ├── event.py                               事件总线
```

### Comparing `hagworm-5.5.7/c_extend/math.c` & `hagworm-5.5.8/c_extend/math.c`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/example/fastapi_demo/service/__init__.py` & `hagworm-5.5.8/example/fastapi_demo/service/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-# -*- coding: utf-8 -*-
-
-__author__ = r'wsb310@gmail.com'
-
-from hagworm.extend.trace import get_trace_id
-from hagworm.extend.error import Ignore, catch_error
-from hagworm.extend.metaclass import Singleton
-from hagworm.extend.asyncio.base import Utils, FuncCache, ShareFuture, MultiTasks
-from hagworm.extend.asyncio.redis import RedisDelegate
-from hagworm.extend.asyncio.mongo import MongoDelegate
-from hagworm.extend.asyncio.mysql import MySQLDelegate
-from hagworm.extend.process import HeartbeatChecker
-
-from setting import ConfigStatic, ConfigDynamic
-
-
-class DataSource(Singleton, RedisDelegate, MongoDelegate, MySQLDelegate):
-
-    def __init__(self):
-
-        RedisDelegate.__init__(self)
-        MongoDelegate.__init__(self)
-        MySQLDelegate.__init__(self)
-
-        self._health_checker = HeartbeatChecker(ConfigDynamic.ServerName)
-
-    @classmethod
-    async def initialize(cls):
-
-        inst = cls()
-
-        (await inst.init_redis_single(
-            ConfigStatic.RedisHost[0], ConfigStatic.RedisHost[1], password=ConfigStatic.RedisPasswd,
-            min_connections=ConfigStatic.RedisMinConn, max_connections=ConfigStatic.RedisMaxConn
-        )).set_key_prefix(ConfigStatic.RedisKeyPrefix)
-
-        inst.init_mongo(
-            ConfigStatic.MongoHost, ConfigStatic.MongoUser, ConfigStatic.MongoPasswd,
-            auth_source=ConfigStatic.MongoAuth,
-            min_pool_size=ConfigStatic.MongoMinConn, max_pool_size=ConfigStatic.MongoMaxConn, max_idle_time=3600
-        )
-
-        if ConfigStatic.MySqlMasterServer:
-
-            await inst.init_mysql_rw(
-                ConfigStatic.MySqlMasterServer[0], ConfigStatic.MySqlMasterServer[1], ConfigStatic.MySqlName,
-                ConfigStatic.MySqlUser, ConfigStatic.MySqlPasswd,
-                minsize=ConfigStatic.MySqlMasterMinConn, maxsize=ConfigStatic.MySqlMasterMaxConn,
-                echo=ConfigDynamic.Debug, pool_recycle=21600, conn_life=43200
-            )
-
-        if ConfigStatic.MySqlSlaveServer:
-
-            await inst.init_mysql_ro(
-                ConfigStatic.MySqlSlaveServer[0], ConfigStatic.MySqlSlaveServer[1], ConfigStatic.MySqlName,
-                ConfigStatic.MySqlUser, ConfigStatic.MySqlPasswd,
-                minsize=ConfigStatic.MySqlSlaveMinConn, maxsize=ConfigStatic.MySqlSlaveMaxConn,
-                echo=ConfigDynamic.Debug, pool_recycle=21600, readonly=True, conn_life=43200
-            )
-
-    @classmethod
-    async def release(cls):
-
-        inst = cls()
-
-        inst._health_checker.release()
-
-        inst.close_mongo_pool()
-
-        await inst.async_close_redis()
-        await inst.close_mysql()
-
-    @classmethod
-    async def check_health(cls):
-
-        return await cls().health()
-
-    @property
-    def online(self):
-
-        return self._health_checker.check()
-
-    @ShareFuture()
-    @FuncCache(ttl=30)
-    async def health(self):
-
-        result = False
-
-        with catch_error():
-
-            tasks = MultiTasks()
-
-            tasks.append(self.redis_health())
-            tasks.append(self.mysql_health())
-            tasks.append(self.mongo_health())
-
-            await tasks
-
-            result = all(tasks)
-
-            if result is True:
-                self._health_checker.refresh()
-
-        return result
-
-
-class ServiceBase(Singleton, Utils):
-
-    def __init__(self):
-
-        self._data_source = DataSource()
-
-    @property
-    def trace_id(self):
-
-        return get_trace_id()
-
-    def Break(self, *args, layers=1):
-
-        raise Ignore(*args, layers=layers)
+# -*- coding: utf-8 -*-
+
+__author__ = r'wsb310@gmail.com'
+
+from hagworm.extend.trace import get_trace_id
+from hagworm.extend.error import Ignore, catch_error
+from hagworm.extend.metaclass import Singleton
+from hagworm.extend.asyncio.base import Utils, FuncCache, ShareFuture, MultiTasks
+from hagworm.extend.asyncio.redis import RedisDelegate
+from hagworm.extend.asyncio.mongo import MongoDelegate
+from hagworm.extend.asyncio.mysql import MySQLDelegate
+from hagworm.extend.process import HeartbeatChecker
+
+from setting import ConfigStatic, ConfigDynamic
+
+
+class DataSource(Singleton, RedisDelegate, MongoDelegate, MySQLDelegate):
+
+    def __init__(self):
+
+        RedisDelegate.__init__(self)
+        MongoDelegate.__init__(self)
+        MySQLDelegate.__init__(self)
+
+        self._health_checker = HeartbeatChecker(ConfigDynamic.ServerName)
+
+    @classmethod
+    async def initialize(cls):
+
+        inst = cls()
+
+        (await inst.init_redis_single(
+            ConfigStatic.RedisHost[0], ConfigStatic.RedisHost[1], password=ConfigStatic.RedisPasswd,
+            min_connections=ConfigStatic.RedisMinConn, max_connections=ConfigStatic.RedisMaxConn
+        )).set_key_prefix(ConfigStatic.RedisKeyPrefix)
+
+        inst.init_mongo(
+            ConfigStatic.MongoHost, ConfigStatic.MongoUser, ConfigStatic.MongoPasswd,
+            auth_source=ConfigStatic.MongoAuth,
+            min_pool_size=ConfigStatic.MongoMinConn, max_pool_size=ConfigStatic.MongoMaxConn, max_idle_time=3600
+        )
+
+        if ConfigStatic.MySqlMasterServer:
+
+            await inst.init_mysql_rw(
+                ConfigStatic.MySqlMasterServer[0], ConfigStatic.MySqlMasterServer[1], ConfigStatic.MySqlName,
+                ConfigStatic.MySqlUser, ConfigStatic.MySqlPasswd,
+                minsize=ConfigStatic.MySqlMasterMinConn, maxsize=ConfigStatic.MySqlMasterMaxConn,
+                echo=ConfigDynamic.Debug, pool_recycle=21600, conn_life=43200
+            )
+
+        if ConfigStatic.MySqlSlaveServer:
+
+            await inst.init_mysql_ro(
+                ConfigStatic.MySqlSlaveServer[0], ConfigStatic.MySqlSlaveServer[1], ConfigStatic.MySqlName,
+                ConfigStatic.MySqlUser, ConfigStatic.MySqlPasswd,
+                minsize=ConfigStatic.MySqlSlaveMinConn, maxsize=ConfigStatic.MySqlSlaveMaxConn,
+                echo=ConfigDynamic.Debug, pool_recycle=21600, readonly=True, conn_life=43200
+            )
+
+    @classmethod
+    async def release(cls):
+
+        inst = cls()
+
+        inst._health_checker.release()
+
+        inst.close_mongo_pool()
+
+        await inst.async_close_redis()
+        await inst.close_mysql()
+
+    @classmethod
+    async def check_health(cls):
+
+        return await cls().health()
+
+    @property
+    def online(self):
+
+        return self._health_checker.check()
+
+    @ShareFuture()
+    @FuncCache(ttl=30)
+    async def health(self):
+
+        result = False
+
+        with catch_error():
+
+            tasks = MultiTasks()
+
+            tasks.append(self.redis_health())
+            tasks.append(self.mysql_health())
+            tasks.append(self.mongo_health())
+
+            await tasks
+
+            result = all(tasks)
+
+            if result is True:
+                self._health_checker.refresh()
+
+        return result
+
+
+class ServiceBase(Singleton, Utils):
+
+    def __init__(self):
+
+        self._data_source = DataSource()
+
+    @property
+    def trace_id(self):
+
+        return get_trace_id()
+
+    def Break(self, *args, layers=1):
+
+        raise Ignore(*args, layers=layers)
```

### Comparing `hagworm-5.5.7/example/fastapi_demo/setting.py` & `hagworm-5.5.8/example/fastapi_demo/setting.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# -*- coding: utf-8 -*-
-
-__author__ = r'wsb310@gmail.com'
-
-from hagworm.extend.base import Utils
-from hagworm.extend.config import Configure, Field, HostType, StrListType
-
-
-class _Static(Configure):
-
-    MySqlMasterServer: HostType = Field(r'MySql')
-    MySqlSlaveServer: HostType = Field(r'MySql')
-    MySqlName: str = Field(r'MySql')
-    MySqlUser: str = Field(r'MySql')
-    MySqlPasswd: str = Field(r'MySql')
-    MySqlMasterMinConn: int = Field(r'MySql')
-    MySqlMasterMaxConn: int = Field(r'MySql')
-    MySqlSlaveMinConn: int = Field(r'MySql')
-    MySqlSlaveMaxConn: int = Field(r'MySql')
-
-    MongoHost: StrListType = Field(r'Mongo')
-    MongoAuth: str = Field(r'Mongo')
-    MongoUser: str = Field(r'Mongo')
-    MongoPasswd: str = Field(r'Mongo')
-    MongoMinConn: int = Field(r'Mongo')
-    MongoMaxConn: int = Field(r'Mongo')
-
-    RedisHost: HostType = Field(r'Redis')
-    RedisPasswd: str = Field(r'Redis')
-    RedisMinConn: int = Field(r'Redis')
-    RedisMaxConn: int = Field(r'Redis')
-    RedisExpire: int = Field(r'Redis')
-    RedisKeyPrefix: str = Field(r'Redis')
-
-
-class _Dynamic(Configure):
-
-    Port: int = Field(r'Base')
-    Debug: bool = Field(r'Base')
-    GZip: bool = Field(r'Base')
-    Secret: str = Field(r'Base')
-    ProcessNum: int = Field(r'Base')
-    ServerName: str = Field(r'Base')
-
-    AllowOrigins: StrListType = Field(r'Cros')
-    AllowMethods: StrListType = Field(r'Cros')
-    AllowHeaders: StrListType = Field(r'Cros')
-    AllowCredentials: bool = Field(r'Cros')
-
-    LogLevel: str = Field(r'Log')
-    LogFilePath: str = Field(r'Log')
-    LogFileSplitSize: int = Field(r'Log')
-    LogFileSplitTime: str = Field(r'Log')
-    LogFileBackups: int = Field(r'Log')
-
-    ThreadPoolMaxWorkers: int = Field(r'ThreadPool')
-
-
-ConfigStatic = _Static()
-ConfigDynamic = _Dynamic()
-
-cluster = Utils.getenv(r'CLUSTER', None)
-
-if cluster is None:
-    ConfigStatic.read(r'./config/static.conf')
-    ConfigDynamic.read(r'./config/dynamic.conf')
-else:
-    ConfigStatic.read(f'./config/static.{cluster.lower()}.conf')
-    ConfigDynamic.read(f'./config/dynamic.{cluster.lower()}.conf')
+# -*- coding: utf-8 -*-
+
+__author__ = r'wsb310@gmail.com'
+
+from hagworm.extend.base import Utils
+from hagworm.extend.config import Configure, Field, HostType, StrListType
+
+
+class _Static(Configure):
+
+    MySqlMasterServer: HostType = Field(r'MySql')
+    MySqlSlaveServer: HostType = Field(r'MySql')
+    MySqlName: str = Field(r'MySql')
+    MySqlUser: str = Field(r'MySql')
+    MySqlPasswd: str = Field(r'MySql')
+    MySqlMasterMinConn: int = Field(r'MySql')
+    MySqlMasterMaxConn: int = Field(r'MySql')
+    MySqlSlaveMinConn: int = Field(r'MySql')
+    MySqlSlaveMaxConn: int = Field(r'MySql')
+
+    MongoHost: StrListType = Field(r'Mongo')
+    MongoAuth: str = Field(r'Mongo')
+    MongoUser: str = Field(r'Mongo')
+    MongoPasswd: str = Field(r'Mongo')
+    MongoMinConn: int = Field(r'Mongo')
+    MongoMaxConn: int = Field(r'Mongo')
+
+    RedisHost: HostType = Field(r'Redis')
+    RedisPasswd: str = Field(r'Redis')
+    RedisMinConn: int = Field(r'Redis')
+    RedisMaxConn: int = Field(r'Redis')
+    RedisExpire: int = Field(r'Redis')
+    RedisKeyPrefix: str = Field(r'Redis')
+
+
+class _Dynamic(Configure):
+
+    Port: int = Field(r'Base')
+    Debug: bool = Field(r'Base')
+    GZip: bool = Field(r'Base')
+    Secret: str = Field(r'Base')
+    ProcessNum: int = Field(r'Base')
+    ServerName: str = Field(r'Base')
+
+    AllowOrigins: StrListType = Field(r'Cros')
+    AllowMethods: StrListType = Field(r'Cros')
+    AllowHeaders: StrListType = Field(r'Cros')
+    AllowCredentials: bool = Field(r'Cros')
+
+    LogLevel: str = Field(r'Log')
+    LogFilePath: str = Field(r'Log')
+    LogFileSplitSize: int = Field(r'Log')
+    LogFileSplitTime: str = Field(r'Log')
+    LogFileBackups: int = Field(r'Log')
+
+    ThreadPoolMaxWorkers: int = Field(r'ThreadPool')
+
+
+ConfigStatic = _Static()
+ConfigDynamic = _Dynamic()
+
+cluster = Utils.getenv(r'CLUSTER', None)
+
+if cluster is None:
+    ConfigStatic.read(r'./config/static.conf')
+    ConfigDynamic.read(r'./config/dynamic.conf')
+else:
+    ConfigStatic.read(f'./config/static.{cluster.lower()}.conf')
+    ConfigDynamic.read(f'./config/dynamic.{cluster.lower()}.conf')
```

### Comparing `hagworm-5.5.7/example/main_test.py` & `hagworm-5.5.8/example/main_test.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/base.py` & `hagworm-5.5.8/hagworm/extend/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/buffer.py` & `hagworm-5.5.8/hagworm/extend/asyncio/buffer.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/command.py` & `hagworm-5.5.8/hagworm/extend/asyncio/command.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,50 @@
 # -*- coding: utf-8 -*-
 
 __author__ = r'wsb310@gmail.com'
 
 from typing import Callable
 
-from ... import hagworm_slogan
-from ... import __version__ as hagworm_version
-
 from .base import install_uvloop, Utils
 from .socket import UnixSocketServer, UnixSocketClient, DEFAULT_LIMIT
 
 from ..interface import RunnableInterface
 from ..process import Daemon
 
 
 class MainProcessAbstract(Daemon):
 
     def __init__(
             self, target: Callable, sub_process_num: int, *,
-            keep_live: bool = False, set_affinity=None,
+            set_affinity=None, join_timeout: int = 10,
             unix_socket_path=r'/tmp/unix_socket_endpoint', unix_socket_limit=DEFAULT_LIMIT,
             **kwargs
     ):
 
-        self._socket_server = UnixSocketServer(self._client_connected_cb, unix_socket_path, unix_socket_limit)
-
         super().__init__(
-            target, sub_process_num, keep_live=keep_live, set_affinity=set_affinity,
+            target, sub_process_num, set_affinity=set_affinity, join_timeout=join_timeout,
             unix_socket_path=unix_socket_path,
             **kwargs
         )
 
+        self._socket_server = UnixSocketServer(self._client_connected_cb, unix_socket_path, unix_socket_limit)
+
     async def _client_connected_cb(self, reader, writer):
         raise NotImplementedError()
 
     async def _run(self):
 
         self._fill_process()
 
-        while self.is_active():
-            self._check_process()
+        while self._check_process():
             await Utils.sleep(1)
 
     def run(self):
 
-        environment = Utils.environment()
-
-        Utils.log.info(
-            f'{hagworm_slogan}'
-            f'hagworm {hagworm_version}\n'
-            f'python {environment["python"]}\n'
-            f'system {" ".join(environment["system"])}'
-        )
+        Utils.print_slogan()
 
         install_uvloop()
 
         Utils.run_until_complete(self._socket_server.open())
         Utils.run_until_complete(self._run())
         Utils.run_until_complete(self._socket_server.close())
```

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/event.py` & `hagworm-5.5.8/hagworm/extend/asyncio/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/file.py` & `hagworm-5.5.8/hagworm/extend/asyncio/file.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/future.py` & `hagworm-5.5.8/hagworm/extend/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/mail.py` & `hagworm-5.5.8/hagworm/extend/asyncio/mail.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/mongo.py` & `hagworm-5.5.8/hagworm/extend/asyncio/mongo.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/mysql.py` & `hagworm-5.5.8/hagworm/extend/asyncio/mysql.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/net.py` & `hagworm-5.5.8/hagworm/extend/asyncio/net.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/ntp.py` & `hagworm-5.5.8/hagworm/extend/asyncio/ntp.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/redis.py` & `hagworm-5.5.8/hagworm/extend/asyncio/redis.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/socket.py` & `hagworm-5.5.8/hagworm/extend/asyncio/socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,16 @@
 import socket
 import asyncio
 import base64
 import msgpack
 
 from typing import List
 
-from hagworm import hagworm_slogan
-from hagworm import __version__ as hagworm_version
-from hagworm.extend.asyncio.base import Utils, install_uvloop
-from hagworm.extend.interface import RunnableInterface
+from ...extend.asyncio.base import Utils, install_uvloop
+from ...extend.interface import RunnableInterface
 
 from ..error import RouterError
 
 
 DEFAULT_LIMIT = 0xffffff
 
 
@@ -240,26 +238,19 @@
                 client_connected_cb, address,
                 family, backlog, reuse_port, buffer_limit
             )
         )
 
     def run(self):
 
-        environment = Utils.environment()
-
-        Utils.log.info(
-            f'{hagworm_slogan}'
-            f'hagworm {hagworm_version}\n'
-            f'python {environment["python"]}\n'
-            f'system {" ".join(environment["system"])}'
-        )
+        Utils.print_slogan()
 
         install_uvloop()
 
-        asyncio.run(self._run())
+        Utils.run_until_complete(self._run())
 
     async def _run(self):
 
         if self._on_startup is not None:
             await self._on_startup()
 
         for config in self._listeners:
```

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/task.py` & `hagworm-5.5.8/hagworm/extend/asyncio/task.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/asyncio/transaction.py` & `hagworm-5.5.8/hagworm/extend/asyncio/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/base.py` & `hagworm-5.5.8/hagworm/extend/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 from cachetools import cached, TTLCache
 from zipfile import ZipFile, ZIP_DEFLATED
 
 from stdnum import luhn
 from dateutil.parser import parse as date_parse
 
 from .text import StrUtils
+from .. import hagworm_slogan
+from .. import __version__ as hagworm_version
 
 
 class Utils:
     """基础工具类
 
     集成常用的工具函数
 
@@ -97,14 +99,26 @@
 
         return {
             r'python': sys.version,
             r'system': [platform.system(), platform.release(), platform.version(), platform.machine()],
         }
 
     @classmethod
+    def print_slogan(cls):
+
+        environment = Utils.environment()
+
+        Utils.log.info(
+            f'{hagworm_slogan}'
+            f'hagworm {hagworm_version}\n'
+            f'python {environment["python"]}\n'
+            f'system {" ".join(environment["system"])}'
+        )
+
+    @classmethod
     def deprecation_warning(cls, val):
 
         warnings.warn(val, DeprecationWarning)
 
     @classmethod
     def get_node_id(cls):
```

### Comparing `hagworm-5.5.7/hagworm/extend/cache.py` & `hagworm-5.5.8/hagworm/extend/cache.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/compile.py` & `hagworm-5.5.8/hagworm/extend/compile.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/config.py` & `hagworm-5.5.8/hagworm/extend/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,18 +152,18 @@
             self._parser.add_section(section)
 
         for option, value in options.items():
             self._parser.set(section, option, value)
 
         self._load_options()
 
-    def read(self, files):
+    def read(self, path):
 
         self._parser.clear()
-        self._parser.read(files, r'utf-8')
+        self._parser.read(path, r'utf-8')
 
         self._load_options()
 
     def read_str(self, val):
 
         self._parser.clear()
         self._parser.read_string(val)
```

### Comparing `hagworm-5.5.7/hagworm/extend/crypto.py` & `hagworm-5.5.8/hagworm/extend/crypto.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/error.py` & `hagworm-5.5.8/hagworm/extend/error.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/event.py` & `hagworm-5.5.8/hagworm/extend/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/igraph.py` & `hagworm-5.5.8/hagworm/extend/igraph.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/interface.py` & `hagworm-5.5.8/hagworm/extend/interface.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/logging.py` & `hagworm-5.5.8/hagworm/extend/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,18 @@
                     if len(messages) < self._bulk_maxsize and (_idx + 1) < self._write_max_delay:
                         time.sleep(1)
                     else:
                         break
 
                 self._write_logs(messages)
 
+            except queue.Empty:
+
+                pass
+
             except Exception as err:
 
                 sys.stderr.write(f'{str(err)}\n')
 
             finally:
 
                 messages.clear()
@@ -220,17 +224,16 @@
         self._producer.flush()
 
 
 class ElasticsearchDataStreamUtil:
 
     def __init__(
             self, elasticsearch: Elasticsearch, stream_name: str, *,
-            rollover_max_age: str = r'1d', rollover_max_primary_shard_size: str = r'50gb',
-            delete_min_age: str = r'30d', refresh_interval: str = r'5s', number_of_replicas=0,
-            timestamp_order: str = r'desc'
+            rollover_max_age: str = r'1d', rollover_max_primary_shard_size: str = r'50gb', delete_min_age: str = r'30d',
+            refresh_interval: str = r'5s', number_of_replicas=0, timestamp_order: str = r'desc'
     ):
 
         self._elasticsearch = elasticsearch
 
         self._stream_name = stream_name
         self._policy_name = f'{stream_name}-ilm-policy'
 
@@ -384,26 +387,30 @@
 class ElasticsearchSink(_BaseSink):
     """Elasticsearch日志投递
     """
 
     def __init__(
             self, hosts, index, *,
             buffer_maxsize: int = 0xffff, bulk_maxsize: int = 0x800, write_max_delay: int = 5,
-            rollover_max_age: str = r'1d', rollover_max_primary_shard_size: str = r'50gb',
-            delete_min_age: str = r'30d',
+            rollover_max_age: str = r'1d', rollover_max_primary_shard_size: str = r'50gb', delete_min_age: str = r'30d',
+            refresh_interval: str = r'5s', number_of_replicas=0, timestamp_order: str = r'desc',
             **kwargs):
 
         super().__init__(buffer_maxsize, bulk_maxsize, write_max_delay)
 
         self._elasticsearch = Elasticsearch(hosts, **kwargs)
 
         ElasticsearchDataStreamUtil(
             self._elasticsearch, index,
-            rollover_max_age=rollover_max_age, rollover_max_primary_shard_size=rollover_max_primary_shard_size,
-            delete_min_age=delete_min_age
+            rollover_max_age=rollover_max_age,
+            rollover_max_primary_shard_size=rollover_max_primary_shard_size,
+            delete_min_age=delete_min_age,
+            refresh_interval=refresh_interval,
+            number_of_replicas=number_of_replicas,
+            timestamp_order=timestamp_order
         ).initialize()
 
         self._index = index
 
     def _write_logs(self, logs):
 
         es_helpers.bulk(
```

### Comparing `hagworm-5.5.7/hagworm/extend/media.py` & `hagworm-5.5.8/hagworm/extend/media.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/metaclass.py` & `hagworm-5.5.8/hagworm/extend/metaclass.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/process.py` & `hagworm-5.5.8/hagworm/extend/process.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,24 +27,23 @@
     return pid
 
 
 class Daemon(RunnableInterface):
 
     def __init__(
             self, target: Callable, sub_process_num: int, *,
-            keep_live: bool = False, set_affinity=None, join_timeout: int = 10, **kwargs
+            set_affinity=None, join_timeout: int = 10, **kwargs
     ):
 
         self._target = target
         self._kwargs = kwargs
 
         self._sub_process = set()
         self._sub_process_num = sub_process_num
 
-        self._keep_live = keep_live
         self._set_affinity = set_affinity
         self._join_timeout = join_timeout
 
         signal.signal(signal.SIGINT, self._kill_process)
         signal.signal(signal.SIGTERM, self._kill_process)
 
         if self._set_affinity:
@@ -56,25 +55,21 @@
 
             for _core in self._set_affinity:
                 if _core >= cpu_count:
                     raise Exception(f'cpu cores num {cpu_count}, cores {self._set_affinity}')
 
     def _kill_process(self, *_):
 
-        self._keep_live = False
-
         for process in self._sub_process:
             os.kill(process.ident, signal.SIGINT)
 
         for process in self._sub_process:
             process.join(self._join_timeout)
             process.kill()
 
-        sys.exit()
-
     def _fill_process(self):
 
         while len(self._sub_process) < self._sub_process_num:
 
             process = Process(target=self._target, kwargs=self._kwargs)
             process.start()
 
@@ -88,36 +83,29 @@
                 _cores = self._set_affinity[_idx: _idx + 1]
 
                 os.sched_setaffinity(_pid, _cores)
                 sys.stdout.write(f'process {_pid} affinity {os.sched_getaffinity(_pid)}\n')
 
     def _check_process(self):
 
-        removed = []
-
         for process in self._sub_process.copy():
 
-            if not process.is_alive():
-                removed.append(process)
-                self._sub_process.remove(process)
-
-        if len(removed) > 0 and self._keep_live is True:
-            sys.stderr.write(f'kill process {removed}\n')
-            self._fill_process()
+            if process.is_alive():
+                continue
 
-    def is_active(self):
+            self._sub_process.remove(process)
+            sys.stderr.write(f'kill process {process.ident}\n')
 
-        return self._keep_live or (len(self._sub_process) > 0)
+        return len(self._sub_process) > 0
 
     def run(self):
 
         self._fill_process()
 
-        while self.is_active():
-            self._check_process()
+        while self._check_process():
             time.sleep(1)
 
 
 class SharedByteArray(ByteArrayAbstract, ContextManager):
 
     def __init__(self, name=None, create=False, size=0):
```

### Comparing `hagworm-5.5.7/hagworm/extend/qrcode.py` & `hagworm-5.5.8/hagworm/extend/qrcode.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/struct.py` & `hagworm-5.5.8/hagworm/extend/struct.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/text.py` & `hagworm-5.5.8/hagworm/extend/text.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/trace.py` & `hagworm-5.5.8/hagworm/extend/trace.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/transaction.py` & `hagworm-5.5.8/hagworm/extend/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/extend/validator.py` & `hagworm-5.5.8/hagworm/extend/validator.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/frame/fastapi/base.py` & `hagworm-5.5.8/hagworm/frame/fastapi/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 import os
 import time
 import fastapi
 
 from starlette.types import ASGIApp, Receive, Scope, Send
 from starlette.status import HTTP_400_BAD_REQUEST
 from starlette.exceptions import HTTPException
-from starlette.routing import iscoroutinefunction_or_partial
+from starlette.routing import is_async_callable
 from starlette.concurrency import run_in_threadpool
 
-from fastapi import __version__ as fastapi_version
 from fastapi.encoders import jsonable_encoder
 from fastapi.exceptions import RequestValidationError
 from fastapi.openapi.docs import get_swagger_ui_html
 
-from ... import hagworm_label, hagworm_slogan
+from ... import hagworm_label
 from ... import __version__ as hagworm_version
 
 from ...extend.trace import get_trace_id, refresh_trace_id
 from ...extend.asyncio.base import Utils, install_uvloop
 from ...extend.logging import DEFAULT_LOG_FILE_NAME, DEFAULT_LOG_FILE_ROTATOR, init_logger
 
 from .response import Response, ErrorResponse
@@ -54,23 +53,15 @@
         file_rotation=log_file_rotation,
         file_retention=log_file_retention,
         extra=log_extra,
         enqueue=log_enqueue,
         debug=debug
     )
 
-    environment = Utils.environment()
-
-    Utils.log.info(
-        f'{hagworm_slogan}'
-        f'hagworm {hagworm_version}\n'
-        f'fastapi {fastapi_version}\n'
-        f'python {environment["python"]}\n'
-        f'system {" ".join(environment["system"])}'
-    )
+    Utils.print_slogan()
 
     setting.setdefault(r'title', r'Hagworm')
     setting.setdefault(r'version', hagworm_version)
 
     install_uvloop()
 
     _fastapi = fastapi.FastAPI(debug=debug, routes=routes, **setting)
@@ -93,15 +84,15 @@
 
         pass
 
     def request_response(self) -> ASGIApp:
 
         func = self.get_route_handler()
 
-        is_coroutine = iscoroutinefunction_or_partial(func)
+        is_coroutine = is_async_callable(func)
 
         async def app(scope: Scope, receive: Receive, send: Send) -> None:
 
             request = Request(scope, receive, send, self)
 
             try:
```

### Comparing `hagworm-5.5.7/hagworm/frame/fastapi/field.py` & `hagworm-5.5.8/hagworm/frame/fastapi/field.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/frame/fastapi/model.py` & `hagworm-5.5.8/hagworm/frame/fastapi/model.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/frame/fastapi/response.py` & `hagworm-5.5.8/hagworm/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/frame/gunicorn.py` & `hagworm-5.5.8/hagworm/frame/gunicorn.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/frame/stress_tests.py` & `hagworm-5.5.8/hagworm/frame/stress_tests.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/static/cacert.pem` & `hagworm-5.5.8/hagworm/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/third/rabbitmq/consume.py` & `hagworm-5.5.8/hagworm/third/rabbitmq/consume.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm/third/rabbitmq/publish.py` & `hagworm-5.5.8/hagworm/third/rabbitmq/publish.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-# -*- coding: utf-8 -*-
-
-__author__ = r'wsb310@gmail.com'
-
-import asyncio
-import aio_pika
-
-from typing import List
-
-from ...extend.base import Utils
-from ...extend.asyncio.pool import ObjectPool
-
-
-class RabbitMQProducer(aio_pika.RobustConnection):
-    """RabbitMQ发布者
-    """
-
-    def __init__(self, url, **kwargs):
-
-        super().__init__(url, **kwargs)
-
-        self._channel: aio_pika.abc.AbstractRobustChannel = None
-
-        self._lock: asyncio.Lock = asyncio.Lock()
-
-    @property
-    def current_channel(self) -> aio_pika.abc.AbstractRobustChannel:
-
-        return self._channel
-
-    async def connect(
-            self, *,
-            channel_number: int = None, publisher_confirms: bool = True, on_return_raises: bool = False,
-            timeout: aio_pika.abc.TimeoutType = None
-    ):
-
-        await super().connect(timeout)
-
-        await self.ready()
-
-        if self._channel is None:
-            self._channel = await self.channel(channel_number, publisher_confirms, on_return_raises)
-
-    async def close(self):
-
-        await self._channel.close()
-        await super().close()
-
-    async def publish(self, message, routing_key, **kwargs):
-
-        async with self._lock:
-            return await self._channel.default_exchange.publish(
-                message if isinstance(message, aio_pika.Message) else aio_pika.Message(message),
-                routing_key, **kwargs
-            )
-
-
-class RabbitMQProducerForExchange(RabbitMQProducer):
-    """RabbitMQ交换机发布者
-    """
-
-    def __init__(self, url, **kwargs):
-
-        super().__init__(url, **kwargs)
-
-        self._exchange: aio_pika.abc.AbstractExchange = None
-
-        self._exchange_name = None
-        self._exchange_type = None
-        self._exchange_config = None
-
-    @property
-    def current_exchange(self) -> aio_pika.abc.AbstractExchange:
-
-        return self._exchange
-
-    def config(
-            self, exchange_name, exchange_type=aio_pika.ExchangeType.FANOUT,
-            *, exchange_config=None
-    ):
-
-        self._exchange_name = exchange_name
-        self._exchange_type = exchange_type
-        self._exchange_config = exchange_config if exchange_config else {}
-
-    async def connect(
-            self, *,
-            channel_number: int = None, publisher_confirms: bool = True, on_return_raises: bool = False,
-            timeout: aio_pika.abc.TimeoutType = None
-    ):
-
-        await super().connect(
-            channel_number=channel_number,
-            publisher_confirms=publisher_confirms,
-            on_return_raises=on_return_raises,
-            timeout=timeout
-        )
-
-        if self._exchange is None:
-            self._exchange = await self._channel.declare_exchange(
-                self._exchange_name, self._exchange_type, **self._exchange_config
-            )
-
-    async def publish(self, message, routing_key=r'', **kwargs):
-
-        async with self._lock:
-            return await self._exchange.publish(
-                message if isinstance(message, aio_pika.Message) else aio_pika.Message(message),
-                routing_key, **kwargs
-            )
-
-
-class RabbitMQProducerPool(ObjectPool):
-    """RabbitMQ发布者连接池
-    """
-
-    def __init__(self, url, pool_size, *, connection_config=None):
-
-        self._mq_url = url
-
-        self._connection_config = connection_config if connection_config else {}
-
-        super().__init__(pool_size)
-
-    async def _create_obj(self):
-
-        connection = RabbitMQProducer(self._mq_url, **self._connection_config)
-
-        return connection
-
-    async def _delete_obj(self, obj):
-
-        await obj.close()
-
-    async def connect(
-            self, *,
-            publisher_confirms: bool = True, on_return_raises: bool = False,
-            timeout: aio_pika.abc.TimeoutType = None
-    ):
-
-        await self.open()
-
-        for _ in range(self._queue.qsize()):
-
-            with self.get_nowait() as connection:
-                await connection.connect(
-                    publisher_confirms=publisher_confirms,
-                    on_return_raises=on_return_raises,
-                    timeout=timeout,
-                )
-
-    async def publish(self, message, routing_key=r'', **kwargs):
-
-        async with self.get() as connection:
-            return await connection.publish(
-                message if isinstance(message, aio_pika.Message) else aio_pika.Message(message),
-                routing_key, **kwargs
-            )
-
-
-class RabbitMQProducerForExchangePool(RabbitMQProducerPool):
-    """RabbitMQ交换机发布者连接池
-    """
-
-    def __init__(
-            self, url, pool_size, exchange_name,
-            *, exchange_type=aio_pika.ExchangeType.FANOUT, exchange_config=None, connection_config=None
-    ):
-
-        self._exchange_name = exchange_name
-        self._exchange_type = exchange_type
-        self._exchange_config = exchange_config
-
-        super().__init__(url, pool_size, connection_config=connection_config)
-
-    async def _create_obj(self):
-
-        connection = RabbitMQProducerForExchange(self._mq_url, **self._connection_config)
-        connection.config(self._exchange_name, self._exchange_type, exchange_config=self._exchange_config)
-
-        return connection
+# -*- coding: utf-8 -*-
+
+__author__ = r'wsb310@gmail.com'
+
+import asyncio
+import aio_pika
+
+from typing import List
+
+from ...extend.base import Utils
+from ...extend.asyncio.pool import ObjectPool
+
+
+class RabbitMQProducer(aio_pika.RobustConnection):
+    """RabbitMQ发布者
+    """
+
+    def __init__(self, url, **kwargs):
+
+        super().__init__(url, **kwargs)
+
+        self._channel: aio_pika.abc.AbstractRobustChannel = None
+
+        self._lock: asyncio.Lock = asyncio.Lock()
+
+    @property
+    def current_channel(self) -> aio_pika.abc.AbstractRobustChannel:
+
+        return self._channel
+
+    async def connect(
+            self, *,
+            channel_number: int = None, publisher_confirms: bool = True, on_return_raises: bool = False,
+            timeout: aio_pika.abc.TimeoutType = None
+    ):
+
+        await super().connect(timeout)
+
+        await self.ready()
+
+        if self._channel is None:
+            self._channel = await self.channel(channel_number, publisher_confirms, on_return_raises)
+
+    async def close(self):
+
+        await self._channel.close()
+        await super().close()
+
+    async def publish(self, message, routing_key, **kwargs):
+
+        async with self._lock:
+            return await self._channel.default_exchange.publish(
+                message if isinstance(message, aio_pika.Message) else aio_pika.Message(message),
+                routing_key, **kwargs
+            )
+
+
+class RabbitMQProducerForExchange(RabbitMQProducer):
+    """RabbitMQ交换机发布者
+    """
+
+    def __init__(self, url, **kwargs):
+
+        super().__init__(url, **kwargs)
+
+        self._exchange: aio_pika.abc.AbstractExchange = None
+
+        self._exchange_name = None
+        self._exchange_type = None
+        self._exchange_config = None
+
+    @property
+    def current_exchange(self) -> aio_pika.abc.AbstractExchange:
+
+        return self._exchange
+
+    def config(
+            self, exchange_name, exchange_type=aio_pika.ExchangeType.FANOUT,
+            *, exchange_config=None
+    ):
+
+        self._exchange_name = exchange_name
+        self._exchange_type = exchange_type
+        self._exchange_config = exchange_config if exchange_config else {}
+
+    async def connect(
+            self, *,
+            channel_number: int = None, publisher_confirms: bool = True, on_return_raises: bool = False,
+            timeout: aio_pika.abc.TimeoutType = None
+    ):
+
+        await super().connect(
+            channel_number=channel_number,
+            publisher_confirms=publisher_confirms,
+            on_return_raises=on_return_raises,
+            timeout=timeout
+        )
+
+        if self._exchange is None:
+            self._exchange = await self._channel.declare_exchange(
+                self._exchange_name, self._exchange_type, **self._exchange_config
+            )
+
+    async def publish(self, message, routing_key=r'', **kwargs):
+
+        async with self._lock:
+            return await self._exchange.publish(
+                message if isinstance(message, aio_pika.Message) else aio_pika.Message(message),
+                routing_key, **kwargs
+            )
+
+
+class RabbitMQProducerPool(ObjectPool):
+    """RabbitMQ发布者连接池
+    """
+
+    def __init__(self, url, pool_size, *, connection_config=None):
+
+        self._mq_url = url
+
+        self._connection_config = connection_config if connection_config else {}
+
+        super().__init__(pool_size)
+
+    async def _create_obj(self):
+
+        connection = RabbitMQProducer(self._mq_url, **self._connection_config)
+
+        return connection
+
+    async def _delete_obj(self, obj):
+
+        await obj.close()
+
+    async def connect(
+            self, *,
+            publisher_confirms: bool = True, on_return_raises: bool = False,
+            timeout: aio_pika.abc.TimeoutType = None
+    ):
+
+        await self.open()
+
+        for _ in range(self._queue.qsize()):
+
+            with self.get_nowait() as connection:
+                await connection.connect(
+                    publisher_confirms=publisher_confirms,
+                    on_return_raises=on_return_raises,
+                    timeout=timeout,
+                )
+
+    async def publish(self, message, routing_key=r'', **kwargs):
+
+        async with self.get() as connection:
+            return await connection.publish(
+                message if isinstance(message, aio_pika.Message) else aio_pika.Message(message),
+                routing_key, **kwargs
+            )
+
+
+class RabbitMQProducerForExchangePool(RabbitMQProducerPool):
+    """RabbitMQ交换机发布者连接池
+    """
+
+    def __init__(
+            self, url, pool_size, exchange_name,
+            *, exchange_type=aio_pika.ExchangeType.FANOUT, exchange_config=None, connection_config=None
+    ):
+
+        self._exchange_name = exchange_name
+        self._exchange_type = exchange_type
+        self._exchange_config = exchange_config
+
+        super().__init__(url, pool_size, connection_config=connection_config)
+
+    async def _create_obj(self):
+
+        connection = RabbitMQProducerForExchange(self._mq_url, **self._connection_config)
+        connection.config(self._exchange_name, self._exchange_type, exchange_config=self._exchange_config)
+
+        return connection
```

### Comparing `hagworm-5.5.7/hagworm/third/rabbitmq/rpc.py` & `hagworm-5.5.8/hagworm/third/rabbitmq/rpc.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.5.7/hagworm.egg-info/PKG-INFO` & `hagworm-5.5.8/hagworm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.5.7
+Version: 5.5.8
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
         
@@ -67,15 +67,15 @@
         │    │    ├── net.py                            网络工具
         │    │    ├── ntp.py                            时间同步
         │    │    ├── pool.py                           对象池抽象
         │    │    ├── redis.py                          Redis工具
         │    │    ├── socket.py                         Socket封装
         │    │    ├── task.py                           任务相关
         │    │    ├── transaction.py                    事务抽象
-        │    │    └── zmq.py                            ZMQ扩展
+        │    │    └── grpc.py                           grpc扩展
         │    ├── base.py                                基础工具
         │    ├── cache.py                               缓存相关
         │    ├── compile.py                             pyc编译
         │    ├── config.py                              配置相关
         │    ├── crypto.py                              加解密相关
         │    ├── error.py                               错误定义
         │    ├── event.py                               事件总线
```

### Comparing `hagworm-5.5.7/hagworm.egg-info/SOURCES.txt` & `hagworm-5.5.8/hagworm.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -51,23 +51,25 @@
 hagworm/extend/asyncio/net.py
 hagworm/extend/asyncio/ntp.py
 hagworm/extend/asyncio/pool.py
 hagworm/extend/asyncio/redis.py
 hagworm/extend/asyncio/socket.py
 hagworm/extend/asyncio/task.py
 hagworm/extend/asyncio/transaction.py
-hagworm/extend/asyncio/zmq.py
 hagworm/frame/__init__.py
 hagworm/frame/gunicorn.py
 hagworm/frame/stress_tests.py
 hagworm/frame/fastapi/__init__.py
 hagworm/frame/fastapi/base.py
 hagworm/frame/fastapi/field.py
 hagworm/frame/fastapi/model.py
 hagworm/frame/fastapi/response.py
 hagworm/static/__init__.py
 hagworm/static/cacert.pem
 hagworm/third/__init__.py
+hagworm/third/grpc/__init__.py
+hagworm/third/grpc/client.py
+hagworm/third/grpc/server.py
 hagworm/third/rabbitmq/__init__.py
 hagworm/third/rabbitmq/consume.py
 hagworm/third/rabbitmq/publish.py
 hagworm/third/rabbitmq/rpc.py
```

### Comparing `hagworm-5.5.7/setup.py` & `hagworm-5.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,29 +41,29 @@
         r'cachetools==5.3.0',
         r'confluent-kafka==2.1.1',
         r'cryptography==40.0.2',
         r'elasticsearch==8.1.1',
         r'fastapi==0.95.2',
         r'fastapi-health==0.4.0',
         r'gunicorn==20.1.0',
+        r'grpcio==1.54.2',
         r'hiredis==2.2.3',
         r'httptools==0.5.0',
         r'igraph==0.10.4',
         r'loguru==0.7.0',
         r'motor==3.1.2',
         r'msgpack==1.0.5',
         r'ntplib==0.4.0',
         r'numpy==1.24.3',
         r'psutil==5.9.5',
         r'pyahocorasick==2.0.0',
         r'pytest-asyncio==0.21.0',
         r'python-dateutil==2.8.2',
         r'python-stdnum==1.18',
         r'python-multipart==0.0.6',
-        r'pyzmq==25.0.2',
         r'qrcode==7.4.2',
         r'texttable==1.6.7',
         r'ujson==5.7.0',
         r'uvicorn[standard]==0.22.0',
         r'uvloop==0.17.0;sys_platform!="win32"',
         r'xmltodict==0.13.0',
     ],
```

