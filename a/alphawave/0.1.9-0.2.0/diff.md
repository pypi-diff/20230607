# Comparing `tmp/alphawave-0.1.9.tar.gz` & `tmp/alphawave-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.1.9.tar", last modified: Wed Jun  7 00:01:38 2023, max compression
+gzip compressed data, was "alphawave-0.2.0.tar", last modified: Wed Jun  7 00:29:06 2023, max compression
```

## Comparing `alphawave-0.1.9.tar` & `alphawave-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:01:38.413982 alphawave-0.1.9/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.1.9/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-07 00:01:38.413982 alphawave-0.1.9/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       57 2023-06-05 21:20:34.000000 alphawave-0.1.9/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      849 2023-06-06 23:55:24.000000 alphawave-0.1.9/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-07 00:01:38.413982 alphawave-0.1.9/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:01:38.409982 alphawave-0.1.9/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:01:38.413982 alphawave-0.1.9/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10339 2023-06-06 23:37:53.000000 alphawave-0.1.9/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1207 2023-06-04 00:33:26.000000 alphawave-0.1.9/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      711 2023-06-06 01:24:12.000000 alphawave-0.1.9/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3211 2023-06-06 23:45:44.000000 alphawave-0.1.9/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.1.9/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6799 2023-06-04 16:26:58.000000 alphawave-0.1.9/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7626 2023-06-06 23:47:49.000000 alphawave-0.1.9/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2301 2023-06-03 23:24:45.000000 alphawave-0.1.9/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      860 2023-06-06 01:26:32.000000 alphawave-0.1.9/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1505 2023-06-06 01:26:50.000000 alphawave-0.1.9/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.1.9/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1348 2023-06-06 23:25:38.000000 alphawave-0.1.9/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.1.9/src/alphawave/internalTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:01:38.413982 alphawave-0.1.9/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-07 00:01:38.000000 alphawave-0.1.9/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1251 2023-06-07 00:01:38.000000 alphawave-0.1.9/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-07 00:01:38.000000 alphawave-0.1.9/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       86 2023-06-07 00:01:38.000000 alphawave-0.1.9/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       27 2023-06-07 00:01:38.000000 alphawave-0.1.9/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:01:38.413982 alphawave-0.1.9/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10353 2023-06-06 21:56:16.000000 alphawave-0.1.9/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1786 2023-06-06 02:43:58.000000 alphawave-0.1.9/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1625 2023-06-06 02:37:59.000000 alphawave-0.1.9/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1462 2023-06-06 21:01:10.000000 alphawave-0.1.9/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2168 2023-06-06 17:01:33.000000 alphawave-0.1.9/src/alphawave_agents/AskCommandTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1863 2023-06-06 22:06:08.000000 alphawave-0.1.9/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.1.9/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1076 2023-06-06 16:53:04.000000 alphawave-0.1.9/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1493 2023-06-06 21:06:39.000000 alphawave-0.1.9/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1956 2023-06-06 16:58:01.000000 alphawave-0.1.9/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3506 2023-06-06 21:03:30.000000 alphawave-0.1.9/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2453 2023-06-06 22:41:49.000000 alphawave-0.1.9/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.1.9/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.1.9/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-06 18:47:10.000000 alphawave-0.1.9/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:01:38.413982 alphawave-0.1.9/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14730 2023-06-06 23:10:09.000000 alphawave-0.1.9/tests/testOpenAiClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.1.9/tests/testSchema.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:29:06.869218 alphawave-0.2.0/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.0/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-07 00:29:06.869218 alphawave-0.2.0/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       57 2023-06-05 21:20:34.000000 alphawave-0.2.0/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      849 2023-06-07 00:27:46.000000 alphawave-0.2.0/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-07 00:29:06.869218 alphawave-0.2.0/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:29:06.865218 alphawave-0.2.0/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:29:06.869218 alphawave-0.2.0/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10339 2023-06-06 23:37:53.000000 alphawave-0.2.0/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1207 2023-06-04 00:33:26.000000 alphawave-0.2.0/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      711 2023-06-06 01:24:12.000000 alphawave-0.2.0/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3211 2023-06-06 23:45:44.000000 alphawave-0.2.0/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.0/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6799 2023-06-04 16:26:58.000000 alphawave-0.2.0/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7626 2023-06-06 23:47:49.000000 alphawave-0.2.0/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2301 2023-06-03 23:24:45.000000 alphawave-0.2.0/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      789 2023-06-07 00:22:15.000000 alphawave-0.2.0/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1505 2023-06-06 01:26:50.000000 alphawave-0.2.0/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.0/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1348 2023-06-06 23:25:38.000000 alphawave-0.2.0/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.0/src/alphawave/internalTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:29:06.869218 alphawave-0.2.0/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-07 00:29:06.000000 alphawave-0.2.0/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1251 2023-06-07 00:29:06.000000 alphawave-0.2.0/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-07 00:29:06.000000 alphawave-0.2.0/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       86 2023-06-07 00:29:06.000000 alphawave-0.2.0/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       27 2023-06-07 00:29:06.000000 alphawave-0.2.0/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:29:06.869218 alphawave-0.2.0/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10353 2023-06-06 21:56:16.000000 alphawave-0.2.0/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1786 2023-06-06 02:43:58.000000 alphawave-0.2.0/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1625 2023-06-06 02:37:59.000000 alphawave-0.2.0/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1462 2023-06-06 21:01:10.000000 alphawave-0.2.0/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2168 2023-06-06 17:01:33.000000 alphawave-0.2.0/src/alphawave_agents/AskCommandTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1863 2023-06-06 22:06:08.000000 alphawave-0.2.0/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.0/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1076 2023-06-06 16:53:04.000000 alphawave-0.2.0/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1493 2023-06-06 21:06:39.000000 alphawave-0.2.0/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1956 2023-06-06 16:58:01.000000 alphawave-0.2.0/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3506 2023-06-06 21:03:30.000000 alphawave-0.2.0/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2453 2023-06-06 22:41:49.000000 alphawave-0.2.0/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.0/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.0/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-06 18:47:10.000000 alphawave-0.2.0/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:29:06.869218 alphawave-0.2.0/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14730 2023-06-06 23:10:09.000000 alphawave-0.2.0/tests/testOpenAiClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.0/tests/testSchema.py
```

### Comparing `alphawave-0.1.9/LICENSE` & `alphawave-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/PKG-INFO` & `alphawave-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.1.9
+Version: 0.2.0
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.1.9/pyproject.toml` & `alphawave-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)"
```

### Comparing `alphawave-0.1.9/src/alphawave/AlphaWave.py` & `alphawave-0.2.0/src/alphawave/AlphaWave.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave/Colorize.py` & `alphawave-0.2.0/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.2.0/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave/JSONResponseValidator.py` & `alphawave-0.2.0/src/alphawave/JSONResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave/MemoryFork.py` & `alphawave-0.2.0/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave/OSClient.py` & `alphawave-0.2.0/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave/OpenAIClient.py` & `alphawave-0.2.0/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave/Response.py` & `alphawave-0.2.0/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave/TestClient.py` & `alphawave-0.2.0/src/alphawave/TestClient.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,9 +5,8 @@
 
 class TestClient(PromptCompletionClient):
     def __init__(self, status: PromptResponseStatus = 'success', response: Union[str, Message] = {'role': 'assistant', 'content': "Hello World"}):
         self.status = status
         self.response = response
 
     async def complete_prompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
