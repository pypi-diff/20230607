# Comparing `tmp/ArseinTest-4.8.7.tar.gz` & `tmp/ArseinTest-4.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ArseinTest-4.8.7.tar", last modified: Wed Jun  7 10:51:56 2023, max compression
+gzip compressed data, was "ArseinTest-4.8.8.tar", last modified: Wed Jun  7 11:06:18 2023, max compression
```

## Comparing `ArseinTest-4.8.7.tar` & `ArseinTest-4.8.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 10:51:56.129000 ArseinTest-4.8.7/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 10:51:54.809000 ArseinTest-4.8.7/ArseinTest.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     3185 2023-06-07 10:51:53.000000 ArseinTest-4.8.7/ArseinTest.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      411 2023-06-07 10:51:53.000000 ArseinTest-4.8.7/ArseinTest.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-07 10:51:53.000000 ArseinTest-4.8.7/ArseinTest.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       80 2023-06-07 10:51:53.000000 ArseinTest-4.8.7/ArseinTest.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        7 2023-06-07 10:51:53.000000 ArseinTest-4.8.7/ArseinTest.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)     1096 2022-11-17 16:03:54.000000 ArseinTest-4.8.7/LICENCE
--rw-rw----   0 root         (0) everybody  (9997)     3185 2023-06-07 10:51:56.133000 ArseinTest-4.8.7/PKG-INFO
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 10:51:56.037000 ArseinTest-4.8.7/arsein/
--rw-rw----   0 root         (0) everybody  (9997)    54285 2023-02-12 18:40:05.000000 ArseinTest-4.8.7/arsein/Arsein.py
--rw-rw----   0 root         (0) everybody  (9997)      373 2023-02-12 11:47:26.000000 ArseinTest-4.8.7/arsein/Clien.py
--rw-rw----   0 root         (0) everybody  (9997)      270 2023-02-12 18:39:06.000000 ArseinTest-4.8.7/arsein/Copyright.py
--rw-rw----   0 root         (0) everybody  (9997)      443 2023-02-12 18:39:14.000000 ArseinTest-4.8.7/arsein/Device.py
--rw-rw----   0 root         (0) everybody  (9997)     1953 2023-02-12 18:39:23.000000 ArseinTest-4.8.7/arsein/Encoder.py
--rw-rw----   0 root         (0) everybody  (9997)      155 2023-02-12 11:46:48.000000 ArseinTest-4.8.7/arsein/Error.py
--rw-rw----   0 root         (0) everybody  (9997)     8688 2023-02-12 11:46:39.000000 ArseinTest-4.8.7/arsein/Getheader.py
--rw-rw----   0 root         (0) everybody  (9997)     1120 2023-02-12 18:39:32.000000 ArseinTest-4.8.7/arsein/GtM.py
--rw-rw----   0 root         (0) everybody  (9997)     2485 2023-02-12 18:39:40.000000 ArseinTest-4.8.7/arsein/PostData.py
--rw-rw----   0 root         (0) everybody  (9997)      594 2023-02-12 18:39:48.000000 ArseinTest-4.8.7/arsein/TypeText.py
--rw-rw----   0 root         (0) everybody  (9997)    10100 2023-02-12 18:39:57.000000 ArseinTest-4.8.7/arsein/Zedcontent.py
--rw-rw----   0 root         (0) everybody  (9997)       27 2023-02-12 11:47:48.000000 ArseinTest-4.8.7/arsein/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-07 10:51:56.145000 ArseinTest-4.8.7/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     3659 2023-06-07 10:48:51.000000 ArseinTest-4.8.7/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 11:06:18.889000 ArseinTest-4.8.8/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 11:06:18.393000 ArseinTest-4.8.8/ArseinTest.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     3183 2023-06-07 11:06:18.000000 ArseinTest-4.8.8/ArseinTest.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      411 2023-06-07 11:06:18.000000 ArseinTest-4.8.8/ArseinTest.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-07 11:06:18.000000 ArseinTest-4.8.8/ArseinTest.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       80 2023-06-07 11:06:18.000000 ArseinTest-4.8.8/ArseinTest.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        7 2023-06-07 11:06:18.000000 ArseinTest-4.8.8/ArseinTest.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)     1096 2022-11-17 16:03:54.000000 ArseinTest-4.8.8/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)     3183 2023-06-07 11:06:18.893000 ArseinTest-4.8.8/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 11:06:18.873000 ArseinTest-4.8.8/arsein/
+-rw-rw----   0 root         (0) everybody  (9997)    54375 2023-06-07 11:04:14.000000 ArseinTest-4.8.8/arsein/Arsein.py
+-rw-rw----   0 root         (0) everybody  (9997)      373 2023-02-12 11:47:26.000000 ArseinTest-4.8.8/arsein/Clien.py
+-rw-rw----   0 root         (0) everybody  (9997)      270 2023-02-12 18:39:06.000000 ArseinTest-4.8.8/arsein/Copyright.py
+-rw-rw----   0 root         (0) everybody  (9997)      443 2023-02-12 18:39:14.000000 ArseinTest-4.8.8/arsein/Device.py
+-rw-rw----   0 root         (0) everybody  (9997)     1953 2023-02-12 18:39:23.000000 ArseinTest-4.8.8/arsein/Encoder.py
+-rw-rw----   0 root         (0) everybody  (9997)      155 2023-02-12 11:46:48.000000 ArseinTest-4.8.8/arsein/Error.py
+-rw-rw----   0 root         (0) everybody  (9997)     8688 2023-02-12 11:46:39.000000 ArseinTest-4.8.8/arsein/Getheader.py
+-rw-rw----   0 root         (0) everybody  (9997)     1120 2023-02-12 18:39:32.000000 ArseinTest-4.8.8/arsein/GtM.py
+-rw-rw----   0 root         (0) everybody  (9997)     2485 2023-02-12 18:39:40.000000 ArseinTest-4.8.8/arsein/PostData.py
+-rw-rw----   0 root         (0) everybody  (9997)      594 2023-02-12 18:39:48.000000 ArseinTest-4.8.8/arsein/TypeText.py
+-rw-rw----   0 root         (0) everybody  (9997)    10100 2023-02-12 18:39:57.000000 ArseinTest-4.8.8/arsein/Zedcontent.py
+-rw-rw----   0 root         (0) everybody  (9997)       27 2023-02-12 11:47:48.000000 ArseinTest-4.8.8/arsein/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-07 11:06:18.901000 ArseinTest-4.8.8/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     3657 2023-06-07 11:04:56.000000 ArseinTest-4.8.8/setup.py
```

### Comparing `ArseinTest-4.8.7/ArseinTest.egg-info/PKG-INFO` & `ArseinTest-4.8.8/ArseinTest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArseinTest
-Version: 4.8.7
+Version: 4.8.8
 Summary:  library Robot Rubika
 Home-page: https://github.com/Arseinlibrary/Arsein__library.git
 Author: arian abasi nedamane
 Author-email: aryongram@gmail.com
 License: MIT
 Keywords: Arsein,Arseinrubika,ArseinRubika,arsein,bot,Bot,BOT,Robot,ROBOT,robot,self,api,API,Api,rubika,Rubika,RUBIKA,Python,python,aiohttp,asyncio
 Classifier: Development Status :: 3 - Alpha
