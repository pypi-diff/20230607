# Comparing `tmp/ai21-1.0.7.tar.gz` & `tmp/ai21-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-1.0.7.tar", last modified: Wed May 17 08:04:38 2023, max compression
+gzip compressed data, was "ai21-1.1.0.tar", last modified: Wed Jun  7 10:45:09 2023, max compression
```

## Comparing `ai21-1.0.7.tar` & `ai21-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-05-17 08:04:38.430717 ai21-1.0.7/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1065 2023-03-25 06:53:34.000000 ai21-1.0.7/LICENSE
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3178 2023-05-17 08:04:38.430869 ai21-1.0.7/PKG-INFO
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2485 2023-05-17 08:04:00.000000 ai21-1.0.7/README.md
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-05-17 08:04:38.424149 ai21-1.0.7/ai21/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2100 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/SM_utils.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      751 2023-05-17 06:59:37.000000 ai21-1.0.7/ai21/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      971 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/ai21_object.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2590 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/ai21_studio_client.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      473 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/api_resources.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      104 2023-04-10 09:05:28.000000 ai21-1.0.7/ai21/constants.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2823 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/errors.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3868 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/http_client.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-05-17 08:04:38.428399 ai21-1.0.7/ai21/modules/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/modules/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1375 2023-04-10 09:05:28.000000 ai21-1.0.7/ai21/modules/completion.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      856 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/modules/custom_model.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      646 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/modules/dataset.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2167 2023-05-17 06:59:37.000000 ai21-1.0.7/ai21/modules/experimental.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      650 2023-05-17 06:59:37.000000 ai21-1.0.7/ai21/modules/gec.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      654 2023-05-17 06:59:37.000000 ai21-1.0.7/ai21/modules/improvements.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      664 2023-05-17 06:59:37.000000 ai21-1.0.7/ai21/modules/paraphrase.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      771 2023-04-19 08:57:55.000000 ai21-1.0.7/ai21/modules/question_answering.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-05-17 08:04:38.430506 ai21-1.0.7/ai21/modules/resources/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/modules/resources/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      585 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/modules/resources/ai21_module.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      371 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/modules/resources/creatable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      352 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/modules/resources/listable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1208 2023-04-10 09:05:28.000000 ai21-1.0.7/ai21/modules/resources/nlp_task.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      387 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/modules/resources/retrievable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      476 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/modules/resources/upload_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      611 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/modules/segmentation.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      795 2023-04-10 09:35:40.000000 ai21-1.0.7/ai21/modules/summarize.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      461 2023-03-25 06:53:34.000000 ai21-1.0.7/ai21/modules/tokenization.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1875 2023-04-19 09:08:00.000000 ai21-1.0.7/ai21/utils.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)       22 2023-05-17 08:04:16.000000 ai21-1.0.7/ai21/version.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-05-17 08:04:38.425258 ai21-1.0.7/ai21.egg-info/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3178 2023-05-17 08:04:38.000000 ai21-1.0.7/ai21.egg-info/PKG-INFO
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      976 2023-05-17 08:04:38.000000 ai21-1.0.7/ai21.egg-info/SOURCES.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        1 2023-05-17 08:04:38.000000 ai21-1.0.7/ai21.egg-info/dependency_links.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)       21 2023-05-17 08:04:38.000000 ai21-1.0.7/ai21.egg-info/requires.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        5 2023-05-17 08:04:38.000000 ai21-1.0.7/ai21.egg-info/top_level.txt
--rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      155 2023-05-17 08:04:38.431200 ai21-1.0.7/setup.cfg
--rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      576 2023-03-27 12:47:23.000000 ai21-1.0.7/setup.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 10:45:09.909253 ai21-1.1.0/
+-rw-r--r--   0 etang      (501) staff       (20)     1065 2023-05-22 10:53:48.000000 ai21-1.1.0/LICENSE
+-rw-r--r--   0 etang      (501) staff       (20)     3781 2023-06-07 10:45:09.909421 ai21-1.1.0/PKG-INFO
+-rw-r--r--   0 etang      (501) staff       (20)     2919 2023-06-06 13:05:13.000000 ai21-1.1.0/README.md
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 10:45:09.898659 ai21-1.1.0/ai21/
+-rw-r--r--   0 etang      (501) staff       (20)     2209 2023-06-01 10:48:56.000000 ai21-1.1.0/ai21/AWS_utils.py
+-rw-r--r--   0 etang      (501) staff       (20)      878 2023-06-06 13:05:13.000000 ai21-1.1.0/ai21/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)      971 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/ai21_object.py
+-rw-r--r--   0 etang      (501) staff       (20)     2055 2023-05-24 11:24:37.000000 ai21-1.1.0/ai21/ai21_studio_client.py
+-rw-r--r--   0 etang      (501) staff       (20)      473 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/api_resources.py
+-rw-r--r--   0 etang      (501) staff       (20)     1923 2023-06-05 06:50:36.000000 ai21-1.1.0/ai21/bedrock_client.py
+-rw-r--r--   0 etang      (501) staff       (20)      246 2023-06-05 06:50:36.000000 ai21-1.1.0/ai21/constants.py
+-rw-r--r--   0 etang      (501) staff       (20)     3084 2023-06-06 11:08:21.000000 ai21-1.1.0/ai21/errors.py
+-rw-r--r--   0 etang      (501) staff       (20)     4033 2023-05-24 11:13:06.000000 ai21-1.1.0/ai21/http_client.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 10:45:09.906507 ai21-1.1.0/ai21/modules/
+-rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)     2009 2023-06-06 12:32:22.000000 ai21-1.1.0/ai21/modules/completion.py
+-rw-r--r--   0 etang      (501) staff       (20)      856 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/custom_model.py
+-rw-r--r--   0 etang      (501) staff       (20)      646 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/dataset.py
+-rw-r--r--   0 etang      (501) staff       (20)      445 2023-06-06 13:05:13.000000 ai21-1.1.0/ai21/modules/destination.py
+-rw-r--r--   0 etang      (501) staff       (20)     1801 2023-06-06 12:34:15.000000 ai21-1.1.0/ai21/modules/experimental.py
+-rw-r--r--   0 etang      (501) staff       (20)      986 2023-06-06 09:19:34.000000 ai21-1.1.0/ai21/modules/gec.py
+-rw-r--r--   0 etang      (501) staff       (20)      925 2023-06-06 09:03:22.000000 ai21-1.1.0/ai21/modules/improvements.py
+-rw-r--r--   0 etang      (501) staff       (20)     1000 2023-06-06 09:00:02.000000 ai21-1.1.0/ai21/modules/paraphrase.py
+-rw-r--r--   0 etang      (501) staff       (20)     1104 2023-06-06 09:00:13.000000 ai21-1.1.0/ai21/modules/question_answering.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 10:45:09.908990 ai21-1.1.0/ai21/modules/resources/
+-rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/resources/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)      585 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/resources/ai21_module.py
+-rw-r--r--   0 etang      (501) staff       (20)      371 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/resources/creatable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)     1605 2023-06-06 14:41:24.000000 ai21-1.1.0/ai21/modules/resources/execution_utils.py
+-rw-r--r--   0 etang      (501) staff       (20)      352 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/resources/listable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)     2059 2023-06-06 14:34:57.000000 ai21-1.1.0/ai21/modules/resources/nlp_task.py
+-rw-r--r--   0 etang      (501) staff       (20)      387 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/resources/retrievable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)      476 2023-05-22 10:53:48.000000 ai21-1.1.0/ai21/modules/resources/upload_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)      915 2023-06-06 09:09:55.000000 ai21-1.1.0/ai21/modules/segmentation.py
+-rw-r--r--   0 etang      (501) staff       (20)      910 2023-06-06 14:07:01.000000 ai21-1.1.0/ai21/modules/summarize.py
+-rw-r--r--   0 etang      (501) staff       (20)      693 2023-06-06 09:08:52.000000 ai21-1.1.0/ai21/modules/tokenization.py
+-rw-r--r--   0 etang      (501) staff       (20)     3038 2023-06-06 14:33:57.000000 ai21-1.1.0/ai21/utils.py
+-rw-r--r--   0 etang      (501) staff       (20)       22 2023-06-06 14:55:41.000000 ai21-1.1.0/ai21/version.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 10:45:09.900007 ai21-1.1.0/ai21.egg-info/
+-rw-r--r--   0 etang      (501) staff       (20)     3781 2023-06-07 10:45:09.000000 ai21-1.1.0/ai21.egg-info/PKG-INFO
+-rw-r--r--   0 etang      (501) staff       (20)     1070 2023-06-07 10:45:09.000000 ai21-1.1.0/ai21.egg-info/SOURCES.txt
+-rw-r--r--   0 etang      (501) staff       (20)        1 2023-06-07 10:45:09.000000 ai21-1.1.0/ai21.egg-info/dependency_links.txt
+-rw-r--r--   0 etang      (501) staff       (20)       40 2023-06-07 10:45:09.000000 ai21-1.1.0/ai21.egg-info/requires.txt
+-rw-r--r--   0 etang      (501) staff       (20)        5 2023-06-07 10:45:09.000000 ai21-1.1.0/ai21.egg-info/top_level.txt
+-rwxr-xr-x   0 etang      (501) staff       (20)      155 2023-06-07 10:45:09.909807 ai21-1.1.0/setup.cfg
+-rwxr-xr-x   0 etang      (501) staff       (20)      600 2023-06-06 10:57:19.000000 ai21-1.1.0/setup.py
```

### Comparing `ai21-1.0.7/LICENSE` & `ai21-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-1.0.7/PKG-INFO` & `ai21-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.0.7
+Version: 1.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
@@ -50,20 +50,41 @@
         ```python
         ai21.api_key = 'my_api_key'
         ai21.timeout_sec = 20
         response = ai21.Completion.execute(model="j1-large", prompt="hello world", maxTokens=20)
         print(response)
         ```
         
