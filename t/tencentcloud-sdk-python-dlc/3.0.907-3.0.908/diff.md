# Comparing `tmp/tencentcloud-sdk-python-dlc-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-dlc-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.907.tar", last modified: Tue Jun  6 02:25:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.908.tar", last modified: Wed Jun  7 00:22:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dlc-3.0.907.tar` & `tencentcloud-sdk-python-dlc-3.0.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/dlc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/dlc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)    81336 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   340367 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud_sdk_python_dlc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:25:19.000000 tencentcloud-sdk-python-dlc-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/dlc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/dlc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)    82270 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   342962 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud_sdk_python_dlc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:22:47.000000 tencentcloud-sdk-python-dlc-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.907/README.rst` & `tencentcloud-sdk-python-dlc-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1885,14 +1885,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifySparkAppBatch(self, request):
+        """本接口（ModifySparkAppBatch）用于批量修改Spark作业参数配置
+
+        :param request: Request instance for ModifySparkAppBatch.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.ModifySparkAppBatchRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.ModifySparkAppBatchResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifySparkAppBatch", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifySparkAppBatchResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyUser(self, request):
         """修改用户信息
 
         :param request: Request instance for ModifyUser.
         :type request: :class:`tencentcloud.dlc.v20210125.models.ModifyUserRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.ModifyUserResponse`
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/dlc/v20210125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6661,14 +6661,79 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifySparkAppBatchRequest(AbstractModel):
+    """ModifySparkAppBatch请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SparkAppId: 需要批量修改的Spark作业任务ID列表
+        :type SparkAppId: list of str
+        :param DataEngine: 引擎ID
+        :type DataEngine: str
+        :param AppDriverSize: driver规格：small,medium,large,xlarge；内存型(引擎类型)：m.small,m.medium,m.large,m.xlarge
+        :type AppDriverSize: str
+        :param AppExecutorSize: executor规格：small,medium,large,xlarge；内存型(引擎类型)：m.small,m.medium,m.large,m.xlarge
+        :type AppExecutorSize: str
+        :param AppExecutorNums: 指定executor数量，最小值为1，最大值小于集群规格
+        :type AppExecutorNums: int
+        :param AppExecutorMaxNumbers: 指定executor max数量（动态配置场景下），最小值为1，最大值小于集群规格（当ExecutorMaxNumbers小于ExecutorNums时，改值设定为ExecutorNums）
+        :type AppExecutorMaxNumbers: int
+        :param IsInherit: 任务资源配置是否继承集群模板，0（默认）不继承，1：继承
+        :type IsInherit: int
+        """
+        self.SparkAppId = None
+        self.DataEngine = None
+        self.AppDriverSize = None
+        self.AppExecutorSize = None
+        self.AppExecutorNums = None
+        self.AppExecutorMaxNumbers = None
+        self.IsInherit = None
+
+
+    def _deserialize(self, params):
+        self.SparkAppId = params.get("SparkAppId")
+        self.DataEngine = params.get("DataEngine")
+        self.AppDriverSize = params.get("AppDriverSize")
+        self.AppExecutorSize = params.get("AppExecutorSize")
+        self.AppExecutorNums = params.get("AppExecutorNums")
+        self.AppExecutorMaxNumbers = params.get("AppExecutorMaxNumbers")
+        self.IsInherit = params.get("IsInherit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifySparkAppBatchResponse(AbstractModel):
+    """ModifySparkAppBatch返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifySparkAppRequest(AbstractModel):
     """ModifySparkApp请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dlc-3.0.908/tencentcloud/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.907'
+__version__ = '3.0.908'
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.908/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.907/setup.py` & `tencentcloud-sdk-python-dlc-3.0.908/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.907/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.908/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

