# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.907.tar", last modified: Tue Jun  6 02:29:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.908.tar", last modified: Wed Jun  7 00:27:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.907.tar` & `tencentcloud-sdk-python-lighthouse-3.0.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    26133 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    92541 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   240370 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:29:48.000000 tencentcloud-sdk-python-lighthouse-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    26133 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    92541 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   240371 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/lighthouse/v20200324/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:27:33.000000 tencentcloud-sdk-python-lighthouse-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.907/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud/lighthouse/v20200324/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5219,16 +5219,16 @@
     """
 
     def __init__(self):
         r"""
         :param AutoGeneratePassword: <li>"YES"代表选择自动生成密码，这时不指定Password字段。</li>
 <li>"NO"代表选择自定义密码，这时要指定Password字段。</li>
         :type AutoGeneratePassword: str
-        :param Password: 实例登录密码。具体按照操作系统的复杂度要求。
-WINDOWS 实例密码必须 12-30 位，不能以“/”开头且不包括用户名，至少包含以下字符中的三种不同字符
+        :param Password: 实例登录密码。具体按照操作系统的复杂度要求。 
+WINDOWS 实例密码必须 12-30 位，不能以“/”开头且不包括用户名, 至少包含以下字符中的三种不同字符 
 <li>小写字母：[a-z]</li>
 <li>大写字母：[A-Z]</li>
 <li>数字： 0-9</li>
 <li>特殊字符：()`~!@#$%^&*-+=_|{}[]:;' <>,.?/</li>
         :type Password: str
         """
         self.AutoGeneratePassword = None
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.907/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.908/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.908/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.907/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.908/setup.py`

 * *Files identical despite different names*

