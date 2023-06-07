# Comparing `tmp/similarweb_rapidapi-0.1.2.tar.gz` & `tmp/similarweb_rapidapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarweb_rapidapi-0.1.2.tar", last modified: Mon May 29 18:22:25 2023, max compression
+gzip compressed data, was "similarweb_rapidapi-0.1.3.tar", last modified: Wed Jun  7 13:57:51 2023, max compression
```

## Comparing `similarweb_rapidapi-0.1.2.tar` & `similarweb_rapidapi-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 18:22:25.628493 similarweb_rapidapi-0.1.2/
--rw-rw-rw-   0        0        0     1995 2023-05-29 18:22:25.628493 similarweb_rapidapi-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1660 2023-05-29 18:22:08.000000 similarweb_rapidapi-0.1.2/README.md
--rw-rw-rw-   0        0        0       86 2023-05-29 18:22:25.630493 similarweb_rapidapi-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      579 2023-05-29 18:22:13.000000 similarweb_rapidapi-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 18:22:25.598492 similarweb_rapidapi-0.1.2/similarweb_rapidapi/
--rw-rw-rw-   0        0        0       35 2023-05-24 11:11:54.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/__init__.py
--rw-rw-rw-   0        0        0     7700 2023-05-25 19:45:05.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/api.py
--rw-rw-rw-   0        0        0      149 2023-05-25 19:47:56.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/logger_mock.py
-drwxrwxrwx   0        0        0        0 2023-05-29 18:22:25.627493 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/
--rw-rw-rw-   0        0        0        8 2023-05-24 11:46:32.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/__init__.py
--rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/base.py
--rw-rw-rw-   0        0        0     1440 2023-05-24 20:09:52.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/basic_domain_data.py
--rw-rw-rw-   0        0        0      216 2023-05-25 18:31:28.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/cancel_task.py
--rw-rw-rw-   0        0        0      283 2023-05-24 18:52:53.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/complete_data_task.py
--rw-rw-rw-   0        0        0      530 2023-05-24 20:09:30.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/my_tasks.py
--rw-rw-rw-   0        0        0     7562 2023-05-25 19:07:43.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/task.py
--rw-rw-rw-   0        0        0      307 2023-05-24 20:04:34.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/task_status.py
-drwxrwxrwx   0        0        0        0 2023-05-29 18:22:25.610494 similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/
--rw-rw-rw-   0        0        0     1995 2023-05-29 18:22:25.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-05-29 18:22:25.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 18:22:25.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 14:10:40.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-29 18:22:25.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 13:57:51.503379 similarweb_rapidapi-0.1.3/
+-rw-rw-rw-   0        0        0     2005 2023-06-07 13:57:51.503379 similarweb_rapidapi-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1670 2023-06-07 13:28:15.000000 similarweb_rapidapi-0.1.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-07 13:57:51.506381 similarweb_rapidapi-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      579 2023-06-07 13:26:38.000000 similarweb_rapidapi-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:57:51.455380 similarweb_rapidapi-0.1.3/similarweb_rapidapi/
+-rw-rw-rw-   0        0        0       35 2023-05-24 11:11:54.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/__init__.py
+-rw-rw-rw-   0        0        0     7814 2023-06-07 13:55:22.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/api.py
+-rw-rw-rw-   0        0        0      149 2023-05-25 19:47:56.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/logger_mock.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:57:51.502380 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/
+-rw-rw-rw-   0        0        0        8 2023-05-24 11:46:32.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/__init__.py
+-rw-rw-rw-   0        0        0     3305 2023-06-07 13:48:59.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/additional_domain_data.py
+-rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/base.py
+-rw-rw-rw-   0        0        0     1440 2023-05-24 20:09:52.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/basic_domain_data.py
+-rw-rw-rw-   0        0        0      216 2023-05-25 18:31:28.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/cancel_task.py
+-rw-rw-rw-   0        0        0      283 2023-05-24 18:52:53.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/complete_data_task.py
+-rw-rw-rw-   0        0        0      530 2023-05-24 20:09:30.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/my_tasks.py
+-rw-rw-rw-   0        0        0     7562 2023-05-25 19:07:43.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/task.py
+-rw-rw-rw-   0        0        0      307 2023-05-24 20:04:34.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/task_status.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:57:51.484380 similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/
+-rw-rw-rw-   0        0        0     2005 2023-06-07 13:57:51.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2023-06-07 13:57:51.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 13:57:51.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-28 14:10:40.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-06-07 13:57:51.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/top_level.txt
```

### Comparing `similarweb_rapidapi-0.1.2/PKG-INFO` & `similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: similarweb_rapidapi
-Version: 0.1.2
+Name: similarweb-rapidapi
+Version: 0.1.3
 Summary: SimilarWeb API on RapidAPI
 Home-page: https://letsscrape.com/scrapers/similarweb-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
 Keywords: rapidapi,similarweb,similarweb api,scraping,parsing,scraper
 Description-Content-Type: text/markdown
 
