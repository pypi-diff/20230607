# Comparing `tmp/lavacli-2.0.tar.gz` & `tmp/lavacli-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavacli-2.0.tar", last modified: Tue Jun  6 11:14:18 2023, max compression
+gzip compressed data, was "lavacli-2.0.1.tar", last modified: Wed Jun  7 07:34:05 2023, max compression
```

## Comparing `lavacli-2.0.tar` & `lavacli-2.0.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.827684 lavacli-2.0/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      105 2018-07-13 09:52:07.000000 lavacli-2.0/.coveragerc
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2112 2023-06-06 09:40:54.000000 lavacli-2.0/.gitlab-ci.yml
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    34520 2018-01-18 08:05:38.000000 lavacli-2.0/LICENSE
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      141 2019-03-13 08:49:12.000000 lavacli-2.0/MANIFEST.in
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1053 2023-06-06 11:14:18.827684 lavacli-2.0/PKG-INFO
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.823685 lavacli-2.0/doc/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      604 2018-04-13 14:07:49.000000 lavacli-2.0/doc/Makefile
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5259 2023-02-24 10:40:23.000000 lavacli-2.0/doc/conf.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2335 2020-09-09 08:32:09.000000 lavacli-2.0/doc/configuration.rst
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      379 2019-11-27 05:33:22.000000 lavacli-2.0/doc/index.rst
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      711 2023-06-06 09:42:05.000000 lavacli-2.0/doc/install.rst
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4624 2022-05-10 09:55:41.000000 lavacli-2.0/doc/usage.rst
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.823685 lavacli-2.0/lavacli/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1334 2023-06-06 10:05:10.000000 lavacli-2.0/lavacli/__about__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9240 2023-06-01 10:18:51.000000 lavacli-2.0/lavacli/__init__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      851 2023-02-24 10:40:23.000000 lavacli-2.0/lavacli/__main__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      111 2022-03-31 04:08:12.000000 lavacli-2.0/lavacli/colors.py
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.823685 lavacli-2.0/lavacli/commands/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2022-05-09 15:46:10.000000 lavacli-2.0/lavacli/commands/__init__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4001 2023-02-24 10:40:23.000000 lavacli-2.0/lavacli/commands/aliases.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    13999 2023-04-07 12:33:18.000000 lavacli-2.0/lavacli/commands/device_types.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    15547 2023-04-07 07:01:47.000000 lavacli-2.0/lavacli/commands/devices.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9742 2023-03-17 09:10:17.000000 lavacli-2.0/lavacli/commands/events.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5767 2023-04-07 12:33:18.000000 lavacli-2.0/lavacli/commands/groups.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4156 2023-02-24 10:40:23.000000 lavacli-2.0/lavacli/commands/identities.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    23030 2023-06-06 09:43:24.000000 lavacli-2.0/lavacli/commands/jobs.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    44186 2023-06-02 12:23:16.000000 lavacli-2.0/lavacli/commands/lab.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3217 2023-02-24 10:40:23.000000 lavacli-2.0/lavacli/commands/results.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9213 2023-03-17 09:10:17.000000 lavacli-2.0/lavacli/commands/system.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3689 2023-02-24 10:40:23.000000 lavacli-2.0/lavacli/commands/tags.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11354 2023-04-12 15:39:33.000000 lavacli-2.0/lavacli/commands/users.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4119 2023-04-07 07:01:44.000000 lavacli-2.0/lavacli/commands/utils.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    12997 2023-04-07 07:01:47.000000 lavacli-2.0/lavacli/commands/workers.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5070 2023-06-02 11:39:40.000000 lavacli-2.0/lavacli/schemas.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1808 2023-03-21 10:08:31.000000 lavacli-2.0/lavacli/utils.py
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.823685 lavacli-2.0/lavacli.egg-info/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1053 2023-06-06 11:14:18.000000 lavacli-2.0/lavacli.egg-info/PKG-INFO
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1283 2023-06-06 11:14:18.000000 lavacli-2.0/lavacli.egg-info/SOURCES.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-06-06 11:14:18.000000 lavacli-2.0/lavacli.egg-info/dependency_links.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       41 2023-06-06 11:14:18.000000 lavacli-2.0/lavacli.egg-info/entry_points.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       47 2023-06-06 11:14:18.000000 lavacli-2.0/lavacli.egg-info/requires.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        8 2023-06-06 11:14:18.000000 lavacli-2.0/lavacli.egg-info/top_level.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-06-06 11:13:47.000000 lavacli-2.0/lavacli.egg-info/zip-safe
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       47 2023-06-01 10:18:51.000000 lavacli-2.0/requirements.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       38 2023-06-06 11:14:18.827684 lavacli-2.0/setup.cfg
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2344 2023-06-06 09:44:15.000000 lavacli-2.0/setup.py
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.823685 lavacli-2.0/share/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      838 2018-04-13 12:29:55.000000 lavacli-2.0/share/lavacli.yaml
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.827684 lavacli-2.0/tests/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 07:02:55.000000 lavacli-2.0/tests/__init__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1806 2023-04-07 07:02:55.000000 lavacli-2.0/tests/conftest.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     8982 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_aliases.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    20063 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_device_types.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    32637 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_devices.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24515 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_events.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1324 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_helpers.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     7504 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_identities.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    58342 2023-04-07 12:33:40.000000 lavacli-2.0/tests/test_jobs.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)   111807 2023-06-02 13:09:33.000000 lavacli-2.0/tests/test_lab.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1615 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_lavacli.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11619 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_results.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3052 2023-06-01 10:18:51.000000 lavacli-2.0/tests/test_schemas.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    25702 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_system.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     6550 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_tags.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5479 2023-04-12 15:39:33.000000 lavacli-2.0/tests/test_users.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24888 2023-04-07 12:33:53.000000 lavacli-2.0/tests/test_workers.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-07 07:34:05.920658 lavacli-2.0.1/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      105 2018-07-13 09:52:07.000000 lavacli-2.0.1/.coveragerc
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2218 2023-06-07 07:29:01.000000 lavacli-2.0.1/.gitlab-ci.yml
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    34520 2018-01-18 08:05:38.000000 lavacli-2.0.1/LICENSE
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      141 2019-03-13 08:49:12.000000 lavacli-2.0.1/MANIFEST.in
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1055 2023-06-07 07:34:05.920658 lavacli-2.0.1/PKG-INFO
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-07 07:34:05.912658 lavacli-2.0.1/doc/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      604 2018-04-13 14:07:49.000000 lavacli-2.0.1/doc/Makefile
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5259 2023-02-24 10:40:23.000000 lavacli-2.0.1/doc/conf.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2335 2020-09-09 08:32:09.000000 lavacli-2.0.1/doc/configuration.rst
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      379 2019-11-27 05:33:22.000000 lavacli-2.0.1/doc/index.rst
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      711 2023-06-06 09:42:05.000000 lavacli-2.0.1/doc/install.rst
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4624 2022-05-10 09:55:41.000000 lavacli-2.0.1/doc/usage.rst
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-07 07:34:05.912658 lavacli-2.0.1/lavacli/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1336 2023-06-07 07:33:30.000000 lavacli-2.0.1/lavacli/__about__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9240 2023-06-01 10:18:51.000000 lavacli-2.0.1/lavacli/__init__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      851 2023-02-24 10:40:23.000000 lavacli-2.0.1/lavacli/__main__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      111 2022-03-31 04:08:12.000000 lavacli-2.0.1/lavacli/colors.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-07 07:34:05.916658 lavacli-2.0.1/lavacli/commands/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2022-05-09 15:46:10.000000 lavacli-2.0.1/lavacli/commands/__init__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4001 2023-02-24 10:40:23.000000 lavacli-2.0.1/lavacli/commands/aliases.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    13999 2023-04-07 12:33:18.000000 lavacli-2.0.1/lavacli/commands/device_types.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    15547 2023-04-07 07:01:47.000000 lavacli-2.0.1/lavacli/commands/devices.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9742 2023-03-17 09:10:17.000000 lavacli-2.0.1/lavacli/commands/events.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5767 2023-04-07 12:33:18.000000 lavacli-2.0.1/lavacli/commands/groups.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4156 2023-02-24 10:40:23.000000 lavacli-2.0.1/lavacli/commands/identities.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    23030 2023-06-06 09:43:24.000000 lavacli-2.0.1/lavacli/commands/jobs.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    44300 2023-06-07 07:29:01.000000 lavacli-2.0.1/lavacli/commands/lab.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3217 2023-02-24 10:40:23.000000 lavacli-2.0.1/lavacli/commands/results.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9213 2023-03-17 09:10:17.000000 lavacli-2.0.1/lavacli/commands/system.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3689 2023-02-24 10:40:23.000000 lavacli-2.0.1/lavacli/commands/tags.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11354 2023-04-12 15:39:33.000000 lavacli-2.0.1/lavacli/commands/users.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4119 2023-04-07 07:01:44.000000 lavacli-2.0.1/lavacli/commands/utils.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    12997 2023-04-07 07:01:47.000000 lavacli-2.0.1/lavacli/commands/workers.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5070 2023-06-02 11:39:40.000000 lavacli-2.0.1/lavacli/schemas.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1808 2023-03-21 10:08:31.000000 lavacli-2.0.1/lavacli/utils.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-07 07:34:05.916658 lavacli-2.0.1/lavacli.egg-info/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1055 2023-06-07 07:34:05.000000 lavacli-2.0.1/lavacli.egg-info/PKG-INFO
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1283 2023-06-07 07:34:05.000000 lavacli-2.0.1/lavacli.egg-info/SOURCES.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-06-07 07:34:05.000000 lavacli-2.0.1/lavacli.egg-info/dependency_links.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       41 2023-06-07 07:34:05.000000 lavacli-2.0.1/lavacli.egg-info/entry_points.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       47 2023-06-07 07:34:05.000000 lavacli-2.0.1/lavacli.egg-info/requires.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        8 2023-06-07 07:34:05.000000 lavacli-2.0.1/lavacli.egg-info/top_level.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-06-07 07:34:05.000000 lavacli-2.0.1/lavacli.egg-info/zip-safe
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       47 2023-06-01 10:18:51.000000 lavacli-2.0.1/requirements.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       38 2023-06-07 07:34:05.920658 lavacli-2.0.1/setup.cfg
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2344 2023-06-06 09:44:15.000000 lavacli-2.0.1/setup.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-07 07:34:05.916658 lavacli-2.0.1/share/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      838 2018-04-13 12:29:55.000000 lavacli-2.0.1/share/lavacli.yaml
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-07 07:34:05.920658 lavacli-2.0.1/tests/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 07:02:55.000000 lavacli-2.0.1/tests/__init__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1806 2023-04-07 07:02:55.000000 lavacli-2.0.1/tests/conftest.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     8982 2023-04-07 07:02:55.000000 lavacli-2.0.1/tests/test_aliases.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    20063 2023-04-07 07:02:55.000000 lavacli-2.0.1/tests/test_device_types.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    32637 2023-04-07 07:02:55.000000 lavacli-2.0.1/tests/test_devices.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24515 2023-04-07 07:02:55.000000 lavacli-2.0.1/tests/test_events.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1324 2023-04-07 07:02:55.000000 lavacli-2.0.1/tests/test_helpers.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     7504 2023-04-07 07:02:55.000000 lavacli-2.0.1/tests/test_identities.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    58342 2023-04-07 12:33:40.000000 lavacli-2.0.1/tests/test_jobs.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)   112568 2023-06-07 07:29:01.000000 lavacli-2.0.1/tests/test_lab.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1615 2023-04-07 07:02:55.000000 lavacli-2.0.1/tests/test_lavacli.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11619 2023-04-07 07:02:55.000000 lavacli-2.0.1/tests/test_results.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3052 2023-06-01 10:18:51.000000 lavacli-2.0.1/tests/test_schemas.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    25702 2023-04-07 07:02:55.000000 lavacli-2.0.1/tests/test_system.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     6550 2023-04-07 07:02:55.000000 lavacli-2.0.1/tests/test_tags.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5479 2023-04-12 15:39:33.000000 lavacli-2.0.1/tests/test_users.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24888 2023-04-07 12:33:53.000000 lavacli-2.0.1/tests/test_workers.py
```

### Comparing `lavacli-2.0/.gitlab-ci.yml` & `lavacli-2.0.1/.gitlab-ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,20 @@
   image: debian:bookworm
 test-ubuntu-20.04:
   <<: *test
   image: ubuntu:20.04
 test-ubuntu-22.04:
   <<: *test
   image: ubuntu:22.04
