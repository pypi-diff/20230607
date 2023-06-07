# Comparing `tmp/synonym_custom-0.0.3.tar.gz` & `tmp/synonym_custom-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synonym_custom-0.0.3.tar", last modified: Wed Jun  7 04:38:38 2023, max compression
+gzip compressed data, was "synonym_custom-0.0.4.tar", last modified: Wed Jun  7 04:31:39 2023, max compression
```

## Comparing `synonym_custom-0.0.3.tar` & `synonym_custom-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 04:38:38.700950 synonym_custom-0.0.3/
--rw-rw-rw-   0        0        0     5514 2023-06-07 04:38:38.700950 synonym_custom-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5361 2023-06-07 04:37:40.000000 synonym_custom-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 04:38:38.700950 synonym_custom-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      584 2023-06-07 04:37:59.000000 synonym_custom-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 04:38:38.667531 synonym_custom-0.0.3/synonym_custom/
--rw-rw-rw-   0        0        0        0 2023-05-25 04:22:02.000000 synonym_custom-0.0.3/synonym_custom/__init__.py
--rw-rw-rw-   0        0        0     8012 2023-06-07 03:14:44.000000 synonym_custom-0.0.3/synonym_custom/synonym_custom.py
-drwxrwxrwx   0        0        0        0 2023-06-07 04:38:38.685000 synonym_custom-0.0.3/synonym_custom.egg-info/
--rw-rw-rw-   0        0        0     5514 2023-06-07 04:38:38.000000 synonym_custom-0.0.3/synonym_custom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-07 04:38:38.000000 synonym_custom-0.0.3/synonym_custom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 04:38:38.000000 synonym_custom-0.0.3/synonym_custom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-06-07 04:38:38.000000 synonym_custom-0.0.3/synonym_custom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-07 04:38:38.000000 synonym_custom-0.0.3/synonym_custom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 04:31:39.872316 synonym_custom-0.0.4/
+-rw-rw-rw-   0        0        0     5479 2023-06-07 04:31:39.872316 synonym_custom-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5326 2023-06-07 04:29:15.000000 synonym_custom-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 04:31:39.872316 synonym_custom-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      584 2023-06-07 04:31:30.000000 synonym_custom-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:31:39.819114 synonym_custom-0.0.4/synonym_custom/
+-rw-rw-rw-   0        0        0        0 2023-05-25 04:22:02.000000 synonym_custom-0.0.4/synonym_custom/__init__.py
+-rw-rw-rw-   0        0        0     8012 2023-06-07 03:14:44.000000 synonym_custom-0.0.4/synonym_custom/synonym_custom.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:31:39.868750 synonym_custom-0.0.4/synonym_custom.egg-info/
+-rw-rw-rw-   0        0        0     5479 2023-06-07 04:31:38.000000 synonym_custom-0.0.4/synonym_custom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-07 04:31:39.000000 synonym_custom-0.0.4/synonym_custom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 04:31:39.000000 synonym_custom-0.0.4/synonym_custom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-06-07 04:31:39.000000 synonym_custom-0.0.4/synonym_custom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-07 04:31:39.000000 synonym_custom-0.0.4/synonym_custom.egg-info/top_level.txt
```

### Comparing `synonym_custom-0.0.3/PKG-INFO` & `synonym_custom-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synonym_custom
-Version: 0.0.3
+Version: 0.0.4
 Author: Sandeep Chataut
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # **KEYWORD AND SYNONYM EXTRACTION PACKAGE**
  The "synonym_custom" package is a versatile tool designed to extract keywords from a given sentence and generate synonyms for those keywords. It combines various modules and libraries to provide multiple approaches for keyword extraction and synonym generation. The package includes the following functionalities:
 
@@ -44,55 +44,48 @@
 
 ## Usage:
 
 Once you have installed the package and obtained the necessary API keys, you can import it in your Python script or interactive session:
 ```from synonym_custom.synonym_custom import Synonym_Generator```
 
 1. Using openai to extract keywords : 
-
 ```syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))```
 ```extracted_keywords = syn_gen.extract_keywords_openai(text)```
