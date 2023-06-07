# Comparing `tmp/lazysdk-0.1.3.tar.gz` & `tmp/lazysdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazysdk-0.1.3.tar", last modified: Wed Jun  7 07:25:15 2023, max compression
+gzip compressed data, was "lazysdk-0.1.4.tar", last modified: Wed Jun  7 07:51:59 2023, max compression
```

## Comparing `lazysdk-0.1.3.tar` & `lazysdk-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-07 07:25:15.659257 lazysdk-0.1.3/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-07 07:25:15.659035 lazysdk-0.1.3/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      993 2023-02-23 03:14:55.000000 lazysdk-0.1.3/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-07 07:25:15.657898 lazysdk-0.1.3/lazysdk/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      402 2023-02-23 03:44:47.000000 lazysdk-0.1.3/lazysdk/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-06-06 09:15:38.000000 lazysdk-0.1.3/lazysdk/lazyCrypto.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      555 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazybase64.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     6829 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazydict.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazyenv.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    13091 2023-02-25 06:33:34.000000 lazysdk-0.1.3/lazysdk/lazyexcel.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    20267 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazyfile.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazyflask.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      607 2023-02-23 03:41:38.000000 lazysdk-0.1.3/lazysdk/lazyid.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      451 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazyip.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    28027 2023-06-07 07:24:43.000000 lazysdk-0.1.3/lazysdk/lazym3u8.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazymd5.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4305 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazypath.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     5079 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazyprocess.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazyproxies.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazyrandom.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazyredis.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2511 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazyrequests.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1448 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazytext.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    23199 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazytime.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3783 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazyua.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     8386 2023-02-23 03:14:55.000000 lazysdk-0.1.3/lazysdk/lazywebhook.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-07 07:25:15.658821 lazysdk-0.1.3/lazysdk.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-07 07:25:15.000000 lazysdk-0.1.3/lazysdk.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      626 2023-06-07 07:25:15.000000 lazysdk-0.1.3/lazysdk.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-06-07 07:25:15.000000 lazysdk-0.1.3/lazysdk.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      163 2023-06-07 07:25:15.000000 lazysdk-0.1.3/lazysdk.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2023-06-07 07:25:15.000000 lazysdk-0.1.3/lazysdk.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-06-07 07:25:15.659319 lazysdk-0.1.3/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1121 2023-06-07 07:24:43.000000 lazysdk-0.1.3/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-07 07:51:59.770670 lazysdk-0.1.4/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-07 07:51:59.770550 lazysdk-0.1.4/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      993 2023-02-23 03:14:55.000000 lazysdk-0.1.4/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-07 07:51:59.769597 lazysdk-0.1.4/lazysdk/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      402 2023-02-23 03:44:47.000000 lazysdk-0.1.4/lazysdk/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-06-06 09:15:38.000000 lazysdk-0.1.4/lazysdk/lazyCrypto.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      555 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazybase64.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     6829 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazydict.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazyenv.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    13091 2023-02-25 06:33:34.000000 lazysdk-0.1.4/lazysdk/lazyexcel.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    20267 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazyfile.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazyflask.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      607 2023-02-23 03:41:38.000000 lazysdk-0.1.4/lazysdk/lazyid.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      451 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazyip.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    31484 2023-06-07 07:51:22.000000 lazysdk-0.1.4/lazysdk/lazym3u8.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazymd5.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4305 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazypath.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5079 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazyprocess.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazyproxies.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazyrandom.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazyredis.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2511 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazyrequests.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1448 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazytext.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    23199 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazytime.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3783 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazyua.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     8386 2023-02-23 03:14:55.000000 lazysdk-0.1.4/lazysdk/lazywebhook.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-07 07:51:59.770326 lazysdk-0.1.4/lazysdk.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-07 07:51:59.000000 lazysdk-0.1.4/lazysdk.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      626 2023-06-07 07:51:59.000000 lazysdk-0.1.4/lazysdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-06-07 07:51:59.000000 lazysdk-0.1.4/lazysdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      163 2023-06-07 07:51:59.000000 lazysdk-0.1.4/lazysdk.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2023-06-07 07:51:59.000000 lazysdk-0.1.4/lazysdk.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-06-07 07:51:59.770725 lazysdk-0.1.4/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1121 2023-06-07 07:32:01.000000 lazysdk-0.1.4/setup.py
```

### Comparing `lazysdk-0.1.3/PKG-INFO` & `lazysdk-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazysdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: 基于Python的懒人包
 Home-page: https://gitee.com/ZeroSeeker/lazysdk
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lazysdk-0.1.3/README.md` & `lazysdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazybase64.py` & `lazysdk-0.1.4/lazysdk/lazybase64.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazydict.py` & `lazysdk-0.1.4/lazysdk/lazydict.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazyenv.py` & `lazysdk-0.1.4/lazysdk/lazyenv.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazyexcel.py` & `lazysdk-0.1.4/lazysdk/lazyexcel.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazyfile.py` & `lazysdk-0.1.4/lazysdk/lazyfile.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazyflask.py` & `lazysdk-0.1.4/lazysdk/lazyflask.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazyid.py` & `lazysdk-0.1.4/lazysdk/lazyid.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazym3u8.py` & `lazysdk-0.1.4/lazysdk/lazym3u8.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # coding = utf8
 from . import lazyCrypto
 from . import lazytime
 from . import lazyfile
 from . import lazypath
 from . import lazymd5