+test-ubuntu-22.10:
+  <<: *test
+  image: ubuntu:22.10
+test-ubuntu-23.04:
+  <<: *test
+  image: ubuntu:23.04
 
 ###########
 # Analyze #
 ###########
 pylint:
   stage: analyze
   image: registry.gitlab.com/lava/ci-images/amd64/analyze
```

### Comparing `lavacli-2.0/LICENSE` & `lavacli-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/PKG-INFO` & `lavacli-2.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavacli
-Version: 2.0
+Version: 2.0.1
 Summary: LAVA XML-RPC command line interface
 Home-page: https://gitlab.com/lava/lavacli
 Author: Rémi Duraffort
 Author-email: remi.duraffort@linaro.org
 License: AGPLv3+
 Project-URL: Bug Tracker, https://gitlab.com/lava/lavacli/issues/
 Project-URL: Source Code, https://gitlab.com/lava/lavacli/
```

### Comparing `lavacli-2.0/doc/Makefile` & `lavacli-2.0.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/doc/conf.py` & `lavacli-2.0.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/doc/configuration.rst` & `lavacli-2.0.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/doc/install.rst` & `lavacli-2.0.1/doc/install.rst`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/doc/usage.rst` & `lavacli-2.0.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/__about__.py` & `lavacli-2.0.1/lavacli/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 
 
 __author__ = "Rémi Duraffort"
 __author_email__ = "remi.duraffort@linaro.org"
 __description__ = "LAVA XML-RPC command line interface"
 __license__ = "AGPLv3+"
 __url__ = "https://gitlab.com/lava/lavacli"
-__version__ = "2.0"
+__version__ = "2.0.1"
```