-2. Using nltk to extract keywords: 
-
+2. Using nltk to generate keywords: 
 ```syn_gen = Synonym_Generator()```
 ```extracted_keywords = syn_gen.extract_keywords_nltk(text)```
-3. Using transformers to extract keywords: 
-
+3. Using transformers to generate keywords: 
 ```syn_gen = Synonym_Generator()```
 ```extracted_keywords = syn_gen.extract_keywords_trans(text)```
-4. Using spacy to extract keywords: 
-
+4. Using spacy to generate keywords: 
 ```syn_gen = Synonym_Generator()```
 ```extracted_keywords = syn_gen.extract_keywords_spacy(text)```
 5. Using dictionary to generate synonyms: 
-
 ```synonym_list = syn_gen.dictionary_syn(keyword)```
 6. Using openai to generate synonyms: 
-
 ```synonym_list = syn_gen.openai_api(keyword)```
 7. Using spacy to generate synonyms: 
-
 ```synonym_list = syn_gen.spacy_syn(keyword)```
  
 By following these steps and providing the necessary API keys, you will be able to install and utilize the "synonym_custom" package to extract keywords from sentences and generate synonyms using multiple modules and libraries.
 
 ## Example:
-text = "Machine learning is a subfield of artificial intelligence (AI) that focuses on developing algorithms and models that enable computers to learn and make predictions or decisions without being explicitly programmed. It involves the study of statistical and computational models and algorithms that allow machines to learn from and analyze data, recognize patterns, and make data-driven predictions or decisions."
 
-`from synonym_custom.synonym_custom import Synonym_Generator`
+from synonym_custom.synonym_custom import Synonym_Generator
+text = "Machine learning is a subfield of artificial intelligence (AI) that focuses on developing algorithms and models that enable computers to learn and make predictions or decisions without being explicitly programmed. It involves the study of statistical and computational models and algorithms that allow machines to learn from and analyze data, recognize patterns, and make data-driven predictions or decisions."
 
-`syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))`  ##when using openai_api
-`syn_gen = Synonym_Generator()`
-`extracted_keywords = syn_gen.extract_keywords_spacy(text)` #using sapcy to generate keywords
-`print("Extracted Keywords:", extracted_keywords)`
-
-`synonyms_dict = {}`
-`for keyword in extracted_keywords:`
-    `synonym_list = syn_gen.dictionary_syn(keyword)` #using dictionary to generate synonyms
-    `synonyms_dict[keyword] = synonym_list`
-
-`print("Synonyms of extracted keywords:")`
-`for keyword, synonyms in synonyms_dict.items():`
-    `print(f"{keyword}: {synonyms}")`
+syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))  ##when using openai_api
+syn_gen = Synonym_Generator()
+extracted_keywords = syn_gen.extract_keywords_spacy(text) #using sapcy to generate keywords
+print("Extracted Keywords:", extracted_keywords)
+
+synonyms_dict = {}
+for keyword in extracted_keywords:
+    synonym_list = syn_gen.dictionary_syn(keyword) #using dictionary to generate synonyms
+    synonyms_dict[keyword] = synonym_list
+
+print("Synonyms of extracted keywords:")
+for keyword, synonyms in synonyms_dict.items():
+    print(f"{keyword}: {synonyms}")
```

### Comparing `synonym_custom-0.0.3/README.md` & `synonym_custom-0.0.4/synonym_custom.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: synonym-custom
+Version: 0.0.4
+Author: Sandeep Chataut
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # **KEYWORD AND SYNONYM EXTRACTION PACKAGE**
  The "synonym_custom" package is a versatile tool designed to extract keywords from a given sentence and generate synonyms for those keywords. It combines various modules and libraries to provide multiple approaches for keyword extraction and synonym generation. The package includes the following functionalities:
 
 1. Dictionary-based synonym generation: Utilizes web scraping techniques to extract synonyms from online thesaurus websites.
 
 2. Spacy-based synonym generation: Relies on the Spacy library and its WordNet annotator to generate synonyms using a lexical database.
 
@@ -37,55 +44,48 @@
 
 ## Usage:
 
 Once you have installed the package and obtained the necessary API keys, you can import it in your Python script or interactive session:
 ```from synonym_custom.synonym_custom import Synonym_Generator```
 
 1. Using openai to extract keywords : 
