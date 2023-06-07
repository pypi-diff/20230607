# Comparing `tmp/chatai-streamer-0.0.3.tar.gz` & `tmp/chatai-streamer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-streamer-0.0.3.tar", last modified: Tue Jun  6 14:04:01 2023, max compression
+gzip compressed data, was "chatai-streamer-1.0.0.tar", last modified: Wed Jun  7 15:48:35 2023, max compression
```

## Comparing `chatai-streamer-0.0.3.tar` & `chatai-streamer-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-06 14:04:01.573235 chatai-streamer-0.0.3/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 12:23:33.000000 chatai-streamer-0.0.3/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-06 14:04:01.573235 chatai-streamer-0.0.3/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    12831 2023-06-06 13:54:02.000000 chatai-streamer-0.0.3/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-06 14:04:01.573235 chatai-streamer-0.0.3/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1172 2023-06-06 13:54:02.000000 chatai-streamer-0.0.3/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-06 14:04:01.573235 chatai-streamer-0.0.3/src/
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      929 2023-06-04 12:04:18.000000 chatai-streamer-0.0.3/src/ChatAIStreamer.py
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     4663 2023-06-06 13:54:02.000000 chatai-streamer-0.0.3/src/GttsAIStreamer.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       83 2023-06-06 13:54:02.000000 chatai-streamer-0.0.3/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-06 14:04:01.573235 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-06 14:04:01.000000 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      342 2023-06-06 14:04:01.000000 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 14:04:01.000000 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 13:54:02.000000 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      104 2023-06-06 14:04:01.000000 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       39 2023-06-06 14:04:01.000000 chatai-streamer-0.0.3/src/chatai_streamer.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 15:48:35.316642 chatai-streamer-1.0.0/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 12:23:33.000000 chatai-streamer-1.0.0/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-07 15:48:35.316642 chatai-streamer-1.0.0/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    13560 2023-06-07 15:26:42.000000 chatai-streamer-1.0.0/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-07 15:48:35.316642 chatai-streamer-1.0.0/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1172 2023-06-07 15:08:16.000000 chatai-streamer-1.0.0/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 15:48:35.316642 chatai-streamer-1.0.0/src/
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     2268 2023-06-07 15:41:22.000000 chatai-streamer-1.0.0/src/ChatAIStreamer.py
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     4694 2023-06-07 14:30:02.000000 chatai-streamer-1.0.0/src/GttsAIStreamer.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       83 2023-06-07 15:08:27.000000 chatai-streamer-1.0.0/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 15:48:35.316642 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-07 15:48:35.000000 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      342 2023-06-07 15:48:35.000000 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-07 15:48:35.000000 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 13:54:02.000000 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      104 2023-06-07 15:48:35.000000 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       39 2023-06-07 15:48:35.000000 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/top_level.txt
```

### Comparing `chatai-streamer-0.0.3/LICENSE` & `chatai-streamer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-streamer-0.0.3/PKG-INFO` & `chatai-streamer-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-streamer
-Version: 0.0.3
+Version: 1.0.0
 Summary: ChatGPT answer aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-streamer-0.0.3/README.md` & `chatai-streamer-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ChatAIStreamer
 Extention of [ChatAIStream](https://github.com/GeneralYadoc/ChatAIStream) for voice generation.
 
 ## The user of this library can
 - pick up massegase from YouTube Chat and generate answer by ChatGPT.
 - easily give role to ChatGPT.
-- add callback of voice generation and get the return through answer_cb.
+- add callback of voice generation and get the return through answer_with_voice_cb.
 
 ## How to install
 
 ### Install from PyPI
 - Install package to your environment.<br>
     ```install
     $ pip install chatai-streamer
@@ -46,15 +46,15 @@
       # There is no restriction of the type of the voice.
       ####
 
       return optimized_text, voice
 
   # callback for getting answer of ChatGPT
   # The voice generated by voiceGenerator is given as an argument.
-  def answer_cb(user_message, completion, voice):
+  def answer_with_voice_cb(user_message, completion, voice):
     #### Add Implementation here.
     # Implement for visualizing message (given as user_message).
     # Implement for visualizing ChatGPT answer (given as completion).
     # Implement for playing voice generated myVoiceGenerator.
     ####
 
   running = False
@@ -65,21 +65,25 @@
 
   # Set params of getting messages from stream source.
   stream_params=casr.streamParams(video_id=sys.argv[1])
 
   # Set params of Chat AI.
   ai_params=casr.aiParams(
     api_key = sys.argv[2],
-    system_role = "You are a cheerful assistant who speek English and can get conversation exciting with user.",
-    answer_cb = answer_cb
+    system_role = "You are a cheerful assistant who speek English and can get conversation exciting with user."
   )
 
   # Create ChatAIStreamer instance.
   ai_streamer =casr.ChatAIStreamer(
-    casr.params(stream_params=stream_params, ai_params=ai_params, voice_generator=myVoiceGenerator())
+    casr.params(
+      stream_params=stream_params,
+      ai_params=ai_params,
+      voice_generator=myVoiceGenerator(),
+      answer_with_voice_cb=answer_with_voice_cb
+    )
   )
 
   running = True
 
   # Wake up internal thread to get chat messages from stream and play voices of reading ChatGPT answers aloud.
   ai_streamer.start()
 
@@ -131,20 +135,22 @@
       time.sleep(0.01)
     if not running:
       return
     time.sleep(frac)
 
   # callback for getting answer of ChatGPT
   # The voice generated by GttsGenerator is given.
-  def answer_cb(user_message, completion, voice):
+  def answer_with_voice_cb(user_message, completion, voice):
     print(f"\n[{user_message.extern.author.name} {user_message.extern.datetime}] {user_message.message}\n")
     time_str = datetime.datetime.now().strftime ('%H:%M:%S')
     message = completion.choices[0]["message"]["content"]
 
     # Play the voice by VoicePlayer of GttsAIStreamer
+    # If you use Python launcher named py, please create proper player as follows.
+    # player = gasr.VoicePlayer(voice, python_command="py")
     player = gasr.VoicePlayer(voice)
     player.start()
 
     interruptible_sleep(3)
     print(f"[ChatGPT {time_str}] ", end='')
     print_incremental(message, 0.05)
     print("\n")
@@ -161,27 +167,31 @@
   # Set params of getting messages from stream source.
   stream_params=gasr.streamParams(video_id=sys.argv[1])
 
   # Set params of Chat AI.
   ai_params=gasr.aiParams(
     api_key = sys.argv[2],
     system_role = "You are a cheerful assistant who speek English and can get conversation exciting with user.",
-    answer_cb = answer_cb
   )
 
   # Create GttsVoiceGenerator
   # You can choose other language by its 'lang=' argument like 'ja'.
   # If you want to change language, Please change the assignment for system role of ai params also.
   # The instance isn't necessary for English generator.
   voice_generator=gasr.GttsGenerator(lang='en')
 
-  # Create GttsAIStream instance.
+  # Create GttsAIStreamer instance.
   # 'voice_generator=' is omittable for English generator.
   ai_streamer =gasr.GttsAIStreamer(
-    gasr.params(stream_params=stream_params, ai_params=ai_params, voice_generator=voice_generator)
+    gasr.params(
+      stream_params=stream_params,
+      ai_params=ai_params,
+      voice_generator=voice_generator,
+      answer_with_voice_cb=answer_with_voice_cb
+    )
   )
 
   running = True
 
   # Wake up internal thread to get chat messages from stream and play gTTS voices of reading ChatGPT answers aloud.
   ai_streamer.start()
 
@@ -225,15 +235,15 @@
   Left outputs are also available by ChatAIStreamer.
   
   [![GttsAIStreamer sample](ReadMeParts/ChatAIStreamer.png)](https://www.youtube.com/embed/sesl9VZHDA8)
 
 ## Arguments of Constructor
 - ChatAIStreamer object can be configured with following params given to constructor.
 
-  ### steamParams
+  ### streamParams
     | name | description | default |
     |------|------------|---------|
     | video_id | String following after 'v=' in url of target YouTube live | - |
     | get_item_cb | Chat items are thrown to this callback | None |
     | pre_filter_cb | Filter set before internal queue | None |
     | post_filter_cb | Filter set between internal queue and get_item_cb | None |
     | max_queue_size | Max slots of internal queue (0 is no limit) | 1000 |
@@ -242,15 +252,16 @@
   ### aiParams
     | name | description | default |
     |------|------------|---------|
     | api_key | API Key string of OpenAI | - |
     | system_role | ChatGPT role in convesation  | "You are a helpful assistant." |
     | ask_cb | user message given to ChatGPT is thrown to this callback | None |
     | max_messages_in_context | Max messages in context given to ChatGPT | 20 |
-    | answer_cb | ChatGPT answer is thrown to this callback with voice data created by your get method of voiceGenerator  | None |
+    | answer_cb | ChatGPT answer is thrown to this callback  | None |
+    | answer_with_voice_cb | ChatGPT answer is thrown to this callback with voice data created by your get method of voiceGenerator  | None |
     | max_queue_size | Max slots of internal queue (0 is no limit) | 10 |
     | model | Model of AI to be used. | None |
     | max_tokens_per_request | Max number of tokens which can be contained in a request | 256 |
     | interval_sec | Interval of ChatGPT API call | 20.0 \[sec\] |
 
   ### voiceGenerator
     | name | description | default |
@@ -310,17 +321,22 @@
 - It's required that edited chat item is returned.
 - You can avoid sending item to get_item_cb by returning None.
 ### ask_cb
 - Callback for getting questions that actually thrown to ChatGPT.
 - If you register external info to user message when you put it, you can obtain the external info here.
 - It's not be assumed that any values are returned.
 ### answer_cb
+- Callback for getting question and answer of ChatGPT.
+- The type of completion is mentioned [here](https://platform.openai.com/docs/guides/chat).
+- It's not be assumed that any values are returned.
+### answer_with_voice_cb
 - Callback for getting question and answer of ChatGPT with voice data created by your generate method of voiceGenerator.
 - The type of completion is mentioned [here](https://platform.openai.com/docs/guides/chat).
 - if you modify the answer of ChatGPT on generate method of voiceGenerator, the modification will be reflect to completion argument of this callback.
+- ask_cb and this callback are not always sequencial, since voice generation is performed on other thread in order to minimize latency.
 - It's not be assumed that any values are returned.
 
 ## Links
  uses following libraries internally.
 
 - [chatai-stream](https://github.com/GeneralYadoc/ChatAIStream)<br>
  Message broker between YouTube chat stream and ChatGPT.
```

### Comparing `chatai-streamer-0.0.3/setup.py` & `chatai-streamer-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-streamer",
-    version="0.0.3",
+    version="1.0.0",
     license="MIT",
     description="ChatGPT answer aloud YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `chatai-streamer-0.0.3/src/GttsAIStreamer.py` & `chatai-streamer-1.0.0/src/GttsAIStreamer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import pydub.playback as pb
 import noisereduce as nr
 from scipy.io import wavfile
 import ChatAIStreamer as casr
 
 ChatAIStreamer = casr.ChatAIStreamer
 streamParams = casr.streamParams
+userMessage = casr.userMessage
 aiParams = casr.aiParams
 
 TMPFILE_POSTFIX = "_GttsAIStreamer"
 
 # Data type of voice used by GttsAIStreamer 
 @dataclass
 class voiceData:
```

### Comparing `chatai-streamer-0.0.3/src/chatai_streamer.egg-info/PKG-INFO` & `chatai-streamer-1.0.0/src/chatai_streamer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-streamer
-Version: 0.0.3
+Version: 1.0.0
 Summary: ChatGPT answer aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