### Comparing `lavacli-2.0/lavacli/__init__.py` & `lavacli-2.0.1/lavacli/__init__.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/__main__.py` & `lavacli-2.0.1/lavacli/__main__.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/aliases.py` & `lavacli-2.0.1/lavacli/commands/aliases.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/device_types.py` & `lavacli-2.0.1/lavacli/commands/device_types.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/devices.py` & `lavacli-2.0.1/lavacli/commands/devices.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/events.py` & `lavacli-2.0.1/lavacli/commands/events.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/groups.py` & `lavacli-2.0.1/lavacli/commands/groups.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/identities.py` & `lavacli-2.0.1/lavacli/commands/identities.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/jobs.py` & `lavacli-2.0.1/lavacli/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/lab.py` & `lavacli-2.0.1/lavacli/commands/lab.py`

 * *Files 0% similar despite different names*

```diff
@@ -821,15 +821,18 @@
                             None,
                         )
 
     print(f"{colors.cyan}> workers{colors.reset}")
     if "workers" not in options.resources:
         print(f"  {colors.yellow}-> SKIP{colors.reset}")
     else:
-        workers = proxy.scheduler.workers.list(True)
+        if config["version"] >= (2023, 3):
+            workers = proxy.scheduler.workers.list(True)
+        else:
+            workers = proxy.scheduler.workers.list()
         for worker in lab.workers.values():
             if worker.hostname in workers:
                 print(f"  {colors.green}* {worker.hostname}{colors.reset}")
             else:
                 print(f"  {colors.yellow}* {worker.hostname}{colors.reset}")
                 if not options.dry_run:
                     proxy.scheduler.workers.add(
```

