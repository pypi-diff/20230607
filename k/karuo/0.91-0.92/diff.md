# Comparing `tmp/karuo-0.91.tar.gz` & `tmp/karuo-0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karuo-0.91.tar", last modified: Thu Mar  2 04:23:23 2023, max compression
+gzip compressed data, was "karuo-0.92.tar", last modified: Wed Jun  7 13:29:11 2023, max compression
```

## Comparing `karuo-0.91.tar` & `karuo-0.92.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-03-02 04:23:23.785601 karuo-0.91/
--rw-rw-r--   0 work      (1001) work      (1001)     1063 2023-01-31 08:56:37.000000 karuo-0.91/LICENSE
--rw-rw-r--   0 work      (1001) work      (1001)      283 2023-03-02 04:23:23.785601 karuo-0.91/PKG-INFO
--rw-rw-r--   0 work      (1001) work      (1001)      140 2023-01-31 08:56:37.000000 karuo-0.91/README.md
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-03-02 04:23:23.781601 karuo-0.91/karuo/
--rw-rw-r--   0 work      (1001) work      (1001)     1738 2023-03-02 04:23:15.000000 karuo-0.91/karuo/__init__.py
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-03-02 04:23:23.782601 karuo-0.91/karuo/baiduai/
--rw-rw-r--   0 work      (1001) work      (1001)      350 2023-01-31 08:56:37.000000 karuo-0.91/karuo/baiduai/__init__.py
--rw-rw-r--   0 work      (1001) work      (1001)     4157 2023-01-31 08:56:37.000000 karuo-0.91/karuo/baiduai/base.py
--rw-rw-r--   0 work      (1001) work      (1001)      788 2023-01-31 08:56:37.000000 karuo-0.91/karuo/baiduai/error_code.py
--rw-rw-r--   0 work      (1001) work      (1001)     6474 2023-01-31 08:56:37.000000 karuo-0.91/karuo/baiduai/func_faces.py
--rw-rw-r--   0 work      (1001) work      (1001)     2199 2023-01-31 08:56:37.000000 karuo-0.91/karuo/baiduai/func_ocr.py
--rw-rw-r--   0 work      (1001) work      (1001)      819 2023-01-31 08:56:37.000000 karuo-0.91/karuo/datadef.py
--rw-rw-r--   0 work      (1001) work      (1001)      590 2023-01-31 08:56:37.000000 karuo-0.91/karuo/decorators.py
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-03-02 04:23:23.783601 karuo-0.91/karuo/helpers/
--rw-rw-r--   0 work      (1001) work      (1001)      281 2023-01-31 08:56:37.000000 karuo-0.91/karuo/helpers/__init__.py
--rw-rw-r--   0 work      (1001) work      (1001)      557 2023-01-31 08:56:37.000000 karuo-0.91/karuo/helpers/char_helper.py
--rw-rw-r--   0 work      (1001) work      (1001)     2839 2023-01-31 08:56:37.000000 karuo-0.91/karuo/helpers/date_helper.py
--rw-rw-r--   0 work      (1001) work      (1001)     2221 2023-01-31 08:56:37.000000 karuo-0.91/karuo/helpers/logger_helper.py
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-03-02 04:23:23.784601 karuo-0.91/karuo/qywx/
--rw-rw-r--   0 work      (1001) work      (1001)    10542 2023-01-31 08:56:37.000000 karuo-0.91/karuo/qywx/WXBizMsgCrypt.py
--rw-rw-r--   0 work      (1001) work      (1001)      280 2023-01-31 08:56:37.000000 karuo-0.91/karuo/qywx/__init__.py
--rw-rw-r--   0 work      (1001) work      (1001)    40735 2023-02-20 08:01:56.000000 karuo-0.91/karuo/qywx/base.py
--rw-rw-r--   0 work      (1001) work      (1001)     5692 2023-01-31 08:56:37.000000 karuo-0.91/karuo/qywx/helper.py
--rw-rw-r--   0 work      (1001) work      (1001)      772 2023-01-31 08:56:37.000000 karuo-0.91/karuo/qywx/ierror.py
--rw-rw-r--   0 work      (1001) work      (1001)    31924 2023-03-02 04:20:58.000000 karuo-0.91/karuo/qywx/provider.py
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-03-02 04:23:23.782601 karuo-0.91/karuo.egg-info/
--rw-rw-r--   0 work      (1001) work      (1001)      283 2023-03-02 04:23:23.000000 karuo-0.91/karuo.egg-info/PKG-INFO
--rw-rw-r--   0 work      (1001) work      (1001)      722 2023-03-02 04:23:23.000000 karuo-0.91/karuo.egg-info/SOURCES.txt
--rw-rw-r--   0 work      (1001) work      (1001)        1 2023-03-02 04:23:23.000000 karuo-0.91/karuo.egg-info/dependency_links.txt
--rw-rw-r--   0 work      (1001) work      (1001)       51 2023-03-02 04:23:23.000000 karuo-0.91/karuo.egg-info/requires.txt
--rw-rw-r--   0 work      (1001) work      (1001)       11 2023-03-02 04:23:23.000000 karuo-0.91/karuo.egg-info/top_level.txt
--rw-rw-r--   0 work      (1001) work      (1001)       38 2023-03-02 04:23:23.785601 karuo-0.91/setup.cfg
--rw-rw-r--   0 work      (1001) work      (1001)      836 2023-01-31 08:56:37.000000 karuo-0.91/setup.py
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-03-02 04:23:23.784601 karuo-0.91/test/
--rw-rw-r--   0 work      (1001) work      (1001)      281 2023-01-31 08:56:37.000000 karuo-0.91/test/__init__.py
--rw-rw-r--   0 work      (1001) work      (1001)     2320 2023-01-31 08:56:37.000000 karuo-0.91/test/test_ai_face.py
--rw-rw-r--   0 work      (1001) work      (1001)      793 2023-01-31 08:56:37.000000 karuo-0.91/test/test_ai_ocr.py
--rw-rw-r--   0 work      (1001) work      (1001)     4023 2023-01-31 08:56:37.000000 karuo-0.91/test/test_helpers.py
--rw-rw-r--   0 work      (1001) work      (1001)     1125 2023-01-31 08:56:37.000000 karuo-0.91/test/test_normal.py
--rw-rw-r--   0 work      (1001) work      (1001)     6584 2023-01-31 08:56:37.000000 karuo-0.91/test/test_qywx.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-07 13:29:11.014935 karuo-0.92/
+-rw-rw-r--   0 work      (1001) work      (1001)     1063 2023-01-31 08:56:37.000000 karuo-0.92/LICENSE
+-rw-rw-r--   0 work      (1001) work      (1001)      283 2023-06-07 13:29:11.014935 karuo-0.92/PKG-INFO
+-rw-rw-r--   0 work      (1001) work      (1001)      140 2023-01-31 08:56:37.000000 karuo-0.92/README.md
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-07 13:29:11.010935 karuo-0.92/karuo/
+-rw-rw-r--   0 work      (1001) work      (1001)     1790 2023-06-07 13:28:59.000000 karuo-0.92/karuo/__init__.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-07 13:29:11.011935 karuo-0.92/karuo/baiduai/
+-rw-rw-r--   0 work      (1001) work      (1001)      350 2023-01-31 08:56:37.000000 karuo-0.92/karuo/baiduai/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)     4157 2023-01-31 08:56:37.000000 karuo-0.92/karuo/baiduai/base.py
+-rw-rw-r--   0 work      (1001) work      (1001)      788 2023-01-31 08:56:37.000000 karuo-0.92/karuo/baiduai/error_code.py
+-rw-rw-r--   0 work      (1001) work      (1001)     6474 2023-01-31 08:56:37.000000 karuo-0.92/karuo/baiduai/func_faces.py
+-rw-rw-r--   0 work      (1001) work      (1001)     2199 2023-01-31 08:56:37.000000 karuo-0.92/karuo/baiduai/func_ocr.py
+-rw-rw-r--   0 work      (1001) work      (1001)      819 2023-01-31 08:56:37.000000 karuo-0.92/karuo/datadef.py
+-rw-rw-r--   0 work      (1001) work      (1001)      590 2023-01-31 08:56:37.000000 karuo-0.92/karuo/decorators.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-07 13:29:11.012935 karuo-0.92/karuo/helpers/
+-rw-rw-r--   0 work      (1001) work      (1001)      281 2023-01-31 08:56:37.000000 karuo-0.92/karuo/helpers/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)      557 2023-01-31 08:56:37.000000 karuo-0.92/karuo/helpers/char_helper.py
+-rw-rw-r--   0 work      (1001) work      (1001)     2839 2023-01-31 08:56:37.000000 karuo-0.92/karuo/helpers/date_helper.py
+-rw-rw-r--   0 work      (1001) work      (1001)     2221 2023-01-31 08:56:37.000000 karuo-0.92/karuo/helpers/logger_helper.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-07 13:29:11.013935 karuo-0.92/karuo/qywx/
+-rw-rw-r--   0 work      (1001) work      (1001)    10542 2023-01-31 08:56:37.000000 karuo-0.92/karuo/qywx/WXBizMsgCrypt.py
+-rw-rw-r--   0 work      (1001) work      (1001)      280 2023-01-31 08:56:37.000000 karuo-0.92/karuo/qywx/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)    40999 2023-06-07 13:21:01.000000 karuo-0.92/karuo/qywx/base.py
+-rw-rw-r--   0 work      (1001) work      (1001)     5692 2023-01-31 08:56:37.000000 karuo-0.92/karuo/qywx/helper.py
+-rw-rw-r--   0 work      (1001) work      (1001)      772 2023-01-31 08:56:37.000000 karuo-0.92/karuo/qywx/ierror.py
+-rw-rw-r--   0 work      (1001) work      (1001)    31924 2023-03-02 04:20:58.000000 karuo-0.92/karuo/qywx/provider.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-07 13:29:11.011935 karuo-0.92/karuo.egg-info/
+-rw-rw-r--   0 work      (1001) work      (1001)      283 2023-06-07 13:29:10.000000 karuo-0.92/karuo.egg-info/PKG-INFO
+-rw-rw-r--   0 work      (1001) work      (1001)      722 2023-06-07 13:29:10.000000 karuo-0.92/karuo.egg-info/SOURCES.txt
+-rw-rw-r--   0 work      (1001) work      (1001)        1 2023-06-07 13:29:10.000000 karuo-0.92/karuo.egg-info/dependency_links.txt
+-rw-rw-r--   0 work      (1001) work      (1001)       51 2023-06-07 13:29:10.000000 karuo-0.92/karuo.egg-info/requires.txt
+-rw-rw-r--   0 work      (1001) work      (1001)       11 2023-06-07 13:29:10.000000 karuo-0.92/karuo.egg-info/top_level.txt
+-rw-rw-r--   0 work      (1001) work      (1001)       38 2023-06-07 13:29:11.014935 karuo-0.92/setup.cfg
+-rw-rw-r--   0 work      (1001) work      (1001)      836 2023-01-31 08:56:37.000000 karuo-0.92/setup.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-07 13:29:11.013935 karuo-0.92/test/
+-rw-rw-r--   0 work      (1001) work      (1001)      281 2023-01-31 08:56:37.000000 karuo-0.92/test/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)     2320 2023-01-31 08:56:37.000000 karuo-0.92/test/test_ai_face.py
+-rw-rw-r--   0 work      (1001) work      (1001)      793 2023-01-31 08:56:37.000000 karuo-0.92/test/test_ai_ocr.py
+-rw-rw-r--   0 work      (1001) work      (1001)     4023 2023-01-31 08:56:37.000000 karuo-0.92/test/test_helpers.py
+-rw-rw-r--   0 work      (1001) work      (1001)     1125 2023-01-31 08:56:37.000000 karuo-0.92/test/test_normal.py
+-rw-rw-r--   0 work      (1001) work      (1001)     6853 2023-06-07 13:27:30.000000 karuo-0.92/test/test_qywx.py
```

### Comparing `karuo-0.91/LICENSE` & `karuo-0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/__init__.py` & `karuo-0.92/karuo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,11 +21,12 @@
 @version 0.83 [2023-02-16] 增加企微获取访问用户身份接口 auth/getuserinfo
 @version 0.84 [2023-02-20] 增加企微置换user_ticket接口功能
 @version 0.85 [2023-02-26] 增加代理开发应用获取用户敏感信息接口
 @version 0.87 [2023-02-27] 修正获取企业用户编号列表的token错误
 @version 0.88 [2023-03-01] 修正了代开发应用获取托管企业通信录信息的接口
 @version 0.89 [2023-03-01] 修正了代开发应用获取托管企业通信录信息的接口
 @version 0.91 [2023-03-02] 修正了代开发应用获取托管企业通信录信息的接口
