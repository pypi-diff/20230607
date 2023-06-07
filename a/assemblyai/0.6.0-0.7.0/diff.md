# Comparing `tmp/assemblyai-0.6.0.tar.gz` & `tmp/assemblyai-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyai-0.6.0.tar", last modified: Fri Jun  2 14:41:37 2023, max compression
+gzip compressed data, was "assemblyai-0.7.0.tar", last modified: Wed Jun  7 08:51:49 2023, max compression
```

## Comparing `assemblyai-0.6.0.tar` & `assemblyai-0.7.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:41:37.603315 assemblyai-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-02 14:41:28.000000 assemblyai-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-06-02 14:41:37.603315 assemblyai-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-02 14:41:28.000000 assemblyai-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:41:37.603315 assemblyai-0.6.0/assemblyai/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-02 14:41:28.000000 assemblyai-0.6.0/assemblyai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-02 14:41:28.000000 assemblyai-0.6.0/assemblyai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-02 14:41:28.000000 assemblyai-0.6.0/assemblyai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-02 14:41:28.000000 assemblyai-0.6.0/assemblyai/lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-06-02 14:41:28.000000 assemblyai-0.6.0/assemblyai/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    46497 2023-06-02 14:41:28.000000 assemblyai-0.6.0/assemblyai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:41:37.603315 assemblyai-0.6.0/assemblyai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-06-02 14:41:37.000000 assemblyai-0.6.0/assemblyai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-02 14:41:37.000000 assemblyai-0.6.0/assemblyai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:41:37.000000 assemblyai-0.6.0/assemblyai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 14:41:37.000000 assemblyai-0.6.0/assemblyai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:41:37.000000 assemblyai-0.6.0/assemblyai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:41:37.603315 assemblyai-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-02 14:41:28.000000 assemblyai-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:41:37.603315 assemblyai-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:41:28.000000 assemblyai-0.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:41:37.603315 assemblyai-0.6.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:41:28.000000 assemblyai-0.6.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-02 14:41:28.000000 assemblyai-0.6.0/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-02 14:41:28.000000 assemblyai-0.6.0/tests/unit/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-02 14:41:28.000000 assemblyai-0.6.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-02 14:41:28.000000 assemblyai-0.6.0/tests/unit/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-02 14:41:28.000000 assemblyai-0.6.0/tests/unit/test_lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-02 14:41:28.000000 assemblyai-0.6.0/tests/unit/test_summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-06-02 14:41:28.000000 assemblyai-0.6.0/tests/unit/test_transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-02 14:41:28.000000 assemblyai-0.6.0/tests/unit/test_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:49.836584 assemblyai-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-07 08:51:35.000000 assemblyai-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-07 08:51:49.836584 assemblyai-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-06-07 08:51:35.000000 assemblyai-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:49.828584 assemblyai-0.7.0/assemblyai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-07 08:51:35.000000 assemblyai-0.7.0/assemblyai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-07 08:51:35.000000 assemblyai-0.7.0/assemblyai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-07 08:51:35.000000 assemblyai-0.7.0/assemblyai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-07 08:51:35.000000 assemblyai-0.7.0/assemblyai/lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22372 2023-06-07 08:51:35.000000 assemblyai-0.7.0/assemblyai/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46689 2023-06-07 08:51:35.000000 assemblyai-0.7.0/assemblyai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:49.832584 assemblyai-0.7.0/assemblyai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-07 08:51:49.000000 assemblyai-0.7.0/assemblyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-07 08:51:49.000000 assemblyai-0.7.0/assemblyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:51:49.000000 assemblyai-0.7.0/assemblyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 08:51:49.000000 assemblyai-0.7.0/assemblyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 08:51:49.000000 assemblyai-0.7.0/assemblyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 08:51:49.836584 assemblyai-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-07 08:51:35.000000 assemblyai-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:49.832584 assemblyai-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:49.836584 assemblyai-0.7.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_auto_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.6.0/LICENSE` & `assemblyai-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `assemblyai-0.6.0/PKG-INFO` & `assemblyai-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.6.0
+Version: 0.7.0
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
@@ -49,15 +49,15 @@
 # Overview
 
 - [Documentation](#documentation)
 - [Installation](#installation)
 - [Example](#examples)
   - [Core Examples](#core-examples)
   - [LeMUR Examples](#lemur-examples)
-  - [Audio Intelligence+ Examples](#audio-intelligence-examples)
+  - [Audio Intelligence Examples](#audio-intelligence-examples)
 - [Playgrounds](#playgrounds)
 - [Advanced](#advanced-todo)
 
 # Documentation
 
 Visit our [AssemblyAI API Documentation](https://www.assemblyai.com/docs) to get an overview of our models!
 
@@ -185,43 +185,14 @@
 transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
 
 print(transcript.text)
 ```
 
 </details>
 
