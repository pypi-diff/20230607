# Comparing `tmp/customChatbot-0.1.0.tar.gz` & `tmp/customChatbot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customChatbot-0.1.0.tar", last modified: Sun May  7 12:45:28 2023, max compression
+gzip compressed data, was "customChatbot-0.1.1.tar", last modified: Wed Jun  7 04:04:43 2023, max compression
```

## Comparing `customChatbot-0.1.0.tar` & `customChatbot-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 haidernakara   (501) staff       (20)        0 2023-05-07 12:45:28.118339 customChatbot-0.1.0/
--rw-r--r--   0 haidernakara   (501) staff       (20)      165 2023-05-07 12:45:28.118393 customChatbot-0.1.0/PKG-INFO
--rw-r--r--   0 haidernakara   (501) staff       (20)        0 2023-03-18 09:37:30.000000 customChatbot-0.1.0/README.md
-drwxr-xr-x   0 haidernakara   (501) staff       (20)        0 2023-05-07 12:45:28.117901 customChatbot-0.1.0/customChatbot.egg-info/
--rw-r--r--   0 haidernakara   (501) staff       (20)      165 2023-05-07 12:45:28.000000 customChatbot-0.1.0/customChatbot.egg-info/PKG-INFO
--rw-r--r--   0 haidernakara   (501) staff       (20)      215 2023-05-07 12:45:28.000000 customChatbot-0.1.0/customChatbot.egg-info/SOURCES.txt
--rw-r--r--   0 haidernakara   (501) staff       (20)        1 2023-05-07 12:45:28.000000 customChatbot-0.1.0/customChatbot.egg-info/dependency_links.txt
--rw-r--r--   0 haidernakara   (501) staff       (20)       10 2023-05-07 12:45:28.000000 customChatbot-0.1.0/customChatbot.egg-info/top_level.txt
-drwxr-xr-x   0 haidernakara   (501) staff       (20)        0 2023-05-07 12:45:28.118086 customChatbot-0.1.0/customGPT/
--rw-r--r--   0 haidernakara   (501) staff       (20)        0 2023-03-18 09:37:54.000000 customChatbot-0.1.0/customGPT/__init__.py
--rw-r--r--   0 haidernakara   (501) staff       (20)     2573 2023-03-18 11:17:07.000000 customChatbot-0.1.0/customGPT/bot.py
--rw-r--r--   0 haidernakara   (501) staff       (20)      107 2023-05-07 12:45:28.118586 customChatbot-0.1.0/setup.cfg
--rw-r--r--   0 haidernakara   (501) staff       (20)      275 2023-05-07 12:42:22.000000 customChatbot-0.1.0/setup.py
+drwxr-xr-x   0 haidernakara   (501) staff       (20)        0 2023-06-07 04:04:43.675574 customChatbot-0.1.1/
+-rw-r--r--   0 haidernakara   (501) staff       (20)      165 2023-06-07 04:04:43.675633 customChatbot-0.1.1/PKG-INFO
+-rw-r--r--   0 haidernakara   (501) staff       (20)        0 2023-03-18 09:37:30.000000 customChatbot-0.1.1/README.md
+drwxr-xr-x   0 haidernakara   (501) staff       (20)        0 2023-06-07 04:04:43.675145 customChatbot-0.1.1/customChatbot.egg-info/
+-rw-r--r--   0 haidernakara   (501) staff       (20)      165 2023-06-07 04:04:43.000000 customChatbot-0.1.1/customChatbot.egg-info/PKG-INFO
+-rw-r--r--   0 haidernakara   (501) staff       (20)      251 2023-06-07 04:04:43.000000 customChatbot-0.1.1/customChatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 haidernakara   (501) staff       (20)        1 2023-06-07 04:04:43.000000 customChatbot-0.1.1/customChatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 haidernakara   (501) staff       (20)      868 2023-06-07 04:04:43.000000 customChatbot-0.1.1/customChatbot.egg-info/requires.txt
+-rw-r--r--   0 haidernakara   (501) staff       (20)       10 2023-06-07 04:04:43.000000 customChatbot-0.1.1/customChatbot.egg-info/top_level.txt
+drwxr-xr-x   0 haidernakara   (501) staff       (20)        0 2023-06-07 04:04:43.675337 customChatbot-0.1.1/customGPT/
+-rw-r--r--   0 haidernakara   (501) staff       (20)        0 2023-03-18 09:37:54.000000 customChatbot-0.1.1/customGPT/__init__.py
+-rw-r--r--   0 haidernakara   (501) staff       (20)     2522 2023-06-07 03:45:27.000000 customChatbot-0.1.1/customGPT/bot.py
+-rw-r--r--   0 haidernakara   (501) staff       (20)      107 2023-06-07 04:04:43.675830 customChatbot-0.1.1/setup.cfg
+-rw-r--r--   0 haidernakara   (501) staff       (20)      397 2023-06-07 04:04:15.000000 customChatbot-0.1.1/setup.py
```

### Comparing `customChatbot-0.1.0/customGPT/bot.py` & `customChatbot-0.1.1/customGPT/bot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import pandas as pd
 import openai
-from openai.embeddings_utils import get_embeddings
+import pandas as pd
 from openai.embeddings_utils import distances_from_embeddings
 
 
 class CustomBot:
     def __init__(self, df, openai, context_column='context', has_embedding=False, file_name='custom_bot'):
         self.df = df
         self.openai = openai
```

