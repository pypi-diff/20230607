# Comparing `tmp/zoo-framework-0.4.1.tar.gz` & `tmp/zoo-framework-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoo-framework-0.4.1.tar", last modified: Mon May  2 03:39:31 2022, max compression
+gzip compressed data, was "zoo-framework-0.4.2.tar", last modified: Wed Jun  7 13:37:19 2023, max compression
```

## Comparing `zoo-framework-0.4.1.tar` & `zoo-framework-0.4.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.343997 zoo-framework-0.4.1/
--rw-rw-rw-   0        0        0       33 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1445 2022-05-02 03:39:31.343342 zoo-framework-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      464 2021-11-22 22:45:06.000000 zoo-framework-0.4.1/README.md
--rw-rw-rw-   0        0        0       42 2022-05-02 03:39:31.344342 zoo-framework-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1243 2022-05-02 03:34:03.000000 zoo-framework-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.281339 zoo-framework-0.4.1/zoo_framework/
--rw-rw-rw-   0        0        0      159 2021-11-12 12:12:40.000000 zoo-framework-0.4.1/zoo_framework/__init__.py
--rw-rw-rw-   0        0        0     3012 2021-12-29 09:23:30.000000 zoo-framework-0.4.1/zoo_framework/__main__.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.294003 zoo-framework-0.4.1/zoo_framework/conf/
--rw-rw-rw-   0        0        0       36 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/conf/__init__.py
--rw-rw-rw-   0        0        0     1458 2021-11-20 03:16:31.000000 zoo-framework-0.4.1/zoo_framework/conf/log_config.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.297014 zoo-framework-0.4.1/zoo_framework/constant/
--rw-rw-rw-   0        0        0       88 2021-12-19 11:14:52.000000 zoo-framework-0.4.1/zoo_framework/constant/__init__.py
--rw-rw-rw-   0        0        0      185 2021-12-19 11:14:52.000000 zoo-framework-0.4.1/zoo_framework/constant/waiter_constant.py
--rw-rw-rw-   0        0        0      500 2021-12-19 11:14:52.000000 zoo-framework-0.4.1/zoo_framework/constant/worker_constant.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.301547 zoo-framework-0.4.1/zoo_framework/core/
--rw-rw-rw-   0        0        0      240 2021-11-18 12:24:23.000000 zoo-framework-0.4.1/zoo_framework/core/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.307555 zoo-framework-0.4.1/zoo_framework/core/aop/
--rw-rw-rw-   0        0        0      274 2021-11-22 23:02:32.000000 zoo-framework-0.4.1/zoo_framework/core/aop/__init__.py
--rw-rw-rw-   0        0        0      195 2021-11-22 23:47:41.000000 zoo-framework-0.4.1/zoo_framework/core/aop/cage.py
--rw-rw-rw-   0        0        0      150 2021-11-08 13:45:38.000000 zoo-framework-0.4.1/zoo_framework/core/aop/configure.py
--rw-rw-rw-   0        0        0      280 2022-05-02 03:34:03.000000 zoo-framework-0.4.1/zoo_framework/core/aop/event.py
--rw-rw-rw-   0        0        0      767 2021-11-08 13:47:50.000000 zoo-framework-0.4.1/zoo_framework/core/aop/params.py
--rw-rw-rw-   0        0        0      602 2021-11-22 23:04:13.000000 zoo-framework-0.4.1/zoo_framework/core/aop/validation.py
--rw-rw-rw-   0        0        0      344 2021-11-18 12:24:23.000000 zoo-framework-0.4.1/zoo_framework/core/aop/worker.py
--rw-rw-rw-   0        0        0     1537 2022-05-02 03:34:03.000000 zoo-framework-0.4.1/zoo_framework/core/master.py
--rw-rw-rw-   0        0        0      274 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/core/meta_singleton.py
--rw-rw-rw-   0        0        0     1635 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/core/params_factory.py
--rw-rw-rw-   0        0        0      237 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/core/params_path.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.312423 zoo-framework-0.4.1/zoo_framework/core/waiter/
--rw-rw-rw-   0        0        0      201 2021-11-20 03:16:31.000000 zoo-framework-0.4.1/zoo_framework/core/waiter/__init__.py
--rw-rw-rw-   0        0        0     5202 2021-12-30 05:39:51.000000 zoo-framework-0.4.1/zoo_framework/core/waiter/base_waiter.py
--rw-rw-rw-   0        0        0     1521 2021-12-19 11:14:52.000000 zoo-framework-0.4.1/zoo_framework/core/waiter/safe_waiter.py
--rw-rw-rw-   0        0        0      401 2021-12-19 11:14:52.000000 zoo-framework-0.4.1/zoo_framework/core/waiter/simple_waiter.py
--rw-rw-rw-   0        0        0      254 2021-12-19 11:14:52.000000 zoo-framework-0.4.1/zoo_framework/core/waiter/stable_waiter.py
--rw-rw-rw-   0        0        0      496 2021-11-20 03:16:31.000000 zoo-framework-0.4.1/zoo_framework/core/waiter/waiter_factory.py
--rw-rw-rw-   0        0        0     1164 2021-12-25 10:08:58.000000 zoo-framework-0.4.1/zoo_framework/core/zoo_thread.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.316422 zoo-framework-0.4.1/zoo_framework/fifo/
--rw-rw-rw-   0        0        0      105 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/fifo/__init__.py
--rw-rw-rw-   0        0        0      603 2022-05-02 03:34:03.000000 zoo-framework-0.4.1/zoo_framework/fifo/base_fifo.py
--rw-rw-rw-   0        0        0       47 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/fifo/delay_fifo.py
--rw-rw-rw-   0        0        0      650 2022-05-02 03:34:03.000000 zoo-framework-0.4.1/zoo_framework/fifo/event_fifo.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.318422 zoo-framework-0.4.1/zoo_framework/fifo/node/
--rw-rw-rw-   0        0        0       86 2022-05-02 03:34:03.000000 zoo-framework-0.4.1/zoo_framework/fifo/node/__init__.py
--rw-rw-rw-   0        0        0      250 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/fifo/node/delay_fifo_node.py
--rw-rw-rw-   0        0        0      191 2022-05-02 03:34:03.000000 zoo-framework-0.4.1/zoo_framework/fifo/node/event_fifo_node.py
--rw-rw-rw-   0        0        0      820 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/fifo/single_fifo.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.321334 zoo-framework-0.4.1/zoo_framework/handler/
--rw-rw-rw-   0        0        0       37 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/handler/__init__.py
--rw-rw-rw-   0        0        0     1021 2022-05-02 03:34:03.000000 zoo-framework-0.4.1/zoo_framework/handler/base_handler.py
--rw-rw-rw-   0        0        0      978 2022-05-02 03:34:03.000000 zoo-framework-0.4.1/zoo_framework/handler/event_reactor.py
--rw-rw-rw-   0        0        0      142 2021-11-22 23:43:39.000000 zoo-framework-0.4.1/zoo_framework/handler/waiter_result_handler.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.323344 zoo-framework-0.4.1/zoo_framework/lock/
--rw-rw-rw-   0        0        0       33 2021-11-20 03:16:31.000000 zoo-framework-0.4.1/zoo_framework/lock/__init__.py
--rw-rw-rw-   0        0        0       25 2021-11-20 03:16:31.000000 zoo-framework-0.4.1/zoo_framework/lock/base_lock.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.326342 zoo-framework-0.4.1/zoo_framework/params/
--rw-rw-rw-   0        0        0      167 2021-12-30 07:45:19.000000 zoo-framework-0.4.1/zoo_framework/params/__init__.py
--rw-rw-rw-   0        0        0      190 2021-12-30 07:44:07.000000 zoo-framework-0.4.1/zoo_framework/params/event_params.py
--rw-rw-rw-   0        0        0      358 2021-11-20 03:16:31.000000 zoo-framework-0.4.1/zoo_framework/params/log_params.py
--rw-rw-rw-   0        0        0      212 2021-11-27 04:39:22.000000 zoo-framework-0.4.1/zoo_framework/params/state_machine_params.py
--rw-rw-rw-   0        0        0      521 2021-12-25 06:12:11.000000 zoo-framework-0.4.1/zoo_framework/params/worker_params.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.329342 zoo-framework-0.4.1/zoo_framework/statemachine/
--rw-rw-rw-   0        0        0       54 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/statemachine/__init__.py
--rw-rw-rw-   0        0        0      142 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/statemachine/base_state_machine.py
--rw-rw-rw-   0        0        0     1334 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/statemachine/state_machine_manager.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.331342 zoo-framework-0.4.1/zoo_framework/templates/
--rw-rw-rw-   0        0        0      825 2021-12-29 09:54:29.000000 zoo-framework-0.4.1/zoo_framework/templates/__init__.py
--rw-rw-rw-   0        0        0      155 2021-12-29 07:10:48.000000 zoo-framework-0.4.1/zoo_framework/templates/main.pyt
--rw-rw-rw-   0        0        0      448 2021-12-29 07:08:52.000000 zoo-framework-0.4.1/zoo_framework/templates/thread.pyt
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.336343 zoo-framework-0.4.1/zoo_framework/utils/
--rw-rw-rw-   0        0        0      175 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/utils/__init__.py
--rw-rw-rw-   0        0        0      189 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/utils/cmd_utils.py
--rw-rw-rw-   0        0        0     1980 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/utils/datetime_utils.py
--rw-rw-rw-   0        0        0     1495 2022-05-02 03:35:03.000000 zoo-framework-0.4.1/zoo_framework/utils/file_utils.py
--rw-rw-rw-   0        0        0     1096 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/utils/log_utils.py
--rw-rw-rw-   0        0        0      620 2021-11-04 15:01:03.000000 zoo-framework-0.4.1/zoo_framework/utils/ws_utils.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.342343 zoo-framework-0.4.1/zoo_framework/workers/
--rw-rw-rw-   0        0        0      188 2022-05-02 03:34:03.000000 zoo-framework-0.4.1/zoo_framework/workers/__init__.py
--rw-rw-rw-   0        0        0     1822 2021-12-19 11:14:52.000000 zoo-framework-0.4.1/zoo_framework/workers/base_worker.py
--rw-rw-rw-   0        0        0     1060 2022-05-02 03:34:03.000000 zoo-framework-0.4.1/zoo_framework/workers/event_worker.py
--rw-rw-rw-   0        0        0     1326 2022-05-02 03:34:03.000000 zoo-framework-0.4.1/zoo_framework/workers/state_machine_work.py
--rw-rw-rw-   0        0        0      173 2021-12-19 11:14:52.000000 zoo-framework-0.4.1/zoo_framework/workers/worker_props.py
--rw-rw-rw-   0        0        0      176 2021-11-23 12:52:56.000000 zoo-framework-0.4.1/zoo_framework/workers/worker_result.py
-drwxrwxrwx   0        0        0        0 2022-05-02 03:39:31.292339 zoo-framework-0.4.1/zoo_framework.egg-info/
--rw-rw-rw-   0        0        0     1445 2022-05-02 03:39:31.000000 zoo-framework-0.4.1/zoo_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2547 2022-05-02 03:39:31.000000 zoo-framework-0.4.1/zoo_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-02 03:39:31.000000 zoo-framework-0.4.1/zoo_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2022-05-02 03:39:31.000000 zoo-framework-0.4.1/zoo_framework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2022-05-02 03:39:31.000000 zoo-framework-0.4.1/zoo_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-05-02 03:39:31.000000 zoo-framework-0.4.1/zoo_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.779628 zoo-framework-0.4.2/
+-rw-rw-rw-   0        0        0       33 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1445 2023-06-07 13:37:19.779628 zoo-framework-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2021-11-22 22:45:06.000000 zoo-framework-0.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 13:37:19.779628 zoo-framework-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-06-07 12:46:37.000000 zoo-framework-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.743600 zoo-framework-0.4.2/zoo_framework/
+-rw-rw-rw-   0        0        0      159 2023-06-07 12:44:50.000000 zoo-framework-0.4.2/zoo_framework/__init__.py
+-rw-rw-rw-   0        0        0     3012 2021-12-29 09:23:30.000000 zoo-framework-0.4.2/zoo_framework/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.748600 zoo-framework-0.4.2/zoo_framework/conf/
+-rw-rw-rw-   0        0        0       36 2023-06-07 12:44:50.000000 zoo-framework-0.4.2/zoo_framework/conf/__init__.py
+-rw-rw-rw-   0        0        0     1458 2021-11-20 03:16:31.000000 zoo-framework-0.4.2/zoo_framework/conf/log_config.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.750599 zoo-framework-0.4.2/zoo_framework/constant/
+-rw-rw-rw-   0        0        0       88 2021-12-19 11:14:52.000000 zoo-framework-0.4.2/zoo_framework/constant/__init__.py
+-rw-rw-rw-   0        0        0      185 2021-12-19 11:14:52.000000 zoo-framework-0.4.2/zoo_framework/constant/waiter_constant.py
+-rw-rw-rw-   0        0        0      500 2021-12-19 11:14:52.000000 zoo-framework-0.4.2/zoo_framework/constant/worker_constant.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.753625 zoo-framework-0.4.2/zoo_framework/core/
+-rw-rw-rw-   0        0        0      240 2023-06-07 12:44:50.000000 zoo-framework-0.4.2/zoo_framework/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.756625 zoo-framework-0.4.2/zoo_framework/core/aop/
+-rw-rw-rw-   0        0        0      274 2021-11-22 23:02:32.000000 zoo-framework-0.4.2/zoo_framework/core/aop/__init__.py
+-rw-rw-rw-   0        0        0      195 2021-11-22 23:47:41.000000 zoo-framework-0.4.2/zoo_framework/core/aop/cage.py
+-rw-rw-rw-   0        0        0      150 2021-11-08 13:45:38.000000 zoo-framework-0.4.2/zoo_framework/core/aop/configure.py
+-rw-rw-rw-   0        0        0      280 2022-05-02 03:34:03.000000 zoo-framework-0.4.2/zoo_framework/core/aop/event.py
+-rw-rw-rw-   0        0        0      767 2021-11-08 13:47:50.000000 zoo-framework-0.4.2/zoo_framework/core/aop/params.py
+-rw-rw-rw-   0        0        0      602 2021-11-22 23:04:13.000000 zoo-framework-0.4.2/zoo_framework/core/aop/validation.py
+-rw-rw-rw-   0        0        0      344 2021-11-18 12:24:23.000000 zoo-framework-0.4.2/zoo_framework/core/aop/worker.py
+-rw-rw-rw-   0        0        0     1537 2023-06-07 12:44:50.000000 zoo-framework-0.4.2/zoo_framework/core/master.py
+-rw-rw-rw-   0        0        0      274 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/core/meta_singleton.py
+-rw-rw-rw-   0        0        0     1635 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/core/params_factory.py
+-rw-rw-rw-   0        0        0      237 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/core/params_path.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.759626 zoo-framework-0.4.2/zoo_framework/core/waiter/
+-rw-rw-rw-   0        0        0      201 2021-11-20 03:16:31.000000 zoo-framework-0.4.2/zoo_framework/core/waiter/__init__.py
+-rw-rw-rw-   0        0        0     5202 2023-06-07 12:44:50.000000 zoo-framework-0.4.2/zoo_framework/core/waiter/base_waiter.py
+-rw-rw-rw-   0        0        0     1521 2023-06-07 12:44:50.000000 zoo-framework-0.4.2/zoo_framework/core/waiter/safe_waiter.py
+-rw-rw-rw-   0        0        0      401 2021-12-19 11:14:52.000000 zoo-framework-0.4.2/zoo_framework/core/waiter/simple_waiter.py
+-rw-rw-rw-   0        0        0      254 2021-12-19 11:14:52.000000 zoo-framework-0.4.2/zoo_framework/core/waiter/stable_waiter.py
+-rw-rw-rw-   0        0        0      496 2021-11-20 03:16:31.000000 zoo-framework-0.4.2/zoo_framework/core/waiter/waiter_factory.py
+-rw-rw-rw-   0        0        0     1164 2021-12-25 10:08:58.000000 zoo-framework-0.4.2/zoo_framework/core/zoo_thread.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.762626 zoo-framework-0.4.2/zoo_framework/fifo/
+-rw-rw-rw-   0        0        0      105 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/fifo/__init__.py
+-rw-rw-rw-   0        0        0      603 2022-05-02 03:34:03.000000 zoo-framework-0.4.2/zoo_framework/fifo/base_fifo.py
+-rw-rw-rw-   0        0        0       47 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/fifo/delay_fifo.py
+-rw-rw-rw-   0        0        0      650 2022-05-02 03:34:03.000000 zoo-framework-0.4.2/zoo_framework/fifo/event_fifo.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.763624 zoo-framework-0.4.2/zoo_framework/fifo/node/
+-rw-rw-rw-   0        0        0       86 2022-05-02 03:34:03.000000 zoo-framework-0.4.2/zoo_framework/fifo/node/__init__.py
+-rw-rw-rw-   0        0        0      250 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/fifo/node/delay_fifo_node.py
+-rw-rw-rw-   0        0        0      191 2022-05-02 03:34:03.000000 zoo-framework-0.4.2/zoo_framework/fifo/node/event_fifo_node.py
+-rw-rw-rw-   0        0        0      820 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/fifo/single_fifo.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.765625 zoo-framework-0.4.2/zoo_framework/handler/
+-rw-rw-rw-   0        0        0       37 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/handler/__init__.py
+-rw-rw-rw-   0        0        0     1021 2022-05-02 03:34:03.000000 zoo-framework-0.4.2/zoo_framework/handler/base_handler.py
+-rw-rw-rw-   0        0        0      978 2023-06-07 12:44:50.000000 zoo-framework-0.4.2/zoo_framework/handler/event_reactor.py
+-rw-rw-rw-   0        0        0      142 2021-11-22 23:43:39.000000 zoo-framework-0.4.2/zoo_framework/handler/waiter_result_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.766627 zoo-framework-0.4.2/zoo_framework/lock/
+-rw-rw-rw-   0        0        0       33 2021-11-20 03:16:31.000000 zoo-framework-0.4.2/zoo_framework/lock/__init__.py
+-rw-rw-rw-   0        0        0       25 2021-11-20 03:16:31.000000 zoo-framework-0.4.2/zoo_framework/lock/base_lock.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.769626 zoo-framework-0.4.2/zoo_framework/params/
+-rw-rw-rw-   0        0        0      167 2021-12-30 07:45:19.000000 zoo-framework-0.4.2/zoo_framework/params/__init__.py
+-rw-rw-rw-   0        0        0      190 2021-12-30 07:44:07.000000 zoo-framework-0.4.2/zoo_framework/params/event_params.py
+-rw-rw-rw-   0        0        0      358 2021-11-20 03:16:31.000000 zoo-framework-0.4.2/zoo_framework/params/log_params.py
+-rw-rw-rw-   0        0        0      212 2021-11-27 04:39:22.000000 zoo-framework-0.4.2/zoo_framework/params/state_machine_params.py
+-rw-rw-rw-   0        0        0      521 2021-12-25 06:12:11.000000 zoo-framework-0.4.2/zoo_framework/params/worker_params.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.770626 zoo-framework-0.4.2/zoo_framework/statemachine/
+-rw-rw-rw-   0        0        0       54 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/statemachine/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-06-07 12:44:50.000000 zoo-framework-0.4.2/zoo_framework/statemachine/base_state_machine.py
+-rw-rw-rw-   0        0        0     1334 2023-06-07 12:44:50.000000 zoo-framework-0.4.2/zoo_framework/statemachine/state_machine_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.772626 zoo-framework-0.4.2/zoo_framework/templates/
+-rw-rw-rw-   0        0        0      825 2021-12-29 09:54:29.000000 zoo-framework-0.4.2/zoo_framework/templates/__init__.py
+-rw-rw-rw-   0        0        0      155 2021-12-29 07:10:48.000000 zoo-framework-0.4.2/zoo_framework/templates/main.pyt
+-rw-rw-rw-   0        0        0      448 2021-12-29 07:08:52.000000 zoo-framework-0.4.2/zoo_framework/templates/thread.pyt
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.775626 zoo-framework-0.4.2/zoo_framework/utils/
+-rw-rw-rw-   0        0        0      175 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/utils/__init__.py
+-rw-rw-rw-   0        0        0      189 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/utils/cmd_utils.py
+-rw-rw-rw-   0        0        0     1980 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/utils/datetime_utils.py
+-rw-rw-rw-   0        0        0     1563 2023-06-07 12:44:50.000000 zoo-framework-0.4.2/zoo_framework/utils/file_utils.py
+-rw-rw-rw-   0        0        0     1096 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/utils/log_utils.py
+-rw-rw-rw-   0        0        0      620 2021-11-04 15:01:03.000000 zoo-framework-0.4.2/zoo_framework/utils/ws_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.778625 zoo-framework-0.4.2/zoo_framework/workers/
+-rw-rw-rw-   0        0        0      188 2022-05-02 03:34:03.000000 zoo-framework-0.4.2/zoo_framework/workers/__init__.py
+-rw-rw-rw-   0        0        0     1822 2021-12-19 11:14:52.000000 zoo-framework-0.4.2/zoo_framework/workers/base_worker.py
+-rw-rw-rw-   0        0        0     1110 2023-06-07 12:57:43.000000 zoo-framework-0.4.2/zoo_framework/workers/event_worker.py
+-rw-rw-rw-   0        0        0     1326 2022-05-02 03:34:03.000000 zoo-framework-0.4.2/zoo_framework/workers/state_machine_work.py
+-rw-rw-rw-   0        0        0      173 2021-12-19 11:14:52.000000 zoo-framework-0.4.2/zoo_framework/workers/worker_props.py
+-rw-rw-rw-   0        0        0      176 2021-11-23 12:52:56.000000 zoo-framework-0.4.2/zoo_framework/workers/worker_result.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:37:19.747598 zoo-framework-0.4.2/zoo_framework.egg-info/
+-rw-rw-rw-   0        0        0     1445 2023-06-07 13:37:19.000000 zoo-framework-0.4.2/zoo_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2547 2023-06-07 13:37:19.000000 zoo-framework-0.4.2/zoo_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 13:37:19.000000 zoo-framework-0.4.2/zoo_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-07 13:37:19.000000 zoo-framework-0.4.2/zoo_framework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-06-07 13:37:19.000000 zoo-framework-0.4.2/zoo_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 13:37:19.000000 zoo-framework-0.4.2/zoo_framework.egg-info/top_level.txt
```

### Comparing `zoo-framework-0.4.1/PKG-INFO` & `zoo-framework-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoo-framework
-Version: 0.4.1
+Version: 0.4.2
 Summary: A simple and quick multi-threaded framework
 Home-page: UNKNOWN
 Author: XiangMeng
 Author-email: mengxiang931015@live.com
 License: Apache License
 Description: ![](https://mxstorage.oss-cn-beijing.aliyuncs.com/oss-accesslog/zf-main-logo.png)
```

### Comparing `zoo-framework-0.4.1/setup.py` & `zoo-framework-0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(name='zoo-framework',  # 包名
-      version='0.4.1',  # 版本号
+      version='0.4.2',  # 版本号
       description='A simple and quick multi-threaded framework',
       long_description_content_type="text/markdown",
       long_description=long_description,
       author='XiangMeng',
       author_email='mengxiang931015@live.com',
       install_requires=["click","jinja2","gevent"],
       license='Apache License',
```

### Comparing `zoo-framework-0.4.1/zoo_framework/__main__.py` & `zoo-framework-0.4.2/zoo_framework/__main__.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/conf/log_config.py` & `zoo-framework-0.4.2/zoo_framework/conf/log_config.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/core/aop/params.py` & `zoo-framework-0.4.2/zoo_framework/core/aop/params.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/core/aop/validation.py` & `zoo-framework-0.4.2/zoo_framework/core/aop/validation.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/core/master.py` & `zoo-framework-0.4.2/zoo_framework/core/master.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/core/params_factory.py` & `zoo-framework-0.4.2/zoo_framework/core/params_factory.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/core/waiter/base_waiter.py` & `zoo-framework-0.4.2/zoo_framework/core/waiter/base_waiter.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/core/waiter/safe_waiter.py` & `zoo-framework-0.4.2/zoo_framework/core/waiter/safe_waiter.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/core/zoo_thread.py` & `zoo-framework-0.4.2/zoo_framework/core/zoo_thread.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/fifo/base_fifo.py` & `zoo-framework-0.4.2/zoo_framework/fifo/base_fifo.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/fifo/event_fifo.py` & `zoo-framework-0.4.2/zoo_framework/fifo/event_fifo.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/fifo/single_fifo.py` & `zoo-framework-0.4.2/zoo_framework/fifo/single_fifo.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/handler/base_handler.py` & `zoo-framework-0.4.2/zoo_framework/handler/base_handler.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/handler/event_reactor.py` & `zoo-framework-0.4.2/zoo_framework/handler/event_reactor.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/params/worker_params.py` & `zoo-framework-0.4.2/zoo_framework/params/worker_params.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/statemachine/state_machine_manager.py` & `zoo-framework-0.4.2/zoo_framework/statemachine/state_machine_manager.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/templates/__init__.py` & `zoo-framework-0.4.2/zoo_framework/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/utils/datetime_utils.py` & `zoo-framework-0.4.2/zoo_framework/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/utils/file_utils.py` & `zoo-framework-0.4.2/zoo_framework/utils/file_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 import os
 import shutil
 
 class FileUtils:
     @classmethod
     def dir_exists(cls, path):
         return os.path.exists(path)
-
+    
     @classmethod
     def file_exists(cls, path):
         if cls.is_dir(path):
             return False
         return os.path.exists(path)
-
+    
     @classmethod
     def get_file_parent(cls, path):
         return os.path.dirname(path)
-
+    
     @classmethod
     def get_file_name(cls, path):
         return os.path.basename(path)
-
+    
     @classmethod
     def mkdir(cls, path):
         if cls.dir_exists(path):
             return
         os.mkdir(path)
-
+    
     @classmethod
     def dir_exists_and_create(cls, path) -> bool:
         if cls.dir_exists(path):
             return True
-
+        
         os.makedirs(path)
         return True
-
+    
     @classmethod
     def is_dir(cls, path):
         os.path.isdir(path)
-
+    
     @classmethod
     def file_remove(cls, path):
         if not cls.file_exists(path):
             return
-
+        
         os.remove(path)
-
+    
     @classmethod
     def get_file_size(cls, path):
         if not cls.file_exists(path):
             raise Exception("File %s not found" % path)
-
+        
         if not os.path.isfile(path):
             raise Exception("File %s not found" % path)
-
+        
         return os.path.getsize(path)
-
+    
     @classmethod
     def create_file(cls, path):
         file = open(path, 'w')
         file.close()
 
     @classmethod
     def copy_file(cls, src_path,target_path):
```

### Comparing `zoo-framework-0.4.1/zoo_framework/utils/log_utils.py` & `zoo-framework-0.4.2/zoo_framework/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/utils/ws_utils.py` & `zoo-framework-0.4.2/zoo_framework/utils/ws_utils.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/workers/base_worker.py` & `zoo-framework-0.4.2/zoo_framework/workers/base_worker.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework/workers/event_worker.py` & `zoo-framework-0.4.2/zoo_framework/workers/event_worker.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,22 +12,24 @@
     def __init__(self):
         BaseWorker.__init__(self, {
             "is_loop": True,
             "delay_time": 5,
             "name": "EventWorker"
         })
         self.is_loop = True
-        
+
         self.eventReactor = EventReactor()
-    
+
     def _execute(self):
         while True:
+            g_list = []
             # 获得需要处理的事件
             while EventFIFO.size() > 0:
                 node: EventFIFONode = EventFIFO.pop_value()
                 if node is None:
                     continue
                 handler = self.eventReactor.get_handler(node.handler_name)
-                g = gevent.spawn(handler.handle, (node.topic, node.content, node.handler_name))
-                # 执行处理方法
-                g.start()
+                g = gevent.spawn(handler.handle, node.topic, node.content, node.handler_name)
+                g_list.append(g)
+            # 执行处理方法
+            gevent.joinall(g_list)
             time.sleep(0.2)
```

### Comparing `zoo-framework-0.4.1/zoo_framework/workers/state_machine_work.py` & `zoo-framework-0.4.2/zoo_framework/workers/state_machine_work.py`

 * *Files identical despite different names*

### Comparing `zoo-framework-0.4.1/zoo_framework.egg-info/PKG-INFO` & `zoo-framework-0.4.2/zoo_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoo-framework
-Version: 0.4.1
+Version: 0.4.2
 Summary: A simple and quick multi-threaded framework
 Home-page: UNKNOWN
 Author: XiangMeng
 Author-email: mengxiang931015@live.com
 License: Apache License
 Description: ![](https://mxstorage.oss-cn-beijing.aliyuncs.com/oss-accesslog/zf-main-logo.png)
```

### Comparing `zoo-framework-0.4.1/zoo_framework.egg-info/SOURCES.txt` & `zoo-framework-0.4.2/zoo_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

