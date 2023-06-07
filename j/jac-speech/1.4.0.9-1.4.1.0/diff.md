# Comparing `tmp/jac_speech-1.4.0.9.tar.gz` & `tmp/jac_speech-1.4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jac_speech-1.4.0.9.tar", last modified: Tue Feb 14 17:26:45 2023, max compression
+gzip compressed data, was "jac_speech-1.4.1.0.tar", last modified: Wed Jun  7 18:25:06 2023, max compression
```

## Comparing `jac_speech-1.4.0.9.tar` & `jac_speech-1.4.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:45.436230 jac_speech-1.4.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-14 17:26:45.436230 jac_speech-1.4.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:45.432230 jac_speech-1.4.0.9/jac_speech/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:45.436230 jac_speech-1.4.0.9/jac_speech/stt/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/stt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/stt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/stt/stt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:45.436230 jac_speech-1.4.0.9/jac_speech/vc_tts/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/vc_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/vc_tts/action_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/vc_tts/models.json
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/vc_tts/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:45.436230 jac_speech-1.4.0.9/jac_speech/vc_tts/text/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/vc_tts/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/vc_tts/text/cleaners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/vc_tts/text/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/jac_speech/vc_tts/vc_tts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:45.432230 jac_speech-1.4.0.9/jac_speech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-14 17:26:45.000000 jac_speech-1.4.0.9/jac_speech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-14 17:26:45.000000 jac_speech-1.4.0.9/jac_speech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 17:26:45.000000 jac_speech-1.4.0.9/jac_speech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-14 17:26:45.000000 jac_speech-1.4.0.9/jac_speech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-14 17:26:45.000000 jac_speech-1.4.0.9/jac_speech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 17:26:45.436230 jac_speech-1.4.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-14 17:25:58.000000 jac_speech-1.4.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.794309 jac_speech-1.4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-07 18:25:06.794309 jac_speech-1.4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.790310 jac_speech-1.4.1.0/jac_speech/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.790310 jac_speech-1.4.1.0/jac_speech/stt/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/stt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/stt/stt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.790310 jac_speech-1.4.1.0/jac_speech/vc_tts/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/vc_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/vc_tts/action_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/vc_tts/models.json
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/vc_tts/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.794309 jac_speech-1.4.1.0/jac_speech/vc_tts/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/vc_tts/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/vc_tts/text/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/vc_tts/text/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/jac_speech/vc_tts/vc_tts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.790310 jac_speech-1.4.1.0/jac_speech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-07 18:25:06.000000 jac_speech-1.4.1.0/jac_speech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-07 18:25:06.000000 jac_speech-1.4.1.0/jac_speech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:25:06.000000 jac_speech-1.4.1.0/jac_speech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-07 18:25:06.000000 jac_speech-1.4.1.0/jac_speech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 18:25:06.000000 jac_speech-1.4.1.0/jac_speech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:25:06.794309 jac_speech-1.4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-07 18:24:40.000000 jac_speech-1.4.1.0/setup.py
```

### Comparing `jac_speech-1.4.0.9/jac_speech/vc_tts/action_utils.py` & `jac_speech-1.4.1.0/jac_speech/vc_tts/action_utils.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.0.9/jac_speech/vc_tts/models.json` & `jac_speech-1.4.1.0/jac_speech/vc_tts/models.json`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.0.9/jac_speech/vc_tts/text/cleaners.py` & `jac_speech-1.4.1.0/jac_speech/vc_tts/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.0.9/jac_speech/vc_tts/text/numbers.py` & `jac_speech-1.4.1.0/jac_speech/vc_tts/text/numbers.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.0.9/jac_speech/vc_tts/vc_tts.py` & `jac_speech-1.4.1.0/jac_speech/vc_tts/vc_tts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 
 from TTS.api import TTS
 
 from fastapi import HTTPException
-from jaseci.actions.live_actions import jaseci_action
-from jaseci.actions.remote_actions import launch_server
+from jaseci.jsorc.live_actions import jaseci_action
+from jaseci.jsorc.remote_actions import launch_server
 
 from .action_utils import synthesizer
 from .text import clean_text
 
 model_name = "tts_models/en/vctk/vits"
 
 model = TTS(model_name)
```

### Comparing `jac_speech-1.4.0.9/jac_speech.egg-info/SOURCES.txt` & `jac_speech-1.4.1.0/jac_speech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