+@version 0.92 [2023-06-07] 增加消息撤回接口
 -------------------------------------------------
 """
 
-__version__ = "0.91"
+__version__ = "0.92"
```

### Comparing `karuo-0.91/karuo/baiduai/base.py` & `karuo-0.92/karuo/baiduai/base.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/baiduai/error_code.py` & `karuo-0.92/karuo/baiduai/error_code.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/baiduai/func_faces.py` & `karuo-0.92/karuo/baiduai/func_faces.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/baiduai/func_ocr.py` & `karuo-0.92/karuo/baiduai/func_ocr.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/datadef.py` & `karuo-0.92/karuo/datadef.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/decorators.py` & `karuo-0.92/karuo/decorators.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/helpers/char_helper.py` & `karuo-0.92/karuo/helpers/char_helper.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/helpers/date_helper.py` & `karuo-0.92/karuo/helpers/date_helper.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/helpers/logger_helper.py` & `karuo-0.92/karuo/helpers/logger_helper.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/qywx/WXBizMsgCrypt.py` & `karuo-0.92/karuo/qywx/WXBizMsgCrypt.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/qywx/base.py` & `karuo-0.92/karuo/qywx/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,14 +632,25 @@
         _params = self._loadSendmsgParams(agentid, "markdown", kwargs)
         _params["markdown"] = {
             "content": markdown
         }
 
         return self.postRequest("https://qyapi.weixin.qq.com/cgi-bin/message/send", params=_params)
 
+
+    def MsgRecall(self, msgid: str):
+        """
+        撤回24小时内发出的消息
+        """
+        _params = {
+            "msgid": msgid
+        }
+        return self.postRequest("https://qyapi.weixin.qq.com/cgi-bin/message/recall", params=_params)
+
+
     ######  辅助功能相关
     
     def UploadTempMedia(self, filetype, filepath=None, content=None):
         """
         :param filepath 图片文件路径
         :param content 图片文件内容 io.BytesIO
         上传临时素材
