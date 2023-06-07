# Comparing `tmp/channel_box-0.5.1-py3-none-any.whl.zip` & `tmp/channel_box-0.5.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7320 bytes, number of entries: 10
+Zip file size: 7331 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx       48 b- defN 23-Jun-07 06:56 channel_box/__init__.py
 -rw-rw-r--  2.0 unx     5746 b- defN 23-Jun-07 08:07 channel_box/src.py
 -rw-rw-r--  2.0 unx        0 b- defN 20-Jul-19 15:17 example/channel/__init__.py
 -rw-rw-r--  2.0 unx      599 b- defN 23-Jun-07 07:55 example/channel/urls.py
 -rw-rw-r--  2.0 unx     6393 b- defN 23-Jun-07 08:13 example/channel/views.py
--rwxr-xr-x  2.0 unx     1094 b- defN 23-Jun-07 08:22 channel_box-0.5.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3054 b- defN 23-Jun-07 08:22 channel_box-0.5.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 08:22 channel_box-0.5.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-Jun-07 08:22 channel_box-0.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      800 b- defN 23-Jun-07 08:22 channel_box-0.5.1.dist-info/RECORD
-10 files, 17846 bytes uncompressed, 5950 bytes compressed:  66.7%
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-Jun-07 08:33 channel_box-0.5.1.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3021 b- defN 23-Jun-07 08:33 channel_box-0.5.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 08:33 channel_box-0.5.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jun-07 08:33 channel_box-0.5.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      810 b- defN 23-Jun-07 08:33 channel_box-0.5.1.1.dist-info/RECORD
+10 files, 17823 bytes uncompressed, 5941 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: example/channel/urls.py
 Comment: 
 
 Filename: example/channel/views.py
 Comment: 
 
-Filename: channel_box-0.5.1.dist-info/LICENSE
+Filename: channel_box-0.5.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: channel_box-0.5.1.dist-info/METADATA
+Filename: channel_box-0.5.1.1.dist-info/METADATA
 Comment: 
 
-Filename: channel_box-0.5.1.dist-info/WHEEL
+Filename: channel_box-0.5.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: channel_box-0.5.1.dist-info/top_level.txt
+Filename: channel_box-0.5.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: channel_box-0.5.1.dist-info/RECORD
+Filename: channel_box-0.5.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `channel_box-0.5.1.dist-info/LICENSE` & `channel_box-0.5.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `channel_box-0.5.1.dist-info/METADATA` & `channel_box-0.5.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: channel-box
-Version: 0.5.1
+Version: 0.5.1.1
 Summary: ChannelBox it is a package for Starlette framework that allows you to make named webscoket channels.
 Home-page: https://github.com/Sobolev5/channel-box
 Author: Sobolev Andrey
 Author-email: email.asobolev@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: starlette (>=0.27.0)
-Requires-Dist: shortuuid (>=1.0.9)
 Requires-Dist: uvicorn[standart] (>=0.22.0)
 
 # channel-box
 `channel-box` it is a simple tool for Starlette & FastAPI framework that allows you send messages to named websocket channels from any part of your code.
 
 Example of use:
 - group chats
```

## Comparing `channel_box-0.5.1.dist-info/RECORD` & `channel_box-0.5.1.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 channel_box/__init__.py,sha256=IQ6PdTXL75hv4rFxJ0Mjns30mHJIX_UFUp28JwsU6CY,48
 channel_box/src.py,sha256=nENCMuVdy-QfUkpfylmSdQ_etE_RUb0OrstCNqLlyz0,5746
 example/channel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 example/channel/urls.py,sha256=R_FB2kG6cMHa_OferyJSll7ixYcnIvxqSTKgjuQFmiI,599
 example/channel/views.py,sha256=JS7xGVULStUowWxpm_-x9jEGrZGf37bL_yrKBz2Z8yk,6393
-channel_box-0.5.1.dist-info/LICENSE,sha256=BvmWh0aXPp8jrD0GS25NwyJ321UbcQ7KIui9wAmwVD0,1094
-channel_box-0.5.1.dist-info/METADATA,sha256=GZaDsYKw8iVBrttbrGbnITywZJVs-3pwseBjdullSl0,3054
-channel_box-0.5.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-channel_box-0.5.1.dist-info/top_level.txt,sha256=mjnxqFEWVz6Q-V_iwda7dXI5euFqxEJoqnhuKt-k6sI,20
-channel_box-0.5.1.dist-info/RECORD,,
+channel_box-0.5.1.1.dist-info/LICENSE,sha256=BvmWh0aXPp8jrD0GS25NwyJ321UbcQ7KIui9wAmwVD0,1094
+channel_box-0.5.1.1.dist-info/METADATA,sha256=6YJUQLh48H9CfZJGx3CqbhnoDqgVj5p9qdBMgL0AWvg,3021
+channel_box-0.5.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+channel_box-0.5.1.1.dist-info/top_level.txt,sha256=mjnxqFEWVz6Q-V_iwda7dXI5euFqxEJoqnhuKt-k6sI,20
+channel_box-0.5.1.1.dist-info/RECORD,,
```

