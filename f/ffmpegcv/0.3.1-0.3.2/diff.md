# Comparing `tmp/ffmpegcv-0.3.1.tar.gz` & `tmp/ffmpegcv-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ffmpegcv-0.3.1.tar", last modified: Tue May 30 19:22:10 2023, max compression
+gzip compressed data, was "dist/ffmpegcv-0.3.2.tar", last modified: Wed Jun  7 05:49:57 2023, max compression
```

## Comparing `ffmpegcv-0.3.1.tar` & `ffmpegcv-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10392 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/PKG-INFO
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10179 2023-05-30 19:12:16.000000 ffmpegcv-0.3.1/README.md
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10453 2023-05-30 19:18:41.000000 ffmpegcv-0.3.1/ffmpegcv/__init__.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5265 2022-05-18 13:48:31.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_framepick.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     9732 2023-05-30 14:58:25.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    15029 2023-05-30 14:58:25.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_camera.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1685 2022-05-19 12:21:02.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_grey.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1474 2022-06-04 11:24:12.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_hflip.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2618 2022-05-19 17:30:20.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_laggy.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3935 2023-05-30 19:00:58.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_stream.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3989 2023-05-30 15:02:00.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_writer.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1053 2023-05-30 17:50:58.000000 ffmpegcv-0.3.1/ffmpegcv/stream_info.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2731 2023-05-30 15:03:32.000000 ffmpegcv-0.3.1/ffmpegcv/video_info.py
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv.egg-info/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10392 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv.egg-info/PKG-INFO
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      487 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv.egg-info/SOURCES.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        1 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv.egg-info/dependency_links.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        6 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv.egg-info/requires.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        9 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv.egg-info/top_level.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)       38 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/setup.cfg
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      643 2023-05-30 19:21:17.000000 ffmpegcv-0.3.1/setup.py
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    11279 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/PKG-INFO
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    11066 2023-06-07 05:48:36.000000 ffmpegcv-0.3.2/README.md
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10453 2023-05-30 19:18:41.000000 ffmpegcv-0.3.2/ffmpegcv/__init__.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5265 2022-05-18 13:48:31.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_framepick.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     9732 2023-05-30 14:58:25.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    15029 2023-05-30 14:58:25.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_camera.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1685 2022-05-19 12:21:02.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_grey.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1474 2022-06-04 11:24:12.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_hflip.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2618 2022-05-19 17:30:20.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_laggy.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3935 2023-05-30 19:00:58.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_stream.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3989 2023-05-30 15:02:00.000000 ffmpegcv-0.3.2/ffmpegcv/ffmpeg_writer.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1053 2023-05-30 17:50:58.000000 ffmpegcv-0.3.2/ffmpegcv/stream_info.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2731 2023-05-30 15:03:32.000000 ffmpegcv-0.3.2/ffmpegcv/video_info.py
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv.egg-info/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    11279 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv.egg-info/PKG-INFO
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      487 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv.egg-info/SOURCES.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        1 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv.egg-info/dependency_links.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        6 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv.egg-info/requires.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        9 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/ffmpegcv.egg-info/top_level.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)       38 2023-06-07 05:49:57.000000 ffmpegcv-0.3.2/setup.cfg
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      650 2023-06-07 05:13:57.000000 ffmpegcv-0.3.2/setup.py
```

### Comparing `ffmpegcv-0.3.1/PKG-INFO` & `ffmpegcv-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpegcv
-Version: 0.3.1
+Version: 0.3.2
 Home-page: https://pypi.org/project/ffmpegcv/
 Author: chenxf
 Author-email: cxf529125853@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # FFMPEGCV is an alternative to OPENCV for video read and write.
@@ -12,40 +12,59 @@
 
 - The ffmpegcv is api **compatible** to open-cv. 
 - The ffmpegcv can use **GPU accelerate** encoding and decoding*. 
 - The ffmpegcv support much more video **codecs** v.s. open-cv.
 - The ffmpegcv support **RGB** & BGR format as you like.
 - The ffmpegcv can support ROI operations.You can **crop**, **resize** and **pad** the ROI.
 
-In all, ffmpegcv is just similar to opencv api. But is faster* and with more codecs.
+In all, ffmpegcv is just similar to opencv api. But is has more codecs and does't require opencv installed.
 