-<details>
-  <summary>Summarize the content of a transcript</summary>
-
-```python
-import assemblyai as aai
-
-transcriber = aai.Transcriber()
-transcript = transcriber.transcribe(
-  "https://example.org/audio.mp3",
-  config=aai.TranscriptionConfig(summarize=True)
-)
-
-print(transcript.summary)
-```
-
-By default, the summarization model will be `informative` and the summarization type will be `bullets`. [Read more about summarization models and types here](https://www.assemblyai.com/docs/Models/summarization#types-and-models).
-
-To change the model and/or type, pass additional parameters to the `TranscriptionConfig`:
-
-```python
-config=aai.TranscriptionConfig(
-  summarize=True,
-  summary_model=aai.SummarizationModel.catchy,
-  summary_type=aai.Summarizationtype.headline
-)
-```
-
-</details>
-
 ---
 
 ### **LeMUR Examples**
 
 <details>
   <summary>Use LeMUR to Summarize Multiple Transcripts</summary>
 
@@ -286,15 +257,15 @@
     print(f"Answer: {result.answer}")
 ```
 
 </details>
 
 ---
 
-### **Audio Intelligence+ Examples**
+### **Audio Intelligence Examples**
 
 <details>
   <summary>PII Redact a Transcript</summary>
 
 ```python
 import assemblyai as aai
 
@@ -313,25 +284,75 @@
 )
 
 transcriber = aai.Transcriber()
 transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
 ```
 
 </details>
+<details>
+  <summary>Summarize the content of a transcript over time</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(auto_chapters=True)
+)
+
+for chapter in transcript.chapters:
+  print(f"Summary: {chapter.summary}")  # A one paragraph summary of the content spoken during this timeframe
+  print(f"Start: {chapter.start}, End: {chapter.end}")  # Timestamps (in milliseconds) of the chapter
+  print(f"Healine: {chapter.headline}")  # A single sentence summary of the content spoken during this timeframe
+  print(f"Gist: {chapter.gist}")  # An ultra-short summary, just a few words, of the content spoken during this timeframe
+```
+
+[Read more about auto chapters here.](https://www.assemblyai.com/docs/Models/auto_chapters)
+
+</details>
+
+<details>
+  <summary>Summarize the content of a transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(summarization=True)
+)
+
+print(transcript.summary)
+```
+
+By default, the summarization model will be `informative` and the summarization type will be `bullets`. [Read more about summarization models and types here](https://www.assemblyai.com/docs/Models/summarization#types-and-models).
+
+To change the model and/or type, pass additional parameters to the `TranscriptionConfig`:
+
+```python
+config=aai.TranscriptionConfig(
+  summarization=True,
+  summary_model=aai.SummarizationModel.catchy,
+  summary_type=aai.SummarizationType.headline
+)
+```
+
+</details>
 
 ---
 
 ## Playgrounds
 
 Visit one of our Playgrounds:
 
 - [LeMUR Playground](https://www.assemblyai.com/playground/v2/source)
 - [Transcription Playground](https://www.assemblyai.com/playground)
 
-
 # Advanced
 
 ## How the SDK handles Default Configurations
 
 ### Defining Defaults
 
 When no `TranscriptionConfig` is being passed to the `Transcriber` or its methods, it will use a default instance of a `TranscriptionConfig`.
@@ -355,15 +376,14 @@
 ```python
 transcriber = aai.Transcriber()
 
 # override the `Transcriber`'s config with a new config
 transcriber.config = aai.TranscriptionConfig(punctuate=False, format_text=False)
 ```
 
-
 In case you want to override the `Transcriber`'s configuration for a specific operation with a different one, you can do so via the `config` parameter of a `.transcribe*(...)` method:
 
 ```python
 config = aai.TranscriptionConfig(punctuate=False, format_text=False)
 # set a default configuration
 transcriber = aai.Transcriber(config=config)