-        ### SageMaker Endpoint
-        This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint. To activate this option, make sure to install with the extra SM dependencies:
+        ### AWS Client
+        This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint or as an AWS Bedrock API.
+        To activate this option, make sure to install with the extra AWS dependencies:
         
-        `pip install -U ai21['SM']`
+        `pip install -U ai21['AWS']`
         
+        #### Sagemaker endpoint request
         You can then generate a completion by running:
         ```python
-        response = ai21.Completion.execute(sm_endpoint="<your_endpoint_name>", prompt="hello world", maxTokens=20)
+        response = ai21.Completion.execute(destination=ai21.SageMakerDestination("<your_endpoint_name>"), prompt="hello world", maxTokens=20)
         print(response)
         ```
+        
+        #### Bedrock API request
+        
+        You can use one of the models offered in the following list:
+        - ai21.j2-grande-instruct
+        - ai21.j2-jumbo-instruct
+        
+        ```python
+        import ai21
+        
+        response = ai21.Completion.execute(
+            destination=ai21.BedrockDestination(model_id=ai21.BedrockModelID.J2_JUMBO_INSTRUCT),
+            prompt="hello world",
+            maxTokens=20,
+        )
+        print(response)
+        ```
+        
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Provides-Extra: SM
+Provides-Extra: AWS
```

### Comparing `ai21-1.0.7/README.md` & `ai21-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -42,17 +42,37 @@
 ```python
 ai21.api_key = 'my_api_key'
 ai21.timeout_sec = 20
 response = ai21.Completion.execute(model="j1-large", prompt="hello world", maxTokens=20)
 print(response)
 ```
 