@@ -43,18 +43,19 @@
 python3 -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
 python3 setup.py sdist bdist_wheel install
 ```
 
 ### How to get RAPID API key
-1. **Register** you account here https://rapidapi.com/auth/sign-up
-2. Go to http://bit.ly/3z3DInS and **Subscribe to test**
-3. After subscribing to test go once again to http://bit.ly/3z3DInS and get your **X-RapidAPI-Key**
-4. Once you get you key set it when creating SimilarWebRapidAPI object
+1. **Register** you account on RapidAPI https://rapidapi.com/auth/sign-up
+2. Go to https://bit.ly/3z3DInS and **Subscribe to test**
+3. After subscribing, please revisit https://bit.ly/3z3DInS to obtain your **X-RapidAPI-Key**.
+4. You will find **X-RapidAPI-Key** on the right side in the Code Snippets.
+
 ```
 from api import SimilarWebRapidAPI
 
 import asyncio
 
 from schemas.task_status import TaskStatus
```

### Comparing `similarweb_rapidapi-0.1.2/setup.py` & `similarweb_rapidapi-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='similarweb_rapidapi',
-    version='0.1.2',
+    version='0.1.3',
     description='SimilarWeb API on RapidAPI',
     packages=['similarweb_rapidapi', 'similarweb_rapidapi.schemas'],
     author_email='hello@letsscrape.com',
     zip_safe=False,
     author='LetsScrape',
     keywords=['rapidapi', 'similarweb', 'similarweb api', 'scraping', 'parsing', 'scraper'],
     classifiers=[],
```

### Comparing `similarweb_rapidapi-0.1.2/similarweb_rapidapi/api.py` & `similarweb_rapidapi-0.1.3/similarweb_rapidapi/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from urllib.parse import urlencode
 from purl import URL
 
 import aiohttp
 
 from schemas.basic_domain_data import SimilarWebBasicDomainDataModel
 from schemas.complete_data_task import SimilarWebCompleteDataTaskModel
+from schemas.additional_domain_data import AdditionalDomainDataModel
 from schemas.task import SimilarWebTaskResultModel
 from schemas.task_status import TaskStatus
 from schemas.my_tasks import SimilarWebMyTasksModel
 from schemas.cancel_task import SimilarWebCancelTaskModel
 from logger_mock import SimilarWebLoggerMock
  
 
@@ -70,14 +71,24 @@
             await asyncio.sleep(0.3)
 
         return json_response
     
     async def __wait(self):
         await asyncio.sleep(1)
 
+
+    async def get_additional_data_from_domain(self, domain: str) -> AdditionalDomainDataModel:
+        """
+        Gets additional domain information like: Backlinks report, SEMrush data, MOZ data and more!
+        """
+        path = f"/similarweb/GetAdditionalDomainData?domain={domain}"
+        response_data = await self.__get_request(path=path)
+        response = AdditionalDomainDataModel.parse_obj(response_data)
+        return response
+    
     async def get_basic_data_from_domain(self, domain: str) -> List[
         SimilarWebBasicDomainDataModel]:
         """
         Gets basic domain data from SimilarWeb. You will receive from this endpoint 
         data like: top country shares, monthly visits, user engagements, ranks and traffic 
         sources. In many cases such data meet the clients needs. If you want complete
         domain data check get_complete_data_task out!
@@ -135,41 +146,33 @@
                     callback_error(last_exception)
 
         return result
 
     async def get_complete_data_task(self, domain:str, callback_url:str="") -> SimilarWebCompleteDataTaskModel:
         """
         Creates task in the system. The task takes a while to complete, so you can check its
