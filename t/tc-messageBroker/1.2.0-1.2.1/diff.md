# Comparing `tmp/tc-messageBroker-1.2.0.tar.gz` & `tmp/tc-messageBroker-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-messageBroker-1.2.0.tar", last modified: Fri Jun  2 17:42:29 2023, max compression
+gzip compressed data, was "tc-messageBroker-1.2.1.tar", last modified: Wed Jun  7 05:58:00 2023, max compression
```

## Comparing `tc-messageBroker-1.2.0.tar` & `tc-messageBroker-1.2.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.267498 tc-messageBroker-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-02 17:42:29.267498 tc-messageBroker-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 17:42:29.267498 tc-messageBroker-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/message_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/db_operations/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/db_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/event/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/event/events_microservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/queue/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/queue/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/choreography.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/choreography_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/saga.py
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-02 17:42:29.000000 tc-messageBroker-1.2.0/tc_messageBroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-02 17:42:29.000000 tc-messageBroker-1.2.0/tc_messageBroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:42:29.000000 tc-messageBroker-1.2.0/tc_messageBroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-02 17:42:29.000000 tc-messageBroker-1.2.0/tc_messageBroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 17:42:29.000000 tc-messageBroker-1.2.0/tc_messageBroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.267498 tc-messageBroker-1.2.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/integration/test_message_broker_exchange_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/integration/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/integration/test_saga.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.267498 tc-messageBroker-1.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_choreagraphy_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_enum_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_message_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_predefined_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_saga_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_saga_next.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_saga_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.651239 tc-messageBroker-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-07 05:58:00.651239 tc-messageBroker-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 05:58:00.651239 tc-messageBroker-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/message_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/db_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/db_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/event/events_microservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/queue/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/choreography.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/choreography_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/saga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/transaction_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-07 05:58:00.000000 tc-messageBroker-1.2.1/tc_messageBroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-07 05:58:00.000000 tc-messageBroker-1.2.1/tc_messageBroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 05:58:00.000000 tc-messageBroker-1.2.1/tc_messageBroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 05:58:00.000000 tc-messageBroker-1.2.1/tc_messageBroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 05:58:00.000000 tc-messageBroker-1.2.1/tc_messageBroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/integration/test_message_broker_exchange_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/integration/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/integration/test_saga.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.651239 tc-messageBroker-1.2.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_choreagraphy_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_enum_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_message_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_predefined_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_saga_next.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_saga_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.2.0/PKG-INFO` & `tc-messageBroker-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.2.0
+Version: 1.2.1
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.2.0/README.md` & `tc-messageBroker-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/setup.py` & `tc-messageBroker-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="tc-messageBroker",
-    version="1.2.0",
+    version="1.2.1",
     author="Mohammad Amin Dadgar, RnDAO",
     maintainer="Mohammad Amin Dadgar",
     maintainer_email="dadgaramin96@gmail.com",
     packages=find_packages(),
     description="Shared library for message broker in Python",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `tc-messageBroker-1.2.0/tc_messageBroker/message_broker.py` & `tc-messageBroker-1.2.1/tc_messageBroker/message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py` & `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/db_operations/mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/choreography.py` & `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/choreography.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 DISCORD_UPDATE_CHANNELS = IChoreography(
     name="DISCORD_UPDATE_CHANNELS",
     transactions=DISCORD_UPDATE_CHANNELS_TRANSACTIONS,
 )
 
 DISCORD_SCHEDULED_JOB = IChoreography(
-    name="DISCORD_UPDATE_CHANNELS",
+    name="DISCORD_SCHEDULED_JOB",
     transactions=DISCORD_SCHEDULED_JOB_TRANSACTIONS,
 )
 
 
 class ChoreographyDict:
     DISCORD_UPDATE_CHANNELS = DISCORD_UPDATE_CHANNELS
     DISCORD_SCHEDULED_JOB = DISCORD_SCHEDULED_JOB
```

### Comparing `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/saga.py` & `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/saga_base.py` & `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/saga_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py` & `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/transaction_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/transactions.py` & `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/transactions.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py` & `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py` & `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tc_messageBroker.egg-info/PKG-INFO` & `tc-messageBroker-1.2.1/tc_messageBroker.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.2.0
+Version: 1.2.1
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.2.0/tc_messageBroker.egg-info/SOURCES.txt` & `tc-messageBroker-1.2.1/tc_messageBroker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tests/integration/test_message_broker_exchange_points.py` & `tc-messageBroker-1.2.1/tests/integration/test_message_broker_exchange_points.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tests/integration/test_mongodb.py` & `tc-messageBroker-1.2.1/tests/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tests/integration/test_saga.py` & `tc-messageBroker-1.2.1/tests/integration/test_saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tests/unit/test_choreagraphy_base.py` & `tc-messageBroker-1.2.1/tests/unit/test_choreagraphy_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tests/unit/test_message_broker.py` & `tc-messageBroker-1.2.1/tests/unit/test_message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tests/unit/test_predefined_transactions.py` & `tc-messageBroker-1.2.1/tests/unit/test_predefined_transactions.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tests/unit/test_saga_base.py` & `tc-messageBroker-1.2.1/tests/unit/test_saga_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tests/unit/test_saga_base_utils.py` & `tc-messageBroker-1.2.1/tests/unit/test_saga_base_utils.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tests/unit/test_saga_next.py` & `tc-messageBroker-1.2.1/tests/unit/test_saga_next.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tests/unit/test_saga_start.py` & `tc-messageBroker-1.2.1/tests/unit/test_saga_start.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.0/tests/unit/test_transactions.py` & `tc-messageBroker-1.2.1/tests/unit/test_transactions.py`

 * *Files identical despite different names*