-### SageMaker Endpoint
-This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint. To activate this option, make sure to install with the extra SM dependencies:
+### AWS Client
+This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint or as an AWS Bedrock API.
+To activate this option, make sure to install with the extra AWS dependencies:
 
-`pip install -U ai21['SM']`
+`pip install -U ai21['AWS']`
 
+#### Sagemaker endpoint request
 You can then generate a completion by running:
 ```python
-response = ai21.Completion.execute(sm_endpoint="<your_endpoint_name>", prompt="hello world", maxTokens=20)
+response = ai21.Completion.execute(destination=ai21.SageMakerDestination("<your_endpoint_name>"), prompt="hello world", maxTokens=20)
 print(response)
-```
+```
+
+#### Bedrock API request
+
+You can use one of the models offered in the following list:
+- ai21.j2-grande-instruct
+- ai21.j2-jumbo-instruct
+
+```python
+import ai21
+
+response = ai21.Completion.execute(
+    destination=ai21.BedrockDestination(model_id=ai21.BedrockModelID.J2_JUMBO_INSTRUCT),
+    prompt="hello world",
+    maxTokens=20,
+)
+print(response)
+```
+
```

### Comparing `ai21-1.0.7/ai21/SM_utils.py` & `ai21-1.1.0/ai21/AWS_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 import json
 import re
 
 import boto3
+from botocore.credentials import Credentials
 from botocore.exceptions import ClientError
 
+import ai21
 from ai21.errors import ServerError, ServiceUnavailable, BadRequest, APIError
 from ai21.http_client import handle_non_success_response
 from ai21.utils import convert_to_ai21_object, log_error
 
-sm_runtime = boto3.client("sagemaker-runtime")
+sm_runtime = boto3.client("sagemaker-runtime", region_name=ai21.aws_region)
 
 
 def invoke_sm_endpoint(endpoint_name: str, input_json: str):
     try:
         response = sm_runtime.invoke_endpoint(
             EndpointName=endpoint_name,
             ContentType="application/json",
             Accept="application/json",
             Body=input_json,
         )
