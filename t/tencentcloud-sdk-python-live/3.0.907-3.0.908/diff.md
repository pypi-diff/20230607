# Comparing `tmp/tencentcloud-sdk-python-live-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.907.tar", last modified: Tue Jun  6 02:29:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.908.tar", last modified: Wed Jun  7 00:27:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.907.tar` & `tencentcloud-sdk-python-live-3.0.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   137451 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    18487 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   433012 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:29:55.000000 tencentcloud-sdk-python-live-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   137299 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    18702 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   433941 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:27:39.000000 tencentcloud-sdk-python-live-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-live-3.0.907/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.908/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.907/README.rst` & `tencentcloud-sdk-python-live-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.908/tencentcloud/live/v20180801/live_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2396,15 +2396,14 @@
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeStreamPlayInfoList(self, request):
         """查询播放数据，支持按流名称查询详细播放数据，也可按播放域名查询详细总数据，数据延迟4分钟左右。
-        注意：按AppName查询请先联系工单申请，开通后配置生效预计需要5个工作日左右，具体时间以最终回复为准。
 
         :param request: Request instance for DescribeStreamPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeStreamPlayInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeStreamPlayInfoListResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.908/tencentcloud/live/v20180801/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,14 +388,20 @@
 
 # 裁剪区域溢出原始图片。
 INVALIDPARAMETER_INVALIDCROPPARAM = 'InvalidParameter.InvalidCropParam'
 
 # 图层参数错误。
 INVALIDPARAMETER_INVALIDLAYERPARAM = 'InvalidParameter.InvalidLayerParam'
 
+# 混流输入参数无效。
+INVALIDPARAMETER_INVALIDMIXINPUTPARAM = 'InvalidParameter.InvalidMixInputParam'
+
+# 输出流参数无效。
+INVALIDPARAMETER_INVALIDOUTPUTPARAM = 'InvalidParameter.InvalidOutputParam'
+
 # 输出流 ID 被占用。
 INVALIDPARAMETER_INVALIDOUTPUTSTREAMID = 'InvalidParameter.InvalidOutputStreamID'
 
 # 非法输出类型，检查 OutputPram-StreamId 与 OutputType 是否匹配。
 INVALIDPARAMETER_INVALIDOUTPUTTYPE = 'InvalidParameter.InvalidOutputType'
 
 # 水印 ID 未设置。
```

### Comparing `tencentcloud-sdk-python-live-3.0.907/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.908/tencentcloud/live/v20180801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1326,15 +1326,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param SourceType: 拉流源的类型：
 PullLivePushLive -直播，
-PullVodPushLive -点播。
+PullVodPushLive -点播，
 PullPicPushLive -图片。
         :type SourceType: str
         :param SourceUrls: 拉流源 url 列表。
 SourceType 为直播（PullLivePushLive）只可以填1个，
 SourceType 为点播（PullVodPushLive）可以填多个，上限30个。
 当前支持的文件格式：flv，mp4，hls。
 当前支持的拉流协议：http，https，rtmp，rtmps，rtsp，srt。
@@ -2565,15 +2565,18 @@
 class DayStreamPlayInfo(AbstractModel):
     """流播放信息
 
     """
 
     def __init__(self):
         r"""
-        :param Time: 数据时间点，格式：yyyy-mm-dd HH:MM:SS。
+        :param Time: 数据时间点，接口返回支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）yyyy-MM-dd HH:mm:ss：使用此格式时，默认代表北京时间。
+接口返回的时间格式和查询请求传入的时间格式一致。
         :type Time: str
         :param Bandwidth: 带宽（单位Mbps）。
         :type Bandwidth: float
         :param Flux: 流量 （单位MB）。
         :type Flux: float
         :param Request: 请求数。
         :type Request: int
@@ -7297,28 +7300,32 @@
 class DescribeStreamPlayInfoListRequest(AbstractModel):
     """DescribeStreamPlayInfoList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param StartTime: 开始时间，北京时间，格式为yyyy-mm-dd HH:MM:SS
+        :param StartTime: 起始时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）yyyy-MM-dd HH:mm:ss：使用此格式时，默认代表北京时间。
+开始时间和结束时间的格式需要保持一致。
         :type StartTime: str
-        :param EndTime: 结束时间，北京时间，格式为yyyy-mm-dd HH:MM:SS，
-结束时间 和 开始时间跨度不支持超过24小时，支持距当前时间一个月内的数据查询。
+        :param EndTime: 结束时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）yyyy-MM-dd HH:mm:ss：使用此格式时，默认代表北京时间。
+开始时间和结束时间的格式需要保持一致。结束时间和开始时间跨度不支持超过24小时，支持距当前时间一个月内的数据查询。
         :type EndTime: str
         :param PlayDomain: 播放域名，
 若不填，则为查询所有播放域名的在线流数据。
         :type PlayDomain: str
         :param StreamName: 流名称，精确匹配。
 若不填，则为查询总体播放数据。
         :type StreamName: str
         :param AppName: 推流路径，与播放地址中的AppName保持一致，会精确匹配，在同时传递了StreamName时生效。
 若不填，则为查询总体播放数据。
-注意：按AppName查询请先联系工单申请，开通后配置生效预计需要5个工作日左右，具体时间以最终回复为准。
         :type AppName: str
         :param ServiceName: 服务名称，可选值包括LVB(标准直播)，LEB(快直播)，不填则查LVB+LEB总值。
         :type ServiceName: str
         """
         self.StartTime = None
         self.EndTime = None
         self.PlayDomain = None
@@ -10467,14 +10474,17 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type WatermarkList: list of PullPushWatermarkInfo
         :param VodLocalMode: 点播源是否启用本地推流模式，默认0，不启用。
 0 - 不启用。
 1 - 启用。
 注意：此字段可能返回 null，表示取不到有效值。
         :type VodLocalMode: int
+        :param RecordTemplateId: 录制模板 ID。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RecordTemplateId: str
         """
         self.TaskId = None
         self.SourceType = None
         self.SourceUrls = None
         self.DomainName = None
         self.AppName = None
         self.StreamName = None
@@ -10495,14 +10505,15 @@
         self.Status = None
         self.RecentPullInfo = None
         self.Comment = None
         self.BackupSourceType = None
         self.BackupSourceUrl = None
         self.WatermarkList = None
         self.VodLocalMode = None
+        self.RecordTemplateId = None
 
 
     def _deserialize(self, params):
         self.TaskId = params.get("TaskId")
         self.SourceType = params.get("SourceType")
         self.SourceUrls = params.get("SourceUrls")
         self.DomainName = params.get("DomainName")
@@ -10532,14 +10543,15 @@
         if params.get("WatermarkList") is not None:
             self.WatermarkList = []
             for item in params.get("WatermarkList"):
                 obj = PullPushWatermarkInfo()
                 obj._deserialize(item)
                 self.WatermarkList.append(obj)
         self.VodLocalMode = params.get("VodLocalMode")
+        self.RecordTemplateId = params.get("RecordTemplateId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-live-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.908/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.908/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.907/setup.py` & `tencentcloud-sdk-python-live-3.0.908/setup.py`

 * *Files identical despite different names*

