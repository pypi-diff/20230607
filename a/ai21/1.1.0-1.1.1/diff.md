# Comparing `tmp/ai21-1.1.0.tar.gz` & `tmp/ai21-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-1.1.0.tar", last modified: Wed Jun  7 10:45:09 2023, max compression
+gzip compressed data, was "ai21-1.1.1.tar", last modified: Wed Jun  7 14:19:30 2023, max compression
```

## Comparing `ai21-1.1.0.tar` & `ai21-1.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 10:45:09.909253 ai21-1.1.0/
--rw-r--r--   0 etang      (501) staff       (20)     1065 2023-05-22 10:53:48.000000 ai21-1.1.0/LICENSE
--rw-r--r--   0 etang      (501) staff       (20)     3781 2023-06-07 10:45:09.909421 ai21-1.1.0/PKG-INFO
--rw-r--r--   0 etang      (501) staff       (20)     2919 2023-06-06 13:05:13.000000 ai21-1.1.0/README.md
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 10:45:09.898659 ai21-1.1.0/ai21/
--rw-r--r--   0 etang      (501) staff       (20)     2209 2023-06-01 10:48:56.000000 ai21-1.1.0/ai21/AWS_utils.py
--rw-r--r--   0 etang      (501) staff       (20)      878 2023-06-06 13:05:13.000000 ai21-1.1.0/ai21/__init__.py
--rw-r--r--   0 etang      (501) staff       (20)      971 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/ai21_object.py
--rw-r--r--   0 etang      (501) staff       (20)     2055 2023-05-24 11:24:37.000000 ai21-1.1.0/ai21/ai21_studio_client.py
--rw-r--r--   0 etang      (501) staff       (20)      473 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/api_resources.py
--rw-r--r--   0 etang      (501) staff       (20)     1923 2023-06-05 06:50:36.000000 ai21-1.1.0/ai21/bedrock_client.py
--rw-r--r--   0 etang      (501) staff       (20)      246 2023-06-05 06:50:36.000000 ai21-1.1.0/ai21/constants.py
--rw-r--r--   0 etang      (501) staff       (20)     3084 2023-06-06 11:08:21.000000 ai21-1.1.0/ai21/errors.py
--rw-r--r--   0 etang      (501) staff       (20)     4033 2023-05-24 11:13:06.000000 ai21-1.1.0/ai21/http_client.py
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 10:45:09.906507 ai21-1.1.0/ai21/modules/
--rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/__init__.py
--rw-r--r--   0 etang      (501) staff       (20)     2009 2023-06-06 12:32:22.000000 ai21-1.1.0/ai21/modules/completion.py
--rw-r--r--   0 etang      (501) staff       (20)      856 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/custom_model.py
--rw-r--r--   0 etang      (501) staff       (20)      646 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/dataset.py
--rw-r--r--   0 etang      (501) staff       (20)      445 2023-06-06 13:05:13.000000 ai21-1.1.0/ai21/modules/destination.py
--rw-r--r--   0 etang      (501) staff       (20)     1801 2023-06-06 12:34:15.000000 ai21-1.1.0/ai21/modules/experimental.py
--rw-r--r--   0 etang      (501) staff       (20)      986 2023-06-06 09:19:34.000000 ai21-1.1.0/ai21/modules/gec.py
--rw-r--r--   0 etang      (501) staff       (20)      925 2023-06-06 09:03:22.000000 ai21-1.1.0/ai21/modules/improvements.py
--rw-r--r--   0 etang      (501) staff       (20)     1000 2023-06-06 09:00:02.000000 ai21-1.1.0/ai21/modules/paraphrase.py
--rw-r--r--   0 etang      (501) staff       (20)     1104 2023-06-06 09:00:13.000000 ai21-1.1.0/ai21/modules/question_answering.py
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 10:45:09.908990 ai21-1.1.0/ai21/modules/resources/
--rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/resources/__init__.py
--rw-r--r--   0 etang      (501) staff       (20)      585 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/resources/ai21_module.py
--rw-r--r--   0 etang      (501) staff       (20)      371 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/resources/creatable_resource.py
--rw-r--r--   0 etang      (501) staff       (20)     1605 2023-06-06 14:41:24.000000 ai21-1.1.0/ai21/modules/resources/execution_utils.py
--rw-r--r--   0 etang      (501) staff       (20)      352 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/resources/listable_resource.py
--rw-r--r--   0 etang      (501) staff       (20)     2059 2023-06-06 14:34:57.000000 ai21-1.1.0/ai21/modules/resources/nlp_task.py
--rw-r--r--   0 etang      (501) staff       (20)      387 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/resources/retrievable_resource.py
--rw-r--r--   0 etang      (501) staff       (20)      476 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/resources/upload_resource.py
--rw-r--r--   0 etang      (501) staff       (20)      915 2023-06-06 09:09:55.000000 ai21-1.1.0/ai21/modules/segmentation.py
--rw-r--r--   0 etang      (501) staff       (20)      910 2023-06-06 14:07:01.000000 ai21-1.1.0/ai21/modules/summarize.py
--rw-r--r--   0 etang      (501) staff       (20)      693 2023-06-06 09:08:52.000000 ai21-1.1.0/ai21/modules/tokenization.py
--rw-r--r--   0 etang      (501) staff       (20)     3038 2023-06-06 14:33:57.000000 ai21-1.1.0/ai21/utils.py
--rw-r--r--   0 etang      (501) staff       (20)       22 2023-06-06 14:55:41.000000 ai21-1.1.0/ai21/version.py
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 10:45:09.900007 ai21-1.1.0/ai21.egg-info/
--rw-r--r--   0 etang      (501) staff       (20)     3781 2023-06-07 10:45:09.000000 ai21-1.1.0/ai21.egg-info/PKG-INFO
--rw-r--r--   0 etang      (501) staff       (20)     1070 2023-06-07 10:45:09.000000 ai21-1.1.0/ai21.egg-info/SOURCES.txt
--rw-r--r--   0 etang      (501) staff       (20)        1 2023-06-07 10:45:09.000000 ai21-1.1.0/ai21.egg-info/dependency_links.txt
--rw-r--r--   0 etang      (501) staff       (20)       40 2023-06-07 10:45:09.000000 ai21-1.1.0/ai21.egg-info/requires.txt
--rw-r--r--   0 etang      (501) staff       (20)        5 2023-06-07 10:45:09.000000 ai21-1.1.0/ai21.egg-info/top_level.txt
--rwxr-xr-x   0 etang      (501) staff       (20)      155 2023-06-07 10:45:09.909807 ai21-1.1.0/setup.cfg
--rwxr-xr-x   0 etang      (501) staff       (20)      600 2023-06-06 10:57:19.000000 ai21-1.1.0/setup.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 14:19:30.906403 ai21-1.1.1/
+-rw-r--r--   0 etang      (501) staff       (20)     1065 2023-05-22 10:53:48.000000 ai21-1.1.1/LICENSE
+-rw-r--r--   0 etang      (501) staff       (20)     3936 2023-06-07 14:19:30.906504 ai21-1.1.1/PKG-INFO
+-rw-r--r--   0 etang      (501) staff       (20)     3002 2023-06-07 13:39:06.000000 ai21-1.1.1/README.md
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 14:19:30.900660 ai21-1.1.1/ai21/
+-rw-r--r--   0 etang      (501) staff       (20)     2209 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/AWS_utils.py
+-rw-r--r--   0 etang      (501) staff       (20)      885 2023-06-07 13:39:06.000000 ai21-1.1.1/ai21/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)      971 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/ai21_object.py
+-rw-r--r--   0 etang      (501) staff       (20)     2055 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/ai21_studio_client.py
+-rw-r--r--   0 etang      (501) staff       (20)      473 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/api_resources.py
+-rw-r--r--   0 etang      (501) staff       (20)     1923 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/bedrock_client.py
+-rw-r--r--   0 etang      (501) staff       (20)      246 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/constants.py
+-rw-r--r--   0 etang      (501) staff       (20)     3084 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/errors.py
+-rw-r--r--   0 etang      (501) staff       (20)     4033 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/http_client.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 14:19:30.904543 ai21-1.1.1/ai21/modules/
+-rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)     2009 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/completion.py
+-rw-r--r--   0 etang      (501) staff       (20)      856 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/custom_model.py
+-rw-r--r--   0 etang      (501) staff       (20)      646 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/dataset.py
+-rw-r--r--   0 etang      (501) staff       (20)      445 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/destination.py
+-rw-r--r--   0 etang      (501) staff       (20)     1801 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/experimental.py
+-rw-r--r--   0 etang      (501) staff       (20)      986 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/gec.py
+-rw-r--r--   0 etang      (501) staff       (20)      925 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/improvements.py
+-rw-r--r--   0 etang      (501) staff       (20)     1000 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/paraphrase.py
+-rw-r--r--   0 etang      (501) staff       (20)     1104 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/question_answering.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 14:19:30.906231 ai21-1.1.1/ai21/modules/resources/
+-rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/resources/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)      585 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/resources/ai21_module.py
+-rw-r--r--   0 etang      (501) staff       (20)      371 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/resources/creatable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)     1605 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/resources/execution_utils.py
+-rw-r--r--   0 etang      (501) staff       (20)      352 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/resources/listable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)     2059 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/resources/nlp_task.py
+-rw-r--r--   0 etang      (501) staff       (20)      387 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/resources/retrievable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)      476 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/resources/upload_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)      915 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/segmentation.py
+-rw-r--r--   0 etang      (501) staff       (20)      910 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/summarize.py
+-rw-r--r--   0 etang      (501) staff       (20)      693 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/tokenization.py
+-rw-r--r--   0 etang      (501) staff       (20)     3038 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/utils.py
+-rw-r--r--   0 etang      (501) staff       (20)       22 2023-06-07 14:18:08.000000 ai21-1.1.1/ai21/version.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 14:19:30.901693 ai21-1.1.1/ai21.egg-info/
+-rw-r--r--   0 etang      (501) staff       (20)     3936 2023-06-07 14:19:30.000000 ai21-1.1.1/ai21.egg-info/PKG-INFO
+-rw-r--r--   0 etang      (501) staff       (20)     1070 2023-06-07 14:19:30.000000 ai21-1.1.1/ai21.egg-info/SOURCES.txt
+-rw-r--r--   0 etang      (501) staff       (20)        1 2023-06-07 14:19:30.000000 ai21-1.1.1/ai21.egg-info/dependency_links.txt
+-rw-r--r--   0 etang      (501) staff       (20)       40 2023-06-07 14:19:30.000000 ai21-1.1.1/ai21.egg-info/requires.txt
+-rw-r--r--   0 etang      (501) staff       (20)        5 2023-06-07 14:19:30.000000 ai21-1.1.1/ai21.egg-info/top_level.txt
+-rwxr-xr-x   0 etang      (501) staff       (20)      155 2023-06-07 14:19:30.906770 ai21-1.1.1/setup.cfg
+-rwxr-xr-x   0 etang      (501) staff       (20)      600 2023-06-07 10:54:53.000000 ai21-1.1.1/setup.py
```

### Comparing `ai21-1.1.0/LICENSE` & `ai21-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/PKG-INFO` & `ai21-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.1.0
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
@@ -44,47 +44,56 @@
         ## Usage
         
         ### Studio API
         In the following example, an AI21 API client is used with an API key and a timeout parameter set globally. 
         This example uses a simple completion call with only prompt and maxTokens arguments supplied
         (all other completion settings are set to their defaults):
         ```python
+        import ai21
+        
         ai21.api_key = 'my_api_key'
         ai21.timeout_sec = 20
         response = ai21.Completion.execute(model="j1-large", prompt="hello world", maxTokens=20)
         print(response)
         ```
         
         ### AWS Client
         This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint or as an AWS Bedrock API.
         To activate this option, make sure to install with the extra AWS dependencies:
         
