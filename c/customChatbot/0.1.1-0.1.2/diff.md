# Comparing `tmp/customChatbot-0.1.1.tar.gz` & `tmp/customChatbot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customChatbot-0.1.1.tar", last modified: Wed Jun  7 04:04:43 2023, max compression
+gzip compressed data, was "customChatbot-0.1.2.tar", last modified: Wed Jun  7 04:10:44 2023, max compression
```

## Comparing `customChatbot-0.1.1.tar` & `customChatbot-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 haidernakara   (501) staff       (20)        0 2023-06-07 04:04:43.675574 customChatbot-0.1.1/
--rw-r--r--   0 haidernakara   (501) staff       (20)      165 2023-06-07 04:04:43.675633 customChatbot-0.1.1/PKG-INFO
--rw-r--r--   0 haidernakara   (501) staff       (20)        0 2023-03-18 09:37:30.000000 customChatbot-0.1.1/README.md
-drwxr-xr-x   0 haidernakara   (501) staff       (20)        0 2023-06-07 04:04:43.675145 customChatbot-0.1.1/customChatbot.egg-info/
--rw-r--r--   0 haidernakara   (501) staff       (20)      165 2023-06-07 04:04:43.000000 customChatbot-0.1.1/customChatbot.egg-info/PKG-INFO
--rw-r--r--   0 haidernakara   (501) staff       (20)      251 2023-06-07 04:04:43.000000 customChatbot-0.1.1/customChatbot.egg-info/SOURCES.txt
--rw-r--r--   0 haidernakara   (501) staff       (20)        1 2023-06-07 04:04:43.000000 customChatbot-0.1.1/customChatbot.egg-info/dependency_links.txt
--rw-r--r--   0 haidernakara   (501) staff       (20)      868 2023-06-07 04:04:43.000000 customChatbot-0.1.1/customChatbot.egg-info/requires.txt
--rw-r--r--   0 haidernakara   (501) staff       (20)       10 2023-06-07 04:04:43.000000 customChatbot-0.1.1/customChatbot.egg-info/top_level.txt
-drwxr-xr-x   0 haidernakara   (501) staff       (20)        0 2023-06-07 04:04:43.675337 customChatbot-0.1.1/customGPT/
--rw-r--r--   0 haidernakara   (501) staff       (20)        0 2023-03-18 09:37:54.000000 customChatbot-0.1.1/customGPT/__init__.py
--rw-r--r--   0 haidernakara   (501) staff       (20)     2522 2023-06-07 03:45:27.000000 customChatbot-0.1.1/customGPT/bot.py
--rw-r--r--   0 haidernakara   (501) staff       (20)      107 2023-06-07 04:04:43.675830 customChatbot-0.1.1/setup.cfg
--rw-r--r--   0 haidernakara   (501) staff       (20)      397 2023-06-07 04:04:15.000000 customChatbot-0.1.1/setup.py
+drwxr-xr-x   0 haidernakara   (501) staff       (20)        0 2023-06-07 04:10:44.746795 customChatbot-0.1.2/
+-rw-r--r--   0 haidernakara   (501) staff       (20)      165 2023-06-07 04:10:44.746870 customChatbot-0.1.2/PKG-INFO
+-rw-r--r--   0 haidernakara   (501) staff       (20)        0 2023-03-18 09:37:30.000000 customChatbot-0.1.2/README.md
+drwxr-xr-x   0 haidernakara   (501) staff       (20)        0 2023-06-07 04:10:44.746331 customChatbot-0.1.2/customChatbot.egg-info/
+-rw-r--r--   0 haidernakara   (501) staff       (20)      165 2023-06-07 04:10:44.000000 customChatbot-0.1.2/customChatbot.egg-info/PKG-INFO
+-rw-r--r--   0 haidernakara   (501) staff       (20)      251 2023-06-07 04:10:44.000000 customChatbot-0.1.2/customChatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 haidernakara   (501) staff       (20)        1 2023-06-07 04:10:44.000000 customChatbot-0.1.2/customChatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 haidernakara   (501) staff       (20)       96 2023-06-07 04:10:44.000000 customChatbot-0.1.2/customChatbot.egg-info/requires.txt
+-rw-r--r--   0 haidernakara   (501) staff       (20)       10 2023-06-07 04:10:44.000000 customChatbot-0.1.2/customChatbot.egg-info/top_level.txt
+drwxr-xr-x   0 haidernakara   (501) staff       (20)        0 2023-06-07 04:10:44.746527 customChatbot-0.1.2/customGPT/
+-rw-r--r--   0 haidernakara   (501) staff       (20)        0 2023-03-18 09:37:54.000000 customChatbot-0.1.2/customGPT/__init__.py
+-rw-r--r--   0 haidernakara   (501) staff       (20)     2522 2023-06-07 03:45:27.000000 customChatbot-0.1.2/customGPT/bot.py
+-rw-r--r--   0 haidernakara   (501) staff       (20)      107 2023-06-07 04:10:44.747088 customChatbot-0.1.2/setup.cfg
+-rw-r--r--   0 haidernakara   (501) staff       (20)      480 2023-06-07 04:10:33.000000 customChatbot-0.1.2/setup.py
```

### Comparing `customChatbot-0.1.1/customGPT/bot.py` & `customChatbot-0.1.2/customGPT/bot.py`

 * *Files identical despite different names*