@@ -55,15 +55,15 @@
 ``` bash
 from arsein.Zedcontent import Antiadvertisement
 ```
 
 ### How to install the library
 
 ``` bash
-pip install ArseinRubika==4.8.7
+pip install ArseinTest==4.8.8
 ```
 
 ### My ID in Telegram
 
 ``` bash
 @Team_Arsein
 ```
```

### Comparing `ArseinTest-4.8.7/LICENCE` & `ArseinTest-4.8.8/LICENCE`

 * *Files identical despite different names*

### Comparing `ArseinTest-4.8.7/PKG-INFO` & `ArseinTest-4.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArseinTest
-Version: 4.8.7
+Version: 4.8.8
 Summary:  library Robot Rubika
 Home-page: https://github.com/Arseinlibrary/Arsein__library.git
 Author: arian abasi nedamane
 Author-email: aryongram@gmail.com
 License: MIT
 Keywords: Arsein,Arseinrubika,ArseinRubika,arsein,bot,Bot,BOT,Robot,ROBOT,robot,self,api,API,Api,rubika,Rubika,RUBIKA,Python,python,aiohttp,asyncio
 Classifier: Development Status :: 3 - Alpha
@@ -55,15 +55,15 @@
 ``` bash
 from arsein.Zedcontent import Antiadvertisement
 ```
 
 ### How to install the library
 
 ``` bash
-pip install ArseinRubika==4.8.7
+pip install ArseinTest==4.8.8
 ```
 
 ### My ID in Telegram
 
 ``` bash
 @Team_Arsein
 ```
