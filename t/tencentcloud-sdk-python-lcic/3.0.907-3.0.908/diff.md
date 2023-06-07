# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.907.tar", last modified: Tue Jun  6 02:29:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.908.tar", last modified: Wed Jun  7 00:27:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.907.tar` & `tencentcloud-sdk-python-lcic-3.0.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/lcic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/lcic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)     4414 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142076 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)    48649 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:29:43.000000 tencentcloud-sdk-python-lcic-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/lcic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/lcic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)     4414 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142076 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)    48649 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:27:28.000000 tencentcloud-sdk-python-lcic-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.907/README.rst` & `tencentcloud-sdk-python-lcic-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/lcic/v20220817/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.908/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.907/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.908/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.908/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.907/setup.py` & `tencentcloud-sdk-python-lcic-3.0.908/setup.py`

 * *Files identical despite different names*
