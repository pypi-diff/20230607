# Comparing `tmp/promptrix-0.1.0.tar.gz` & `tmp/promptrix-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptrix-0.1.0.tar", last modified: Mon Jun  5 23:20:20 2023, max compression
+gzip compressed data, was "promptrix-0.1.9.tar", last modified: Wed Jun  7 00:00:22 2023, max compression
```

## Comparing `promptrix-0.1.0.tar` & `promptrix-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:20:20.844457 promptrix-0.1.0/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.1.0/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-05 23:20:20.844457 promptrix-0.1.0/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       78 2023-06-01 23:37:06.000000 promptrix-0.1.0/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      777 2023-06-05 23:20:10.000000 promptrix-0.1.0/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-05 23:20:20.844457 promptrix-0.1.0/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:20:20.844457 promptrix-0.1.0/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:20:20.844457 promptrix-0.1.0/src/promptrix/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      746 2023-06-03 03:50:31.000000 promptrix-0.1.0/src/promptrix/AssistantMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2542 2023-06-05 23:16:40.000000 promptrix-0.1.0/src/promptrix/ConversationHistory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.1.0/src/promptrix/FunctionRegistry.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      551 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/GPT3Tokenizer.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1092 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/GroupSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5158 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/LayoutEngine.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/Prompt.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2193 2023-06-05 23:06:31.000000 promptrix-0.1.0/src/promptrix/PromptSectionBase.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/SystemMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5352 2023-06-03 03:50:22.000000 promptrix-0.1.0/src/promptrix/TemplateSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/TextSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      621 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/UserMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/Utilities.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/VolatileMemory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/promptrixTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1733 2023-06-02 18:46:08.000000 promptrix-0.1.0/src/promptrix/types.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-05 23:20:20.844457 promptrix-0.1.0/src/promptrix.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-05 23:20:20.000000 promptrix-0.1.0/src/promptrix.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      707 2023-06-05 23:20:20.000000 promptrix-0.1.0/src/promptrix.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-05 23:20:20.000000 promptrix-0.1.0/src/promptrix.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-05 23:20:20.000000 promptrix-0.1.0/src/promptrix.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-05 23:20:20.000000 promptrix-0.1.0/src/promptrix.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:00:22.707123 promptrix-0.1.9/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.1.9/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-07 00:00:22.707123 promptrix-0.1.9/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       78 2023-06-01 23:37:06.000000 promptrix-0.1.9/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      777 2023-06-06 23:55:53.000000 promptrix-0.1.9/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-07 00:00:22.707123 promptrix-0.1.9/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:00:22.703123 promptrix-0.1.9/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:00:22.707123 promptrix-0.1.9/src/promptrix/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      746 2023-06-03 03:50:31.000000 promptrix-0.1.9/src/promptrix/AssistantMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2542 2023-06-05 23:16:40.000000 promptrix-0.1.9/src/promptrix/ConversationHistory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.1.9/src/promptrix/FunctionRegistry.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      551 2023-06-02 18:46:08.000000 promptrix-0.1.9/src/promptrix/GPT3Tokenizer.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1092 2023-06-02 18:46:08.000000 promptrix-0.1.9/src/promptrix/GroupSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-06 16:17:29.000000 promptrix-0.1.9/src/promptrix/LayoutEngine.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.1.9/src/promptrix/Prompt.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2193 2023-06-06 16:18:05.000000 promptrix-0.1.9/src/promptrix/PromptSectionBase.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.1.9/src/promptrix/SystemMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5352 2023-06-03 03:50:22.000000 promptrix-0.1.9/src/promptrix/TemplateSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.1.9/src/promptrix/TextSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      621 2023-06-02 18:46:08.000000 promptrix-0.1.9/src/promptrix/UserMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-02 18:46:08.000000 promptrix-0.1.9/src/promptrix/Utilities.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-02 18:46:08.000000 promptrix-0.1.9/src/promptrix/VolatileMemory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.1.9/src/promptrix/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.1.9/src/promptrix/promptrixTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1733 2023-06-02 18:46:08.000000 promptrix-0.1.9/src/promptrix/types.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:00:22.707123 promptrix-0.1.9/src/promptrix.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-07 00:00:22.000000 promptrix-0.1.9/src/promptrix.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      733 2023-06-07 00:00:22.000000 promptrix-0.1.9/src/promptrix.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-07 00:00:22.000000 promptrix-0.1.9/src/promptrix.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-07 00:00:22.000000 promptrix-0.1.9/src/promptrix.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-07 00:00:22.000000 promptrix-0.1.9/src/promptrix.egg-info/top_level.txt
```

### Comparing `promptrix-0.1.0/LICENSE` & `promptrix-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/PKG-INFO` & `promptrix-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.1.0
+Version: 0.1.9
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.1.0/pyproject.toml` & `promptrix-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "promptrix"
-version = "0.1.0"
+version = "0.1.9"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "Promptrix. A prompt layout manager for LLMs"
```

### Comparing `promptrix-0.1.0/src/promptrix/AssistantMessage.py` & `promptrix-0.1.9/src/promptrix/AssistantMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix/ConversationHistory.py` & `promptrix-0.1.9/src/promptrix/ConversationHistory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix/FunctionRegistry.py` & `promptrix-0.1.9/src/promptrix/FunctionRegistry.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix/GPT3Tokenizer.py` & `promptrix-0.1.9/src/promptrix/GPT3Tokenizer.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix/GroupSection.py` & `promptrix-0.1.9/src/promptrix/GroupSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix/LayoutEngine.py` & `promptrix-0.1.9/src/promptrix/LayoutEngine.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         )
 
         output = [section.layout.output for section in layout if section.layout]
         text = self.separator.join(output)
         return RenderedPromptSection(text, len(tokenizer.encode(text)), remaining < 0)
 
     async def renderAsMessages(self, memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer', maxTokens: int) -> RenderedPromptSection:
+
         layout = []
         self.addSectionsToLayout(self.sections, layout)
 
         remaining = await self.layoutSections(
             layout,
             maxTokens,
             lambda section: section.renderAsMessages(memory, functions, tokenizer, maxTokens),
```

### Comparing `promptrix-0.1.0/src/promptrix/PromptSectionBase.py` & `promptrix-0.1.9/src/promptrix/PromptSectionBase.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix/TemplateSection.py` & `promptrix-0.1.9/src/promptrix/TemplateSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix/TextSection.py` & `promptrix-0.1.9/src/promptrix/TextSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix/UserMessage.py` & `promptrix-0.1.9/src/promptrix/UserMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix/Utilities.py` & `promptrix-0.1.9/src/promptrix/Utilities.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix/VolatileMemory.py` & `promptrix-0.1.9/src/promptrix/VolatileMemory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix/promptrixTypes.py` & `promptrix-0.1.9/src/promptrix/promptrixTypes.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix/types.py` & `promptrix-0.1.9/src/promptrix/types.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.1.0/src/promptrix.egg-info/PKG-INFO` & `promptrix-0.1.9/src/promptrix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.1.0
+Version: 0.1.9
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.1.0/src/promptrix.egg-info/SOURCES.txt` & `promptrix-0.1.9/src/promptrix.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/promptrix/PromptSectionBase.py
 src/promptrix/SystemMessage.py
 src/promptrix/TemplateSection.py
 src/promptrix/TextSection.py
 src/promptrix/UserMessage.py
 src/promptrix/Utilities.py
 src/promptrix/VolatileMemory.py
+src/promptrix/__init__.py
 src/promptrix/promptrixTypes.py
 src/promptrix/types.py
 src/promptrix.egg-info/PKG-INFO
 src/promptrix.egg-info/SOURCES.txt
 src/promptrix.egg-info/dependency_links.txt
 src/promptrix.egg-info/requires.txt
 src/promptrix.egg-info/top_level.txt
```

