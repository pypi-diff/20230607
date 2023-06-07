# Comparing `tmp/lazysdk-0.1.6.tar.gz` & `tmp/lazysdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazysdk-0.1.6.tar", last modified: Wed Jun  7 09:08:56 2023, max compression
+gzip compressed data, was "lazysdk-0.1.7.tar", last modified: Wed Jun  7 09:34:49 2023, max compression
```

## Comparing `lazysdk-0.1.6.tar` & `lazysdk-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-07 09:08:56.316112 lazysdk-0.1.6/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-07 09:08:56.315995 lazysdk-0.1.6/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      993 2023-02-23 03:14:55.000000 lazysdk-0.1.6/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-07 09:08:56.315302 lazysdk-0.1.6/lazysdk/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      402 2023-02-23 03:44:47.000000 lazysdk-0.1.6/lazysdk/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-06-06 09:15:38.000000 lazysdk-0.1.6/lazysdk/lazyCrypto.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      555 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazybase64.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     6829 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazydict.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazyenv.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    13091 2023-02-25 06:33:34.000000 lazysdk-0.1.6/lazysdk/lazyexcel.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    20267 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazyfile.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazyflask.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      607 2023-02-23 03:41:38.000000 lazysdk-0.1.6/lazysdk/lazyid.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      451 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazyip.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    31653 2023-06-07 09:08:18.000000 lazysdk-0.1.6/lazysdk/lazym3u8.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazymd5.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4305 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazypath.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     5079 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazyprocess.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazyproxies.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazyrandom.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazyredis.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2511 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazyrequests.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1448 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazytext.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    23199 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazytime.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3783 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazyua.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     8386 2023-02-23 03:14:55.000000 lazysdk-0.1.6/lazysdk/lazywebhook.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-07 09:08:56.315829 lazysdk-0.1.6/lazysdk.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-07 09:08:56.000000 lazysdk-0.1.6/lazysdk.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      626 2023-06-07 09:08:56.000000 lazysdk-0.1.6/lazysdk.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-06-07 09:08:56.000000 lazysdk-0.1.6/lazysdk.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      163 2023-06-07 09:08:56.000000 lazysdk-0.1.6/lazysdk.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2023-06-07 09:08:56.000000 lazysdk-0.1.6/lazysdk.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-06-07 09:08:56.316151 lazysdk-0.1.6/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1121 2023-06-07 09:08:18.000000 lazysdk-0.1.6/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-07 09:34:49.691319 lazysdk-0.1.7/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-07 09:34:49.691201 lazysdk-0.1.7/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      993 2023-02-23 03:14:55.000000 lazysdk-0.1.7/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-07 09:34:49.690447 lazysdk-0.1.7/lazysdk/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      402 2023-02-23 03:44:47.000000 lazysdk-0.1.7/lazysdk/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-06-06 09:15:38.000000 lazysdk-0.1.7/lazysdk/lazyCrypto.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      555 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazybase64.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     6829 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazydict.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazyenv.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    13091 2023-02-25 06:33:34.000000 lazysdk-0.1.7/lazysdk/lazyexcel.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    20267 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazyfile.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazyflask.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      607 2023-02-23 03:41:38.000000 lazysdk-0.1.7/lazysdk/lazyid.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      451 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazyip.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    31675 2023-06-07 09:24:50.000000 lazysdk-0.1.7/lazysdk/lazym3u8.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazymd5.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4305 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazypath.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5159 2023-06-07 09:23:18.000000 lazysdk-0.1.7/lazysdk/lazyprocess.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazyproxies.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazyrandom.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazyredis.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2511 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazyrequests.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1448 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazytext.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    23199 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazytime.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3783 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazyua.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     8386 2023-02-23 03:14:55.000000 lazysdk-0.1.7/lazysdk/lazywebhook.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-07 09:34:49.691040 lazysdk-0.1.7/lazysdk.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-07 09:34:49.000000 lazysdk-0.1.7/lazysdk.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      626 2023-06-07 09:34:49.000000 lazysdk-0.1.7/lazysdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-06-07 09:34:49.000000 lazysdk-0.1.7/lazysdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      163 2023-06-07 09:34:49.000000 lazysdk-0.1.7/lazysdk.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2023-06-07 09:34:49.000000 lazysdk-0.1.7/lazysdk.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-06-07 09:34:49.691360 lazysdk-0.1.7/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1121 2023-06-07 09:24:50.000000 lazysdk-0.1.7/setup.py
```

### Comparing `lazysdk-0.1.6/PKG-INFO` & `lazysdk-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazysdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: 基于Python的懒人包
 Home-page: https://gitee.com/ZeroSeeker/lazysdk
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lazysdk-0.1.6/README.md` & `lazysdk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazybase64.py` & `lazysdk-0.1.7/lazysdk/lazybase64.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazydict.py` & `lazysdk-0.1.7/lazysdk/lazydict.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazyenv.py` & `lazysdk-0.1.7/lazysdk/lazyenv.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazyexcel.py` & `lazysdk-0.1.7/lazysdk/lazyexcel.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazyfile.py` & `lazysdk-0.1.7/lazysdk/lazyfile.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazyflask.py` & `lazysdk-0.1.7/lazysdk/lazyflask.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazyid.py` & `lazysdk-0.1.7/lazysdk/lazyid.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazym3u8.py` & `lazysdk-0.1.7/lazysdk/lazym3u8.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,24 +517,24 @@
     :param headers:请求头
     :param fragment_suffix:碎片文件后缀名
     :return:
     """
     fragment_url = task_info['fragment_url']
     fragment_url_name = task_info['fragment_url_name']
     fragment_path = task_info['fragment_path']
-    aes_key = None,
+    aes_key = None
     fragment_suffix = task_info['fragment_suffix']
     headers = task_info['headers']
 
     if headers:
         headers_local = headers
     else:
         headers_local = default_headers
 
-    print('正在下载', fragment_url_name, fragment_url)
+    # print('正在下载', fragment_url_name, fragment_url)
     fragment_file_name = '%s%s%s.%s' % (fragment_path, path_separator, fragment_url_name, fragment_suffix)  # 生成碎片文件名
     # 开始下载碎片文件
     while True:
         try:
             with open(fragment_file_name, "ab+") as f:
                 response = requests.get(
                     url=fragment_url,
@@ -547,28 +547,28 @@
                 if total_length is None:
                     print("Attention: There is no content length in header!")  # 未返回长度信息
                 else:
                     dl = 0
                     total_length = int(total_length)
                     for data in track(
                             sequence=response.iter_content(chunk_size=8192),
-                            description='下载中',
+                            description=f'{fragment_url_name} 下载中',
                             total=total_length/8192,
                             show_speed=True
                     ):
                         dl += len(data)
                         if aes_key is None:
                             data_decode = data
                         else:
                             data_decode = lazyCrypto.aes_decode(data, aes_key)
                         f.write(data_decode)
                         f.flush()
             break
         except:
-            showlog.warning('下载超时，将在1秒后重试...')
+            showlog.error('下载超时，将在1秒后重试...')
             os.remove(fragment_file_name)
             time.sleep(1)
             pass
 
 
 def download_fragment_quick(
         url_list,
@@ -588,19 +588,21 @@
                 'fragment_path': fragment_path,
                 'fragment_suffix': fragment_suffix,
                 'headers': headers
             }
         )
         fragment_file_name = '%s%s%s.%s' % (fragment_path, path_separator, url_index, fragment_suffix)  # 生成碎片文件名
         fragment_file_name_list.append(fragment_file_name)
+
     lazyprocess.run(
         task_list=task_list,
         task_function=download_fragment_single,
         subprocess_limit=subprocess_limit
     )
+
     download_res = {
         'fragment_path': fragment_path,
         'fragment_suffix': fragment_suffix,
         'fragment_file_name_list': fragment_file_name_list
     }
     return download_res
```

### Comparing `lazysdk-0.1.6/lazysdk/lazymd5.py` & `lazysdk-0.1.7/lazysdk/lazymd5.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazypath.py` & `lazysdk-0.1.7/lazysdk/lazypath.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazyprocess.py` & `lazysdk-0.1.7/lazysdk/lazyprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 os_cpu_count = os.cpu_count()  # CPU核心数
 
 
 def run(
         task_list: list,
         task_function,
         subprocess_keep: bool = False,
-        subprocess_limit: int = os_cpu_count * 2,
+        subprocess_limit: int = None,
         master_process_delay: int = 1,
         return_data: bool = False,
 
         silence: bool = False
 ):
     """
     多进程 进程控制
