# Comparing `tmp/tencentcloud-sdk-python-sms-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-sms-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.907.tar", last modified: Tue Jun  6 02:33:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.908.tar", last modified: Wed Jun  7 00:31:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sms-3.0.907.tar` & `tencentcloud-sdk-python-sms-3.0.908.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20190711/
--rw-r--r--   0 root         (0) root         (0)    26567 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20190711/sms_client.py
--rw-r--r--   0 root         (0) root         (0)    18520 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20190711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20190711/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60142 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20190711/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20210111/
--rw-r--r--   0 root         (0) root         (0)    28333 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20210111/sms_client.py
--rw-r--r--   0 root         (0) root         (0)    19342 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20210111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20210111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68439 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20210111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud_sdk_python_sms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/tencentcloud_sdk_python_sms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:33:33.000000 tencentcloud-sdk-python-sms-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/
+-rw-r--r--   0 root         (0) root         (0)    26567 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)    18520 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60142 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/
+-rw-r--r--   0 root         (0) root         (0)    28333 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)    19342 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68439 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-sms-3.0.907/README.rst` & `tencentcloud-sdk-python-sms-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20190711/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/sms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20190711/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20190711/models.py` & `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20210111/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/sms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20210111/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.907/tencentcloud/sms/v20210111/models.py` & `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sms-3.0.907/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.907/tencentcloud_sdk_python_sms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.908/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.907/setup.py` & `tencentcloud-sdk-python-sms-3.0.908/setup.py`

 * *Files identical despite different names*