### Comparing `lavacli-2.0/lavacli/commands/results.py` & `lavacli-2.0.1/lavacli/commands/results.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/system.py` & `lavacli-2.0.1/lavacli/commands/system.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/tags.py` & `lavacli-2.0.1/lavacli/commands/tags.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/users.py` & `lavacli-2.0.1/lavacli/commands/users.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/utils.py` & `lavacli-2.0.1/lavacli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/commands/workers.py` & `lavacli-2.0.1/lavacli/commands/workers.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/schemas.py` & `lavacli-2.0.1/lavacli/schemas.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli/utils.py` & `lavacli-2.0.1/lavacli/utils.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/lavacli.egg-info/PKG-INFO` & `lavacli-2.0.1/lavacli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavacli
-Version: 2.0
+Version: 2.0.1
 Summary: LAVA XML-RPC command line interface
 Home-page: https://gitlab.com/lava/lavacli
 Author: Rémi Duraffort
 Author-email: remi.duraffort@linaro.org
 License: AGPLv3+
 Project-URL: Bug Tracker, https://gitlab.com/lava/lavacli/issues/
 Project-URL: Source Code, https://gitlab.com/lava/lavacli/
```

### Comparing `lavacli-2.0/lavacli.egg-info/SOURCES.txt` & `lavacli-2.0.1/lavacli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/setup.py` & `lavacli-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/share/lavacli.yaml` & `lavacli-2.0.1/share/lavacli.yaml`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/conftest.py` & `lavacli-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_aliases.py` & `lavacli-2.0.1/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_device_types.py` & `lavacli-2.0.1/tests/test_device_types.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_devices.py` & `lavacli-2.0.1/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_events.py` & `lavacli-2.0.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_helpers.py` & `lavacli-2.0.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_identities.py` & `lavacli-2.0.1/tests/test_identities.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_jobs.py` & `lavacli-2.0.1/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_lab.py` & `lavacli-2.0.1/tests/test_lab.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,14 +303,19 @@
                 "ret": ["worker01", "worker02"],
             }
             self.scheduler_workers_list_all = {
                 "request": "scheduler.workers.list",
                 "args": (True,),
                 "ret": ["worker01", "worker02"],
             }
+            self.scheduler_workers_list_all_2023_2 = {
+                "request": "scheduler.workers.list",
+                "args": (),
+                "ret": ["worker01", "worker02"],
+            }
             self.scheduler_workers_show_worker01 = {
                 "request": "scheduler.workers.show",
                 "args": ("worker01",),
                 "ret": {
                     "hostname": "worker01",
                     "description": "",
                     "state": "Online",
@@ -2051,14 +2056,34 @@
             mock_get.system_version_2023_3,
             mock_get.scheduler_workers_list_all,
             mock_get.scheduler_workers_show_worker01,
             mock_get.scheduler_workers_show_worker02,
         ],
     )
 
+
+def test_lab_apply_workers_list_2023_2(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "workers", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_2,
+            mock_get.scheduler_workers_list_all_2023_2,
+            mock_get.scheduler_workers_show_worker01,
+            mock_get.scheduler_workers_show_worker02,
+        ],
+    )
+
     config_file.write_text(config_def, encoding="utf-8")
     expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[32m* worker01\x1b[0m\n  \x1b[32m* worker02\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n"
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
     assert err == ""
```

### Comparing `lavacli-2.0/tests/test_lavacli.py` & `lavacli-2.0.1/tests/test_lavacli.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_results.py` & `lavacli-2.0.1/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_schemas.py` & `lavacli-2.0.1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_system.py` & `lavacli-2.0.1/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_tags.py` & `lavacli-2.0.1/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_users.py` & `lavacli-2.0.1/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `lavacli-2.0/tests/test_workers.py` & `lavacli-2.0.1/tests/test_workers.py`

 * *Files identical despite different names*

