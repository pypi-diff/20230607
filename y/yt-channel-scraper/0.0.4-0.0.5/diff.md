# Comparing `tmp/yt-channel-scraper-0.0.4.tar.gz` & `tmp/yt-channel-scraper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-channel-scraper-0.0.4.tar", last modified: Wed Jun  7 19:04:53 2023, max compression
+gzip compressed data, was "yt-channel-scraper-0.0.5.tar", last modified: Wed Jun  7 19:13:23 2023, max compression
```

## Comparing `yt-channel-scraper-0.0.4.tar` & `yt-channel-scraper-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:04:53.145811 yt-channel-scraper-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-07 19:04:53.145811 yt-channel-scraper-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-07 19:04:43.000000 yt-channel-scraper-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:04:53.145811 yt-channel-scraper-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-07 19:04:43.000000 yt-channel-scraper-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:04:53.145811 yt-channel-scraper-0.0.4/yt_channel_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-07 19:04:43.000000 yt-channel-scraper-0.0.4/yt_channel_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-07 19:04:43.000000 yt-channel-scraper-0.0.4/yt_channel_scraper/yt_channel_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:04:53.145811 yt-channel-scraper-0.0.4/yt_channel_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-07 19:04:53.000000 yt-channel-scraper-0.0.4/yt_channel_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-07 19:04:53.000000 yt-channel-scraper-0.0.4/yt_channel_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:04:53.000000 yt-channel-scraper-0.0.4/yt_channel_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 19:04:53.000000 yt-channel-scraper-0.0.4/yt_channel_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 19:04:53.000000 yt-channel-scraper-0.0.4/yt_channel_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:13:23.725865 yt-channel-scraper-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-07 19:13:23.725865 yt-channel-scraper-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-07 19:13:05.000000 yt-channel-scraper-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:13:23.725865 yt-channel-scraper-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-07 19:13:05.000000 yt-channel-scraper-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:13:23.721865 yt-channel-scraper-0.0.5/yt_channel_scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-07 19:13:05.000000 yt-channel-scraper-0.0.5/yt_channel_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-07 19:13:05.000000 yt-channel-scraper-0.0.5/yt_channel_scraper/yt_channel_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:13:23.725865 yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-07 19:13:23.000000 yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-07 19:13:23.000000 yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:13:23.000000 yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 19:13:23.000000 yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 19:13:23.000000 yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/top_level.txt
```

### Comparing `yt-channel-scraper-0.0.4/PKG-INFO` & `yt-channel-scraper-0.0.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: yt-channel-scraper
-Version: 0.0.4
-Summary: Fetch channel_id, videos, transcript from a youtube channel
-Author: Priyanshu Panwar
-Author-email: priyanshu009ch@gmail.com
-Description-Content-Type: text/markdown
-
 # yt-channel-scraper
 Helps you fetch the following things of a youtube channel:
 - channel_id
 - videos (video_ids)
 - video transcripts
 
 ## channel_id
```

### Comparing `yt-channel-scraper-0.0.4/README.md` & `yt-channel-scraper-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: yt-channel-scraper
+Version: 0.0.5
+Summary: Fetch channel_id, videos, transcript from a youtube channel
+Author: Priyanshu Panwar
+Author-email: priyanshu009ch@gmail.com
+Project-URL: Source, https://github.com/priyanshu-panwar/yt-channel-scraper
+Description-Content-Type: text/markdown
+
 # yt-channel-scraper
 Helps you fetch the following things of a youtube channel:
 - channel_id
 - videos (video_ids)
 - video transcripts
 
 ## channel_id
```

### Comparing `yt-channel-scraper-0.0.4/setup.py` & `yt-channel-scraper-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 
 readme_file = Path(__file__).resolve().parent / "README.md"
 with open(readme_file, encoding="utf-8") as f:
     readme_content = f.read()
 
 setup(
     name="yt-channel-scraper",
-    version="0.0.4",
+    version="0.0.5",
     description="Fetch channel_id, videos, transcript from a youtube channel",
     long_description=readme_content,
     long_description_content_type="text/markdown",
     author="Priyanshu Panwar",
     author_email="priyanshu009ch@gmail.com",
     packages=["yt_channel_scraper"],
+    project_urls={
+        "Source": "https://github.com/priyanshu-panwar/yt-channel-scraper",
+    },
     install_requires=[
         "scrapetube",
         "youtube-transcript-api",
         "requests",
         "beautifulsoup4",
     ],
 )
```

### Comparing `yt-channel-scraper-0.0.4/yt_channel_scraper/yt_channel_scraper.py` & `yt-channel-scraper-0.0.5/yt_channel_scraper/yt_channel_scraper.py`

 * *Files identical despite different names*

### Comparing `yt-channel-scraper-0.0.4/yt_channel_scraper.egg-info/PKG-INFO` & `yt-channel-scraper-0.0.5/yt_channel_scraper.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: yt-channel-scraper
-Version: 0.0.4
+Version: 0.0.5
 Summary: Fetch channel_id, videos, transcript from a youtube channel
 Author: Priyanshu Panwar
 Author-email: priyanshu009ch@gmail.com
+Project-URL: Source, https://github.com/priyanshu-panwar/yt-channel-scraper
 Description-Content-Type: text/markdown
 
 # yt-channel-scraper
 Helps you fetch the following things of a youtube channel:
 - channel_id
 - videos (video_ids)
 - video transcripts
```