-
 ```syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))```
 ```extracted_keywords = syn_gen.extract_keywords_openai(text)```
-2. Using nltk to extract keywords: 
-
+2. Using nltk to generate keywords: 
 ```syn_gen = Synonym_Generator()```
 ```extracted_keywords = syn_gen.extract_keywords_nltk(text)```
-3. Using transformers to extract keywords: 
-
+3. Using transformers to generate keywords: 
 ```syn_gen = Synonym_Generator()```
 ```extracted_keywords = syn_gen.extract_keywords_trans(text)```
-4. Using spacy to extract keywords: 
-
+4. Using spacy to generate keywords: 
 ```syn_gen = Synonym_Generator()```
 ```extracted_keywords = syn_gen.extract_keywords_spacy(text)```
 5. Using dictionary to generate synonyms: 
-
 ```synonym_list = syn_gen.dictionary_syn(keyword)```
 6. Using openai to generate synonyms: 
-
 ```synonym_list = syn_gen.openai_api(keyword)```
 7. Using spacy to generate synonyms: 
-
 ```synonym_list = syn_gen.spacy_syn(keyword)```
  
 By following these steps and providing the necessary API keys, you will be able to install and utilize the "synonym_custom" package to extract keywords from sentences and generate synonyms using multiple modules and libraries.
 
 ## Example:
-text = "Machine learning is a subfield of artificial intelligence (AI) that focuses on developing algorithms and models that enable computers to learn and make predictions or decisions without being explicitly programmed. It involves the study of statistical and computational models and algorithms that allow machines to learn from and analyze data, recognize patterns, and make data-driven predictions or decisions."
 
-`from synonym_custom.synonym_custom import Synonym_Generator`
+from synonym_custom.synonym_custom import Synonym_Generator
+text = "Machine learning is a subfield of artificial intelligence (AI) that focuses on developing algorithms and models that enable computers to learn and make predictions or decisions without being explicitly programmed. It involves the study of statistical and computational models and algorithms that allow machines to learn from and analyze data, recognize patterns, and make data-driven predictions or decisions."
 
-`syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))`  ##when using openai_api
-`syn_gen = Synonym_Generator()`
-`extracted_keywords = syn_gen.extract_keywords_spacy(text)` #using sapcy to generate keywords
-`print("Extracted Keywords:", extracted_keywords)`
-
-`synonyms_dict = {}`
-`for keyword in extracted_keywords:`
-    `synonym_list = syn_gen.dictionary_syn(keyword)` #using dictionary to generate synonyms
-    `synonyms_dict[keyword] = synonym_list`
-
-`print("Synonyms of extracted keywords:")`
-`for keyword, synonyms in synonyms_dict.items():`
-    `print(f"{keyword}: {synonyms}")`
+syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))  ##when using openai_api
+syn_gen = Synonym_Generator()
+extracted_keywords = syn_gen.extract_keywords_spacy(text) #using sapcy to generate keywords
+print("Extracted Keywords:", extracted_keywords)
+
+synonyms_dict = {}
+for keyword in extracted_keywords:
+    synonym_list = syn_gen.dictionary_syn(keyword) #using dictionary to generate synonyms
+    synonyms_dict[keyword] = synonym_list
+
+print("Synonyms of extracted keywords:")
+for keyword, synonyms in synonyms_dict.items():
+    print(f"{keyword}: {synonyms}")
```

### Comparing `synonym_custom-0.0.3/setup.py` & `synonym_custom-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
 
     name='synonym_custom',
-    version='0.0.3',
+    version='0.0.4',
     packages=['synonym_custom'],
     author="Sandeep Chataut",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'openai',
         'requests',
