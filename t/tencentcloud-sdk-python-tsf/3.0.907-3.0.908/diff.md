# Comparing `tmp/tencentcloud-sdk-python-tsf-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-tsf-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.907.tar", last modified: Tue Jun  6 02:38:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.908.tar", last modified: Wed Jun  7 00:35:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tsf-3.0.907.tar` & `tencentcloud-sdk-python-tsf-3.0.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:38:30.000000 tencentcloud-sdk-python-tsf-3.0.907/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:38:29.000000 tencentcloud-sdk-python-tsf-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:38:30.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:38:30.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/tsf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:38:30.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/tsf/v20180326/
--rw-r--r--   0 root         (0) root         (0)    49851 2023-06-06 02:38:29.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/tsf/v20180326/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   195353 2023-06-06 02:38:29.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/tsf/v20180326/tsf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:38:29.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/tsf/v20180326/__init__.py
--rw-r--r--   0 root         (0) root         (0)   802528 2023-06-06 02:38:29.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/tsf/v20180326/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:38:29.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/tsf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:38:29.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:38:30.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud_sdk_python_tsf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:38:30.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 02:38:30.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:38:30.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:38:30.000000 tencentcloud-sdk-python-tsf-3.0.907/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:38:30.000000 tencentcloud-sdk-python-tsf-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:38:29.000000 tencentcloud-sdk-python-tsf-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:38:30.000000 tencentcloud-sdk-python-tsf-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/tsf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/tsf/v20180326/
+-rw-r--r--   0 root         (0) root         (0)    49851 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/tsf/v20180326/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   196336 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/tsf/v20180326/tsf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/tsf/v20180326/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   806878 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/tsf/v20180326/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/tsf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud_sdk_python_tsf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:35:46.000000 tencentcloud-sdk-python-tsf-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.907/README.rst` & `tencentcloud-sdk-python-tsf-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/tsf/v20180326/errorcodes.py` & `tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/tsf/v20180326/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/tsf/v20180326/tsf_client.py` & `tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/tsf/v20180326/tsf_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1978,14 +1978,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeContainerGroupAttribute(self, request):
+        """获取部署组其他字段-用于前端并发调用
+
+        :param request: Request instance for DescribeContainerGroupAttribute.
+        :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeContainerGroupAttributeRequest`
+        :rtype: :class:`tencentcloud.tsf.v20180326.models.DescribeContainerGroupAttributeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeContainerGroupAttribute", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeContainerGroupAttributeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeContainerGroupDeployInfo(self, request):
         """获取部署组详情
 
         :param request: Request instance for DescribeContainerGroupDeployInfo.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeContainerGroupDeployInfoRequest`
         :rtype: :class:`tencentcloud.tsf.v20180326.models.DescribeContainerGroupDeployInfoResponse`
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/tsf/v20180326/models.py` & `tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/tsf/v20180326/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2920,14 +2920,92 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ContainerGroupOther(AbstractModel):
+    """部署组列表-其它字段
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceNum: 实例总数
+        :type InstanceNum: int
+        :param CurrentNum: 已启动实例总数
+        :type CurrentNum: int
+        :param LbIp: 负载均衡ip
+        :type LbIp: str
+        :param ClusterIp: Service ip
+        :type ClusterIp: str
+        :param Status: 服务状态，请参考后面的的状态定义
+        :type Status: str
+        :param Message: 服务状态，请参考后面的的状态定义
+        :type Message: str
+        :param Envs: 环境变量
+        :type Envs: list of Env
+        :param NodePort: Service NodePort
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NodePort: int
+        :param SubnetId: 子网ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubnetId: str
+        :param HealthCheckSettings: 健康检查相关字段
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HealthCheckSettings: list of HealthCheckSetting
+        :param IsNotEqualServiceConfig: 服务配置信息是否匹配
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsNotEqualServiceConfig: bool
+        """
+        self.InstanceNum = None
+        self.CurrentNum = None
+        self.LbIp = None
+        self.ClusterIp = None
+        self.Status = None
+        self.Message = None
+        self.Envs = None
+        self.NodePort = None
+        self.SubnetId = None
+        self.HealthCheckSettings = None
+        self.IsNotEqualServiceConfig = None
+
+
+    def _deserialize(self, params):
+        self.InstanceNum = params.get("InstanceNum")
+        self.CurrentNum = params.get("CurrentNum")
+        self.LbIp = params.get("LbIp")
+        self.ClusterIp = params.get("ClusterIp")
+        self.Status = params.get("Status")
+        self.Message = params.get("Message")
+        if params.get("Envs") is not None:
+            self.Envs = []
+            for item in params.get("Envs"):
+                obj = Env()
+                obj._deserialize(item)
+                self.Envs.append(obj)
+        self.NodePort = params.get("NodePort")
+        self.SubnetId = params.get("SubnetId")
+        if params.get("HealthCheckSettings") is not None:
+            self.HealthCheckSettings = []
+            for item in params.get("HealthCheckSettings"):
+                obj = HealthCheckSetting()
+                obj._deserialize(item)
+                self.HealthCheckSettings.append(obj)
+        self.IsNotEqualServiceConfig = params.get("IsNotEqualServiceConfig")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ContinueRunFailedTaskBatchRequest(AbstractModel):
     """ContinueRunFailedTaskBatch请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8273,14 +8351,61 @@
     def _deserialize(self, params):
         if params.get("Result") is not None:
             self.Result = TsfPageContainerEvent()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeContainerGroupAttributeRequest(AbstractModel):
+    """DescribeContainerGroupAttribute请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param GroupId: 部署组ID
+        :type GroupId: str
+        """
+        self.GroupId = None
+
+
+    def _deserialize(self, params):
+        self.GroupId = params.get("GroupId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeContainerGroupAttributeResponse(AbstractModel):
+    """DescribeContainerGroupAttribute返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Result: 部署组列表-其它字段
+        :type Result: :class:`tencentcloud.tsf.v20180326.models.ContainerGroupOther`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Result = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Result") is not None:
+            self.Result = ContainerGroupOther()
+            self.Result._deserialize(params.get("Result"))
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeContainerGroupDeployInfoRequest(AbstractModel):
     """DescribeContainerGroupDeployInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tsf-3.0.908/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tsf-3.0.907/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.908/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.908/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.907/setup.py` & `tencentcloud-sdk-python-tsf-3.0.908/setup.py`

 * *Files identical despite different names*

