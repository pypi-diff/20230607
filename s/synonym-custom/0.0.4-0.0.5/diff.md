# Comparing `tmp/synonym_custom-0.0.4.tar.gz` & `tmp/synonym_custom-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synonym_custom-0.0.4.tar", last modified: Wed Jun  7 04:31:39 2023, max compression
+gzip compressed data, was "synonym_custom-0.0.5.tar", last modified: Wed Jun  7 04:44:00 2023, max compression
```

## Comparing `synonym_custom-0.0.4.tar` & `synonym_custom-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 04:31:39.872316 synonym_custom-0.0.4/
--rw-rw-rw-   0        0        0     5479 2023-06-07 04:31:39.872316 synonym_custom-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5326 2023-06-07 04:29:15.000000 synonym_custom-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 04:31:39.872316 synonym_custom-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      584 2023-06-07 04:31:30.000000 synonym_custom-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 04:31:39.819114 synonym_custom-0.0.4/synonym_custom/
--rw-rw-rw-   0        0        0        0 2023-05-25 04:22:02.000000 synonym_custom-0.0.4/synonym_custom/__init__.py
--rw-rw-rw-   0        0        0     8012 2023-06-07 03:14:44.000000 synonym_custom-0.0.4/synonym_custom/synonym_custom.py
-drwxrwxrwx   0        0        0        0 2023-06-07 04:31:39.868750 synonym_custom-0.0.4/synonym_custom.egg-info/
--rw-rw-rw-   0        0        0     5479 2023-06-07 04:31:38.000000 synonym_custom-0.0.4/synonym_custom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-07 04:31:39.000000 synonym_custom-0.0.4/synonym_custom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 04:31:39.000000 synonym_custom-0.0.4/synonym_custom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-06-07 04:31:39.000000 synonym_custom-0.0.4/synonym_custom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-07 04:31:39.000000 synonym_custom-0.0.4/synonym_custom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 04:44:00.418612 synonym_custom-0.0.5/
+-rw-rw-rw-   0        0        0     5554 2023-06-07 04:44:00.418612 synonym_custom-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5401 2023-06-07 04:43:04.000000 synonym_custom-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 04:44:00.418612 synonym_custom-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      584 2023-06-07 04:43:40.000000 synonym_custom-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:44:00.402977 synonym_custom-0.0.5/synonym_custom/
+-rw-rw-rw-   0        0        0        0 2023-05-25 04:22:02.000000 synonym_custom-0.0.5/synonym_custom/__init__.py
+-rw-rw-rw-   0        0        0     8012 2023-06-07 03:14:44.000000 synonym_custom-0.0.5/synonym_custom/synonym_custom.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:44:00.418612 synonym_custom-0.0.5/synonym_custom.egg-info/
+-rw-rw-rw-   0        0        0     5554 2023-06-07 04:43:59.000000 synonym_custom-0.0.5/synonym_custom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-07 04:44:00.000000 synonym_custom-0.0.5/synonym_custom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 04:43:59.000000 synonym_custom-0.0.5/synonym_custom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-06-07 04:43:59.000000 synonym_custom-0.0.5/synonym_custom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-07 04:43:59.000000 synonym_custom-0.0.5/synonym_custom.egg-info/top_level.txt
```

### Comparing `synonym_custom-0.0.4/PKG-INFO` & `synonym_custom-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synonym_custom
-Version: 0.0.4
+Version: 0.0.5
 Author: Sandeep Chataut
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # **KEYWORD AND SYNONYM EXTRACTION PACKAGE**
  The "synonym_custom" package is a versatile tool designed to extract keywords from a given sentence and generate synonyms for those keywords. It combines various modules and libraries to provide multiple approaches for keyword extraction and synonym generation. The package includes the following functionalities:
 