+Functions:
+- `VideoWriter`: Write a video file.
+- `VideoCapture`: Read a video file.
+- `VideoCaptureCAM`: Read a camera.
+- `VideoCaptureStream`: Read a RTP/RTSP/RTMP/HTTP stream.
+
+## Install
+You need to download ffmpeg before you can use ffmpegcv.
+```
+ #1A. LINUX: sudo apt install ffmpeg
+ #1B. MAC: brew install ffmpeg
+ #1C. WINDOWS: download ffmpeg and add to the path
+ 
+ conda install ffmpeg  #1D. CONDA
+ pip install ffmpegcv
+ ```
+
+## When should choose `ffmpegcv` other than `opencv`:
+- The `opencv` is hard to install. The ffmpegcv only requires `numpy` and `FFmpeg`, works across Mac/Windows/Linux platforms.
+- The `opencv` packages too much image processing toolbox. You just want a simple video/camero IO with GPU accessible.
+- The `opencv` didn't support `h264`/`h265` and other video writers.
+- You want to **crop**, **resize** and **pad** the video/camero ROI.
 
 ## Basic example
 Read a video by CPU, and rewrite it by GPU.
 ```python
 vidin = ffmpegcv.VideoCapture(vfile_in)
 vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)
 
 with vidin, vidout:
     for frame in vidin:
         cv2.imshow('image', frame)
         vidout.write(frame)
 ```
 
-Read the camera by device name.
+Read the camera.
 ```python
+# by device ID
+cap = ffmpegcv.VideoCaptureCAM(0)
+# by device name
 cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
 ```
 