-        `pip install -U ai21['AWS']`
+        `pip install -U "ai21[AWS]"`
         
         #### Sagemaker endpoint request
         You can then generate a completion by running:
         ```python
-        response = ai21.Completion.execute(destination=ai21.SageMakerDestination("<your_endpoint_name>"), prompt="hello world", maxTokens=20)
+        import ai21
+        ai21.aws_region = 'us-east-1'
+        response = ai21.Completion.execute(
+            destination=ai21.SageMakerDestination("<your_endpoint_name>"),
+            prompt="hello world",
+            maxTokens=20,
+        )
+        
         print(response)
         ```
         
         #### Bedrock API request
         
-        You can use one of the models offered in the following list:
+        You can use one of the models offered in the following list as model_id:
         - ai21.j2-grande-instruct
         - ai21.j2-jumbo-instruct
         
         ```python
         import ai21
         
         response = ai21.Completion.execute(
             destination=ai21.BedrockDestination(model_id=ai21.BedrockModelID.J2_JUMBO_INSTRUCT),
             prompt="hello world",
             maxTokens=20,
         )
+        
         print(response)
         ```
         
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: AWS
```

### Comparing `ai21-1.1.0/README.md` & `ai21-1.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -36,43 +36,52 @@
 ## Usage
 
 ### Studio API
 In the following example, an AI21 API client is used with an API key and a timeout parameter set globally. 
 This example uses a simple completion call with only prompt and maxTokens arguments supplied
 (all other completion settings are set to their defaults):
 ```python
+import ai21
+
 ai21.api_key = 'my_api_key'
 ai21.timeout_sec = 20
 response = ai21.Completion.execute(model="j1-large", prompt="hello world", maxTokens=20)
 print(response)
 ```
 
 ### AWS Client
 This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint or as an AWS Bedrock API.
 To activate this option, make sure to install with the extra AWS dependencies:
 