@@ -41,51 +41,81 @@
 API Keys: Depending on the functionalities you want to use, you may need to obtain API keys or set up accounts with specific services. The package requires the following API keys:
 OpenAI API Key: To use the OpenAI-based synonym generation and keyword extraction functionalities, you need to have an OpenAI API key. If you don't have one, you can sign up for an account and obtain the API key from the [OpenAI](https://openai.com/) website. 
 Optional: Some functionalities, such as dictionary-based synonym generation, do not require API keys.
 
 ## Usage:
 
 Once you have installed the package and obtained the necessary API keys, you can import it in your Python script or interactive session:
+
 ```from synonym_custom.synonym_custom import Synonym_Generator```
 
 1. Using openai to extract keywords : 
+
 ```syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))```
+
 ```extracted_keywords = syn_gen.extract_keywords_openai(text)```
-2. Using nltk to generate keywords: 
+
+2. Using nltk to extract keywords: 
+
 ```syn_gen = Synonym_Generator()```
+
 ```extracted_keywords = syn_gen.extract_keywords_nltk(text)```
-3. Using transformers to generate keywords: 
+
+3. Using transformers to extract keywords: 
+
 ```syn_gen = Synonym_Generator()```
+
 ```extracted_keywords = syn_gen.extract_keywords_trans(text)```
-4. Using spacy to generate keywords: 
+
+4. Using spacy to extract keywords: 
+
 ```syn_gen = Synonym_Generator()```
+
 ```extracted_keywords = syn_gen.extract_keywords_spacy(text)```
+
 5. Using dictionary to generate synonyms: 
+
 ```synonym_list = syn_gen.dictionary_syn(keyword)```
+
 6. Using openai to generate synonyms: 
+
 ```synonym_list = syn_gen.openai_api(keyword)```
+
 7. Using spacy to generate synonyms: 
+
 ```synonym_list = syn_gen.spacy_syn(keyword)```
  
 By following these steps and providing the necessary API keys, you will be able to install and utilize the "synonym_custom" package to extract keywords from sentences and generate synonyms using multiple modules and libraries.
 
 ## Example:
 
-from synonym_custom.synonym_custom import Synonym_Generator
 text = "Machine learning is a subfield of artificial intelligence (AI) that focuses on developing algorithms and models that enable computers to learn and make predictions or decisions without being explicitly programmed. It involves the study of statistical and computational models and algorithms that allow machines to learn from and analyze data, recognize patterns, and make data-driven predictions or decisions."
 
-syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))  ##when using openai_api
-syn_gen = Synonym_Generator()
-extracted_keywords = syn_gen.extract_keywords_spacy(text) #using sapcy to generate keywords
-print("Extracted Keywords:", extracted_keywords)
+`from synonym_custom.synonym_custom import Synonym_Generator`
+
+`syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))`  ##when using openai_api
+
+`syn_gen = Synonym_Generator()`
+
+`extracted_keywords = syn_gen.extract_keywords_spacy(text)` #using sapcy to generate keywords
+
+`print("Extracted Keywords:", extracted_keywords)`
+
+
+`synonyms_dict = {}`
+
+`for keyword in extracted_keywords:`
 
-synonyms_dict = {}
-for keyword in extracted_keywords:
     synonym_list = syn_gen.dictionary_syn(keyword) #using dictionary to generate synonyms
+
     synonyms_dict[keyword] = synonym_list
 
-print("Synonyms of extracted keywords:")
-for keyword, synonyms in synonyms_dict.items():
+
+`print("Synonyms of extracted keywords:")`
+
+`for keyword, synonyms in synonyms_dict.items():`
+
     print(f"{keyword}: {synonyms}")
 
 
 
+
```

### Comparing `synonym_custom-0.0.4/README.md` & `synonym_custom-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -34,51 +34,81 @@
 API Keys: Depending on the functionalities you want to use, you may need to obtain API keys or set up accounts with specific services. The package requires the following API keys:
 OpenAI API Key: To use the OpenAI-based synonym generation and keyword extraction functionalities, you need to have an OpenAI API key. If you don't have one, you can sign up for an account and obtain the API key from the [OpenAI](https://openai.com/) website. 
 Optional: Some functionalities, such as dictionary-based synonym generation, do not require API keys.
 
 ## Usage:
 
 Once you have installed the package and obtained the necessary API keys, you can import it in your Python script or interactive session:
