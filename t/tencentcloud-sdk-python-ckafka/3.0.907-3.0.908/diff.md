# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.907.tar", last modified: Tue Jun  6 02:22:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.908.tar", last modified: Wed Jun  7 00:20:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.907.tar` & `tencentcloud-sdk-python-ckafka-3.0.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/ckafka/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)     3315 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)   468503 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)    70209 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/ckafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:22:23.000000 tencentcloud-sdk-python-ckafka-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   468693 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)    70209 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.907/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2341,19 +2341,19 @@
         :type ClusterId: int
         :param RenewFlag: 预付费自动续费标记，0表示默认状态(用户未设置，即初始状态)， 1表示自动续费，2表示明确不自动续费(用户设置)
         :type RenewFlag: int
         :param KafkaVersion: CKafka版本号[0.10.2、1.1.1、2.4.1], 默认是1.1.1
         :type KafkaVersion: str
         :param SpecificationsType: 实例类型: [标准版实例]填写 standard(默认), [专业版实例]填写 profession
         :type SpecificationsType: str
-        :param DiskSize: 磁盘大小,专业版不填写默认最小磁盘,填写后根据磁盘带宽分区数弹性计算
+        :param DiskSize: 磁盘大小，专业版不填写默认最小磁盘，如果跟控制台规格配比不相符，则无法创建成功
         :type DiskSize: int
-        :param BandWidth: 带宽,专业版不填写默认最小带宽,填写后根据磁盘带宽分区数弹性计算
+        :param BandWidth: 带宽，专业版不填写默认最小带宽，如果跟控制台规格配比不相符，则无法创建成功
         :type BandWidth: int
-        :param Partition: 分区大小,专业版不填写默认最小分区数,填写后根据磁盘带宽分区数弹性计算
+        :param Partition: 分区大小，专业版不填写默认最小分区数，如果跟控制台规格配比不相符，则无法创建成功
         :type Partition: int
         :param Tags: 标签
         :type Tags: list of Tag
         :param DiskType: 磁盘类型（ssd填写CLOUD_SSD，sata填写CLOUD_BASIC）
         :type DiskType: str
         :param MultiZoneFlag: 跨可用区，zoneIds必填
         :type MultiZoneFlag: bool
@@ -5779,20 +5779,24 @@
 
     """
 
     def __init__(self):
         r"""
         :param InstanceId: 实例唯一id
         :type InstanceId: str
+        :param RouteId: 路由id
+        :type RouteId: int
         """
         self.InstanceId = None
+        self.RouteId = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
+        self.RouteId = params.get("RouteId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.907/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.908/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.907/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.908/setup.py`

 * *Files identical despite different names*

