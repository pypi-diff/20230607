# Comparing `tmp/tencentcloud-sdk-python-apigateway-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-apigateway-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.907.tar", last modified: Tue Jun  6 02:18:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.908.tar", last modified: Wed Jun  7 00:16:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apigateway-3.0.907.tar` & `tencentcloud-sdk-python-apigateway-3.0.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/
--rw-r--r--   0 root         (0) root         (0)    95967 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/apigateway_client.py
--rw-r--r--   0 root         (0) root         (0)    20869 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)   402836 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:18:27.000000 tencentcloud-sdk-python-apigateway-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/apigateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/apigateway/v20180808/
+-rw-r--r--   0 root         (0) root         (0)    95982 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/apigateway/v20180808/apigateway_client.py
+-rw-r--r--   0 root         (0) root         (0)    20869 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/apigateway/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/apigateway/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   402836 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/apigateway/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud_sdk_python_apigateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:16:28.000000 tencentcloud-sdk-python-apigateway-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.907/README.rst` & `tencentcloud-sdk-python-apigateway-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/apigateway_client.py` & `tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/apigateway/v20180808/apigateway_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2253,15 +2253,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpdateService(self, request):
-        """本接口（UpdateService）用于从服务发布的环境中运行版本切换到特定版本。用户在使用 API 网关创建服务并发布服务到某个环境后，多因开发过程会产生多个版本，此时可调用本接口。
+        """本接口（UpdateService）用于从服务已发布的环境中将运行版本切换到特定版本。用户在使用 API 网关创建服务并发布服务到某个环境后，如在开发过程产生多个版本需要切换，此时可调用本接口。
 
         :param request: Request instance for UpdateService.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.UpdateServiceRequest`
         :rtype: :class:`tencentcloud.apigateway.v20180808.models.UpdateServiceResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/errorcodes.py` & `tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/apigateway/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/apigateway/v20180808/models.py` & `tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/apigateway/v20180808/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.907/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.908/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.908/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.907/setup.py` & `tencentcloud-sdk-python-apigateway-3.0.908/setup.py`

 * *Files identical despite different names*