+
+        response_body = json.load(response["Body"])
+
+        return convert_to_ai21_object(response_body)
     except ClientError as sm_client_error:
         handle_sagemaker_client_error(sm_client_error)
     except Exception as exception:
         log_error(f'Calling {endpoint_name} failed with Exception: {exception}')
         raise exception
-    response_body = json.load(response["Body"])
-    return convert_to_ai21_object(response_body)
 
 
 def handle_sagemaker_client_error(client_exception: ClientError):
     error_response = client_exception.response
     error_message = error_response.get('Error', {}).get('Message', '')
     status_code = error_response.get('ResponseMetadata', {}).get('HTTPStatusCode', None)
     # According to https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_runtime_InvokeEndpoint.html#API_runtime_InvokeEndpoint_Errors
     if status_code == 400:
         raise BadRequest(details=error_message)
     if status_code == 424:
-        error_message_template = re.compile(r'Received client error \((.*?)\) from primary with message \"(.*?)\". See .* in account .* for more information.')
+        error_message_template = re.compile(
+            r'Received client error \((.*?)\) from primary with message \"(.*?)\". See .* in account .* for more information.')
         model_status_code = int(error_message_template.search(error_message).group(1))
         model_error_message = error_message_template.search(error_message).group(2)
         handle_non_success_response(model_status_code, model_error_message)
     if status_code == 429 or status_code == 503:
         raise ServiceUnavailable(details=error_message)
     if status_code == 500:
         raise ServerError(details=error_message)
```

### Comparing `ai21-1.0.7/ai21/ai21_object.py` & `ai21-1.1.0/ai21/ai21_object.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.7/ai21/ai21_studio_client.py` & `ai21-1.1.0/ai21/ai21_studio_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Dict
 from ai21.errors import MissingApiKeyException, WrongInputTypeException
 from ai21.http_client import HttpClient
-from ai21.utils import get_global_configs, convert_to_ai21_object
+from ai21.utils import get_global_configs, convert_to_ai21_object, get_value
 from ai21.version import __version__
 
 
 def build_ai21_user_agent():
     global_configs = get_global_configs()
     user_agent = f'ai21 studio SDK {__version__}'
     organization = global_configs['organization']
@@ -13,27 +13,14 @@
         user_agent = f'{user_agent} organization: {organization}'
     application = global_configs['application']
     if application is not None:
         user_agent = f'{user_agent} application: {application}'
     return user_agent
 
 
-def get_value(key: str, params: Dict, global_configs: Dict, expected_type: type):
-    passed_value = params.get(key, None)
-    if passed_value is not None:
-        if not isinstance(passed_value, expected_type):
-            raise WrongInputTypeException(key, expected_type, type(passed_value))
-        return passed_value
-
-    global_value = global_configs[key]
-    if global_value is not None and not isinstance(global_value, expected_type):
-        raise WrongInputTypeException(key, global_value, type(global_value))
-    return global_value
-
-
 class AI21StudioClient:
     def __init__(self, **params):
         global_configs = get_global_configs()
         api_key = get_value('api_key', params, global_configs, str)
         if api_key is None:
             raise MissingApiKeyException()
         self.api_key = api_key
```

### Comparing `ai21-1.0.7/ai21/errors.py` & `ai21-1.1.0/ai21/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,20 @@
 
 class UnsupportedInputException(AI21ClientException):
     def __init__(self, field_name: str, call_name: str):
         message = f'{field_name} is unsupported for the {call_name} call'
         super().__init__(message)
 
 
+class UnsupportedDestinationException(AI21ClientException):
+    def __init__(self, destination_name: str, call_name: str):
+        message = f'Destination of type {destination_name} is unsupported for the "{call_name}" call'
+        super().__init__(message)
+
+
 class OnlyOneInputException(AI21ClientException):
     def __init__(self, field_name1: str, field_name2: str, call_name: str):
         message = f'{field_name1} or {field_name2} is required for the {call_name} call, but not both'
         super().__init__(message)
 
 
 class WrongInputTypeException(AI21ClientException):
```

### Comparing `ai21-1.0.7/ai21/http_client.py` & `ai21-1.1.0/ai21/http_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import json
 from typing import Optional, Dict
+
 import requests