+
 ```from synonym_custom.synonym_custom import Synonym_Generator```
 
 1. Using openai to extract keywords : 
+
 ```syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))```
+
 ```extracted_keywords = syn_gen.extract_keywords_openai(text)```
-2. Using nltk to generate keywords: 
+
+2. Using nltk to extract keywords: 
+
 ```syn_gen = Synonym_Generator()```
+
 ```extracted_keywords = syn_gen.extract_keywords_nltk(text)```
-3. Using transformers to generate keywords: 
+
+3. Using transformers to extract keywords: 
+
 ```syn_gen = Synonym_Generator()```
+
 ```extracted_keywords = syn_gen.extract_keywords_trans(text)```
-4. Using spacy to generate keywords: 
+
+4. Using spacy to extract keywords: 
+
 ```syn_gen = Synonym_Generator()```
+
 ```extracted_keywords = syn_gen.extract_keywords_spacy(text)```
+
 5. Using dictionary to generate synonyms: 
+
 ```synonym_list = syn_gen.dictionary_syn(keyword)```
+
 6. Using openai to generate synonyms: 
+
 ```synonym_list = syn_gen.openai_api(keyword)```
+
 7. Using spacy to generate synonyms: 
+
 ```synonym_list = syn_gen.spacy_syn(keyword)```
  
 By following these steps and providing the necessary API keys, you will be able to install and utilize the "synonym_custom" package to extract keywords from sentences and generate synonyms using multiple modules and libraries.
 
 ## Example:
 
-from synonym_custom.synonym_custom import Synonym_Generator
 text = "Machine learning is a subfield of artificial intelligence (AI) that focuses on developing algorithms and models that enable computers to learn and make predictions or decisions without being explicitly programmed. It involves the study of statistical and computational models and algorithms that allow machines to learn from and analyze data, recognize patterns, and make data-driven predictions or decisions."
 
-syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))  ##when using openai_api
-syn_gen = Synonym_Generator()
-extracted_keywords = syn_gen.extract_keywords_spacy(text) #using sapcy to generate keywords
-print("Extracted Keywords:", extracted_keywords)
+`from synonym_custom.synonym_custom import Synonym_Generator`
+
+`syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))`  ##when using openai_api
+
+`syn_gen = Synonym_Generator()`
+
+`extracted_keywords = syn_gen.extract_keywords_spacy(text)` #using sapcy to generate keywords
+
+`print("Extracted Keywords:", extracted_keywords)`
+
+
+`synonyms_dict = {}`
+
+`for keyword in extracted_keywords:`
 
-synonyms_dict = {}
-for keyword in extracted_keywords:
     synonym_list = syn_gen.dictionary_syn(keyword) #using dictionary to generate synonyms
+
     synonyms_dict[keyword] = synonym_list
 
-print("Synonyms of extracted keywords:")
-for keyword, synonyms in synonyms_dict.items():
+
+`print("Synonyms of extracted keywords:")`
+
+`for keyword, synonyms in synonyms_dict.items():`
+
     print(f"{keyword}: {synonyms}")
 
 
 
+
```

### Comparing `synonym_custom-0.0.4/setup.py` & `synonym_custom-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
 
     name='synonym_custom',
-    version='0.0.4',
+    version='0.0.5',
     packages=['synonym_custom'],
     author="Sandeep Chataut",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'openai',
         'requests',
```

### Comparing `synonym_custom-0.0.4/synonym_custom/synonym_custom.py` & `synonym_custom-0.0.5/synonym_custom/synonym_custom.py`

 * *Files identical despite different names*

### Comparing `synonym_custom-0.0.4/synonym_custom.egg-info/PKG-INFO` & `synonym_custom-0.0.5/synonym_custom.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synonym-custom
-Version: 0.0.4
+Version: 0.0.5
 Author: Sandeep Chataut
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # **KEYWORD AND SYNONYM EXTRACTION PACKAGE**
  The "synonym_custom" package is a versatile tool designed to extract keywords from a given sentence and generate synonyms for those keywords. It combines various modules and libraries to provide multiple approaches for keyword extraction and synonym generation. The package includes the following functionalities:
 
