# Comparing `tmp/chatai-streamer-1.0.0.tar.gz` & `tmp/chatai-streamer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-streamer-1.0.0.tar", last modified: Wed Jun  7 15:48:35 2023, max compression
+gzip compressed data, was "chatai-streamer-2.0.0.tar", last modified: Wed Jun  7 18:31:07 2023, max compression
```

## Comparing `chatai-streamer-1.0.0.tar` & `chatai-streamer-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 15:48:35.316642 chatai-streamer-1.0.0/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 12:23:33.000000 chatai-streamer-1.0.0/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-07 15:48:35.316642 chatai-streamer-1.0.0/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    13560 2023-06-07 15:26:42.000000 chatai-streamer-1.0.0/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-07 15:48:35.316642 chatai-streamer-1.0.0/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1172 2023-06-07 15:08:16.000000 chatai-streamer-1.0.0/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 15:48:35.316642 chatai-streamer-1.0.0/src/
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     2268 2023-06-07 15:41:22.000000 chatai-streamer-1.0.0/src/ChatAIStreamer.py
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     4694 2023-06-07 14:30:02.000000 chatai-streamer-1.0.0/src/GttsAIStreamer.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       83 2023-06-07 15:08:27.000000 chatai-streamer-1.0.0/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 15:48:35.316642 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-07 15:48:35.000000 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      342 2023-06-07 15:48:35.000000 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-07 15:48:35.000000 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 13:54:02.000000 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      104 2023-06-07 15:48:35.000000 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       39 2023-06-07 15:48:35.000000 chatai-streamer-1.0.0/src/chatai_streamer.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 18:31:07.236641 chatai-streamer-2.0.0/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 12:23:33.000000 chatai-streamer-2.0.0/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-07 18:31:07.236641 chatai-streamer-2.0.0/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    13838 2023-06-07 18:22:28.000000 chatai-streamer-2.0.0/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-07 18:31:07.236641 chatai-streamer-2.0.0/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1172 2023-06-07 18:23:04.000000 chatai-streamer-2.0.0/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 18:31:07.236641 chatai-streamer-2.0.0/src/
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     2455 2023-06-07 18:21:52.000000 chatai-streamer-2.0.0/src/ChatAIStreamer.py
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     4821 2023-06-07 17:58:19.000000 chatai-streamer-2.0.0/src/GttsAIStreamer.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       83 2023-06-07 18:23:19.000000 chatai-streamer-2.0.0/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 18:31:07.236641 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-07 18:31:07.000000 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      342 2023-06-07 18:31:07.000000 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-07 18:31:07.000000 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 13:54:02.000000 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      104 2023-06-07 18:31:07.000000 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       39 2023-06-07 18:31:07.000000 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/top_level.txt
```

### Comparing `chatai-streamer-1.0.0/LICENSE` & `chatai-streamer-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-streamer-1.0.0/PKG-INFO` & `chatai-streamer-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-streamer
-Version: 1.0.0
+Version: 2.0.0
 Summary: ChatGPT answer aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-streamer-1.0.0/README.md` & `chatai-streamer-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,21 +68,26 @@
 
   # Set params of Chat AI.
   ai_params=casr.aiParams(
     api_key = sys.argv[2],
     system_role = "You are a cheerful assistant who speek English and can get conversation exciting with user."
   )
 
+  # Set params of streamer
+  streamer_params=casr.streamerParams(
+    voice_generator=myVoiceGenerator(),
+    answer_with_voice_cb=answer_with_voice_cb
+  )
+
   # Create ChatAIStreamer instance.
   ai_streamer =casr.ChatAIStreamer(
     casr.params(
       stream_params=stream_params,
       ai_params=ai_params,
-      voice_generator=myVoiceGenerator(),
-      answer_with_voice_cb=answer_with_voice_cb
+      streamer_params=streamer_params
     )
   )
 
   running = True
 
   # Wake up internal thread to get chat messages from stream and play voices of reading ChatGPT answers aloud.
   ai_streamer.start()
@@ -173,24 +178,26 @@
     system_role = "You are a cheerful assistant who speek English and can get conversation exciting with user.",
   )
 
   # Create GttsVoiceGenerator
   # You can choose other language by its 'lang=' argument like 'ja'.
   # If you want to change language, Please change the assignment for system role of ai params also.
   # The instance isn't necessary for English generator.
-  voice_generator=gasr.GttsGenerator(lang='en')
+  streamer_params=gasr.streamerParams(
+    voice_generator=gasr.GttsGenerator(lang='en'),
+    answer_with_voice_cb=answer_with_voice_cb
+  )
 
   # Create GttsAIStreamer instance.
   # 'voice_generator=' is omittable for English generator.
   ai_streamer =gasr.GttsAIStreamer(
     gasr.params(
       stream_params=stream_params,
       ai_params=ai_params,
-      voice_generator=voice_generator,
-      answer_with_voice_cb=answer_with_voice_cb
+      streamer_params=streamer_params
     )
   )
 
   running = True
 
   # Wake up internal thread to get chat messages from stream and play gTTS voices of reading ChatGPT answers aloud.
   ai_streamer.start()