-`pip install -U ai21['AWS']`
+`pip install -U "ai21[AWS]"`
 
 #### Sagemaker endpoint request
 You can then generate a completion by running:
 ```python
-response = ai21.Completion.execute(destination=ai21.SageMakerDestination("<your_endpoint_name>"), prompt="hello world", maxTokens=20)
+import ai21
+ai21.aws_region = 'us-east-1'
+response = ai21.Completion.execute(
+    destination=ai21.SageMakerDestination("<your_endpoint_name>"),
+    prompt="hello world",
+    maxTokens=20,
+)
+
 print(response)
 ```
 
 #### Bedrock API request
 
-You can use one of the models offered in the following list:
+You can use one of the models offered in the following list as model_id:
 - ai21.j2-grande-instruct
 - ai21.j2-jumbo-instruct
 
 ```python
 import ai21
 
 response = ai21.Completion.execute(
     destination=ai21.BedrockDestination(model_id=ai21.BedrockModelID.J2_JUMBO_INSTRUCT),
     prompt="hello world",
     maxTokens=20,
 )
+
 print(response)
 ```
-
```

### Comparing `ai21-1.1.0/ai21/AWS_utils.py` & `ai21-1.1.1/ai21/AWS_utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/__init__.py` & `ai21-1.1.1/ai21/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 api_key = None
 organization = None
 application = None
 api_version = DEFAULT_API_VERSION
 api_host = STUDIO_HOST
 timeout_sec = None
 num_retries = None
