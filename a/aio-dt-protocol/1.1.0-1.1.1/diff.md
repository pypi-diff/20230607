# Comparing `tmp/aio_dt_protocol-1.1.0.tar.gz` & `tmp/aio_dt_protocol-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_dt_protocol-1.1.0.tar", last modified: Sat May 27 18:48:58 2023, max compression
+gzip compressed data, was "aio_dt_protocol-1.1.1.tar", last modified: Wed Jun  7 06:21:54 2023, max compression
```

## Comparing `aio_dt_protocol-1.1.0.tar` & `aio_dt_protocol-1.1.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.681686 aio_dt_protocol-1.1.0/
--rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     7959 2023-05-27 18:48:58.681686 aio_dt_protocol-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7215 2023-05-27 15:28:49.000000 aio_dt_protocol-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.317815 aio_dt_protocol-1.1.0/aio_dt_protocol/
--rw-rw-rw-   0        0        0      503 2023-05-27 17:32:49.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/__init__.py
--rw-rw-rw-   0        0        0    10780 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/actions.py
--rw-rw-rw-   0        0        0    56559 2023-05-27 18:33:35.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/browser.py
--rw-rw-rw-   0        0        0    16843 2023-05-27 14:24:00.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/connection.py
--rw-rw-rw-   0        0        0    25804 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/data.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.324813 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/
--rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.327812 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/background_service/
--rw-rw-rw-   0        0        0      107 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/background_service/__init__.py
--rw-rw-rw-   0        0        0     3279 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/background_service/background_service.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/background_service/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.343807 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/browser/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/browser/__init__.py
--rw-rw-rw-   0        0        0    13585 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/browser/browser.py
--rw-rw-rw-   0        0        0     1346 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/browser/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.393790 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/css/
--rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/css/__init__.py
--rw-rw-rw-   0        0        0     6353 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/css/css.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/css/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.396787 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/device_orientation/
--rw-rw-rw-   0        0        0       51 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/device_orientation/__init__.py
--rw-rw-rw-   0        0        0     1455 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/device_orientation/device_orientation.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/device_orientation/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.432775 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/
--rw-rw-rw-   0        0        0       80 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/__init__.py
--rw-rw-rw-   0        0        0    16508 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/dom.py
--rw-rw-rw-   0        0        0    35568 2023-05-24 16:56:17.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/dom_element.py
--rw-rw-rw-   0        0        0      798 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.457767 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/emulation/
--rw-rw-rw-   0        0        0       73 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/emulation/__init__.py
--rw-rw-rw-   0        0        0    24489 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/emulation/emulation.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/emulation/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.478758 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/fetch/
--rw-rw-rw-   0        0        0       57 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/fetch/__init__.py
--rw-rw-rw-   0        0        0    17264 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/fetch/fetch.py
--rw-rw-rw-   0        0        0     5210 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/fetch/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.519743 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/input/
--rw-rw-rw-   0        0        0       26 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/input/__init__.py
--rw-rw-rw-   0        0        0    23645 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/input/input.py
--rw-rw-rw-   0        0        0     2778 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/input/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.549733 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/log/
--rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/log/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/log/log.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/log/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.571725 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/network/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/network/__init__.py
--rw-rw-rw-   0        0        0    18941 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/network/network.py
--rw-rw-rw-   0        0        0     3522 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/network/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.604713 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/overlay/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/overlay/__init__.py
--rw-rw-rw-   0        0        0     1731 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/overlay/overlay.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/overlay/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.626705 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/page/
--rw-rw-rw-   0        0        0       53 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/page/__init__.py
--rw-rw-rw-   0        0        0    33682 2023-05-24 16:56:23.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/page/page.py
--rw-rw-rw-   0        0        0     3104 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/page/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.640700 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/runtime/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/runtime/__init__.py
--rw-rw-rw-   0        0        0    33744 2023-05-27 18:14:28.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/runtime/runtime.py
--rw-rw-rw-   0        0        0     8104 2023-05-26 16:33:22.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/runtime/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.655695 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/system_info/
--rw-rw-rw-   0        0        0       37 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/system_info/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/system_info/system_info.py
--rw-rw-rw-   0        0        0      784 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/system_info/types.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.680687 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/target/
--rw-rw-rw-   0        0        0       61 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/target/__init__.py
--rw-rw-rw-   0        0        0    17276 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/target/target.py
--rw-rw-rw-   0        0        0      408 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/target/types.py
--rw-rw-rw-   0        0        0     3753 2023-05-26 18:01:07.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/exceptions.py
--rw-rw-rw-   0        0        0     8527 2023-05-27 18:13:13.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/extend_connection.py
--rw-rw-rw-   0        0        0     5683 2023-05-27 18:33:35.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.323813 aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/
--rw-rw-rw-   0        0        0     7959 2023-05-27 18:48:58.000000 aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2504 2023-05-27 18:48:58.000000 aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 18:48:58.000000 aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-27 18:48:58.000000 aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-27 18:48:58.000000 aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 18:48:58.682686 aio_dt_protocol-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-04-06 10:09:07.000000 aio_dt_protocol-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:54.130775 aio_dt_protocol-1.1.1/
+-rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     8670 2023-06-07 06:21:54.131773 aio_dt_protocol-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7926 2023-06-07 06:11:50.000000 aio_dt_protocol-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.541980 aio_dt_protocol-1.1.1/aio_dt_protocol/
+-rw-rw-rw-   0        0        0      503 2023-06-07 06:18:44.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/__init__.py
+-rw-rw-rw-   0        0        0    10780 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/actions.py
+-rw-rw-rw-   0        0        0    56559 2023-05-27 18:33:35.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/browser.py
+-rw-rw-rw-   0        0        0    16933 2023-06-07 06:00:16.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/connection.py
+-rw-rw-rw-   0        0        0    25804 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/data.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.558974 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/
+-rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.571970 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/background_service/
+-rw-rw-rw-   0        0        0      107 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/background_service/__init__.py
+-rw-rw-rw-   0        0        0     3279 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/background_service/background_service.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/background_service/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.584966 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/browser/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/browser/__init__.py
+-rw-rw-rw-   0        0        0    13585 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/browser/browser.py
+-rw-rw-rw-   0        0        0     1346 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/browser/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.608958 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/css/
+-rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/css/__init__.py
+-rw-rw-rw-   0        0        0     6353 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/css/css.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/css/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.621952 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/device_orientation/
+-rw-rw-rw-   0        0        0       51 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/device_orientation/__init__.py
+-rw-rw-rw-   0        0        0     1455 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/device_orientation/device_orientation.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/device_orientation/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.663937 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/
+-rw-rw-rw-   0        0        0       80 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/__init__.py
+-rw-rw-rw-   0        0        0    16508 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/dom.py
+-rw-rw-rw-   0        0        0    35568 2023-05-24 16:56:17.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/dom_element.py
+-rw-rw-rw-   0        0        0      798 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.683930 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/emulation/
+-rw-rw-rw-   0        0        0       73 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/emulation/__init__.py
+-rw-rw-rw-   0        0        0    24489 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/emulation/emulation.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/emulation/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.709921 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/fetch/
+-rw-rw-rw-   0        0        0       57 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/fetch/__init__.py
+-rw-rw-rw-   0        0        0    17264 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/fetch/fetch.py
+-rw-rw-rw-   0        0        0     5210 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/fetch/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.750906 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/input/
+-rw-rw-rw-   0        0        0       26 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/input/__init__.py
+-rw-rw-rw-   0        0        0    23645 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/input/input.py
+-rw-rw-rw-   0        0        0     2778 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/input/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.763901 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/log/
+-rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/log/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/log/log.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/log/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.786893 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/network/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/network/__init__.py
+-rw-rw-rw-   0        0        0    18941 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/network/network.py
+-rw-rw-rw-   0        0        0     3522 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/network/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.819882 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/overlay/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/overlay/__init__.py
+-rw-rw-rw-   0        0        0     1731 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/overlay/overlay.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/overlay/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.849871 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/page/
+-rw-rw-rw-   0        0        0       53 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/page/__init__.py
+-rw-rw-rw-   0        0        0    33682 2023-05-24 16:56:23.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/page/page.py
+-rw-rw-rw-   0        0        0     3104 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/page/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.901852 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/runtime/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/runtime/__init__.py
+-rw-rw-rw-   0        0        0    33744 2023-05-27 18:14:28.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/runtime/runtime.py
+-rw-rw-rw-   0        0        0     8104 2023-05-26 16:33:22.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/runtime/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.920846 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/system_info/
+-rw-rw-rw-   0        0        0       37 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/system_info/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/system_info/system_info.py
+-rw-rw-rw-   0        0        0      784 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/system_info/types.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:54.128773 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/target/
+-rw-rw-rw-   0        0        0       61 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/target/__init__.py
+-rw-rw-rw-   0        0        0    17276 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/target/target.py
+-rw-rw-rw-   0        0        0      408 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/target/types.py
+-rw-rw-rw-   0        0        0     3753 2023-05-26 18:01:07.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/exceptions.py
+-rw-rw-rw-   0        0        0     9252 2023-06-07 06:00:16.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/extend_connection.py
+-rw-rw-rw-   0        0        0     5683 2023-05-27 18:33:35.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.557976 aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/
+-rw-rw-rw-   0        0        0     8670 2023-06-07 06:21:53.000000 aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2504 2023-06-07 06:21:53.000000 aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 06:21:53.000000 aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-07 06:21:53.000000 aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-07 06:21:53.000000 aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 06:21:54.133772 aio_dt_protocol-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2023-04-06 10:09:07.000000 aio_dt_protocol-1.1.1/setup.py
```

### Comparing `aio_dt_protocol-1.1.0/LICENSE` & `aio_dt_protocol-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/PKG-INFO` & `aio_dt_protocol-1.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,11 @@
-Metadata-Version: 2.1
-Name: aio_dt_protocol
-Version: 1.1.0
-Summary: Asynchronous wrapper over Chromium browser debugger protocol.
-Home-page: https://github.com/PieceOfGood/aio_dt_protocol
-Author: PieceOfGood
-Author-email: 78sanchezz@gmail.com
-License: BSD 3-Clause
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Асинхронная обёртка над [протоколом](https://chromedevtools.github.io/devtools-protocol/) отладчика браузера Chromium.
 
+Запуски проводятся только в ОС Windows и Linux.
+
 ### Установка
 ```shell
 pip install aio-dt-protocol
 ```
 
 Имеет одну зависимость:
 https://github.com/aaugustin/websockets
@@ -104,15 +87,19 @@
     print("[- DONE -]")
 
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
-На страницу можно легко зарегистрировать слушателей, которые будут вызываться на стороне клиентского(Python) кода. Для этого необходимо выполнить в браузере JavaScript, передав в `console.info()` JSON-строку из JavaScript-объекта с двумя обязательными полями `func_name` - имя вызываемой python-функции и `args` - список аргументов, которые будут ей переданы. Например:
+На страницу можно легко зарегистрировать слушателей, которые будут вызываться на стороне клиентского(Python) кода. Для этого необходимо зарегистрировать вызываемую функцию в качестве такого слушателя. Это возможно выполнить двумя способами:
+1. Вручную передав методу `addBinding()` домена `Runtime` имя функции в виде строки.
+2. Воспользоваться более функциональной обёрткой первого способа, выраженной в методе `bindFunction()` соединения.
+
+Второй способ менее многословен. Под капотом он добавляет в контекст страницы утилиту `py_call()`, первым аргументом принимающую имя функции, после чего, любое кол-во позиционных аргументов, которые ожидает эта функция, а так же позволяет прикрепить любое кол-во аргументов, передаваемых в функцию последними. Например:
 
 ```python
     html = """\
     <html lang="ru">
     <head>
         <meta charset="utf-8" />
         <title>Test application</title>
@@ -124,31 +111,28 @@
         const btn = document.querySelector('#knopka');
         btn.addEventListener('click', () => {
             py_call("test_func", 1, "test")
         });
     </script>
     </html>"""
     
-    # ? Добавляем на страницу `py_call()`
-    await conn.extend.pyCallAddOnload()
-    
     # ? number и text будут переданы из браузера, а bind_arg указан при регистрации
     async def test_func(number: int, text: str, bind_arg: dict) -> None:
         print(f"[- test_func -] Called with args:\n\tnumber: {number}"
               f"\n\ttext: {text}\n\tbing_arg: {bind_arg}")
     
     
     await conn.bindFunction(
         test_func,  # ! слушатель
         {"name": "test", "value": True}  # ! bind_arg
     )
     
     # ? Если ожидается внушительный функционал прикрутить к странице, то это можно
     # ? сделать за один раз.
-    # await conn.addListeners(
+    # await conn.bindFunctions(
     #     (test_func, [ {"name": "test", "value": True} ]),
     #     # (any_awaitable1, [1, 2, 3])
     #     # (any_awaitable2, [])
     # )
     
     await conn.Page.navigate(html)
 ```
@@ -195,8 +179,8 @@
     await conn.Browser.close()
     print("[- DONE -]")
 
 
 if __name__ == '__main__':
     asyncio.run(main())
 
-```
+```
```

### Comparing `aio_dt_protocol-1.1.0/README.md` & `aio_dt_protocol-1.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,30 @@
+Metadata-Version: 2.1
+Name: aio_dt_protocol
+Version: 1.1.1
+Summary: Asynchronous wrapper over Chromium browser debugger protocol.
+Home-page: https://github.com/PieceOfGood/aio_dt_protocol
+Author: PieceOfGood
+Author-email: 78sanchezz@gmail.com
+License: BSD 3-Clause
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Асинхронная обёртка над [протоколом](https://chromedevtools.github.io/devtools-protocol/) отладчика браузера Chromium.
 
+Запуски проводятся только в ОС Windows и Linux.
+
 ### Установка
 ```shell
 pip install aio-dt-protocol
 ```
 
 Имеет одну зависимость:
 https://github.com/aaugustin/websockets
@@ -85,15 +106,19 @@
     print("[- DONE -]")
 
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
-На страницу можно легко зарегистрировать слушателей, которые будут вызываться на стороне клиентского(Python) кода. Для этого необходимо выполнить в браузере JavaScript, передав в `console.info()` JSON-строку из JavaScript-объекта с двумя обязательными полями `func_name` - имя вызываемой python-функции и `args` - список аргументов, которые будут ей переданы. Например:
+На страницу можно легко зарегистрировать слушателей, которые будут вызываться на стороне клиентского(Python) кода. Для этого необходимо зарегистрировать вызываемую функцию в качестве такого слушателя. Это возможно выполнить двумя способами:
+1. Вручную передав методу `addBinding()` домена `Runtime` имя функции в виде строки.
+2. Воспользоваться более функциональной обёрткой первого способа, выраженной в методе `bindFunction()` соединения.
+
+Второй способ менее многословен. Под капотом он добавляет в контекст страницы утилиту `py_call()`, первым аргументом принимающую имя функции, после чего, любое кол-во позиционных аргументов, которые ожидает эта функция, а так же позволяет прикрепить любое кол-во аргументов, передаваемых в функцию последними. Например:
 
 ```python
     html = """\
     <html lang="ru">
     <head>
         <meta charset="utf-8" />
         <title>Test application</title>
@@ -105,31 +130,28 @@
         const btn = document.querySelector('#knopka');
         btn.addEventListener('click', () => {
             py_call("test_func", 1, "test")
         });
     </script>
     </html>"""
     
-    # ? Добавляем на страницу `py_call()`
-    await conn.extend.pyCallAddOnload()
-    
     # ? number и text будут переданы из браузера, а bind_arg указан при регистрации
     async def test_func(number: int, text: str, bind_arg: dict) -> None:
         print(f"[- test_func -] Called with args:\n\tnumber: {number}"
               f"\n\ttext: {text}\n\tbing_arg: {bind_arg}")
     
     
     await conn.bindFunction(
         test_func,  # ! слушатель
         {"name": "test", "value": True}  # ! bind_arg
     )
     
     # ? Если ожидается внушительный функционал прикрутить к странице, то это можно
     # ? сделать за один раз.
-    # await conn.addListeners(
+    # await conn.bindFunctions(
     #     (test_func, [ {"name": "test", "value": True} ]),
     #     # (any_awaitable1, [1, 2, 3])
     #     # (any_awaitable2, [])
     # )
     
     await conn.Page.navigate(html)
 ```
@@ -176,8 +198,8 @@
     await conn.Browser.close()
     print("[- DONE -]")
 
 
 if __name__ == '__main__':
     asyncio.run(main())
 
-```
+```
```

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/actions.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/actions.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/browser.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/browser.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/connection.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,26 +287,28 @@
         в тело события `Runtime.bindingCalled`.
         """
         if not iscoroutinefunction(function):
             raise TypeError("Listener must be a async callable object!")
 
         self._bindings[function.__name__] = function, args
         await self.Runtime.addBinding(function.__name__)
+        await self.extend.pyCallAddOnload()
 
     async def bindFunctions(
             self, *handlers_n_args: Tuple[Callable[[any], CoroTypeNone], Iterable]) -> None:
         """ Выполняет множественную регистрацию.
         :param handlers_n_args:     Список двухэлементных последовательностей,
         в которых:
             - первый элемент: awaitable-объект
             - второй элемент: последовательность аргументов любой длины, которая
                 будет передана первому элементу в последнюю очередь.
         """
         for function, args in handlers_n_args:
             await self.bindFunction(function, *args)
+        await self.extend.pyCallAddOnload()
 
     async def unbindFunctions(self, *functions: Union[Callable[[any], CoroTypeNone], str]) -> None:
         """ Прекращает генерацию событий `Runtime.bindingCalled` для указанных имён.
         :param functions:  Список функций, или их имён.
         """
         for function in functions:
             name = function if type(function) is str else function.__name__
```

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/data.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/data.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/background_service/background_service.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/background_service/background_service.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/browser/browser.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/browser/browser.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/browser/types.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/browser/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/css/css.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/css/css.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/device_orientation/device_orientation.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/device_orientation/device_orientation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/dom.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/dom.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/dom_element.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/dom_element.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/types.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/emulation/emulation.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/emulation/emulation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/fetch/fetch.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/fetch/types.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/fetch/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/input/input.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/input/input.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/input/types.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/input/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/log/log.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/log/log.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/network/network.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/network/network.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/network/types.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/network/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/overlay/overlay.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/overlay/overlay.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/page/page.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/page/page.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/page/types.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/page/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/runtime/runtime.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/runtime/types.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/runtime/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/system_info/system_info.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/system_info/system_info.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/system_info/types.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/system_info/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/target/target.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/target/target.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/exceptions.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/extend_connection.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/extend_connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,31 @@
 
 from .exceptions import EvaluateError, JavaScriptError, NullProperty
 
 
 class Extend:
     """ Расширение для 'Page' некоторыми полезными методами.
     """
-    __slots__ = ("_connection", "action")
+    __slots__ = ("_connection", "action", "_py_call_script_id")
 
     def __init__(self, conn) -> None:
 
         from .connection import Connection
 
         self._connection: Connection = conn
+        self._py_call_script_id: str = ""
         self.action = Actions(conn)             # Совершает действия на странице. Клики;
                                                 # движения мыши; события клавиш
+
+    @property
+    def py_call_enabled(self) -> bool:
+        """ Был ли обработчик `py_call()` зарегистрирован на страницу.
+        """
+        return bool(self._py_call_script_id)
+
     async def pyCallAddOnload(self) -> None:
         """ Включает автоматически добавляющийся JavaScript, вызывающий слушателей
         клиента, добавленных на страницу с помощью await <Connection>.bindFunction(...)
         и await <Connection>.bindFunctions(...).
 
         Например, `test_func()` объявленная следующим образом:
         async def test_func(number: int, text: str, bind_arg: dict) -> None:
@@ -39,30 +47,40 @@
             test_func,                          # ! слушатель
             {"name": "test", "value": True}     # ! bind_arg
         )
 
         Может быть вызвана со страницы браузера, так:
         py_call("test_func", 1, "testtt");
         """
+        if self.py_call_enabled:
+            return
+
         py_call_js = """\
         function py_call(funcName,...args){eval(funcName+"(`"+JSON.stringify(args)+"`)");}"""
-        await self._connection.Page.addScriptOnLoad(py_call_js)
+        self._py_call_script_id = await self._connection.Page.addScriptOnLoad(py_call_js)
         await self.injectJS(py_call_js)
 
+    async def pyCallRemoveOnLoad(self) -> None:
+        """ Удаляет автоматическое добавление JavaScript, установленного
+        pyCallAddOnload().
+        """
+        if self.py_call_enabled:
+            await self._connection.Page.removeScriptOnLoad(self._py_call_script_id)
+            self._py_call_script_id = ""
+
+
     async def getViewportRect(self) -> ViewportRect:
-        """
-        Возвращает список с длиной и шириной вьюпорта браузера.
+        """ Возвращает список с длиной и шириной вьюпорта браузера.
         """
         code = "(()=>{return JSON.stringify([window.innerWidth,window.innerHeight]);})();"
         data = json.loads(await self.injectJS(code))
         return ViewportRect(int(data[0]), int(data[1]))
 
     async def getWindowRect(self) -> WindowRect:
-        """
-        Возвращает список с длиной и шириной окна браузера.
+        """ Возвращает список с длиной и шириной окна браузера.
         """
         code = "(()=>{return JSON.stringify([window.outerWidth,window.outerHeight]);})();"
         data = json.loads(await self.injectJS(code))
         return WindowRect(int(data[0]), int(data[1]))
 
     async def getUrl(self) -> str:
         return (await self._connection.Target.getTargetInfo()).url
@@ -73,16 +91,15 @@
     async def makeScreenshot(
             self,
                  format_: str = "",
                  quality: int = -1,
                    clip: Optional[dict] = None,
             fromSurface: bool = True
     ) -> bytes:
-        """
-        Сделать скриншот. Возвращает набор байт, представляющий скриншот.
+        """  Сделать скриншот. Возвращает набор байт, представляющий скриншот.
         :param format_:         jpeg или png (по умолчанию png).
         :param quality:         Качество изображения в диапазоне [0..100] (только для jpeg).
         :param clip:            {
                                     "x": "number => X offset in device independent pixels (dip).",
                                     "y": "number => Y offset in device independent pixels (dip).",
                                     "width": "number => Rectangle width in device independent pixels (dip).",
                                     "height": "number => Rectangle height in device independent pixels (dip).",
```

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol/utils.py` & `aio_dt_protocol-1.1.1/aio_dt_protocol/utils.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/PKG-INFO` & `aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-dt-protocol
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
@@ -15,14 +15,16 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Асинхронная обёртка над [протоколом](https://chromedevtools.github.io/devtools-protocol/) отладчика браузера Chromium.
 
+Запуски проводятся только в ОС Windows и Linux.
+
 ### Установка
 ```shell
 pip install aio-dt-protocol
 ```
 
 Имеет одну зависимость:
 https://github.com/aaugustin/websockets
@@ -104,15 +106,19 @@
     print("[- DONE -]")
 
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
-На страницу можно легко зарегистрировать слушателей, которые будут вызываться на стороне клиентского(Python) кода. Для этого необходимо выполнить в браузере JavaScript, передав в `console.info()` JSON-строку из JavaScript-объекта с двумя обязательными полями `func_name` - имя вызываемой python-функции и `args` - список аргументов, которые будут ей переданы. Например:
+На страницу можно легко зарегистрировать слушателей, которые будут вызываться на стороне клиентского(Python) кода. Для этого необходимо зарегистрировать вызываемую функцию в качестве такого слушателя. Это возможно выполнить двумя способами:
+1. Вручную передав методу `addBinding()` домена `Runtime` имя функции в виде строки.
+2. Воспользоваться более функциональной обёрткой первого способа, выраженной в методе `bindFunction()` соединения.
+
+Второй способ менее многословен. Под капотом он добавляет в контекст страницы утилиту `py_call()`, первым аргументом принимающую имя функции, после чего, любое кол-во позиционных аргументов, которые ожидает эта функция, а так же позволяет прикрепить любое кол-во аргументов, передаваемых в функцию последними. Например:
 
 ```python
     html = """\
     <html lang="ru">
     <head>
         <meta charset="utf-8" />
         <title>Test application</title>
@@ -124,31 +130,28 @@
         const btn = document.querySelector('#knopka');
         btn.addEventListener('click', () => {
             py_call("test_func", 1, "test")
         });
     </script>
     </html>"""
     
-    # ? Добавляем на страницу `py_call()`
-    await conn.extend.pyCallAddOnload()
-    
     # ? number и text будут переданы из браузера, а bind_arg указан при регистрации
     async def test_func(number: int, text: str, bind_arg: dict) -> None:
         print(f"[- test_func -] Called with args:\n\tnumber: {number}"
               f"\n\ttext: {text}\n\tbing_arg: {bind_arg}")
     
     
     await conn.bindFunction(
         test_func,  # ! слушатель
         {"name": "test", "value": True}  # ! bind_arg
     )
     
     # ? Если ожидается внушительный функционал прикрутить к странице, то это можно
     # ? сделать за один раз.
-    # await conn.addListeners(
+    # await conn.bindFunctions(
     #     (test_func, [ {"name": "test", "value": True} ]),
     #     # (any_awaitable1, [1, 2, 3])
     #     # (any_awaitable2, [])
     # )
     
     await conn.Page.navigate(html)
 ```
```

### Comparing `aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/SOURCES.txt` & `aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.0/setup.py` & `aio_dt_protocol-1.1.1/setup.py`

 * *Files identical despite different names*