```

### Comparing `karuo-0.91/karuo/qywx/helper.py` & `karuo-0.92/karuo/qywx/helper.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/qywx/ierror.py` & `karuo-0.92/karuo/qywx/ierror.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo/qywx/provider.py` & `karuo-0.92/karuo/qywx/provider.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/karuo.egg-info/SOURCES.txt` & `karuo-0.92/karuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `karuo-0.91/setup.py` & `karuo-0.92/setup.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/test/test_ai_face.py` & `karuo-0.92/test/test_ai_face.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/test/test_ai_ocr.py` & `karuo-0.92/test/test_ai_ocr.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/test/test_helpers.py` & `karuo-0.92/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/test/test_normal.py` & `karuo-0.92/test/test_normal.py`

 * *Files identical despite different names*

### Comparing `karuo-0.91/test/test_qywx.py` & `karuo-0.92/test/test_qywx.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,14 +117,19 @@
         qywx_client = QywxClient("wx1ac9c673f281add6", "ghmdKl8bQZYS2cyXTTfk9rH4fnzDSBRqMwo0PFzManE")
         dir(qywx_client)
         # res = qywx_client.UserIdListBatch(1000)
         # qywx_client = QywxClient("wx1ac9c673f281add6", "wvDJd8FojHu9jNR0JfJ_xNJD9LfpCQU2cQMuGABQIXc")
         res = qywx_client.UserIdListFull(1000)
         pprint(res)
 