-aws_region = None
+aws_region = 'us-east-1'
 log_level = 'error'
```

### Comparing `ai21-1.1.0/ai21/ai21_object.py` & `ai21-1.1.1/ai21/ai21_object.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/ai21_studio_client.py` & `ai21-1.1.1/ai21/ai21_studio_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/bedrock_client.py` & `ai21-1.1.1/ai21/bedrock_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/errors.py` & `ai21-1.1.1/ai21/errors.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/http_client.py` & `ai21-1.1.1/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/completion.py` & `ai21-1.1.1/ai21/modules/completion.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/custom_model.py` & `ai21-1.1.1/ai21/modules/custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/dataset.py` & `ai21-1.1.1/ai21/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/experimental.py` & `ai21-1.1.1/ai21/modules/experimental.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/gec.py` & `ai21-1.1.1/ai21/modules/gec.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/improvements.py` & `ai21-1.1.1/ai21/modules/improvements.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/paraphrase.py` & `ai21-1.1.1/ai21/modules/paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/question_answering.py` & `ai21-1.1.1/ai21/modules/question_answering.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/resources/ai21_module.py` & `ai21-1.1.1/ai21/modules/resources/ai21_module.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/resources/execution_utils.py` & `ai21-1.1.1/ai21/modules/resources/execution_utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/resources/nlp_task.py` & `ai21-1.1.1/ai21/modules/resources/nlp_task.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/segmentation.py` & `ai21-1.1.1/ai21/modules/segmentation.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/summarize.py` & `ai21-1.1.1/ai21/modules/summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/modules/tokenization.py` & `ai21-1.1.1/ai21/modules/tokenization.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21/utils.py` & `ai21-1.1.1/ai21/utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/ai21.egg-info/PKG-INFO` & `ai21-1.1.1/ai21.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.1.0
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
@@ -44,47 +44,56 @@
         ## Usage
         
         ### Studio API
         In the following example, an AI21 API client is used with an API key and a timeout parameter set globally. 
         This example uses a simple completion call with only prompt and maxTokens arguments supplied
         (all other completion settings are set to their defaults):
         ```python
+        import ai21
+        
         ai21.api_key = 'my_api_key'
         ai21.timeout_sec = 20
         response = ai21.Completion.execute(model="j1-large", prompt="hello world", maxTokens=20)
         print(response)
         ```
         
         ### AWS Client
         This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint or as an AWS Bedrock API.
         To activate this option, make sure to install with the extra AWS dependencies:
         
-        `pip install -U ai21['AWS']`
+        `pip install -U "ai21[AWS]"`
         
         #### Sagemaker endpoint request
         You can then generate a completion by running:
         ```python
-        response = ai21.Completion.execute(destination=ai21.SageMakerDestination("<your_endpoint_name>"), prompt="hello world", maxTokens=20)
+        import ai21
+        ai21.aws_region = 'us-east-1'
+        response = ai21.Completion.execute(
+            destination=ai21.SageMakerDestination("<your_endpoint_name>"),
+            prompt="hello world",
+            maxTokens=20,
+        )
+        
         print(response)
         ```
         
         #### Bedrock API request
         
-        You can use one of the models offered in the following list:
+        You can use one of the models offered in the following list as model_id:
         - ai21.j2-grande-instruct
         - ai21.j2-jumbo-instruct
         
         ```python
         import ai21
         
         response = ai21.Completion.execute(
             destination=ai21.BedrockDestination(model_id=ai21.BedrockModelID.J2_JUMBO_INSTRUCT),
             prompt="hello world",
             maxTokens=20,
         )
+        
         print(response)
         ```
         
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: AWS
```

### Comparing `ai21-1.1.0/ai21.egg-info/SOURCES.txt` & `ai21-1.1.1/ai21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai21-1.1.0/setup.py` & `ai21-1.1.1/setup.py`

 * *Files identical despite different names*

