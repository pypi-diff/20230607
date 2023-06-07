# Comparing `tmp/tencentcloud-sdk-python-ccc-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-ccc-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.907.tar", last modified: Tue Jun  6 02:20:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.908.tar", last modified: Wed Jun  7 00:18:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ccc-3.0.907.tar` & `tencentcloud-sdk-python-ccc-3.0.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/ccc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/ccc/v20200210/
--rw-r--r--   0 root         (0) root         (0)    36406 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/ccc/v20200210/ccc_client.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/ccc/v20200210/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/ccc/v20200210/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142129 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/ccc/v20200210/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud_sdk_python_ccc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:20:56.000000 tencentcloud-sdk-python-ccc-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/
+-rw-r--r--   0 root         (0) root         (0)    36406 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/ccc_client.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142129 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud_sdk_python_ccc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.907/README.rst` & `tencentcloud-sdk-python-ccc-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/ccc/v20200210/ccc_client.py` & `tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/ccc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/ccc/v20200210/errorcodes.py` & `tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/ccc/v20200210/models.py` & `tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3160,15 +3160,15 @@
         :type Type: int
         :param CapacitySize: 套餐包总量
         :type CapacitySize: int
         :param CapacityRemain: 套餐包剩余量
         :type CapacityRemain: int
         :param BuyTime: 购买时间戳
         :type BuyTime: int
-        :param EndTime: 截至时间戳
+        :param EndTime: 截止时间戳
         :type EndTime: int
         """
         self.PackageId = None
         self.Type = None
         self.CapacitySize = None
         self.CapacityRemain = None
         self.BuyTime = None
@@ -3202,15 +3202,15 @@
         :type PhoneNum: str
         :param Type: 号码类型，0-固话|1-虚商号码|2-运营商号码|3-400号码
         :type Type: int
         :param CallType: 号码呼叫类型，1-呼入|2-呼出|3-呼入呼出
         :type CallType: int
         :param BuyTime: 购买时间戳
         :type BuyTime: int
-        :param EndTime: 截至时间戳
+        :param EndTime: 截止时间戳
         :type EndTime: int
         :param State: 号码状态，1正常|2欠费停用|4管理员停用|5违规停用
         :type State: int
         """
         self.PhoneNum = None
         self.Type = None
         self.CallType = None
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ccc-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.908/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.907/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.908/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.907/setup.py` & `tencentcloud-sdk-python-ccc-3.0.908/setup.py`

 * *Files identical despite different names*