```

### Comparing `assemblyai-0.6.0/README.md` & `assemblyai-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # Overview
 
 - [Documentation](#documentation)
 - [Installation](#installation)
 - [Example](#examples)
   - [Core Examples](#core-examples)
   - [LeMUR Examples](#lemur-examples)
-  - [Audio Intelligence+ Examples](#audio-intelligence-examples)
+  - [Audio Intelligence Examples](#audio-intelligence-examples)
 - [Playgrounds](#playgrounds)
 - [Advanced](#advanced-todo)
 
 # Documentation
 
 Visit our [AssemblyAI API Documentation](https://www.assemblyai.com/docs) to get an overview of our models!
 
@@ -155,43 +155,14 @@
 transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
 
 print(transcript.text)
 ```
 
 </details>
 
-<details>
-  <summary>Summarize the content of a transcript</summary>
-
-```python
-import assemblyai as aai
-
-transcriber = aai.Transcriber()
-transcript = transcriber.transcribe(
-  "https://example.org/audio.mp3",
-  config=aai.TranscriptionConfig(summarize=True)
-)
-
-print(transcript.summary)
-```
-
-By default, the summarization model will be `informative` and the summarization type will be `bullets`. [Read more about summarization models and types here](https://www.assemblyai.com/docs/Models/summarization#types-and-models).
-
-To change the model and/or type, pass additional parameters to the `TranscriptionConfig`:
-
-```python
-config=aai.TranscriptionConfig(
-  summarize=True,
-  summary_model=aai.SummarizationModel.catchy,
-  summary_type=aai.Summarizationtype.headline
-)
-```
-
-</details>
-
 ---
 
 ### **LeMUR Examples**
 
 <details>
   <summary>Use LeMUR to Summarize Multiple Transcripts</summary>
 
@@ -256,15 +227,15 @@
     print(f"Answer: {result.answer}")
 ```
 
 </details>
 
 ---
 
-### **Audio Intelligence+ Examples**
+### **Audio Intelligence Examples**
 
 <details>
   <summary>PII Redact a Transcript</summary>
 
 ```python
 import assemblyai as aai
 
@@ -283,25 +254,75 @@
 )
 
 transcriber = aai.Transcriber()
 transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
 ```
 
 </details>
+<details>
+  <summary>Summarize the content of a transcript over time</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(auto_chapters=True)
+)
+
+for chapter in transcript.chapters:
+  print(f"Summary: {chapter.summary}")  # A one paragraph summary of the content spoken during this timeframe
+  print(f"Start: {chapter.start}, End: {chapter.end}")  # Timestamps (in milliseconds) of the chapter
+  print(f"Healine: {chapter.headline}")  # A single sentence summary of the content spoken during this timeframe
+  print(f"Gist: {chapter.gist}")  # An ultra-short summary, just a few words, of the content spoken during this timeframe
+```
+
+[Read more about auto chapters here.](https://www.assemblyai.com/docs/Models/auto_chapters)
+
+</details>
+
+<details>
+  <summary>Summarize the content of a transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(summarization=True)
+)
+
+print(transcript.summary)
+```
+
+By default, the summarization model will be `informative` and the summarization type will be `bullets`. [Read more about summarization models and types here](https://www.assemblyai.com/docs/Models/summarization#types-and-models).
+
+To change the model and/or type, pass additional parameters to the `TranscriptionConfig`:
+
+```python
+config=aai.TranscriptionConfig(
+  summarization=True,
+  summary_model=aai.SummarizationModel.catchy,
+  summary_type=aai.SummarizationType.headline
+)
+```
+
+</details>
 
 ---
 
 ## Playgrounds
 
 Visit one of our Playgrounds:
 
 - [LeMUR Playground](https://www.assemblyai.com/playground/v2/source)
 - [Transcription Playground](https://www.assemblyai.com/playground)
 
-
 # Advanced
 
 ## How the SDK handles Default Configurations
 
 ### Defining Defaults
 
 When no `TranscriptionConfig` is being passed to the `Transcriber` or its methods, it will use a default instance of a `TranscriptionConfig`.
@@ -325,15 +346,14 @@
 ```python
 transcriber = aai.Transcriber()
 
 # override the `Transcriber`'s config with a new config
 transcriber.config = aai.TranscriptionConfig(punctuate=False, format_text=False)
 ```
 
-
 In case you want to override the `Transcriber`'s configuration for a specific operation with a different one, you can do so via the `config` parameter of a `.transcribe*(...)` method:
 
 ```python
 config = aai.TranscriptionConfig(punctuate=False, format_text=False)
 # set a default configuration
 transcriber = aai.Transcriber(config=config)
```

### Comparing `assemblyai-0.6.0/assemblyai/__init__.py` & `assemblyai-0.7.0/assemblyai/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.6.0/assemblyai/api.py` & `assemblyai-0.7.0/assemblyai/api.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.6.0/assemblyai/client.py` & `assemblyai-0.7.0/assemblyai/client.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.6.0/assemblyai/lemur.py` & `assemblyai-0.7.0/assemblyai/lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.6.0/assemblyai/transcriber.py` & `assemblyai-0.7.0/assemblyai/transcriber.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,18 @@
     @property
     def summary(self) -> Optional[str]:
         "The summarization of the transcript"
 
         return self._impl.transcript.summary
 
     @property
+    def chapters(self) -> Optional[List[types.Chapter]]:
+        return self._impl.transcript.chapters
+
+    @property
     def status(self) -> types.TranscriptStatus:
         "The current status of the transcript"
 
         return self._impl.transcript.status
 
     @property
     def error(self) -> Optional[str]:
```

### Comparing `assemblyai-0.6.0/assemblyai/types.py` & `assemblyai-0.7.0/assemblyai/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,16 +350,16 @@
 
     disfluencies: Optional[bool]
     "Transcribe Filler Words, like 'umm', in your media file."
 
     # sentiment_analysis: bool = False
     # "Enable Sentiment Analysis."
 
-    # auto_chapters: bool = False
-    # "Enable Auto Chapters."
+    auto_chapters: Optional[bool]
+    "Enable Auto Chapters."
 
     # entity_detection: bool = False
     # "Enable Entity Detection."
 
     summarization: Optional[bool]
     "Enable Summarization"
     summary_model: Optional[SummarizationModel]
@@ -411,15 +411,15 @@
         speaker_labels: Optional[bool] = None,
         speakers_expected: Optional[int] = None,
         # content_safety: bool = False,
         # iab_categories: bool = False,
         custom_spelling: Optional[Dict[str, Union[str, Sequence[str]]]] = None,
         disfluencies: Optional[bool] = None,
         # sentiment_analysis: bool = False,
-        # auto_chapters: bool = False,
+        auto_chapters: Optional[bool] = None,
         # entity_detection: bool = False,
         summarization: Optional[bool] = None,
         summary_model: Optional[SummarizationModel] = None,
         summary_type: Optional[SummarizationType] = None,
         # auto_highlights: bool = False,
         language_detection: Optional[bool] = None,
         raw_transcription_config: Optional[RawTranscriptionConfig] = None,
@@ -487,15 +487,15 @@
         )
         self.set_speaker_diarization(speaker_labels, speakers_expected)
         # self.content_safety = content_safety
         # self.iab_categories = iab_categories
         self.set_custom_spelling(custom_spelling, override=True)
         self.disfluencies = disfluencies
         # self.sentiment_analysis = sentiment_analysis
-        # self.auto_chapters = auto_chapters
+        self.auto_chapters = auto_chapters
         # self.entity_detection = entity_detection
         self.set_summarize(
             summarization,
             summary_model,
             summary_type,
         )
         # self.auto_highlights = auto_highlights
@@ -703,25 +703,31 @@
 
     # @sentiment_analysis.setter
     # def sentiment_analysis(self, enable: bool) -> None:
     #     "Enable Sentiment Analysis."
 
     #     self._raw_transcription_config.sentiment_analysis = enable
 
-    # @property
-    # def auto_chapters(self) -> bool:
-    #     "Returns the status of the Auto Chapters feature."
+    @property
+    def auto_chapters(self) -> bool:
+        "Returns the status of the Auto Chapters feature."
+
+        return self._raw_transcription_config.auto_chapters
 
-    #     return self._raw_transcription_config.auto_chapters
+    @auto_chapters.setter
+    def auto_chapters(self, enable: bool) -> None:
+        "Enable Auto Chapters."
 
-    # @auto_chapters.setter
-    # def auto_chapters(self, enable: bool) -> None:
-    #     "Enable Auto Chapters."
+        # Validate required params are also set
+        if self.punctuate == False:
+            raise ValueError(
+                "If `auto_chapters` is enabled, then `punctuate` must not be disabled"
+            )
 
-    #     self._raw_transcription_config.auto_chapters = enable
+        self._raw_transcription_config.auto_chapters = enable
 
     # @property
     # def entity_detection(self) -> bool:
     #     "Returns whether Entity Detection feature is enabled or not."
 
     #     return self._raw_transcription_config.entity_detection
 
@@ -1313,16 +1319,16 @@
 
     disfluencies: Optional[bool]
     "Transcribe Filler Words, like 'umm', in your media file."
 
     # sentiment_analysis: bool = False
     # "Enable Sentiment Analysis."
 
-    # auto_chapters: bool = False
-    # "Enable Auto Chapters."
+    auto_chapters: Optional[bool]
+    "Enable Auto Chapters."
 
     # entity_detection: bool = False
     # "Enable Entity Detection."
 
     summarization: Optional[bool]
     "Enable Summarization"
     summary_model: Optional[SummarizationModel]
@@ -1397,15 +1403,15 @@
 
     # content_safety_labels: Optional[ContentSafetyResponse] = None
     # "The list of results when Content Safety is enabled"
 
     # iab_categories_result: Optional[IABResponse] = None
     # "The list of results when Topic Detection is enabled"
 
-    # chapters: Optional[List[Chapter]] = None
+    chapters: Optional[List[Chapter]]
     # "When Auto Chapters is enabled, the list of Auto Chapters results"
 
     # sentiment_analysis_results: Optional[List[Sentiment]] = None
     # "When Sentiment Analysis is enabled, the list of Sentiment Analysis results"
 
     # entities: Optional[List[Entity]] = None
     # "When Entity Detection is enabled, the list of detected Entities"
```

### Comparing `assemblyai-0.6.0/assemblyai.egg-info/PKG-INFO` & `assemblyai-0.7.0/assemblyai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.6.0
+Version: 0.7.0
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
@@ -49,15 +49,15 @@
 # Overview
 
 - [Documentation](#documentation)
 - [Installation](#installation)
 - [Example](#examples)
   - [Core Examples](#core-examples)
   - [LeMUR Examples](#lemur-examples)
-  - [Audio Intelligence+ Examples](#audio-intelligence-examples)
+  - [Audio Intelligence Examples](#audio-intelligence-examples)
 - [Playgrounds](#playgrounds)
 - [Advanced](#advanced-todo)
 
 # Documentation
 
 Visit our [AssemblyAI API Documentation](https://www.assemblyai.com/docs) to get an overview of our models!
 
@@ -185,43 +185,14 @@
 transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
 
 print(transcript.text)
 ```
 
 </details>
 
-<details>
-  <summary>Summarize the content of a transcript</summary>
-
-```python
-import assemblyai as aai
-
-transcriber = aai.Transcriber()
-transcript = transcriber.transcribe(
-  "https://example.org/audio.mp3",
-  config=aai.TranscriptionConfig(summarize=True)
-)
-
-print(transcript.summary)
-```
-
-By default, the summarization model will be `informative` and the summarization type will be `bullets`. [Read more about summarization models and types here](https://www.assemblyai.com/docs/Models/summarization#types-and-models).
-
-To change the model and/or type, pass additional parameters to the `TranscriptionConfig`:
-
-```python
-config=aai.TranscriptionConfig(
-  summarize=True,
-  summary_model=aai.SummarizationModel.catchy,
-  summary_type=aai.Summarizationtype.headline
-)
-```
-
-</details>
-
 ---
 
 ### **LeMUR Examples**
 
 <details>
   <summary>Use LeMUR to Summarize Multiple Transcripts</summary>
 
@@ -286,15 +257,15 @@
     print(f"Answer: {result.answer}")
 ```
 
 </details>
 
 ---
 
-### **Audio Intelligence+ Examples**
+### **Audio Intelligence Examples**
 
 <details>
   <summary>PII Redact a Transcript</summary>
 
 ```python
 import assemblyai as aai
 
@@ -313,25 +284,75 @@
 )
 
 transcriber = aai.Transcriber()
 transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
 ```
 
 </details>
+<details>
+  <summary>Summarize the content of a transcript over time</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(auto_chapters=True)
+)
+
+for chapter in transcript.chapters:
+  print(f"Summary: {chapter.summary}")  # A one paragraph summary of the content spoken during this timeframe
+  print(f"Start: {chapter.start}, End: {chapter.end}")  # Timestamps (in milliseconds) of the chapter
+  print(f"Healine: {chapter.headline}")  # A single sentence summary of the content spoken during this timeframe
+  print(f"Gist: {chapter.gist}")  # An ultra-short summary, just a few words, of the content spoken during this timeframe
+```
+
+[Read more about auto chapters here.](https://www.assemblyai.com/docs/Models/auto_chapters)
+
+</details>
+
+<details>
+  <summary>Summarize the content of a transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(summarization=True)
+)
+
+print(transcript.summary)
+```
+
+By default, the summarization model will be `informative` and the summarization type will be `bullets`. [Read more about summarization models and types here](https://www.assemblyai.com/docs/Models/summarization#types-and-models).
+
+To change the model and/or type, pass additional parameters to the `TranscriptionConfig`:
+
+```python
+config=aai.TranscriptionConfig(
+  summarization=True,
+  summary_model=aai.SummarizationModel.catchy,
+  summary_type=aai.SummarizationType.headline
+)
+```
+
+</details>
 
 ---
 
 ## Playgrounds
 
 Visit one of our Playgrounds:
 
 - [LeMUR Playground](https://www.assemblyai.com/playground/v2/source)
 - [Transcription Playground](https://www.assemblyai.com/playground)
 
-
 # Advanced
 
 ## How the SDK handles Default Configurations
 
 ### Defining Defaults
 
 When no `TranscriptionConfig` is being passed to the `Transcriber` or its methods, it will use a default instance of a `TranscriptionConfig`.
@@ -355,15 +376,14 @@
 ```python
 transcriber = aai.Transcriber()
 
 # override the `Transcriber`'s config with a new config
 transcriber.config = aai.TranscriptionConfig(punctuate=False, format_text=False)
 ```
 
-
 In case you want to override the `Transcriber`'s configuration for a specific operation with a different one, you can do so via the `config` parameter of a `.transcribe*(...)` method:
 
 ```python
 config = aai.TranscriptionConfig(punctuate=False, format_text=False)
 # set a default configuration
 transcriber = aai.Transcriber(config=config)
```

### Comparing `assemblyai-0.6.0/assemblyai.egg-info/SOURCES.txt` & `assemblyai-0.7.0/assemblyai.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 assemblyai.egg-info/dependency_links.txt
 assemblyai.egg-info/requires.txt
 assemblyai.egg-info/top_level.txt
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/factories.py
+tests/unit/test_auto_chapters.py
 tests/unit/test_config.py
 tests/unit/test_domains.py
 tests/unit/test_lemur.py
 tests/unit/test_summarization.py
 tests/unit/test_transcriber.py
 tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.6.0/setup.py` & `assemblyai-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="assemblyai",
-    version="0.6.0",
+    version="0.7.0",
     description="AssemblyAI Python SDK",
     author="AssemblyAI",
     author_email="engineering.sdk@assemblyai.com",
     packages=find_packages(),
     install_requires=[
         "httpx>=0.19.0",
         "pydantic>=1.7.0",
```

### Comparing `assemblyai-0.6.0/tests/unit/factories.py` & `assemblyai-0.7.0/tests/unit/factories.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,25 @@
 class UtteranceFactory(UtteranceWordFactory):
     class Meta:
         model = aai.Utterance
 
     words = factory.List([factory.SubFactory(UtteranceWordFactory)])
 
 
+class ChapterFactory(factory.Factory):
+    class Meta:
+        model = types.Chapter
+
+    summary = factory.Faker("sentence")
+    headline = factory.Faker("sentence")
+    gist = factory.Faker("sentence")
+    start = factory.Faker("pyint")
+    end = factory.Faker("pyint")
+
+
 class BaseTranscriptFactory(factory.Factory):
     class Meta:
         model = types.BaseTranscript
 
     language_code = aai.LanguageCode.en
     audio_url = factory.Faker("url")
     punctuate = True
```

### Comparing `assemblyai-0.6.0/tests/unit/test_domains.py` & `assemblyai-0.7.0/tests/unit/test_domains.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.6.0/tests/unit/test_lemur.py` & `assemblyai-0.7.0/tests/unit/test_lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.6.0/tests/unit/test_summarization.py` & `assemblyai-0.7.0/tests/unit/test_summarization.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.6.0/tests/unit/test_transcriber.py` & `assemblyai-0.7.0/tests/unit/test_transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.6.0/tests/unit/test_transcript.py` & `assemblyai-0.7.0/tests/unit/test_transcript.py`

 * *Files identical despite different names*