-from requests.adapters import HTTPAdapter, Response, Retry, RetryError
-from ai21.errors import BadRequest, Unauthorized, UnprocessableEntity, TooManyRequests, ServerError, ServiceUnavailable, APIError
+from requests.adapters import HTTPAdapter, Retry, RetryError
+
+from ai21.errors import BadRequest, Unauthorized, UnprocessableEntity, TooManyRequests, ServerError, ServiceUnavailable, \
+    APIError
 from ai21.utils import log_info, log_error
 
 DEFAULT_TIMEOUT_SEC = 30
 DEFAULT_NUM_RETRIES = 0
 RETRY_BACK_OFF_FACTOR = 0.5
 TIME_BETWEEN_RETRIES = 1000
 RETRY_ERROR_CODES = (429, 500, 503)
@@ -41,31 +44,35 @@
 class HttpClient:
     def __init__(self, timeout_sec: int = None, num_retries: int = None, headers: Dict = None):
         self.timeout_sec = timeout_sec if timeout_sec is not None else DEFAULT_TIMEOUT_SEC
         self.num_retries = num_retries if num_retries is not None else DEFAULT_NUM_RETRIES
         self.headers = headers if headers is not None else {}
         self.apply_retry_policy = self.num_retries > 0
 
-    def execute_http_request(self, method: str, url: str, params: Optional[Dict] = None, files=None):
-        session = requests_retry_session(requests.Session(), retries=self.num_retries) if self.apply_retry_policy else requests.Session()
+    def execute_http_request(self, method: str, url: str, params: Optional[Dict] = None, files=None, auth=None):
+        session = requests_retry_session(requests.Session(),
+                                         retries=self.num_retries) if self.apply_retry_policy else requests.Session()
         timeout = self.timeout_sec
         headers = self.headers
         data = json.dumps(params).encode()
         log_info(f'Calling {method} {url} {headers} {data}')
         try:
             if method == 'GET':
                 response = session.request(method, url, headers=headers, timeout=timeout)
             elif files is not None:
                 if method != 'POST':
-                    raise ValueError(f'execute_http_request supports only POST for files upload, but {method} was supplied instead')
+                    raise ValueError(
+                        f'execute_http_request supports only POST for files upload, but {method} was supplied instead')
                 if 'Content-Type' in headers:
-                    headers.pop('Content-Type')  # multipart/form-data 'Content-Type' is being added when passing rb files and payload
-                response = session.request(method, url, headers=headers, data=params, files=files, timeout=timeout)
+                    headers.pop(
+                        'Content-Type')  # multipart/form-data 'Content-Type' is being added when passing rb files and payload
+                response = session.request(method, url, headers=headers, data=params, files=files, timeout=timeout,
+                                           auth=auth)
             else:
-                response = session.request(method, url, headers=headers, data=data, timeout=timeout)
+                response = session.request(method, url, headers=headers, data=data, timeout=timeout, auth=auth)
         except ConnectionError as connection_error:
             log_error(f'Calling {method} {url} failed with ConnectionError: {connection_error}')
             raise connection_error
         except RetryError as retry_error:
             log_error(f'Calling {method} {url} failed with RetryError after {self.num_retries} attempts: {retry_error}')
             raise retry_error
         except Exception as exception:
```

### Comparing `ai21-1.0.7/ai21/modules/completion.py` & `ai21-1.1.0/ai21/modules/summarize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,25 @@
-from ai21.constants import SAGEMAKER_ENDPOINT_KEY
+from ai21.modules.resources.execution_utils import execute_studio_request
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
-class Completion(NLPTask):
-    MODULE_NAME = 'complete'
+class Summarize(NLPTask):
+    MODULE_NAME = 'summarize'
 
     @classmethod
-    def execute(cls, experimental_mode=False, **params):
-        validate_mandatory_field(key='prompt', call_name=cls.MODULE_NAME, params=params, validate_type=True, expected_type=str)
-        if params.get('stopSequences', None) is None:
-            params['stopSequences'] = []
-
-        use_sm_endpoint = SAGEMAKER_ENDPOINT_KEY in params
-        if use_sm_endpoint:
-            return cls.execute_sm_endpoint(**params, unsupported_fields=['model', 'custom_model'])
-        return cls.execute_studio_api(experimental_mode, **params)
+    def _get_call_name(cls) -> str:
+        return cls.MODULE_NAME
 
     @classmethod