-        print( f"'status': {self.status}, 'message': {self.response}")
         return {'status': self.status, 'message': self.response}
```

### Comparing `alphawave-0.1.9/src/alphawave/TestClientTest.py` & `alphawave-0.2.0/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave/alphawaveTypes.py` & `alphawave-0.2.0/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave/internalTypes.py` & `alphawave-0.2.0/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.2.0/src/alphawave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.1.9
+Version: 0.2.0
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.1.9/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.2.0/src/alphawave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/Agent.py` & `alphawave-0.2.0/src/alphawave_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.2.0/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.2.0/src/alphawave_agents/AgentCommandValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/AskCommand.py` & `alphawave-0.2.0/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/AskCommandTest.py` & `alphawave-0.2.0/src/alphawave_agents/AskCommandTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.2.0/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.2.0/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.2.0/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/MathCommand.py` & `alphawave-0.2.0/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/PromptCommand.py` & `alphawave-0.2.0/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.2.0/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.2.0/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.2.0/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/src/alphawave_agents/agentTypes.py` & `alphawave-0.2.0/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/tests/testOpenAiClient.py` & `alphawave-0.2.0/tests/testOpenAiClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.1.9/tests/testSchema.py` & `alphawave-0.2.0/tests/testSchema.py`

 * *Files identical despite different names*