-        status by calling GetTaskResultAsync or set a callbackUrl where the result will be sent.
+        status by calling get_task_result or set a callback_url where the result will be sent.
         About callbacks you can read more here https://rapidapi.com/letsscrape/api/similarweb-working-api/tutorials/use-callbacks-when-using-async-endpoints!
         :param domain: domain
         :param callback_url: url where to send response (domain data)
         """
         path = f"/similarweb/GetCompleteDataAsync?domain={domain}&callback_url={callback_url}"
         response_data = await self.__get_request(path=path)
         response = SimilarWebCompleteDataTaskModel.parse_obj(response_data)
         return response
 
     async def get_task_result(self, task_id) -> SimilarWebTaskResultModel:
         """ 
-        After calling GetCompleteDataAsync just use this method to get the result.
+        After calling get_complete_data_task just use this method to get the result.
         """
         path = f"/similarweb/GetTaskResult?task_id={task_id}"
         response_data = await self.__get_request(path=path)        
         response = SimilarWebTaskResultModel.parse_obj(response_data)
         return response
 
-    async def get_task_result(self, task_id) -> SimilarWebTaskResultModel:
-        """ 
-        After calling GetCompleteDataAsync just use this method to get the result.
-        """
-        path = f"/similarweb/GetTaskResult?task_id={task_id}"
-        response_data = await self.__get_request(path=path)        
-        response = SimilarWebTaskResultModel.parse_obj(response_data)
-        return response
 
     async def get_my_tasks(self, task_status: TaskStatus) -> SimilarWebTaskResultModel:
         """ 
         Returns the list of you all tasks.
         """
         ts = "" if task_status == TaskStatus.ALL else str(task_status)
         path = f"/similarweb/GetMyTasks?task_status={ts}"
```

### Comparing `similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/basic_domain_data.py` & `similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/basic_domain_data.py`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/my_tasks.py` & `similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/my_tasks.py`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/task.py` & `similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/task.py`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/PKG-INFO` & `similarweb_rapidapi-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: similarweb-rapidapi
-Version: 0.1.2
+Name: similarweb_rapidapi
+Version: 0.1.3
 Summary: SimilarWeb API on RapidAPI
 Home-page: https://letsscrape.com/scrapers/similarweb-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
 Keywords: rapidapi,similarweb,similarweb api,scraping,parsing,scraper
 Description-Content-Type: text/markdown
 
@@ -43,18 +43,19 @@
 python3 -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
 python3 setup.py sdist bdist_wheel install
 ```
 
 ### How to get RAPID API key
-1. **Register** you account here https://rapidapi.com/auth/sign-up
-2. Go to http://bit.ly/3z3DInS and **Subscribe to test**
-3. After subscribing to test go once again to http://bit.ly/3z3DInS and get your **X-RapidAPI-Key**
-4. Once you get you key set it when creating SimilarWebRapidAPI object
+1. **Register** you account on RapidAPI https://rapidapi.com/auth/sign-up
+2. Go to https://bit.ly/3z3DInS and **Subscribe to test**
+3. After subscribing, please revisit https://bit.ly/3z3DInS to obtain your **X-RapidAPI-Key**.
+4. You will find **X-RapidAPI-Key** on the right side in the Code Snippets.
+
 ```
 from api import SimilarWebRapidAPI
 
 import asyncio
 
 from schemas.task_status import TaskStatus
```

### Comparing `similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/SOURCES.txt` & `similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 similarweb_rapidapi/logger_mock.py
 similarweb_rapidapi.egg-info/PKG-INFO
 similarweb_rapidapi.egg-info/SOURCES.txt
 similarweb_rapidapi.egg-info/dependency_links.txt
 similarweb_rapidapi.egg-info/not-zip-safe
 similarweb_rapidapi.egg-info/top_level.txt
 similarweb_rapidapi/schemas/__init__.py
+similarweb_rapidapi/schemas/additional_domain_data.py
 similarweb_rapidapi/schemas/base.py
 similarweb_rapidapi/schemas/basic_domain_data.py
 similarweb_rapidapi/schemas/cancel_task.py
 similarweb_rapidapi/schemas/complete_data_task.py
 similarweb_rapidapi/schemas/my_tasks.py
 similarweb_rapidapi/schemas/task.py
 similarweb_rapidapi/schemas/task_status.py
```