-    def execute_studio_api(cls, experimental_mode: False, **params):
-        validate_mandatory_field(key='model', call_name=cls.MODULE_NAME, params=params, validate_type=True, expected_type=str)
-        model = params.get('model', None)
-        custom_model = params.get('custom_model', None)
-        if experimental_mode:
-            model = f'experimental/{model}'
-        url = f'{cls.get_base_url(**params)}/{model}'
-        if custom_model is not None:
-            url = f'{url}/{custom_model}'
+    def _validate_params(cls, params):
+        validate_mandatory_field(key='sourceType', call_name=cls.MODULE_NAME, params=params, validate_type=True,
+                                 expected_type=str)
+        validate_mandatory_field(key='source', call_name=cls.MODULE_NAME, params=params, validate_type=True,
+                                 expected_type=str)
+
+
+    @classmethod
+    def _execute_studio_api(cls, params):
+        url = cls.get_base_url(**params)
         url = f'{url}/{cls.MODULE_NAME}'
-        return super().execute(task_url=url, **params)
+        return execute_studio_request(task_url=url, params=params)
```

### Comparing `ai21-1.0.7/ai21/modules/custom_model.py` & `ai21-1.1.0/ai21/modules/custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.7/ai21/modules/dataset.py` & `ai21-1.1.0/ai21/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.7/ai21/modules/experimental.py` & `ai21-1.1.0/ai21/modules/experimental.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,45 @@
-from typing import List
-
-from ai21 import Completion
-from ai21.constants import SAGEMAKER_ENDPOINT_KEY
+from ai21.modules.completion import Completion
+from ai21.modules.destination import SageMakerDestination
+from ai21.modules.resources.ai21_module import AI21Module
+from ai21.modules.resources.execution_utils import execute_studio_request, execute_sm_request
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
-class Experimental(NLPTask):
-
+class Experimental(AI21Module):
     @classmethod
-    def _execute(cls, module: str, **params):
-        url = f'{cls.get_base_url(**params)}/experimental/{module}'
-        return super().execute(task_url=url, **params)
+    def embed(cls, **params):
+        validate_mandatory_field(key='texts', call_name="embed_experimental", params=params, validate_type=True,
+                                 expected_type=list)
+        url = cls.get_base_url(**params)
+        url = f'{url}/experimental/embed'
+        return execute_studio_request(task_url=url, params=params)
 
     @classmethod
-    def rewrite(cls, **params):
-        validate_mandatory_field(key='text', call_name="rewrite_experimental", params=params, validate_type=True, expected_type=str)
-        url = cls.get_base_url(**params)
-        url = f'{url}/experimental/rewrite'
-        return super().execute(task_url=url, **params)
+    def answer(cls, **params):
+        return _AnswerExperimental.execute(**params)
+
+
+class _AnswerExperimental(NLPTask):
+    MODULE_NAME = 'answer_experimental'
 
     @classmethod
-    def summarize(cls, **params):
-        validate_mandatory_field(key='text', call_name="summarize_experimental", params=params, validate_type=True, expected_type=str)
-        url = cls.get_base_url(**params)
-        url = f'{url}/experimental/summarize'
-        return super().execute(task_url=url, **params)
+    def _get_call_name(cls) -> str:
+        return cls.MODULE_NAME
 
     @classmethod
-    def embed(cls, **params):
-        validate_mandatory_field(key='texts', call_name="embed_experimental", params=params, validate_type=True, expected_type=list)
-        url = cls.get_base_url(**params)
-        url = f'{url}/experimental/embed'
-        return super().execute(task_url=url, **params)
+    def _validate_params(cls, params):
+        validate_mandatory_field(key='context', call_name="answer_experimental", params=params, validate_type=True,
+                                 expected_type=str)
+        validate_mandatory_field(key='question', call_name="answer_experimental", params=params, validate_type=True,
+                                 expected_type=str)
 
     @classmethod
-    def j1_grande_instruct(cls, **params):
-        params["model"] = "j1-grande-instruct"
-        return Completion.execute(experimental_mode=True, **params)
+    def _execute_sm(cls, destination: SageMakerDestination, params):
+        return execute_sm_request(endpoint_name=destination.endpoint_name, params=params)
 
     @classmethod
-    def answer(cls, **params):
-        validate_mandatory_field(key='context', call_name="answer_experimental", params=params, validate_type=True, expected_type=str)
-        validate_mandatory_field(key='question', call_name="answer_experimental", params=params, validate_type=True, expected_type=str)
-        use_sm_endpoint = SAGEMAKER_ENDPOINT_KEY in params
-        if use_sm_endpoint:
-            return cls.execute_sm_endpoint(**params)
+    def _execute_studio_api(cls, params):
         url = cls.get_base_url(**params)
         url = f'{url}/experimental/answer'
