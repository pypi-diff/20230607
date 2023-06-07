# Comparing `tmp/yt-channel-scraper-0.0.5.tar.gz` & `tmp/yt-channel-scraper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-channel-scraper-0.0.5.tar", last modified: Wed Jun  7 19:13:23 2023, max compression
+gzip compressed data, was "yt-channel-scraper-0.1.0.tar", last modified: Wed Jun  7 19:52:00 2023, max compression
```

## Comparing `yt-channel-scraper-0.0.5.tar` & `yt-channel-scraper-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:13:23.725865 yt-channel-scraper-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-07 19:13:23.725865 yt-channel-scraper-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-07 19:13:05.000000 yt-channel-scraper-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:13:23.725865 yt-channel-scraper-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-07 19:13:05.000000 yt-channel-scraper-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:13:23.721865 yt-channel-scraper-0.0.5/yt_channel_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-07 19:13:05.000000 yt-channel-scraper-0.0.5/yt_channel_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-07 19:13:05.000000 yt-channel-scraper-0.0.5/yt_channel_scraper/yt_channel_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:13:23.725865 yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-07 19:13:23.000000 yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-07 19:13:23.000000 yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:13:23.000000 yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 19:13:23.000000 yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 19:13:23.000000 yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:52:00.258614 yt-channel-scraper-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-07 19:52:00.258614 yt-channel-scraper-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-07 19:51:44.000000 yt-channel-scraper-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:52:00.258614 yt-channel-scraper-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-07 19:51:44.000000 yt-channel-scraper-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:52:00.258614 yt-channel-scraper-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-07 19:51:44.000000 yt-channel-scraper-0.1.0/tests/test_get_channel_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-07 19:51:44.000000 yt-channel-scraper-0.1.0/tests/test_get_video_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-07 19:51:44.000000 yt-channel-scraper-0.1.0/tests/test_get_video_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:52:00.258614 yt-channel-scraper-0.1.0/yt_channel_scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-07 19:51:44.000000 yt-channel-scraper-0.1.0/yt_channel_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-07 19:51:44.000000 yt-channel-scraper-0.1.0/yt_channel_scraper/yt_channel_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:52:00.258614 yt-channel-scraper-0.1.0/yt_channel_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-07 19:52:00.000000 yt-channel-scraper-0.1.0/yt_channel_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-07 19:52:00.000000 yt-channel-scraper-0.1.0/yt_channel_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:52:00.000000 yt-channel-scraper-0.1.0/yt_channel_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 19:52:00.000000 yt-channel-scraper-0.1.0/yt_channel_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 19:52:00.000000 yt-channel-scraper-0.1.0/yt_channel_scraper.egg-info/top_level.txt
```

### Comparing `yt-channel-scraper-0.0.5/PKG-INFO` & `yt-channel-scraper-0.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,10 @@
-Metadata-Version: 2.1
-Name: yt-channel-scraper
-Version: 0.0.5
-Summary: Fetch channel_id, videos, transcript from a youtube channel
-Author: Priyanshu Panwar
-Author-email: priyanshu009ch@gmail.com
-Project-URL: Source, https://github.com/priyanshu-panwar/yt-channel-scraper
-Description-Content-Type: text/markdown
-
 # yt-channel-scraper
+[![📦️Upload PyPi Package](https://github.com/priyanshu-panwar/yt-channel-scraper/actions/workflows/publish.yml/badge.svg)](https://github.com/priyanshu-panwar/yt-channel-scraper/actions/workflows/publish.yml) [![🧪Test](https://github.com/priyanshu-panwar/yt-channel-scraper/actions/workflows/test.yml/badge.svg)](https://github.com/priyanshu-panwar/yt-channel-scraper/actions/workflows/test.yml)
+
 Helps you fetch the following things of a youtube channel:
 - channel_id
 - videos (video_ids)
 - video transcripts
 
 ## channel_id
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yt-channel-scraper-0.0.5/setup.py` & `yt-channel-scraper-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme_file = Path(__file__).resolve().parent / "README.md"
 with open(readme_file, encoding="utf-8") as f:
     readme_content = f.read()
 
 setup(
     name="yt-channel-scraper",
-    version="0.0.5",
+    version="0.1.0",
     description="Fetch channel_id, videos, transcript from a youtube channel",
     long_description=readme_content,
     long_description_content_type="text/markdown",
     author="Priyanshu Panwar",
     author_email="priyanshu009ch@gmail.com",
     packages=["yt_channel_scraper"],
     project_urls={
```

### Comparing `yt-channel-scraper-0.0.5/yt_channel_scraper/yt_channel_scraper.py` & `yt-channel-scraper-0.1.0/yt_channel_scraper/yt_channel_scraper.py`

 * *Files identical despite different names*

### Comparing `yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/PKG-INFO` & `yt-channel-scraper-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: yt-channel-scraper
-Version: 0.0.5
+Version: 0.1.0
 Summary: Fetch channel_id, videos, transcript from a youtube channel
 Author: Priyanshu Panwar
 Author-email: priyanshu009ch@gmail.com
 Project-URL: Source, https://github.com/priyanshu-panwar/yt-channel-scraper
 Description-Content-Type: text/markdown
 
 # yt-channel-scraper
+[![📦️Upload PyPi Package](https://github.com/priyanshu-panwar/yt-channel-scraper/actions/workflows/publish.yml/badge.svg)](https://github.com/priyanshu-panwar/yt-channel-scraper/actions/workflows/publish.yml) [![🧪Test](https://github.com/priyanshu-panwar/yt-channel-scraper/actions/workflows/test.yml/badge.svg)](https://github.com/priyanshu-panwar/yt-channel-scraper/actions/workflows/test.yml)
+
 Helps you fetch the following things of a youtube channel:
 - channel_id
 - videos (video_ids)
 - video transcripts
 
 ## channel_id
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