```

### Comparing `synonym_custom-0.0.3/synonym_custom/synonym_custom.py` & `synonym_custom-0.0.4/synonym_custom/synonym_custom.py`

 * *Files identical despite different names*

### Comparing `synonym_custom-0.0.3/synonym_custom.egg-info/PKG-INFO` & `synonym_custom-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: synonym-custom
-Version: 0.0.3
-Author: Sandeep Chataut
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # **KEYWORD AND SYNONYM EXTRACTION PACKAGE**
  The "synonym_custom" package is a versatile tool designed to extract keywords from a given sentence and generate synonyms for those keywords. It combines various modules and libraries to provide multiple approaches for keyword extraction and synonym generation. The package includes the following functionalities:
 
 1. Dictionary-based synonym generation: Utilizes web scraping techniques to extract synonyms from online thesaurus websites.
 
 2. Spacy-based synonym generation: Relies on the Spacy library and its WordNet annotator to generate synonyms using a lexical database.
 
@@ -44,55 +37,48 @@
 
 ## Usage:
 
 Once you have installed the package and obtained the necessary API keys, you can import it in your Python script or interactive session:
 ```from synonym_custom.synonym_custom import Synonym_Generator```
 
 1. Using openai to extract keywords : 
-
 ```syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))```
 ```extracted_keywords = syn_gen.extract_keywords_openai(text)```
-2. Using nltk to extract keywords: 
-
+2. Using nltk to generate keywords: 
 ```syn_gen = Synonym_Generator()```
 ```extracted_keywords = syn_gen.extract_keywords_nltk(text)```
-3. Using transformers to extract keywords: 
-
+3. Using transformers to generate keywords: 
 ```syn_gen = Synonym_Generator()```
 ```extracted_keywords = syn_gen.extract_keywords_trans(text)```
-4. Using spacy to extract keywords: 
-
+4. Using spacy to generate keywords: 
 ```syn_gen = Synonym_Generator()```
 ```extracted_keywords = syn_gen.extract_keywords_spacy(text)```
 5. Using dictionary to generate synonyms: 
-
 ```synonym_list = syn_gen.dictionary_syn(keyword)```
 6. Using openai to generate synonyms: 
-
 ```synonym_list = syn_gen.openai_api(keyword)```
 7. Using spacy to generate synonyms: 
-
 ```synonym_list = syn_gen.spacy_syn(keyword)```
  
 By following these steps and providing the necessary API keys, you will be able to install and utilize the "synonym_custom" package to extract keywords from sentences and generate synonyms using multiple modules and libraries.
 
 ## Example:
-text = "Machine learning is a subfield of artificial intelligence (AI) that focuses on developing algorithms and models that enable computers to learn and make predictions or decisions without being explicitly programmed. It involves the study of statistical and computational models and algorithms that allow machines to learn from and analyze data, recognize patterns, and make data-driven predictions or decisions."
 
-`from synonym_custom.synonym_custom import Synonym_Generator`
+from synonym_custom.synonym_custom import Synonym_Generator
+text = "Machine learning is a subfield of artificial intelligence (AI) that focuses on developing algorithms and models that enable computers to learn and make predictions or decisions without being explicitly programmed. It involves the study of statistical and computational models and algorithms that allow machines to learn from and analyze data, recognize patterns, and make data-driven predictions or decisions."
 
-`syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))`  ##when using openai_api
-`syn_gen = Synonym_Generator()`
-`extracted_keywords = syn_gen.extract_keywords_spacy(text)` #using sapcy to generate keywords
-`print("Extracted Keywords:", extracted_keywords)`
-
-`synonyms_dict = {}`
-`for keyword in extracted_keywords:`
-    `synonym_list = syn_gen.dictionary_syn(keyword)` #using dictionary to generate synonyms
-    `synonyms_dict[keyword] = synonym_list`
-
-`print("Synonyms of extracted keywords:")`
-`for keyword, synonyms in synonyms_dict.items():`
-    `print(f"{keyword}: {synonyms}")`
+syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))  ##when using openai_api
+syn_gen = Synonym_Generator()
+extracted_keywords = syn_gen.extract_keywords_spacy(text) #using sapcy to generate keywords
+print("Extracted Keywords:", extracted_keywords)
+
+synonyms_dict = {}
+for keyword in extracted_keywords:
+    synonym_list = syn_gen.dictionary_syn(keyword) #using dictionary to generate synonyms
+    synonyms_dict[keyword] = synonym_list
+
+print("Synonyms of extracted keywords:")
+for keyword, synonyms in synonyms_dict.items():
+    print(f"{keyword}: {synonyms}")
```