@@ -41,51 +41,81 @@
 API Keys: Depending on the functionalities you want to use, you may need to obtain API keys or set up accounts with specific services. The package requires the following API keys:
 OpenAI API Key: To use the OpenAI-based synonym generation and keyword extraction functionalities, you need to have an OpenAI API key. If you don't have one, you can sign up for an account and obtain the API key from the [OpenAI](https://openai.com/) website. 
 Optional: Some functionalities, such as dictionary-based synonym generation, do not require API keys.
 
 ## Usage:
 
 Once you have installed the package and obtained the necessary API keys, you can import it in your Python script or interactive session:
+
 ```from synonym_custom.synonym_custom import Synonym_Generator```
 
 1. Using openai to extract keywords : 
+
 ```syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))```
+
 ```extracted_keywords = syn_gen.extract_keywords_openai(text)```
-2. Using nltk to generate keywords: 
+
+2. Using nltk to extract keywords: 
+
 ```syn_gen = Synonym_Generator()```
+
 ```extracted_keywords = syn_gen.extract_keywords_nltk(text)```
-3. Using transformers to generate keywords: 
+
+3. Using transformers to extract keywords: 
+
 ```syn_gen = Synonym_Generator()```
+
 ```extracted_keywords = syn_gen.extract_keywords_trans(text)```
-4. Using spacy to generate keywords: 
+
+4. Using spacy to extract keywords: 
+
 ```syn_gen = Synonym_Generator()```
+
 ```extracted_keywords = syn_gen.extract_keywords_spacy(text)```
+
 5. Using dictionary to generate synonyms: 
+
 ```synonym_list = syn_gen.dictionary_syn(keyword)```
+
 6. Using openai to generate synonyms: 
+
 ```synonym_list = syn_gen.openai_api(keyword)```
+
 7. Using spacy to generate synonyms: 
+
 ```synonym_list = syn_gen.spacy_syn(keyword)```
  
 By following these steps and providing the necessary API keys, you will be able to install and utilize the "synonym_custom" package to extract keywords from sentences and generate synonyms using multiple modules and libraries.
 
 ## Example:
 
-from synonym_custom.synonym_custom import Synonym_Generator
 text = "Machine learning is a subfield of artificial intelligence (AI) that focuses on developing algorithms and models that enable computers to learn and make predictions or decisions without being explicitly programmed. It involves the study of statistical and computational models and algorithms that allow machines to learn from and analyze data, recognize patterns, and make data-driven predictions or decisions."
 
-syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))  ##when using openai_api
-syn_gen = Synonym_Generator()
-extracted_keywords = syn_gen.extract_keywords_spacy(text) #using sapcy to generate keywords
-print("Extracted Keywords:", extracted_keywords)
+`from synonym_custom.synonym_custom import Synonym_Generator`
+
+`syn_gen = Synonym_Generator(os.getenv('OPENAI_API_KEY'))`  ##when using openai_api
+
+`syn_gen = Synonym_Generator()`
+
+`extracted_keywords = syn_gen.extract_keywords_spacy(text)` #using sapcy to generate keywords
+
+`print("Extracted Keywords:", extracted_keywords)`
+
+
+`synonyms_dict = {}`
+
+`for keyword in extracted_keywords:`
 
-synonyms_dict = {}
-for keyword in extracted_keywords:
     synonym_list = syn_gen.dictionary_syn(keyword) #using dictionary to generate synonyms
+
     synonyms_dict[keyword] = synonym_list
 
-print("Synonyms of extracted keywords:")
-for keyword, synonyms in synonyms_dict.items():
+
+`print("Synonyms of extracted keywords:")`
+
+`for keyword, synonyms in synonyms_dict.items():`
+
     print(f"{keyword}: {synonyms}")
 
 
 
+
```