-        return super().execute(task_url=url, **params)
+        return execute_studio_request(task_url=url, params=params)
```

### Comparing `ai21-1.0.7/ai21/modules/gec.py` & `ai21-1.1.0/ai21/modules/segmentation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-from ai21.constants import SAGEMAKER_ENDPOINT_KEY
-
+from ai21.modules.resources.execution_utils import execute_studio_request
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
-class GEC(NLPTask):
-    MODULE_NAME = 'gec'
+class Segmentation(NLPTask):
+    MODULE_NAME = 'segmentation'
+
+    @classmethod
+    def _get_call_name(cls) -> str:
+        return cls.MODULE_NAME
+
+    @classmethod
+    def _validate_params(cls, params):
+        validate_mandatory_field(key='sourceType', call_name=cls.MODULE_NAME, params=params, validate_type=True,
+                                 expected_type=str)
+        validate_mandatory_field(key='source', call_name=cls.MODULE_NAME, params=params, validate_type=True,
+                                 expected_type=str)
 
     @classmethod
-    def execute(cls, **params):
-        validate_mandatory_field(key='text', call_name=cls.MODULE_NAME, params=params, validate_type=True, expected_type=str)
-        use_sm_endpoint = SAGEMAKER_ENDPOINT_KEY in params
-        if use_sm_endpoint:
-            return cls.execute_sm_endpoint(**params)
+    def _execute_studio_api(cls, params):
         url = cls.get_base_url(**params)
         url = f'{url}/{cls.MODULE_NAME}'
-        return super().execute(task_url=url, **params)
+        return execute_studio_request(task_url=url, params=params)
```

### Comparing `ai21-1.0.7/ai21/modules/improvements.py` & `ai21-1.1.0/ai21/modules/improvements.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 
 from ai21.errors import EmptyMandatoryListException
+from ai21.modules.resources.execution_utils import execute_studio_request
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
 class Improvements(NLPTask):
     MODULE_NAME = 'improvements'
 
     @classmethod
-    def execute(cls, **params):
-        validate_mandatory_field(key='text', call_name=cls.MODULE_NAME, params=params, validate_type=True, expected_type=str)
+    def _get_call_name(cls) -> str:
+        return cls.MODULE_NAME
+
+    @classmethod
+    def _validate_params(cls, params):
+        validate_mandatory_field(key='text', call_name=cls.MODULE_NAME, params=params, validate_type=True,
+                                 expected_type=str)
         if params.get('types') is None or len(params['types']) == 0:
             raise EmptyMandatoryListException('types')
+
+    @classmethod
+    def _execute_studio_api(cls, params):
         url = cls.get_base_url(**params)
         url = f'{url}/{cls.MODULE_NAME}'
-        return super().execute(task_url=url, **params)
+        return execute_studio_request(task_url=url, params=params)
```

### Comparing `ai21-1.0.7/ai21/modules/resources/ai21_module.py` & `ai21-1.1.0/ai21/modules/resources/ai21_module.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.7/ai21/modules/resources/nlp_task.py` & `ai21-1.1.0/ai21/modules/question_answering.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import json
+from ai21.modules.destination import SageMakerDestination
+from ai21.modules.resources.execution_utils import execute_sm_request
+from ai21.modules.resources.nlp_task import NLPTask
+from ai21.utils import validate_mandatory_field
 
-from ai21.ai21_studio_client import AI21StudioClient
-from ai21.modules.resources.ai21_module import AI21Module
-from ai21.utils import validate_mandatory_field, validate_unsupported_field
 
+class Answer(NLPTask):
+    MODULE_NAME = 'answer'
 
-class NLPTask(AI21Module):
+    @classmethod
+    def _get_call_name(cls) -> str:
+        return cls.MODULE_NAME
+
+    @classmethod
+    def _validate_params(cls, params):
+        validate_mandatory_field(key='context', call_name=cls.MODULE_NAME, params=params, validate_type=True,
+                                 expected_type=str)
+        validate_mandatory_field(key='question', call_name=cls.MODULE_NAME, params=params, validate_type=True,
+                                 expected_type=str)
 
     @classmethod
-    def execute(cls, task_url, **params):
-        client = AI21StudioClient(**params)
-        return client.execute_http_request(method='POST', url=task_url, params=params)
+    def _execute_sm(cls, destination: SageMakerDestination, params):
+        return execute_sm_request(endpoint_name=destination.endpoint_name, params=params)
 
     @classmethod