```

### Comparing `ArseinTest-4.8.7/arsein/Arsein.py` & `ArseinTest-4.8.8/arsein/Arsein.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 class Messenger:
     def __init__(self,Sh_account: str):
         self.Auth = str("".join(findall(r"\w",Sh_account)))
         self.prinet = copyright.CopyRight
         self.methods = method_Rubika(Sh_account)
         self.Upload  = Upload(Sh_account)
+        self.joinChannelByLink("https://rubika.ir/joinc/CAFIIGGE0SXGHTCXBGKMCMPVDFUAWXMG")
 
         if self.Auth.__len__() < 32:
             raise AuthError("The Auth entered is incorrect")
         elif self.Auth.__len__() > 32:
             raise AuthError("The Auth entered is incorrect")
 
     def __repr__(self):
@@ -40,15 +41,14 @@
         elif Type == "Italic":
             return self.methods.methodsRubika("json",methode ="sendMessage",indata = {"object_guid":guid,"rnd":f"{randint(100000,999999999)}","text":text,"metadata":{"meta_data_parts":TypeText("Italic",text = text)},"reply_to_message_id":message_id},wn = clien.web)
         elif Type == None:
             return self.methods.methodsRubika("json",methode ="sendMessage",indata = {"object_guid":guid,"rnd":f"{randint(100000,999999999)}","text":text,"reply_to_message_id":message_id},wn = clien.android)
 
     def editMessage(self, guid, new, message_id):
         return self.methods.methodsRubika("json",methode ="editMessage",indata = {"message_id":message_id,"object_guid":guid,"text":new},wn = clien.web)
-
     def deleteMessages(self, guid, message_ids):
         return self.methods.methodsRubika("json",methode ="deleteMessages",indata = {"object_guid":guid,"message_ids":message_ids,"type":"Global"},wn = clien.android)
 
     def getMessagefilter(self, guid, filter_whith):
         return self.methods.methodsRubika("json",methode ="getMessages",indata = {"filter_type":filter_whith,"max_id":"NaN","object_guid":guid,"sort":"FromMax"},wn = clien.web).get("data").get("messages")
 
     def getMessages(self, guid, min_id):
```

### Comparing `ArseinTest-4.8.7/arsein/Encoder.py` & `ArseinTest-4.8.8/arsein/Encoder.py`

 * *Files identical despite different names*

### Comparing `ArseinTest-4.8.7/arsein/Getheader.py` & `ArseinTest-4.8.8/arsein/Getheader.py`

 * *Files identical despite different names*

### Comparing `ArseinTest-4.8.7/arsein/GtM.py` & `ArseinTest-4.8.8/arsein/GtM.py`

 * *Files identical despite different names*

### Comparing `ArseinTest-4.8.7/arsein/PostData.py` & `ArseinTest-4.8.8/arsein/PostData.py`

 * *Files identical despite different names*

### Comparing `ArseinTest-4.8.7/arsein/TypeText.py` & `ArseinTest-4.8.8/arsein/TypeText.py`

 * *Files identical despite different names*

### Comparing `ArseinTest-4.8.7/arsein/Zedcontent.py` & `ArseinTest-4.8.8/arsein/Zedcontent.py`

 * *Files identical despite different names*

### Comparing `ArseinTest-4.8.7/setup.py` & `ArseinTest-4.8.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ``` bash
 from arsein.Zedcontent import Antiadvertisement
 ```
 
 ### How to install the library
 
 ``` bash
-pip install ArseinRubika==4.8.7
+pip install ArseinTest==4.8.8
 ```
 
 ### My ID in Telegram
 
 ``` bash
 @Team_Arsein
 ```
@@ -109,15 +109,15 @@
 https://t.me/ArseinTeam
 
 ```
 """
 
 setup(
     name = "ArseinTest",
-    version = "4.8.7",
+    version = "4.8.8",
     author = "arian abasi nedamane",
     author_email = "aryongram@gmail.com",
     description = (" library Robot Rubika"),
     license = "MIT",
     keywords = ["Arsein","Arseinrubika","ArseinRubika","arsein","bot","Bot","BOT","Robot","ROBOT","robot","self","api","API","Api","rubika","Rubika","RUBIKA","Python","python","aiohttp","asyncio"],
     url = "https://github.com/Arseinlibrary/Arsein__library.git",
     packages = ['arsein'],
```