+from . import lazyprocess
 import subprocess
 import threading
 import requests
 import showlog
 import shutil
 import queue
 import m3u8
@@ -499,14 +500,111 @@
         'fragment_path': fragment_path_new,
         'fragment_suffix': fragment_suffix,
         'fragment_file_name_list': fragment_file_name_list
     }
     return download_res
 
 
+def download_fragment_single(
+        task_index,
+        task_info,
+):
+    """
+    模块功能：下载单个碎片到指定文件夹
+    :param fragment_url: 碎片下载地址
+    :param fragment_url_name: 碎片名
+    :param fragment_path:碎片保存路径
+    :param aes_key: aes解密key
+    :param headers:请求头
+    :param fragment_suffix:碎片文件后缀名
+    :return:
+    """
+    fragment_url = task_info['fragment_url']
+    fragment_url_name = task_info['fragment_url_name']
+    fragment_path = task_info['fragment_path']
+    aes_key = None,
+    headers = None,
+    fragment_suffix = task_info['fragment_suffix']
+
+    if headers is None:
+        headers_local = default_headers
+    else:
+        headers_local = headers
+
+    print('正在下载', fragment_url_name, fragment_url)
+    fragment_file_name = '%s%s%s.%s' % (fragment_path, path_separator, fragment_url_name, fragment_suffix)  # 生成碎片文件名
+    # 开始下载碎片文件
+    while True:
+        try:
+            with open(fragment_file_name, "ab+") as f:
+                response = requests.get(
+                    url=fragment_url,
+                    headers=headers_local,
+                    stream=True,
+                    timeout=timeout
+                )
+                total_length = response.headers.get('content-length')
+
+                if total_length is None:
+                    print("Attention: There is no content length in header!")  # 未返回长度信息
+                else:
+                    dl = 0
+                    total_length = int(total_length)
+                    for data in track(
+                            sequence=response.iter_content(chunk_size=8192),
+                            description='下载中',
+                            total=total_length/8192,
+                            show_speed=True
+                    ):
+                        dl += len(data)
+                        if aes_key is None:
+                            data_decode = data
+                        else:
+                            data_decode = lazyCrypto.aes_decode(data, aes_key)
+                        f.write(data_decode)
+                        f.flush()
+            break
+        except:
+            showlog.warning('下载超时，将在1秒后重试...')
+            os.remove(fragment_file_name)
+            time.sleep(1)
+            pass
+
+
+def download_fragment_quick(
+        url_list
+):
+    fragment_path = 'fragment_%s' % str(time.time()).replace('.', '')  # 使用时间戳命名
+    fragment_suffix = 'ts'
+    lazypath.make_path(fragment_path)
+    task_list = list()
+    fragment_file_name_list = list()
+    for url_index, each_url in enumerate(url_list):
+        task_list.append(
+            {
+                'fragment_url': each_url,
+                'fragment_url_name': url_index,
+                'fragment_path': fragment_path,
+                'fragment_suffix': fragment_suffix
+            }
+        )
+        fragment_file_name = '%s%s%s.%s' % (fragment_path, path_separator, url_index, fragment_suffix)  # 生成碎片文件名
+        fragment_file_name_list.append(fragment_file_name)
+    lazyprocess.run(
+        task_list=url_list,
+        task_function=download_fragment_single
+    )
+    download_res = {
+        'fragment_path': fragment_path,
+        'fragment_suffix': fragment_suffix,
+        'fragment_file_name_list': fragment_file_name_list
+    }
+    return download_res
+
+
 def download_m3u8(
         m3u8_link=None,
         m3u8_file_path=None,
         filename=lazytime.get_file_name(),
         url_v=None,
         video_suffix_name="ts",
         aes_key=None,
```

### Comparing `lazysdk-0.1.3/lazysdk/lazymd5.py` & `lazysdk-0.1.4/lazysdk/lazymd5.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazypath.py` & `lazysdk-0.1.4/lazysdk/lazypath.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazyprocess.py` & `lazysdk-0.1.4/lazysdk/lazyprocess.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazyproxies.py` & `lazysdk-0.1.4/lazysdk/lazyproxies.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazyrandom.py` & `lazysdk-0.1.4/lazysdk/lazyrandom.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazyredis.py` & `lazysdk-0.1.4/lazysdk/lazyredis.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazyrequests.py` & `lazysdk-0.1.4/lazysdk/lazyrequests.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazytext.py` & `lazysdk-0.1.4/lazysdk/lazytext.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazytime.py` & `lazysdk-0.1.4/lazysdk/lazytime.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazyua.py` & `lazysdk-0.1.4/lazysdk/lazyua.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk/lazywebhook.py` & `lazysdk-0.1.4/lazysdk/lazywebhook.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/lazysdk.egg-info/PKG-INFO` & `lazysdk-0.1.4/lazysdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazysdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: 基于Python的懒人包
 Home-page: https://gitee.com/ZeroSeeker/lazysdk
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lazysdk-0.1.3/lazysdk.egg-info/SOURCES.txt` & `lazysdk-0.1.4/lazysdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.3/setup.py` & `lazysdk-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazysdk",
-    version="0.1.3",
+    version="0.1.4",
     description="基于Python的懒人包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazysdk",
     packages=setuptools.find_packages(),
```

