# Comparing `tmp/yt-channel-scraper-0.0.2.tar.gz` & `tmp/yt-channel-scraper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-channel-scraper-0.0.2.tar", last modified: Wed Jun  7 18:49:10 2023, max compression
+gzip compressed data, was "yt-channel-scraper-0.0.3.tar", last modified: Wed Jun  7 18:52:02 2023, max compression
```

## Comparing `yt-channel-scraper-0.0.2.tar` & `yt-channel-scraper-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 18:49:10.646115 yt-channel-scraper-0.0.2/
--rw-rw-rw-   0        0        0     1028 2023-06-07 18:49:10.641128 yt-channel-scraper-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      782 2023-06-07 18:16:01.000000 yt-channel-scraper-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 18:49:10.646115 yt-channel-scraper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      689 2023-06-07 18:49:01.000000 yt-channel-scraper-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 18:49:10.508483 yt-channel-scraper-0.0.2/yt_channel_scraper/
--rw-rw-rw-   0        0        0       47 2023-06-07 18:48:18.000000 yt-channel-scraper-0.0.2/yt_channel_scraper/__init__.py
--rw-rw-rw-   0        0        0      107 2023-06-07 18:22:08.000000 yt-channel-scraper-0.0.2/yt_channel_scraper/test.py
--rw-rw-rw-   0        0        0     1557 2023-06-07 18:06:00.000000 yt-channel-scraper-0.0.2/yt_channel_scraper/yt_channel_scraper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 18:49:10.628163 yt-channel-scraper-0.0.2/yt_channel_scraper.egg-info/
--rw-rw-rw-   0        0        0     1028 2023-06-07 18:49:10.000000 yt-channel-scraper-0.0.2/yt_channel_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-06-07 18:49:10.000000 yt-channel-scraper-0.0.2/yt_channel_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 18:49:10.000000 yt-channel-scraper-0.0.2/yt_channel_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-07 18:49:10.000000 yt-channel-scraper-0.0.2/yt_channel_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-07 18:49:10.000000 yt-channel-scraper-0.0.2/yt_channel_scraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 18:52:02.275991 yt-channel-scraper-0.0.3/
+-rw-rw-rw-   0        0        0     1028 2023-06-07 18:52:02.272001 yt-channel-scraper-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      782 2023-06-07 18:16:01.000000 yt-channel-scraper-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 18:52:02.275991 yt-channel-scraper-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-06-07 18:51:52.000000 yt-channel-scraper-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:52:02.220141 yt-channel-scraper-0.0.3/yt_channel_scraper/
+-rw-rw-rw-   0        0        0       66 2023-06-07 18:51:39.000000 yt-channel-scraper-0.0.3/yt_channel_scraper/__init__.py
+-rw-rw-rw-   0        0        0      107 2023-06-07 18:51:25.000000 yt-channel-scraper-0.0.3/yt_channel_scraper/test.py
+-rw-rw-rw-   0        0        0     1557 2023-06-07 18:06:00.000000 yt-channel-scraper-0.0.3/yt_channel_scraper/yt_channel_scraper.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:52:02.271004 yt-channel-scraper-0.0.3/yt_channel_scraper.egg-info/
+-rw-rw-rw-   0        0        0     1028 2023-06-07 18:52:01.000000 yt-channel-scraper-0.0.3/yt_channel_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-06-07 18:52:02.000000 yt-channel-scraper-0.0.3/yt_channel_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 18:52:01.000000 yt-channel-scraper-0.0.3/yt_channel_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-07 18:52:01.000000 yt-channel-scraper-0.0.3/yt_channel_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-07 18:52:01.000000 yt-channel-scraper-0.0.3/yt_channel_scraper.egg-info/top_level.txt
```

### Comparing `yt-channel-scraper-0.0.2/PKG-INFO` & `yt-channel-scraper-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-channel-scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fetch channel_id, videos, transcript from a youtube channel
 Author: Priyanshu Panwar
 Author-email: priyanshu009ch@gmail.com
 Description-Content-Type: text/markdown
 
 # yt-scraper
 Helps you fetch the following things of a youtube channel:
```

### Comparing `yt-channel-scraper-0.0.2/README.md` & `yt-channel-scraper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `yt-channel-scraper-0.0.2/setup.py` & `yt-channel-scraper-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme_file = Path(__file__).resolve().parent / "README.md"
 with open(readme_file, encoding="utf-8") as f:
     readme_content = f.read()
 
 setup(
     name="yt-channel-scraper",
-    version="0.0.2",
+    version="0.0.3",
     description="Fetch channel_id, videos, transcript from a youtube channel",
     long_description=readme_content,
     long_description_content_type="text/markdown",
     author="Priyanshu Panwar",
     author_email="priyanshu009ch@gmail.com",
     packages=["yt_channel_scraper"],
     install_requires=[
```

### Comparing `yt-channel-scraper-0.0.2/yt_channel_scraper/yt_channel_scraper.py` & `yt-channel-scraper-0.0.3/yt_channel_scraper/yt_channel_scraper.py`

 * *Files identical despite different names*

### Comparing `yt-channel-scraper-0.0.2/yt_channel_scraper.egg-info/PKG-INFO` & `yt-channel-scraper-0.0.3/yt_channel_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-channel-scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fetch channel_id, videos, transcript from a youtube channel
 Author: Priyanshu Panwar
 Author-email: priyanshu009ch@gmail.com
 Description-Content-Type: text/markdown
 
 # yt-scraper
 Helps you fetch the following things of a youtube channel:
```