+    def test_recall_msg(self):
+        qywx_client = QywxClient("wx1ac9c673f281add6", "XlXsii63MDIkNW3iPeodXudxWcjjHqREGrYQVkA3DJ4")
+        res = qywx_client.MsgRecall("Dv0oBVNA9p2BIWPODPqgkn5Wqi8RUCCP7cVOVDaeUW2m6JsIQpXZrW195Ctsh8FErPeqZZbM85076hcrsnwGIA")
+        print(res)
+
     def testSingleMethod(self):
         self._tDocGetShareurl()
         # client = QywxClient("wx1ac9c673f281add6",
         #                 "lClGIPazrIcIFbeTkX13wBdRPbFm17tsslTQhMgvcd8")
         # result = client.CreateSchedule("long", 1607997600, 1608001200, ["caimmy", "long", "wangtao", "liangchaowei", "demouser"], "测试会议日程", "alsdkfjaslkdf asldfsadf拉丝机的弗拉sdf", "五楼会议室")
         
         # result = client.UpdateSchedule("caimmy", "8ace6b79414a03040d7b1569900b30a7", 1607997600, 1608001200, ["caimmy", "long", "wangtao", "liangchaowei"], "测试会议日程更新", "alsdkfjaslkdf asldfsadf拉丝机的弗拉sdf", "董事长办公室")
@@ -149,12 +154,14 @@
         #     ])
         # print(result)
         # print("----------------------")
 
         # result = client.GetDocFilesList("long", test_space_id)
         # print(result)
 
+    
+
 if "__main__" == __name__:
     suite = unittest.TestSuite()
-    suite.addTest(TestQywxClient("test_modified_address_interface"))
+    suite.addTest(TestQywxClient("test_recall_msg"))
     runner = unittest.TextTestRunner()
     runner.run(suite)
```