-## Install
-You need to download ffmpeg before you can use ffmpegcv
-> conda install ffmpeg 
->
-> pip install ffmpegcv
-
 ## GPU Accelation
 - Support NVIDIA card only.
 - Perfect in the **Windows**. That ffmpeg supports NVIDIA acceleration just by conda install.
 - Struggle in the **Linux**. That ffmpeg didn't orginally support NVIDIA accelerate.
 Please re-compile the ffmpeg by yourself.
 See the [link](https://docs.nvidia.com/video-technologies/video-codec-sdk/ffmpeg-with-nvidia-gpu/)
 - Works in the **Google Colab** notebook without pain (no need to recompile ffmpeg). 
@@ -200,15 +219,15 @@
 ## Camera Reader
 ---
 **Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. 
 
 - The `VideoCaptureCAM` aims to support ROI operations. The Opencv will be general fascinating than ffmpegcv in camera read. **I recommand the opencv in most camera reading case**.
 - The ffmpegcv can use name to retrieve the camera device. Use `ffmpegcv.VideoCaptureCAM("Integrated Camera")` is readable than `cv2.VideoCaptureCAM(0)`.
 - The `VideoCaptureCAM` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
-- The `VideoCaptureCAM` is continously working on background even if you didn't read it. Please release it in time.
+- The `VideoCaptureCAM` is continously working on background even if you didn't read it. **Please release it in time**.
 - Works perfect in Windows, not-perfect in Linux and macOS.
 
 ```python
 import cv2
 cap = cv2.VideoCapture(0)
 while True:
     ret, frame = cap.read()
@@ -237,15 +256,15 @@
 
 # ffmpegcv use camera with ROI operations
 cap = ffmpegcv.VideoCaptureCAM("Integrated Camera", crop_xywh=(0, 0, 640, 480), resize=(512, 512), resize_keepratio=True)
 
 
 ```
 
-**list all camera devices**
+**List all camera devices**
 ```python
 from ffmpegcv.ffmpeg_reader_camera import query_camera_devices
 
 devices = query_camera_devices()
 print(devices)
 ```
 >{0: ('Integrated Camera', '@device_pnp_\\\\?\\usb#vid_2304&pid_oot#media#0001#{65e8773d-8f56-11d0-a3b9-00a0c9223196}\\global'),  
@@ -266,42 +285,44 @@
 **Known issues**
 1. The VideoCaptureCAM didn't give a smooth experience in macOS. You must specify all the camera parameters. And the query_camera_options woun't give any suggestion. That's because the `ffmpeg` cannot list device options using mac native `avfoundation`. 
 ```python
 # The macOS requires full argument.
 cap = ffmpegcv.VideoCaptureCAM('FaceTime HD Camera', camsize_wh=(1280,720), camfps=30, campix_fmt='nv12')
 ```
 
-2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS blank.
+2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS empty.
 
 
 ## Stream Reader
-**Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. The feature is like a camera.
+**Experimental feature**. The ffmpegcv offers Stream reader. Which is consistent with VideoFiler reader, and more similiar to the camera.
 Becareful when using it.
 
 - Support `RTSP`, `RTP`, `RTMP`, `HTTP`, `HTTPS` streams.
 - The `VideoCaptureStream` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
-- The `VideoCaptureStream` is continously working on background even if you didn't read it. Please release it in time.
+- The `VideoCaptureStream` is continously working on background even if you didn't read it. **Please release it in time**.
+- It's still experimental. Recommand you to use opencv.
 
 
 ```python
+# opencv
 import cv2
 stream_url = 'http://devimages.apple.com.edgekey.net/streaming/examples/bipbop_4x3/gear2/prog_index.m3u8'
 cap = cv2.VideoCapture(stream_url, cv2.CAP_FFMPEG)
 
 if not cap.isOpened():
     print('Cannot open the stream')
     exit(-1)
 
 while True:
     ret, frame = cap.read()
     if not ret:
         break
     pass
 
-# ffmpegcv, in Windows&Linux
+# ffmpegcv
 import ffmpegcv
 cap = ffmpegcv.VideoCaptureStream(stream_url)
 while True:
     ret, frame = cap.read()
     if not ret:
         break
     pass
```

### Comparing `ffmpegcv-0.3.1/README.md` & `ffmpegcv-0.3.2/ffmpegcv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,70 @@
+Metadata-Version: 2.1
+Name: ffmpegcv
+Version: 0.3.2
+Home-page: https://pypi.org/project/ffmpegcv/
+Author: chenxf
+Author-email: cxf529125853@163.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # FFMPEGCV is an alternative to OPENCV for video read and write.
 The ffmpegcv provide Video Reader and Video Witer with ffmpeg backbone, which are faster and powerful than cv2.
 
 - The ffmpegcv is api **compatible** to open-cv. 
 - The ffmpegcv can use **GPU accelerate** encoding and decoding*. 
 - The ffmpegcv support much more video **codecs** v.s. open-cv.
 - The ffmpegcv support **RGB** & BGR format as you like.
 - The ffmpegcv can support ROI operations.You can **crop**, **resize** and **pad** the ROI.
 
-In all, ffmpegcv is just similar to opencv api. But is faster* and with more codecs.
+In all, ffmpegcv is just similar to opencv api. But is has more codecs and does't require opencv installed.
 
+Functions:
+- `VideoWriter`: Write a video file.
+- `VideoCapture`: Read a video file.
+- `VideoCaptureCAM`: Read a camera.
+- `VideoCaptureStream`: Read a RTP/RTSP/RTMP/HTTP stream.
+
+## Install
+You need to download ffmpeg before you can use ffmpegcv.
+```
+ #1A. LINUX: sudo apt install ffmpeg
+ #1B. MAC: brew install ffmpeg
+ #1C. WINDOWS: download ffmpeg and add to the path
+ 
+ conda install ffmpeg  #1D. CONDA
+ pip install ffmpegcv
+ ```
+
+## When should choose `ffmpegcv` other than `opencv`:
+- The `opencv` is hard to install. The ffmpegcv only requires `numpy` and `FFmpeg`, works across Mac/Windows/Linux platforms.
+- The `opencv` packages too much image processing toolbox. You just want a simple video/camero IO with GPU accessible.
+- The `opencv` didn't support `h264`/`h265` and other video writers.
+- You want to **crop**, **resize** and **pad** the video/camero ROI.
 
 ## Basic example
 Read a video by CPU, and rewrite it by GPU.
 ```python
 vidin = ffmpegcv.VideoCapture(vfile_in)
 vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)
 
 with vidin, vidout:
     for frame in vidin:
         cv2.imshow('image', frame)
         vidout.write(frame)
 ```
 
-Read the camera by device name.
+Read the camera.
 ```python
+# by device ID
+cap = ffmpegcv.VideoCaptureCAM(0)
+# by device name
 cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
 ```
 
-## Install
-You need to download ffmpeg before you can use ffmpegcv
-> conda install ffmpeg 
->
-> pip install ffmpegcv
-
 ## GPU Accelation
 - Support NVIDIA card only.
 - Perfect in the **Windows**. That ffmpeg supports NVIDIA acceleration just by conda install.
 - Struggle in the **Linux**. That ffmpeg didn't orginally support NVIDIA accelerate.
 Please re-compile the ffmpeg by yourself.
 See the [link](https://docs.nvidia.com/video-technologies/video-codec-sdk/ffmpeg-with-nvidia-gpu/)
 - Works in the **Google Colab** notebook without pain (no need to recompile ffmpeg). 
@@ -191,15 +219,15 @@
 ## Camera Reader
 ---
 **Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. 
 
 - The `VideoCaptureCAM` aims to support ROI operations. The Opencv will be general fascinating than ffmpegcv in camera read. **I recommand the opencv in most camera reading case**.
 - The ffmpegcv can use name to retrieve the camera device. Use `ffmpegcv.VideoCaptureCAM("Integrated Camera")` is readable than `cv2.VideoCaptureCAM(0)`.
 - The `VideoCaptureCAM` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
-- The `VideoCaptureCAM` is continously working on background even if you didn't read it. Please release it in time.
+- The `VideoCaptureCAM` is continously working on background even if you didn't read it. **Please release it in time**.
 - Works perfect in Windows, not-perfect in Linux and macOS.
 
 ```python
 import cv2
 cap = cv2.VideoCapture(0)
 while True:
     ret, frame = cap.read()
@@ -228,15 +256,15 @@
 
 # ffmpegcv use camera with ROI operations
 cap = ffmpegcv.VideoCaptureCAM("Integrated Camera", crop_xywh=(0, 0, 640, 480), resize=(512, 512), resize_keepratio=True)
 
 
 ```
 
-**list all camera devices**
+**List all camera devices**
 ```python
 from ffmpegcv.ffmpeg_reader_camera import query_camera_devices
 
 devices = query_camera_devices()
 print(devices)
 ```
 >{0: ('Integrated Camera', '@device_pnp_\\\\?\\usb#vid_2304&pid_oot#media#0001#{65e8773d-8f56-11d0-a3b9-00a0c9223196}\\global'),  
@@ -257,43 +285,45 @@
 **Known issues**
 1. The VideoCaptureCAM didn't give a smooth experience in macOS. You must specify all the camera parameters. And the query_camera_options woun't give any suggestion. That's because the `ffmpeg` cannot list device options using mac native `avfoundation`. 
 ```python
 # The macOS requires full argument.
 cap = ffmpegcv.VideoCaptureCAM('FaceTime HD Camera', camsize_wh=(1280,720), camfps=30, campix_fmt='nv12')
 ```
 
-2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS blank.
+2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS empty.
 
 
 ## Stream Reader
-**Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. The feature is like a camera.
+**Experimental feature**. The ffmpegcv offers Stream reader. Which is consistent with VideoFiler reader, and more similiar to the camera.
 Becareful when using it.
 
 - Support `RTSP`, `RTP`, `RTMP`, `HTTP`, `HTTPS` streams.
 - The `VideoCaptureStream` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
-- The `VideoCaptureStream` is continously working on background even if you didn't read it. Please release it in time.
+- The `VideoCaptureStream` is continously working on background even if you didn't read it. **Please release it in time**.
+- It's still experimental. Recommand you to use opencv.
 
 
 ```python
+# opencv
 import cv2
 stream_url = 'http://devimages.apple.com.edgekey.net/streaming/examples/bipbop_4x3/gear2/prog_index.m3u8'
 cap = cv2.VideoCapture(stream_url, cv2.CAP_FFMPEG)
 
 if not cap.isOpened():
     print('Cannot open the stream')
     exit(-1)
 
 while True:
     ret, frame = cap.read()
     if not ret:
         break
     pass
 
-# ffmpegcv, in Windows&Linux
+# ffmpegcv
 import ffmpegcv
 cap = ffmpegcv.VideoCaptureStream(stream_url)
 while True:
     ret, frame = cap.read()
     if not ret:
         break
     pass
-```
+```
```

### Comparing `ffmpegcv-0.3.1/ffmpegcv/__init__.py` & `ffmpegcv-0.3.2/ffmpegcv/__init__.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.1/ffmpegcv/ffmpeg_framepick.py` & `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_framepick.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader.py` & `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_camera.py` & `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_camera.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_grey.py` & `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_grey.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_hflip.py` & `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_hflip.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_laggy.py` & `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_laggy.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_stream.py` & `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_reader_stream.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.1/ffmpegcv/ffmpeg_writer.py` & `ffmpegcv-0.3.2/ffmpegcv/ffmpeg_writer.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.1/ffmpegcv/stream_info.py` & `ffmpegcv-0.3.2/ffmpegcv/stream_info.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.1/ffmpegcv/video_info.py` & `ffmpegcv-0.3.2/ffmpegcv/video_info.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.3.1/ffmpegcv.egg-info/PKG-INFO` & `ffmpegcv-0.3.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,61 @@
-Metadata-Version: 2.1
-Name: ffmpegcv
-Version: 0.3.1
-Home-page: https://pypi.org/project/ffmpegcv/
-Author: chenxf
-Author-email: cxf529125853@163.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # FFMPEGCV is an alternative to OPENCV for video read and write.
 The ffmpegcv provide Video Reader and Video Witer with ffmpeg backbone, which are faster and powerful than cv2.
 
 - The ffmpegcv is api **compatible** to open-cv. 
 - The ffmpegcv can use **GPU accelerate** encoding and decoding*. 
 - The ffmpegcv support much more video **codecs** v.s. open-cv.
 - The ffmpegcv support **RGB** & BGR format as you like.
 - The ffmpegcv can support ROI operations.You can **crop**, **resize** and **pad** the ROI.
 
-In all, ffmpegcv is just similar to opencv api. But is faster* and with more codecs.
+In all, ffmpegcv is just similar to opencv api. But is has more codecs and does't require opencv installed.
 
+Functions:
+- `VideoWriter`: Write a video file.
+- `VideoCapture`: Read a video file.
+- `VideoCaptureCAM`: Read a camera.
+- `VideoCaptureStream`: Read a RTP/RTSP/RTMP/HTTP stream.
+
+## Install
+You need to download ffmpeg before you can use ffmpegcv.
+```
+ #1A. LINUX: sudo apt install ffmpeg
+ #1B. MAC: brew install ffmpeg
+ #1C. WINDOWS: download ffmpeg and add to the path
+ 
+ conda install ffmpeg  #1D. CONDA
+ pip install ffmpegcv
+ ```
+
+## When should choose `ffmpegcv` other than `opencv`:
+- The `opencv` is hard to install. The ffmpegcv only requires `numpy` and `FFmpeg`, works across Mac/Windows/Linux platforms.
+- The `opencv` packages too much image processing toolbox. You just want a simple video/camero IO with GPU accessible.
+- The `opencv` didn't support `h264`/`h265` and other video writers.
+- You want to **crop**, **resize** and **pad** the video/camero ROI.
 
 ## Basic example
 Read a video by CPU, and rewrite it by GPU.
 ```python
 vidin = ffmpegcv.VideoCapture(vfile_in)
 vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)
 
 with vidin, vidout:
     for frame in vidin:
         cv2.imshow('image', frame)
         vidout.write(frame)
 ```
 
-Read the camera by device name.
+Read the camera.
 ```python
+# by device ID
+cap = ffmpegcv.VideoCaptureCAM(0)
+# by device name
 cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
 ```
 
-## Install
-You need to download ffmpeg before you can use ffmpegcv
-> conda install ffmpeg 
->
-> pip install ffmpegcv
-
 ## GPU Accelation
 - Support NVIDIA card only.
 - Perfect in the **Windows**. That ffmpeg supports NVIDIA acceleration just by conda install.
 - Struggle in the **Linux**. That ffmpeg didn't orginally support NVIDIA accelerate.
 Please re-compile the ffmpeg by yourself.
 See the [link](https://docs.nvidia.com/video-technologies/video-codec-sdk/ffmpeg-with-nvidia-gpu/)
 - Works in the **Google Colab** notebook without pain (no need to recompile ffmpeg). 
@@ -200,15 +210,15 @@
 ## Camera Reader
 ---
 **Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. 
 
 - The `VideoCaptureCAM` aims to support ROI operations. The Opencv will be general fascinating than ffmpegcv in camera read. **I recommand the opencv in most camera reading case**.
 - The ffmpegcv can use name to retrieve the camera device. Use `ffmpegcv.VideoCaptureCAM("Integrated Camera")` is readable than `cv2.VideoCaptureCAM(0)`.
 - The `VideoCaptureCAM` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
-- The `VideoCaptureCAM` is continously working on background even if you didn't read it. Please release it in time.
+- The `VideoCaptureCAM` is continously working on background even if you didn't read it. **Please release it in time**.
 - Works perfect in Windows, not-perfect in Linux and macOS.
 
 ```python
 import cv2
 cap = cv2.VideoCapture(0)
 while True:
     ret, frame = cap.read()
@@ -237,15 +247,15 @@
 
 # ffmpegcv use camera with ROI operations
 cap = ffmpegcv.VideoCaptureCAM("Integrated Camera", crop_xywh=(0, 0, 640, 480), resize=(512, 512), resize_keepratio=True)
 
 
 ```
 
-**list all camera devices**
+**List all camera devices**
 ```python
 from ffmpegcv.ffmpeg_reader_camera import query_camera_devices
 
 devices = query_camera_devices()
 print(devices)
 ```
 >{0: ('Integrated Camera', '@device_pnp_\\\\?\\usb#vid_2304&pid_oot#media#0001#{65e8773d-8f56-11d0-a3b9-00a0c9223196}\\global'),  
@@ -266,43 +276,45 @@
 **Known issues**
 1. The VideoCaptureCAM didn't give a smooth experience in macOS. You must specify all the camera parameters. And the query_camera_options woun't give any suggestion. That's because the `ffmpeg` cannot list device options using mac native `avfoundation`. 
 ```python
 # The macOS requires full argument.
 cap = ffmpegcv.VideoCaptureCAM('FaceTime HD Camera', camsize_wh=(1280,720), camfps=30, campix_fmt='nv12')
 ```
 
-2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS blank.
+2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS empty.
 
 
 ## Stream Reader
-**Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. The feature is like a camera.
+**Experimental feature**. The ffmpegcv offers Stream reader. Which is consistent with VideoFiler reader, and more similiar to the camera.
 Becareful when using it.
 
 - Support `RTSP`, `RTP`, `RTMP`, `HTTP`, `HTTPS` streams.
 - The `VideoCaptureStream` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
-- The `VideoCaptureStream` is continously working on background even if you didn't read it. Please release it in time.
+- The `VideoCaptureStream` is continously working on background even if you didn't read it. **Please release it in time**.
+- It's still experimental. Recommand you to use opencv.
 
 
 ```python
+# opencv
 import cv2
 stream_url = 'http://devimages.apple.com.edgekey.net/streaming/examples/bipbop_4x3/gear2/prog_index.m3u8'
 cap = cv2.VideoCapture(stream_url, cv2.CAP_FFMPEG)
 
 if not cap.isOpened():
     print('Cannot open the stream')
     exit(-1)
 
 while True:
     ret, frame = cap.read()
     if not ret:
         break
     pass
 
-# ffmpegcv, in Windows&Linux
+# ffmpegcv
 import ffmpegcv
 cap = ffmpegcv.VideoCaptureStream(stream_url)
 while True:
     ret, frame = cap.read()
     if not ret:
         break
     pass
-```
+```
```

### Comparing `ffmpegcv-0.3.1/setup.py` & `ffmpegcv-0.3.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #setup.py
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
+long_description = (this_directory / "README.md").read_text('utf-8')
 
 setup(
     name='ffmpegcv', # 应用名
-    version='0.3.1', # 版本号
+    version='0.3.2', # 版本号
     packages=find_packages(include=['ffmpegcv*']), # 包括在安装包内的 Python 包
     author='chenxf',
     author_email='cxf529125853@163.com',
     url='https://pypi.org/project/ffmpegcv/',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

