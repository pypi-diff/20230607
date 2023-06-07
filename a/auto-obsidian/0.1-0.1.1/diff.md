# Comparing `tmp/auto-obsidian-0.1.tar.gz` & `tmp/auto-obsidian-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-obsidian-0.1.tar", last modified: Tue Jun  6 23:57:54 2023, max compression
+gzip compressed data, was "auto-obsidian-0.1.1.tar", last modified: Wed Jun  7 02:07:35 2023, max compression
```

## Comparing `auto-obsidian-0.1.tar` & `auto-obsidian-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-06 23:57:54.149651 auto-obsidian-0.1/
--rw-r--r--   0 iyevenko   (501) staff       (20)     2198 2023-06-06 23:57:54.149337 auto-obsidian-0.1/PKG-INFO
--rw-r--r--   0 iyevenko   (501) staff       (20)       10 2022-10-14 01:13:43.000000 auto-obsidian-0.1/README.md
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-06 23:57:54.138316 auto-obsidian-0.1/auto_obsidian.egg-info/
--rw-r--r--   0 iyevenko   (501) staff       (20)     2198 2023-06-06 23:57:54.000000 auto-obsidian-0.1/auto_obsidian.egg-info/PKG-INFO
--rw-r--r--   0 iyevenko   (501) staff       (20)      969 2023-06-06 23:57:54.000000 auto-obsidian-0.1/auto_obsidian.egg-info/SOURCES.txt
--rw-r--r--   0 iyevenko   (501) staff       (20)        1 2023-06-06 23:57:54.000000 auto-obsidian-0.1/auto_obsidian.egg-info/dependency_links.txt
--rw-r--r--   0 iyevenko   (501) staff       (20)       50 2023-06-06 23:57:54.000000 auto-obsidian-0.1/auto_obsidian.egg-info/entry_points.txt
--rw-r--r--   0 iyevenko   (501) staff       (20)      239 2023-06-06 23:57:54.000000 auto-obsidian-0.1/auto_obsidian.egg-info/requires.txt
--rw-r--r--   0 iyevenko   (501) staff       (20)       10 2023-06-06 23:57:54.000000 auto-obsidian-0.1/auto_obsidian.egg-info/top_level.txt
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-06 23:57:54.142993 auto-obsidian-0.1/metalayer/
--rw-r--r--   0 iyevenko   (501) staff       (20)      501 2023-06-06 21:18:25.000000 auto-obsidian-0.1/metalayer/__init__.py
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-06 23:57:54.144017 auto-obsidian-0.1/metalayer/auto_obsidian/
--rw-r--r--   0 iyevenko   (501) staff       (20)        0 2023-05-26 22:54:04.000000 auto-obsidian-0.1/metalayer/auto_obsidian/__init__.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     7626 2023-06-04 06:46:44.000000 auto-obsidian-0.1/metalayer/auto_obsidian/engine.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     9717 2023-06-04 05:52:33.000000 auto-obsidian-0.1/metalayer/auto_obsidian/graph.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     1623 2023-05-28 19:41:35.000000 auto-obsidian-0.1/metalayer/cache.py
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-06 23:57:54.146783 auto-obsidian-0.1/metalayer/chatgpt/
--rw-r--r--   0 iyevenko   (501) staff       (20)       46 2023-05-09 20:44:01.000000 auto-obsidian-0.1/metalayer/chatgpt/__init__.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     3906 2023-05-17 22:51:51.000000 auto-obsidian-0.1/metalayer/chatgpt/activity_log.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     2051 2023-05-26 18:01:48.000000 auto-obsidian-0.1/metalayer/chatgpt/chatgpt.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      920 2023-05-10 23:11:25.000000 auto-obsidian-0.1/metalayer/chatgpt/info_extraction.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     1095 2023-05-23 20:24:41.000000 auto-obsidian-0.1/metalayer/chatgpt/logger.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      681 2023-05-10 20:30:01.000000 auto-obsidian-0.1/metalayer/chatgpt/ocr_filtering.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     1537 2023-05-23 19:22:02.000000 auto-obsidian-0.1/metalayer/chatgpt/utils.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     6063 2023-06-06 23:19:01.000000 auto-obsidian-0.1/metalayer/consumer.py
-drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-06 23:57:54.148867 auto-obsidian-0.1/metalayer/macos/
--rw-r--r--   0 iyevenko   (501) staff       (20)        0 2023-03-19 08:53:10.000000 auto-obsidian-0.1/metalayer/macos/__init__.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      439 2023-03-19 09:22:07.000000 auto-obsidian-0.1/metalayer/macos/applescript.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      919 2023-03-19 10:13:21.000000 auto-obsidian-0.1/metalayer/macos/battery.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     7735 2023-06-06 04:44:47.000000 auto-obsidian-0.1/metalayer/macos/capture.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     2695 2023-06-02 06:18:02.000000 auto-obsidian-0.1/metalayer/macos/ocr.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      785 2023-03-19 09:22:07.000000 auto-obsidian-0.1/metalayer/macos/utils.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     2448 2023-06-06 04:13:38.000000 auto-obsidian-0.1/metalayer/main.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     5087 2023-05-27 17:07:22.000000 auto-obsidian-0.1/metalayer/obsidianize.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     3520 2023-06-03 02:33:12.000000 auto-obsidian-0.1/metalayer/ocr.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     5022 2023-06-03 04:44:47.000000 auto-obsidian-0.1/metalayer/ocr_heuristics.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     3943 2023-05-10 18:36:00.000000 auto-obsidian-0.1/metalayer/producer.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      936 2023-05-17 22:58:03.000000 auto-obsidian-0.1/metalayer/reindex.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      729 2023-06-06 23:57:34.000000 auto-obsidian-0.1/metalayer/setup.py
--rw-r--r--   0 iyevenko   (501) staff       (20)      331 2023-05-13 16:54:14.000000 auto-obsidian-0.1/metalayer/system.py
--rw-r--r--   0 iyevenko   (501) staff       (20)     2240 2023-05-05 18:06:18.000000 auto-obsidian-0.1/metalayer/utils.py
--rw-r--r--   0 iyevenko   (501) staff       (20)       38 2023-06-06 23:57:54.149765 auto-obsidian-0.1/setup.cfg
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 02:07:35.922565 auto-obsidian-0.1.1/
+-rw-r--r--   0 iyevenko   (501) staff       (20)     2200 2023-06-07 02:07:35.922309 auto-obsidian-0.1.1/PKG-INFO
+-rw-r--r--   0 iyevenko   (501) staff       (20)       10 2022-10-14 01:13:43.000000 auto-obsidian-0.1.1/README.md
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 02:07:35.913180 auto-obsidian-0.1.1/auto_obsidian.egg-info/
+-rw-r--r--   0 iyevenko   (501) staff       (20)     2200 2023-06-07 02:07:35.000000 auto-obsidian-0.1.1/auto_obsidian.egg-info/PKG-INFO
+-rw-r--r--   0 iyevenko   (501) staff       (20)      969 2023-06-07 02:07:35.000000 auto-obsidian-0.1.1/auto_obsidian.egg-info/SOURCES.txt
+-rw-r--r--   0 iyevenko   (501) staff       (20)        1 2023-06-07 02:07:35.000000 auto-obsidian-0.1.1/auto_obsidian.egg-info/dependency_links.txt
+-rw-r--r--   0 iyevenko   (501) staff       (20)       50 2023-06-07 02:07:35.000000 auto-obsidian-0.1.1/auto_obsidian.egg-info/entry_points.txt
+-rw-r--r--   0 iyevenko   (501) staff       (20)      239 2023-06-07 02:07:35.000000 auto-obsidian-0.1.1/auto_obsidian.egg-info/requires.txt
+-rw-r--r--   0 iyevenko   (501) staff       (20)       10 2023-06-07 02:07:35.000000 auto-obsidian-0.1.1/auto_obsidian.egg-info/top_level.txt
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 02:07:35.917061 auto-obsidian-0.1.1/metalayer/
+-rw-r--r--   0 iyevenko   (501) staff       (20)      468 2023-06-07 02:07:02.000000 auto-obsidian-0.1.1/metalayer/__init__.py
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 02:07:35.917932 auto-obsidian-0.1.1/metalayer/auto_obsidian/
+-rw-r--r--   0 iyevenko   (501) staff       (20)        0 2023-05-26 22:54:04.000000 auto-obsidian-0.1.1/metalayer/auto_obsidian/__init__.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     7626 2023-06-04 06:46:44.000000 auto-obsidian-0.1.1/metalayer/auto_obsidian/engine.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     9717 2023-06-04 05:52:33.000000 auto-obsidian-0.1.1/metalayer/auto_obsidian/graph.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     1623 2023-05-28 19:41:35.000000 auto-obsidian-0.1.1/metalayer/cache.py
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 02:07:35.920129 auto-obsidian-0.1.1/metalayer/chatgpt/
+-rw-r--r--   0 iyevenko   (501) staff       (20)       46 2023-05-09 20:44:01.000000 auto-obsidian-0.1.1/metalayer/chatgpt/__init__.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     3906 2023-05-17 22:51:51.000000 auto-obsidian-0.1.1/metalayer/chatgpt/activity_log.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     2051 2023-05-26 18:01:48.000000 auto-obsidian-0.1.1/metalayer/chatgpt/chatgpt.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      920 2023-05-10 23:11:25.000000 auto-obsidian-0.1.1/metalayer/chatgpt/info_extraction.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     1095 2023-05-23 20:24:41.000000 auto-obsidian-0.1.1/metalayer/chatgpt/logger.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      681 2023-05-10 20:30:01.000000 auto-obsidian-0.1.1/metalayer/chatgpt/ocr_filtering.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     1537 2023-05-23 19:22:02.000000 auto-obsidian-0.1.1/metalayer/chatgpt/utils.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     6063 2023-06-06 23:19:01.000000 auto-obsidian-0.1.1/metalayer/consumer.py
+drwxr-xr-x   0 iyevenko   (501) staff       (20)        0 2023-06-07 02:07:35.921893 auto-obsidian-0.1.1/metalayer/macos/
+-rw-r--r--   0 iyevenko   (501) staff       (20)        0 2023-03-19 08:53:10.000000 auto-obsidian-0.1.1/metalayer/macos/__init__.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      439 2023-03-19 09:22:07.000000 auto-obsidian-0.1.1/metalayer/macos/applescript.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      919 2023-03-19 10:13:21.000000 auto-obsidian-0.1.1/metalayer/macos/battery.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     7735 2023-06-06 04:44:47.000000 auto-obsidian-0.1.1/metalayer/macos/capture.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     2695 2023-06-02 06:18:02.000000 auto-obsidian-0.1.1/metalayer/macos/ocr.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      785 2023-03-19 09:22:07.000000 auto-obsidian-0.1.1/metalayer/macos/utils.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     2448 2023-06-06 04:13:38.000000 auto-obsidian-0.1.1/metalayer/main.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     5087 2023-05-27 17:07:22.000000 auto-obsidian-0.1.1/metalayer/obsidianize.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     3520 2023-06-03 02:33:12.000000 auto-obsidian-0.1.1/metalayer/ocr.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     5022 2023-06-03 04:44:47.000000 auto-obsidian-0.1.1/metalayer/ocr_heuristics.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     3943 2023-05-10 18:36:00.000000 auto-obsidian-0.1.1/metalayer/producer.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      936 2023-05-17 22:58:03.000000 auto-obsidian-0.1.1/metalayer/reindex.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      731 2023-06-07 02:07:32.000000 auto-obsidian-0.1.1/metalayer/setup.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)      331 2023-05-13 16:54:14.000000 auto-obsidian-0.1.1/metalayer/system.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)     2240 2023-05-05 18:06:18.000000 auto-obsidian-0.1.1/metalayer/utils.py
+-rw-r--r--   0 iyevenko   (501) staff       (20)       38 2023-06-07 02:07:35.922694 auto-obsidian-0.1.1/setup.cfg
```

### Comparing `auto-obsidian-0.1/PKG-INFO` & `auto-obsidian-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-obsidian
-Version: 0.1
+Version: 0.1.1
 Summary: A layer on top of your OS that understands what you're doing
 Author: Ivan Yevenko
 Author-email: iyevenko@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `auto-obsidian-0.1/auto_obsidian.egg-info/PKG-INFO` & `auto-obsidian-0.1.1/auto_obsidian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-obsidian
-Version: 0.1
+Version: 0.1.1
 Summary: A layer on top of your OS that understands what you're doing
 Author: Ivan Yevenko
 Author-email: iyevenko@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `auto-obsidian-0.1/auto_obsidian.egg-info/SOURCES.txt` & `auto-obsidian-0.1.1/auto_obsidian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/auto_obsidian/engine.py` & `auto-obsidian-0.1.1/metalayer/auto_obsidian/engine.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/auto_obsidian/graph.py` & `auto-obsidian-0.1.1/metalayer/auto_obsidian/graph.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/cache.py` & `auto-obsidian-0.1.1/metalayer/cache.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/chatgpt/activity_log.py` & `auto-obsidian-0.1.1/metalayer/chatgpt/activity_log.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/chatgpt/chatgpt.py` & `auto-obsidian-0.1.1/metalayer/chatgpt/chatgpt.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/chatgpt/info_extraction.py` & `auto-obsidian-0.1.1/metalayer/chatgpt/info_extraction.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/chatgpt/logger.py` & `auto-obsidian-0.1.1/metalayer/chatgpt/logger.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/chatgpt/ocr_filtering.py` & `auto-obsidian-0.1.1/metalayer/chatgpt/ocr_filtering.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/chatgpt/utils.py` & `auto-obsidian-0.1.1/metalayer/chatgpt/utils.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/consumer.py` & `auto-obsidian-0.1.1/metalayer/consumer.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/macos/battery.py` & `auto-obsidian-0.1.1/metalayer/macos/battery.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/macos/capture.py` & `auto-obsidian-0.1.1/metalayer/macos/capture.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/macos/ocr.py` & `auto-obsidian-0.1.1/metalayer/macos/ocr.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/macos/utils.py` & `auto-obsidian-0.1.1/metalayer/macos/utils.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/main.py` & `auto-obsidian-0.1.1/metalayer/main.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/obsidianize.py` & `auto-obsidian-0.1.1/metalayer/obsidianize.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/ocr.py` & `auto-obsidian-0.1.1/metalayer/ocr.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/ocr_heuristics.py` & `auto-obsidian-0.1.1/metalayer/ocr_heuristics.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/producer.py` & `auto-obsidian-0.1.1/metalayer/producer.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/reindex.py` & `auto-obsidian-0.1.1/metalayer/reindex.py`

 * *Files identical despite different names*

### Comparing `auto-obsidian-0.1/metalayer/setup.py` & `auto-obsidian-0.1.1/metalayer/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 with open('metalayer/requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='auto-obsidian',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     description="A layer on top of your OS that understands what you're doing",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ivan Yevenko',
     author_email='iyevenko@gmail.com',
     license='MIT',
```

### Comparing `auto-obsidian-0.1/metalayer/utils.py` & `auto-obsidian-0.1.1/metalayer/utils.py`

 * *Files identical despite different names*