@@ -39,14 +39,18 @@
     def task_function(
             task_index,
             task_info
     ):
         # 进程详细的内容
         print(task_index, task_info)
     """
+    if subprocess_limit:
+        pass
+    else:
+        subprocess_limit = os_cpu_count * 2
     active_process = dict()  # 活跃进程，存放进程，以task_index为key，进程信息为value的dict
     task_count = len(task_list)  # 总任务数量
     task_index_start = 0  # 用来计算启动的累计进程数
     q = Queue()  # 生成一个队列对象，以实现进程通信
 
     showlog.info(f'正在准备多进程执行任务，总任务数为：{task_count}，进程数限制为：{subprocess_limit}...')
     # 创建并启动线程
```

### Comparing `lazysdk-0.1.6/lazysdk/lazyproxies.py` & `lazysdk-0.1.7/lazysdk/lazyproxies.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazyrandom.py` & `lazysdk-0.1.7/lazysdk/lazyrandom.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazyredis.py` & `lazysdk-0.1.7/lazysdk/lazyredis.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazyrequests.py` & `lazysdk-0.1.7/lazysdk/lazyrequests.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazytext.py` & `lazysdk-0.1.7/lazysdk/lazytext.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazytime.py` & `lazysdk-0.1.7/lazysdk/lazytime.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazyua.py` & `lazysdk-0.1.7/lazysdk/lazyua.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk/lazywebhook.py` & `lazysdk-0.1.7/lazysdk/lazywebhook.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/lazysdk.egg-info/PKG-INFO` & `lazysdk-0.1.7/lazysdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazysdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: 基于Python的懒人包
 Home-page: https://gitee.com/ZeroSeeker/lazysdk
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lazysdk-0.1.6/lazysdk.egg-info/SOURCES.txt` & `lazysdk-0.1.7/lazysdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.6/setup.py` & `lazysdk-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazysdk",
-    version="0.1.6",
+    version="0.1.7",
     description="基于Python的懒人包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazysdk",
     packages=setuptools.find_packages(),
```

