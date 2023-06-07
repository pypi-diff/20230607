# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.907.tar", last modified: Tue Jun  6 02:39:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.908.tar", last modified: Wed Jun  7 00:36:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.907.tar` & `tencentcloud-sdk-python-waf-3.0.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)    46563 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)     2711 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   180770 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:39:21.000000 tencentcloud-sdk-python-waf-3.0.907/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)    46563 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   180770 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:36:42.000000 tencentcloud-sdk-python-waf-3.0.908/tencentcloud_sdk_python_waf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-waf-3.0.907/README.rst` & `tencentcloud-sdk-python-waf-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.908/tencentcloud/waf/v20180125/waf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.908/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.907/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.908/tencentcloud/waf/v20180125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4871,15 +4871,15 @@
 class ResponseCode(AbstractModel):
     """响应体的返回码
 
     """
 
     def __init__(self):
         r"""
-        :param Code: 如果成功则返回Success，失败则返回yunapi定义的错误码
+        :param Code: 如果成功则返回Success，失败则返回云api定义的错误码
         :type Code: str
         :param Message: 如果成功则返回Success，失败则返回WAF定义的二级错误码
         :type Message: str
         """
         self.Code = None
         self.Message = None
```

### Comparing `tencentcloud-sdk-python-waf-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.908/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-waf-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.908/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.907/setup.py` & `tencentcloud-sdk-python-waf-3.0.908/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.907/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.908/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

