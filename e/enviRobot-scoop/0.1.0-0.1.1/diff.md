# Comparing `tmp/enviRobot_scoop-0.1.0.tar.gz` & `tmp/enviRobot_scoop-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enviRobot_scoop-0.1.0.tar", last modified: Wed Jun  7 21:23:37 2023, max compression
+gzip compressed data, was "enviRobot_scoop-0.1.1.tar", last modified: Wed Jun  7 21:41:00 2023, max compression
```

## Comparing `enviRobot_scoop-0.1.0.tar` & `enviRobot_scoop-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 21:23:37.812420 enviRobot_scoop-0.1.0/
--rw-rw-rw-   0        0        0     1061 2023-06-07 20:47:04.000000 enviRobot_scoop-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      595 2023-06-07 21:23:37.811423 enviRobot_scoop-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      126 2023-06-06 11:02:18.000000 enviRobot_scoop-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 21:23:37.796422 enviRobot_scoop-0.1.0/enviRobot_scoop/
--rw-rw-rw-   0        0        0        0 2023-06-07 20:27:34.000000 enviRobot_scoop-0.1.0/enviRobot_scoop/__init__.py
--rw-rw-rw-   0        0        0     1111 2023-05-17 08:59:45.000000 enviRobot_scoop-0.1.0/enviRobot_scoop/aiot_screenshot.py
--rw-rw-rw-   0        0        0     3636 2023-06-07 21:18:05.000000 enviRobot_scoop-0.1.0/enviRobot_scoop/enviRobot_scoop.py
--rw-rw-rw-   0        0        0    15025 2023-06-07 21:09:27.000000 enviRobot_scoop-0.1.0/enviRobot_scoop/gpt.py
--rw-rw-rw-   0        0        0      419 2023-06-07 21:09:59.000000 enviRobot_scoop-0.1.0/enviRobot_scoop/upload_to_imgur.py
-drwxrwxrwx   0        0        0        0 2023-06-07 21:23:37.810423 enviRobot_scoop-0.1.0/enviRobot_scoop.egg-info/
--rw-rw-rw-   0        0        0      595 2023-06-07 21:23:37.000000 enviRobot_scoop-0.1.0/enviRobot_scoop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-06-07 21:23:37.000000 enviRobot_scoop-0.1.0/enviRobot_scoop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 21:23:37.000000 enviRobot_scoop-0.1.0/enviRobot_scoop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-06-07 21:23:37.000000 enviRobot_scoop-0.1.0/enviRobot_scoop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-07 21:23:37.000000 enviRobot_scoop-0.1.0/enviRobot_scoop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 21:23:37.812420 enviRobot_scoop-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-06-07 21:23:12.000000 enviRobot_scoop-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:41:00.250644 enviRobot_scoop-0.1.1/
+-rw-rw-rw-   0        0        0     1061 2023-06-07 20:47:04.000000 enviRobot_scoop-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      835 2023-06-07 21:41:00.249643 enviRobot_scoop-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-07 21:32:41.000000 enviRobot_scoop-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 21:41:00.241644 enviRobot_scoop-0.1.1/enviRobot_scoop/
+-rw-rw-rw-   0        0        0        0 2023-06-07 20:27:34.000000 enviRobot_scoop-0.1.1/enviRobot_scoop/__init__.py
+-rw-rw-rw-   0        0        0     1111 2023-05-17 08:59:45.000000 enviRobot_scoop-0.1.1/enviRobot_scoop/aiot_screenshot.py
+-rw-rw-rw-   0        0        0     3636 2023-06-07 21:18:05.000000 enviRobot_scoop-0.1.1/enviRobot_scoop/enviRobot_scoop.py
+-rw-rw-rw-   0        0        0    15025 2023-06-07 21:09:27.000000 enviRobot_scoop-0.1.1/enviRobot_scoop/gpt.py
+-rw-rw-rw-   0        0        0      419 2023-06-07 21:09:59.000000 enviRobot_scoop-0.1.1/enviRobot_scoop/upload_to_imgur.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:41:00.248644 enviRobot_scoop-0.1.1/enviRobot_scoop.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-06-07 21:41:00.000000 enviRobot_scoop-0.1.1/enviRobot_scoop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-06-07 21:41:00.000000 enviRobot_scoop-0.1.1/enviRobot_scoop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 21:41:00.000000 enviRobot_scoop-0.1.1/enviRobot_scoop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-06-07 21:41:00.000000 enviRobot_scoop-0.1.1/enviRobot_scoop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-07 21:41:00.000000 enviRobot_scoop-0.1.1/enviRobot_scoop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 21:41:00.250644 enviRobot_scoop-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-06-07 21:40:50.000000 enviRobot_scoop-0.1.1/setup.py
```

### Comparing `enviRobot_scoop-0.1.0/LICENSE` & `enviRobot_scoop-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enviRobot_scoop-0.1.0/enviRobot_scoop/aiot_screenshot.py` & `enviRobot_scoop-0.1.1/enviRobot_scoop/aiot_screenshot.py`

 * *Files identical despite different names*

### Comparing `enviRobot_scoop-0.1.0/enviRobot_scoop/enviRobot_scoop.py` & `enviRobot_scoop-0.1.1/enviRobot_scoop/enviRobot_scoop.py`

 * *Files identical despite different names*

### Comparing `enviRobot_scoop-0.1.0/enviRobot_scoop/gpt.py` & `enviRobot_scoop-0.1.1/enviRobot_scoop/gpt.py`

 * *Files identical despite different names*

### Comparing `enviRobot_scoop-0.1.0/setup.py` & `enviRobot_scoop-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 # 若Discription.md中有中文 須加上 encoding="utf-8"
 with open("README.md", "r",encoding="utf-8") as f:
     long_description = f.read()
     
 setuptools.setup(
     name = "enviRobot_scoop",
-    version = "0.1.0",
+    version = "0.1.1",
     author = "JcXGTcW",
     author_email="jcxgtcw@cameo.tw",
     description="enviRobot service that can be held by Scoop.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bohachu/ask_enviRobot",
     packages=setuptools.find_packages(),
```

