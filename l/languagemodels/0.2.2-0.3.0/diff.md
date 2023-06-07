# Comparing `tmp/languagemodels-0.2.2.tar.gz` & `tmp/languagemodels-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.2.2.tar", last modified: Tue Jun  6 12:48:41 2023, max compression
+gzip compressed data, was "languagemodels-0.3.0.tar", last modified: Wed Jun  7 12:50:38 2023, max compression
```

## Comparing `languagemodels-0.2.2.tar` & `languagemodels-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-06 12:48:41.980648 languagemodels-0.2.2/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6295 2023-06-06 12:48:41.980648 languagemodels-0.2.2/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-06 12:48:41.976648 languagemodels-0.2.2/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8559 2023-06-06 02:10:02.000000 languagemodels-0.2.2/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     1384 2023-06-05 16:58:20.000000 languagemodels-0.2.2/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7183 2023-06-06 12:46:45.000000 languagemodels-0.2.2/languagemodels/inference.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-06 12:48:41.980648 languagemodels-0.2.2/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6295 2023-06-06 12:48:41.000000 languagemodels-0.2.2/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-06-06 12:48:41.000000 languagemodels-0.2.2/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-06 12:48:41.000000 languagemodels-0.2.2/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       49 2023-06-06 12:48:41.000000 languagemodels-0.2.2/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-06 12:48:41.000000 languagemodels-0.2.2/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-06 12:48:41.980648 languagemodels-0.2.2/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      788 2023-06-06 12:48:10.000000 languagemodels-0.2.2/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-07 12:50:38.754071 languagemodels-0.3.0/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7371 2023-06-07 12:50:38.754071 languagemodels-0.3.0/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-07 12:50:38.754071 languagemodels-0.3.0/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9821 2023-06-07 12:13:43.000000 languagemodels-0.3.0/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4414 2023-06-07 12:14:49.000000 languagemodels-0.3.0/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7633 2023-06-07 10:27:54.000000 languagemodels-0.3.0/languagemodels/inference.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-07 12:50:38.754071 languagemodels-0.3.0/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7371 2023-06-07 12:50:38.000000 languagemodels-0.3.0/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-06-07 12:50:38.000000 languagemodels-0.3.0/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-07 12:50:38.000000 languagemodels-0.3.0/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       53 2023-06-07 12:50:38.000000 languagemodels-0.3.0/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-07 12:50:38.000000 languagemodels-0.3.0/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-07 12:50:38.754071 languagemodels-0.3.0/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      792 2023-06-07 12:30:29.000000 languagemodels-0.3.0/setup.py
```

### Comparing `languagemodels-0.2.2/PKG-INFO` & `languagemodels-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.2.2
+Version: 0.3.0
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
         
         [![PyPI version](https://badge.fury.io/py/languagemodels.svg)](https://badge.fury.io/py/languagemodels)
         [![docs](https://img.shields.io/badge/docs-online-brightgreen)](https://languagemodels.netlify.app/)
-        [![Build](https://github.com/jncraton/languagemodels/actions/workflows/build.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/build.yml)
-        [![Netlify Status](https://api.netlify.com/api/v1/badges/722e625a-c6bc-4373-bd88-c017adc58c00/deploy-status)](https://app.netlify.com/sites/languagemodels/deploys)
+        [![x64 Build](https://github.com/jncraton/languagemodels/actions/workflows/build.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/build.yml)
+        [![ARM64 Build](https://github.com/jncraton/languagemodels/actions/workflows/pi.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/pi.yml)[![Netlify Status](https://api.netlify.com/api/v1/badges/722e625a-c6bc-4373-bd88-c017adc58c00/deploy-status)](https://app.netlify.com/sites/languagemodels/deploys)
         [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jncraton/languagemodels/blob/master/examples/translate.ipynb)
         [![Try with Replit Badge](https://replit.com/badge?caption=Try%20with%20Replit&variant=small)](https://replit.com/@jncraton/langaugemodels#main.py)
         
         A Python package providing simple building blocks for exploring natural language processing.
         
         ![Translation hello world example](media/hello.gif)
         
@@ -65,27 +65,14 @@
         ```python
         >>> import languagemodels as lm
         
         >>> lm.classify("Language models are useful", "positive", "negative")
         'positive'
         ```
         
-        ### Semantic Search
-        
-        Semantic search is provided to retrieve documents that may provide helpful context from a document store.
-        
-        ```python
-        >>> import languagemodels as lm
-        
-        >>> lm.store_doc("Mars is a planet")
-        >>> lm.store_doc("The sun is hot")
-        >>> lm.load_doc("What is Mars?")
-        'Mars is a planet'
-        ```
-        
         ### Extractive Question Answering
         
         ```python
         >>> import languagemodels as lm
         
         >>> lm.extract_answer("What color is the ball?", "There is a green ball and a red box")
         'green'
@@ -97,23 +84,46 @@
         >>> import languagemodels as lm
         
         >>> lm.fetch_wiki('Chemistry')
         'Chemistry is the scientific study...
         
         >>> lm.fetch_weather(41.8, -87.6)
         'Partly cloudy with a chance of rain...
+        
+        >>> lm.get_date()
+        'Friday, May 12, 2023 at 09:27AM'
         ```
         
-        ### Misc Text Tools
+        ### Semantic Search
+        
+        Semantic search is provided to retrieve documents that may provide helpful context from a document store.
         
         ```python
         >>> import languagemodels as lm
         
-        >>> get_date()
-        'Friday, May 12, 2023 at 09:27AM'
+        >>> lm.store_doc("Mars is a planet")
+        >>> lm.store_doc("The sun is hot")
+        >>> lm.load_doc("What is Mars?")
+        'Mars is a planet'
+        ```
+        
+        This can also be used to get a blend of context from stored documents:
+        
+        ```python
+        >>> import languagemodels as lm
+        
+        >>> lm.store_doc(lm.fetch_wiki("Python"))
+        >>> lm.store_doc(lm.fetch_wiki("C++"))
+        >>> lm.store_doc(lm.fetch_wiki("Javascript"))
+        >>> lm.store_doc(lm.fetch_wiki("Fortran"))
+        'multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming. It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language
+        
+        C, or c, is the third letter in the Latin alphabet, used in the modern English alphabet, the alphabets of other western European languages and others worldwide. Its name in English is cee (pronounced ), plural cees.
+        
+        a measure of the popularity of programming languages.'
         ```
         
         [Full documentation](https://languagemodels.netlify.app/)
         
         System Requirements
         -------------------
```

### Comparing `languagemodels-0.2.2/languagemodels/__init__.py` & `languagemodels-0.3.0/languagemodels/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,36 @@
 
     tokens = list_tokens(prompt)
 
     for token in tokens:
         print(f"'{token[0].replace('▁',' ')}' (token {token[1]})")
 
 
+def count_tokens(prompt: str) -> None:
+    """Counts tokens in a prompt
+
+    This function is provided for exploratory purposes only. It may return
+    slightly different counts than the underlying model and may not match the
+    tokenization of any backend API being used.
+
+    :param prompt: Prompt to use as input to tokenizer
+    :return: Nothing
+
+    Examples:
+
+    >>> count_tokens("Hello world")
+    2
+
+    >>> count_tokens("Hola mundo")
+    5
+    """
+
+    return len(list_tokens(prompt))
+
+
 def complete(prompt: str) -> str:
     """Provide one completion for a given open-ended prompt
 
     :param prompt: Prompt to use as input to the model
     :return: Completion returned from the language model
 
     Examples:
@@ -51,15 +73,24 @@
 
     >>> complete("There are many mythical creatures who") #doctest: +SKIP
     'are able to fly'
 
     >>> complete("She hid in her room until") #doctest: +SKIP
     'she was sure she was safe'
     """
-    return generate_instruct(prompt, max_tokens=200, temperature=0.7)
+
+    result = generate_instruct(
+        "Write a sentence", max_tokens=200, temperature=0.7, prefix=prompt
+    )
+
+    if result.startswith(prompt):
+        prefix_length = len(prompt)
+        return result[prefix_length:]
+    else:
+        return result
 
 
 def do(prompt: str) -> str:
     """Follow a single-turn instructional prompt
 
     :param prompt: Instructional prompt to follow
     :return: Completion returned from the language model
@@ -217,14 +248,32 @@
     >>> store_doc("The sky is blue.")
     >>> load_doc("Where is Paris?")
     'Paris is in France.'
     """
     return docs.get_match(query)
 
 
+def get_doc_context(query: str) -> str:
+    """Loads context from documents
+
+    A string representing the most relevant content from all stored documents
+    will be returned. This may be a blend of chunks from multiple documents.
+
+    :param query: Query to compare to stored documents
+    :return: Up to 128 tokens of context
+
+    >>> store_doc("Paris is in France.")
+    >>> store_doc("Paris is nice.")
+    >>> store_doc("The sky is blue.")
+    >>> get_doc_context("Where is Paris?")
+    'Paris is in France.\\n\\nParis is nice.'
+    """
+    return docs.get_context(query)
+
+
 def fetch_wiki(topic: str) -> str:
     """
     Return Wikipedia summary for a topic
 
     This function ignores the complexity of disambiguation pages and simply
     returns the first result that is not a disambiguation page
```

### Comparing `languagemodels-0.2.2/languagemodels/inference.py` & `languagemodels-0.3.0/languagemodels/inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 import os
 from huggingface_hub import hf_hub_download
 import ctranslate2
 import re
 import sentencepiece
+from tokenizers import Tokenizer
 
 
 class InferenceException(Exception):
     pass
 
 
 modelcache = {}
@@ -87,26 +88,37 @@
 
     if os.environ.get("LANGUAGEMODELS_SIZE") == "large":
         model_name = model_name.replace("base", "large")
         model_name = model_name.replace("248M", "783M")
 
     if model_name not in modelcache:
         hf_hub_download(model_name, "config.json")
-        hf_hub_download(model_name, "shared_vocabulary.txt")
-        tokenizer_path = hf_hub_download(model_name, "spiece.model")
         model_path = hf_hub_download(model_name, "model.bin")
         model_base_path = model_path[:-10]
 
-        tokenizer = sentencepiece.SentencePieceProcessor()
-        tokenizer.Load(tokenizer_path)
-
-        modelcache[model_name] = (
-            tokenizer,
-            ctranslate2.Translator(model_base_path),
-        )
+        if "minilm" in model_name.lower():
+            hf_hub_download(model_name, "vocabulary.txt")
+            tokenizer = Tokenizer.from_pretrained(model_name)
+            tokenizer.no_padding()
+            tokenizer.no_truncation()
+            modelcache[model_name] = (
+                tokenizer,
+                ctranslate2.Encoder(model_base_path),
+            )
+        else:
+            hf_hub_download(model_name, "shared_vocabulary.txt")
+            tokenizer_path = hf_hub_download(model_name, "spiece.model")
+
+            tokenizer = sentencepiece.SentencePieceProcessor()
+            tokenizer.Load(tokenizer_path)
+
+            modelcache[model_name] = (
+                tokenizer,
+                ctranslate2.Translator(model_base_path),
+            )
 
     return modelcache[model_name]
 
 
 def generate_instruct(
     prompt,
     max_tokens=200,
```

### Comparing `languagemodels-0.2.2/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.3.0/languagemodels.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.2.2
+Version: 0.3.0
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
         
         [![PyPI version](https://badge.fury.io/py/languagemodels.svg)](https://badge.fury.io/py/languagemodels)
         [![docs](https://img.shields.io/badge/docs-online-brightgreen)](https://languagemodels.netlify.app/)
-        [![Build](https://github.com/jncraton/languagemodels/actions/workflows/build.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/build.yml)
-        [![Netlify Status](https://api.netlify.com/api/v1/badges/722e625a-c6bc-4373-bd88-c017adc58c00/deploy-status)](https://app.netlify.com/sites/languagemodels/deploys)
+        [![x64 Build](https://github.com/jncraton/languagemodels/actions/workflows/build.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/build.yml)
+        [![ARM64 Build](https://github.com/jncraton/languagemodels/actions/workflows/pi.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/pi.yml)[![Netlify Status](https://api.netlify.com/api/v1/badges/722e625a-c6bc-4373-bd88-c017adc58c00/deploy-status)](https://app.netlify.com/sites/languagemodels/deploys)
         [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jncraton/languagemodels/blob/master/examples/translate.ipynb)
         [![Try with Replit Badge](https://replit.com/badge?caption=Try%20with%20Replit&variant=small)](https://replit.com/@jncraton/langaugemodels#main.py)
         
         A Python package providing simple building blocks for exploring natural language processing.
         
         ![Translation hello world example](media/hello.gif)
         
@@ -65,27 +65,14 @@
         ```python
         >>> import languagemodels as lm
         
         >>> lm.classify("Language models are useful", "positive", "negative")
         'positive'
         ```
         
-        ### Semantic Search
-        
-        Semantic search is provided to retrieve documents that may provide helpful context from a document store.
-        
-        ```python
-        >>> import languagemodels as lm
-        
-        >>> lm.store_doc("Mars is a planet")
-        >>> lm.store_doc("The sun is hot")
-        >>> lm.load_doc("What is Mars?")
-        'Mars is a planet'
-        ```
-        
         ### Extractive Question Answering
         
         ```python
         >>> import languagemodels as lm
         
         >>> lm.extract_answer("What color is the ball?", "There is a green ball and a red box")
         'green'
@@ -97,23 +84,46 @@
         >>> import languagemodels as lm
         
         >>> lm.fetch_wiki('Chemistry')
         'Chemistry is the scientific study...
         
         >>> lm.fetch_weather(41.8, -87.6)
         'Partly cloudy with a chance of rain...
+        
+        >>> lm.get_date()
+        'Friday, May 12, 2023 at 09:27AM'
         ```
         
-        ### Misc Text Tools
+        ### Semantic Search
+        
+        Semantic search is provided to retrieve documents that may provide helpful context from a document store.
         
         ```python
         >>> import languagemodels as lm
         
-        >>> get_date()
-        'Friday, May 12, 2023 at 09:27AM'
+        >>> lm.store_doc("Mars is a planet")
+        >>> lm.store_doc("The sun is hot")
+        >>> lm.load_doc("What is Mars?")
+        'Mars is a planet'
+        ```
+        
+        This can also be used to get a blend of context from stored documents:
+        
+        ```python
+        >>> import languagemodels as lm
+        
+        >>> lm.store_doc(lm.fetch_wiki("Python"))
+        >>> lm.store_doc(lm.fetch_wiki("C++"))
+        >>> lm.store_doc(lm.fetch_wiki("Javascript"))
+        >>> lm.store_doc(lm.fetch_wiki("Fortran"))
+        'multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming. It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language
+        
+        C, or c, is the third letter in the Latin alphabet, used in the modern English alphabet, the alphabets of other western European languages and others worldwide. Its name in English is cee (pronounced ), plural cees.
+        
+        a measure of the popularity of programming languages.'
         ```
         
         [Full documentation](https://languagemodels.netlify.app/)
         
         System Requirements
         -------------------
```