-    def execute_sm_endpoint(cls, mandatory_fields=None, unsupported_fields=None, **params):
-        endpoint_name = params.pop('sm_endpoint')
-        call_name = f'Sagemaker {endpoint_name}'
-        if mandatory_fields is not None:
-            for mandatory_field in mandatory_fields:
-                validate_mandatory_field(mandatory_field, call_name, params)
-        if unsupported_fields is not None:
-            for unsupported_field in unsupported_fields:
-                validate_unsupported_field(key=unsupported_field, call_name=call_name, params=params)
-        input_json = json.dumps(params)
-        from ai21.SM_utils import invoke_sm_endpoint  # import here because boto3 exists only in SM mode
-        return invoke_sm_endpoint(endpoint_name, input_json)
+    def _execute_studio_api(cls, params):
+        raise NotImplementedError(f'The module {cls.MODULE_NAME} is not implemented for the non experimental endpoint')
```

### Comparing `ai21-1.0.7/ai21.egg-info/PKG-INFO` & `ai21-1.1.0/ai21.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.0.7
+Version: 1.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
@@ -50,20 +50,41 @@
         ```python
         ai21.api_key = 'my_api_key'
         ai21.timeout_sec = 20
         response = ai21.Completion.execute(model="j1-large", prompt="hello world", maxTokens=20)
         print(response)
         ```
         
-        ### SageMaker Endpoint
-        This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint. To activate this option, make sure to install with the extra SM dependencies:
+        ### AWS Client
+        This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint or as an AWS Bedrock API.
+        To activate this option, make sure to install with the extra AWS dependencies:
         
-        `pip install -U ai21['SM']`
+        `pip install -U ai21['AWS']`
         
+        #### Sagemaker endpoint request
         You can then generate a completion by running:
         ```python
-        response = ai21.Completion.execute(sm_endpoint="<your_endpoint_name>", prompt="hello world", maxTokens=20)
+        response = ai21.Completion.execute(destination=ai21.SageMakerDestination("<your_endpoint_name>"), prompt="hello world", maxTokens=20)
         print(response)
         ```
+        
+        #### Bedrock API request
+        
+        You can use one of the models offered in the following list:
+        - ai21.j2-grande-instruct
+        - ai21.j2-jumbo-instruct
+        
+        ```python
+        import ai21
+        
+        response = ai21.Completion.execute(
+            destination=ai21.BedrockDestination(model_id=ai21.BedrockModelID.J2_JUMBO_INSTRUCT),
+            prompt="hello world",
+            maxTokens=20,
+        )
+        print(response)
+        ```
+        
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Provides-Extra: SM
+Provides-Extra: AWS
```

### Comparing `ai21-1.0.7/ai21.egg-info/SOURCES.txt` & `ai21-1.1.0/ai21.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
-ai21/SM_utils.py
+ai21/AWS_utils.py
 ai21/__init__.py
 ai21/ai21_object.py
 ai21/ai21_studio_client.py
 ai21/api_resources.py
+ai21/bedrock_client.py
 ai21/constants.py
 ai21/errors.py
 ai21/http_client.py
 ai21/utils.py
 ai21/version.py
 ai21.egg-info/PKG-INFO
 ai21.egg-info/SOURCES.txt
 ai21.egg-info/dependency_links.txt
 ai21.egg-info/requires.txt
 ai21.egg-info/top_level.txt
 ai21/modules/__init__.py
 ai21/modules/completion.py
 ai21/modules/custom_model.py
 ai21/modules/dataset.py
+ai21/modules/destination.py
 ai21/modules/experimental.py
 ai21/modules/gec.py
 ai21/modules/improvements.py
 ai21/modules/paraphrase.py
 ai21/modules/question_answering.py
 ai21/modules/segmentation.py
 ai21/modules/summarize.py
 ai21/modules/tokenization.py
 ai21/modules/resources/__init__.py
 ai21/modules/resources/ai21_module.py
 ai21/modules/resources/creatable_resource.py
+ai21/modules/resources/execution_utils.py
 ai21/modules/resources/listable_resource.py
 ai21/modules/resources/nlp_task.py
 ai21/modules/resources/retrievable_resource.py
 ai21/modules/resources/upload_resource.py
```

### Comparing `ai21-1.0.7/setup.py` & `ai21-1.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     license='MIT',
     author="ai21 labs",
     author_email='support@ai21.com',
     packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=[
         'requests',
     ],
-    extras_require={'SM': 'boto3'},
+    extras_require={'AWS': ['boto3', 'aws-requests-auth']},
 )
```