@@ -253,24 +260,25 @@
     | name | description | default |
     |------|------------|---------|
     | api_key | API Key string of OpenAI | - |
     | system_role | ChatGPT role in convesation  | "You are a helpful assistant." |
     | ask_cb | user message given to ChatGPT is thrown to this callback | None |
     | max_messages_in_context | Max messages in context given to ChatGPT | 20 |
     | answer_cb | ChatGPT answer is thrown to this callback  | None |
-    | answer_with_voice_cb | ChatGPT answer is thrown to this callback with voice data created by your get method of voiceGenerator  | None |
     | max_queue_size | Max slots of internal queue (0 is no limit) | 10 |
     | model | Model of AI to be used. | None |
     | max_tokens_per_request | Max number of tokens which can be contained in a request | 256 |
     | interval_sec | Interval of ChatGPT API call | 20.0 \[sec\] |
 
-  ### voiceGenerator
+  ### streamerParams
     | name | description | default |
     |------|------------|---------|
-    | voice_generator | the instance of inherited class of voiceGenerater made by you | - |
+    | voice_generator | the instance of inherited class of voiceGenerater made by you | None |
+    | answer_with_voice_cb | ChatGPT answer is thrown to this callback with voice data created by your get method of voiceGenerator  | None |
+    | max_queue_size | max size of internal queue which stocks GPT answer which will be given to voice Generator | 1 |
  
 ### Notice
 - Please refer [pytchat README](https://github.com/taizan-hokuto/pytchat) to know the type of YouTube Chat item used by get_item_cb, pre_filter_cb and post filter_cb.
 - Stamps in a message and messages consisted by stamps only are removed defaultly even if user doesn't set pre_filter_cb.
 - Default value of interval_sec is 20.0, since free user of OpenAI API can get only 3 completions per minitue.
 - The system role given by user remains ever as the oldest sentence of current context even if the number of messages is reached to the maximum, so ChatGPT doesn't forgot the role while current cunversation.
```

### Comparing `chatai-streamer-1.0.0/setup.py` & `chatai-streamer-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-streamer",
-    version="1.0.0",
+    version="2.0.0",
     license="MIT",
     description="ChatGPT answer aloud YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `chatai-streamer-1.0.0/src/ChatAIStreamer.py` & `chatai-streamer-2.0.0/src/ChatAIStreamer.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,30 @@
 from dataclasses import dataclass
 import ChatAIStream as cas
 
 streamParams = cas.streamParams
 userMessage = cas.userMessage
 aiParams = cas.aiParams
 
+
 class voiceGenerator(ABC):
   @abstractmethod
   def generate(self, text):
     pass
 
 @dataclass
-class params(cas.params):
+class streamerParams():
   voice_generator : voiceGenerator = None
   answer_with_voice_cb: Callable[[userMessage, any, any], None] = None
+  max_queue_size : int = 1
+
+
+@dataclass
+class params(cas.params):
+  streamer_params : streamerParams = streamerParams()
 
 @dataclass
 class answerSlot():
   user_message: any
   completion: any
 
 class ChatAIStreamer(cas.ChatAIStream):
@@ -44,21 +51,21 @@
       while self.__keeping_connection and self.__answer_queue.full():
         time.sleep(0.01)
       if self.__keeping_connection:
         self.__answer_queue.put(answerSlot(user_message=user_message, completion=completion))
 
   def __init__(self, params):
     self.__keeping_connection = False
-    self.voice_generator = params.voice_generator
+    self.voice_generator = params.streamer_params.voice_generator
     self.__answer_queue = None
     self.__answer_thread = None
     if (self.voice_generator):
-      self.__answer_queue = queue.Queue(5)
+      self.__answer_queue = queue.Queue(params.streamer_params.max_queue_size)
       self.__answer_thread = threading.Thread(target=self.__generateVoice, daemon=True)
-    self.answer_with_voice_cb = params.answer_with_voice_cb
+    self.answer_with_voice_cb = params.streamer_params.answer_with_voice_cb
 
     self.answer_cb = params.ai_params.answer_cb
     params.ai_params.answer_cb = self.my_answer_cb
     super(ChatAIStreamer, self).__init__(params)
 
   def run(self):
     self.__keeping_connection = True
```

### Comparing `chatai-streamer-1.0.0/src/GttsAIStreamer.py` & `chatai-streamer-2.0.0/src/GttsAIStreamer.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,19 +57,22 @@
       frame_rate=segment.frame_rate,
       channels=segment.channels,
       duration_seconds=segment.duration_seconds )
 
     # return voice with translated text.
     return text_en, voice
 
-# Extend params to hold voiceGenerator instance.
+# Extend streamerParams and params to hold voiceGenerator instance.
 # voice_generator is defaultly intialized with English voiceGenerator.
 @dataclass
-class params(casr.params):
+class streamerParams(casr.streamerParams):
   voice_generator : casr.voiceGenerator = GttsGenerator()
+@dataclass
+class params(casr.params):
+  streamer_params : streamerParams = streamerParams()
 
 # VoicePlayer class which plays the voice generated by GttsGenerator.
 class VoicePlayer(threading.Thread):
   def __init__(self, voice, volume=100, python_command="python3"):
     self.__voice = voice
     self.__volume = volume
     self.__python_command = python_command
```

### Comparing `chatai-streamer-1.0.0/src/chatai_streamer.egg-info/PKG-INFO` & `chatai-streamer-2.0.0/src/chatai_streamer.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-streamer
-Version: 1.0.0
+Version: 2.0.0
 Summary: ChatGPT answer aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

