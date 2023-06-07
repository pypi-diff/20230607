# Comparing `tmp/pyxk-0.6.1.tar.gz` & `tmp/pyxk-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.6.1.tar", last modified: Tue Jun  6 07:19:41 2023, max compression
+gzip compressed data, was "pyxk-0.6.2.tar", last modified: Wed Jun  7 02:35:28 2023, max compression
```

## Comparing `pyxk-0.6.1.tar` & `pyxk-0.6.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.839747 pyxk-0.6.1/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.6.1/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      357 2023-06-06 07:19:41.839747 pyxk-0.6.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.6.1/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.829747 pyxk-0.6.1/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)      502 2023-06-06 03:59:16.000000 pyxk-0.6.1/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.839747 pyxk-0.6.1/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-06 06:59:00.000000 pyxk-0.6.1/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    19536 2023-06-06 06:59:38.000000 pyxk-0.6.1/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      510 2023-06-06 06:55:14.000000 pyxk-0.6.1/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.839747 pyxk-0.6.1/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-06-06 06:43:24.000000 pyxk-0.6.1/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3209 2023-06-06 06:37:44.000000 pyxk-0.6.1/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4871 2023-06-06 06:37:44.000000 pyxk-0.6.1/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.839747 pyxk-0.6.1/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       56 2023-06-06 07:01:26.000000 pyxk-0.6.1/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3354 2023-06-06 05:01:50.000000 pyxk-0.6.1/pyxk/m3u8/enter_point.py
--rw-rw----   0 root         (0) everybody  (9997)     4938 2023-06-06 05:32:52.000000 pyxk-0.6.1/pyxk/m3u8/m3u8download.py
--rw-rw----   0 root         (0) everybody  (9997)     3061 2023-06-06 04:41:28.000000 pyxk-0.6.1/pyxk/m3u8/m3u8parse.py
--rw-rw----   0 root         (0) everybody  (9997)    12418 2023-06-06 06:45:56.000000 pyxk-0.6.1/pyxk/m3u8/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.839747 pyxk-0.6.1/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      247 2023-06-06 04:23:26.000000 pyxk-0.6.1/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-25 11:04:02.000000 pyxk-0.6.1/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3493 2023-06-06 04:26:26.000000 pyxk-0.6.1/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    16488 2023-06-06 05:27:26.000000 pyxk-0.6.1/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    19058 2023-06-06 03:59:16.000000 pyxk-0.6.1/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-06 07:19:41.839747 pyxk-0.6.1/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      357 2023-06-06 07:19:41.000000 pyxk-0.6.1/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      577 2023-06-06 07:19:41.000000 pyxk-0.6.1/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-06 07:19:41.000000 pyxk-0.6.1/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       89 2023-06-06 07:19:41.000000 pyxk-0.6.1/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-06-06 07:19:41.000000 pyxk-0.6.1/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-06-06 07:19:41.000000 pyxk-0.6.1/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-06 07:19:41.839747 pyxk-0.6.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      919 2023-06-06 07:19:39.000000 pyxk-0.6.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.709720 pyxk-0.6.2/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.6.2/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      357 2023-06-07 02:35:28.709720 pyxk-0.6.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.6.2/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.699720 pyxk-0.6.2/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)      502 2023-06-06 03:59:16.000000 pyxk-0.6.2/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.709720 pyxk-0.6.2/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-06 06:59:00.000000 pyxk-0.6.2/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    19536 2023-06-06 06:59:38.000000 pyxk-0.6.2/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      510 2023-06-06 06:55:14.000000 pyxk-0.6.2/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.709720 pyxk-0.6.2/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-06-06 06:43:24.000000 pyxk-0.6.2/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3226 2023-06-07 02:28:36.000000 pyxk-0.6.2/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4873 2023-06-07 02:30:15.000000 pyxk-0.6.2/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.709720 pyxk-0.6.2/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       56 2023-06-06 07:01:26.000000 pyxk-0.6.2/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3354 2023-06-06 05:01:50.000000 pyxk-0.6.2/pyxk/m3u8/enter_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     4690 2023-06-07 02:27:20.000000 pyxk-0.6.2/pyxk/m3u8/m3u8download.py
+-rw-rw----   0 root         (0) everybody  (9997)     2946 2023-06-07 02:27:51.000000 pyxk-0.6.2/pyxk/m3u8/m3u8parse.py
+-rw-rw----   0 root         (0) everybody  (9997)    12424 2023-06-07 02:25:09.000000 pyxk-0.6.2/pyxk/m3u8/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.709720 pyxk-0.6.2/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      247 2023-06-06 04:23:26.000000 pyxk-0.6.2/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-25 11:04:02.000000 pyxk-0.6.2/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3493 2023-06-06 04:26:26.000000 pyxk-0.6.2/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    16522 2023-06-07 02:31:20.000000 pyxk-0.6.2/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    18885 2023-06-07 02:31:53.000000 pyxk-0.6.2/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.699720 pyxk-0.6.2/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      357 2023-06-07 02:35:28.000000 pyxk-0.6.2/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      577 2023-06-07 02:35:28.000000 pyxk-0.6.2/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-07 02:35:28.000000 pyxk-0.6.2/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       89 2023-06-07 02:35:28.000000 pyxk-0.6.2/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-06-07 02:35:28.000000 pyxk-0.6.2/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-06-07 02:35:28.000000 pyxk-0.6.2/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-07 02:35:28.709720 pyxk-0.6.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      919 2023-06-07 02:35:16.000000 pyxk-0.6.2/setup.py
```

### Comparing `pyxk-0.6.1/LICENSE` & `pyxk-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.1/pyxk/aclient/client.py` & `pyxk-0.6.2/pyxk/aclient/client.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.1/pyxk/aes/_fmtdata.py` & `pyxk-0.6.2/pyxk/aes/_fmtdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,13 +110,14 @@
     @mode.setter
     def mode(self, value):
         self._mode = value
         self.__mode_fmt()
 
     @property
     def iv(self):
+        """iv"""
         return self._iv
 
     @iv.setter
     def iv(self, value):
         self._iv = value
         self.__iv_to_bytes()
```

### Comparing `pyxk-0.6.1/pyxk/aes/cryptor.py` & `pyxk-0.6.2/pyxk/aes/cryptor.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,30 +73,30 @@
 
         :param plaintext: 加密明文
         :return: bytes
         """
         if isinstance(plaintext, str):
             plaintext = plaintext.encode(self._encode)
         elif not isinstance(plaintext, bytes):
-            raise TypeError("'plaintext' type must be 'str' or 'bytes', not {type(plaintext).__name__!r}")
+            raise TypeError(f"'plaintext' type must be 'str' or 'bytes', not {type(plaintext).__name__!r}")
         # 创建 cipher - 加密
         self.__create_cipher()
         padding_func = PADDING_ALL[self.padding]
         return self._cipher.encrypt(padding_func(plaintext))
 
     def decrypt(self, ciphertext: Union[str, bytes]) -> bytes:
         """AES 解密
 
         :param ciphertext: 解密密文
         :return: bytes
         """
         if isinstance(ciphertext, str):
             ciphertext = ciphertext.encode(self._encode)
         elif not isinstance(ciphertext, bytes):
-            raise TypeError("'plaintext' type must be 'str' or 'bytes', not {type(ciphertext).__name__!r}")
+            raise TypeError(f"'plaintext' type must be 'str' or 'bytes', not {type(ciphertext).__name__!r}")
         # 创建 cipher - 解密
         self.__create_cipher()
         padding_func = PADDING_ALL[self.padding]
         return padding_func(self._cipher.decrypt(ciphertext), True)
 
     def __create_cipher(self):
         """创建 cipher - 加解密工具"""
```

### Comparing `pyxk-0.6.1/pyxk/m3u8/enter_point.py` & `pyxk-0.6.2/pyxk/m3u8/enter_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.1/pyxk/m3u8/m3u8download.py` & `pyxk-0.6.2/pyxk/m3u8/m3u8download.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,23 +8,16 @@
 
 from pyxk.aes import Cryptor
 from pyxk.utils import make_open
 from pyxk.aclient import Client
 
 
 class Downloader(Client):
-    """m3u8 - segments 下载器
+    """m3u8 - segments 下载器"""
 
-    :param m3obj: pyxk.m3u8downloader.main.M3U8
-    :param m3u8keys: m3u8资源加密密钥
-    :param segments: m3u8 segments
-    :param progress: rich.progress.Progress
-    :param download: rich.progress.Progress
-    :param kwargs: **kwargs
-    """
     timeout = 30
     maximum_retry = 30
     error_status_code = list(range(404, 411))
     until_request_succeed = True
 
     def __init__(
         self, *, m3obj, m3u8keys=None, segments=None, progress=None, download=None, **kwargs
```

### Comparing `pyxk-0.6.1/pyxk/m3u8/m3u8parse.py` & `pyxk-0.6.2/pyxk/m3u8/m3u8parse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 """m3u8资源解析器"""
 from pyxk.utils import LazyLoader
 
 m3u8 = LazyLoader("m3u8", globals(), "m3u8")
 
 
 class M3U8Parse:
-    """m3u8资源 解析器
+    """m3u8资源解析器"""
 
-    :param content: m3u8 content
-    :param url: m3u8 url
-    :param instance: pyxk.m3u8downloader.main.M3U8
-    """
     def __init__(self, *, content, url, instance):
         """m3u8资源 解析器
 
         :param content: m3u8 content
         :param url: m3u8 url
         :param instance: pyxk.m3u8downloader.main.M3U8
         """
```

### Comparing `pyxk-0.6.1/pyxk/m3u8/main.py` & `pyxk-0.6.2/pyxk/m3u8/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         if self._verify is False:
             import urllib3
             urllib3.disable_warnings()
         content = self.get_m3u8_content(url)
         # 无效m3u8内容
         if not self._is_m3u8_content(content):
             self._console.print("[red b]m3u8 url is not available!")
-            return
+            return None
         # 解析m3u8
         return self.start_parse(content=content, url=url)
 
     def load_content(
         self,
         content: str,
         url: Optional[str] = None,
@@ -138,18 +138,18 @@
         if not self._is_m3u8_content(content):
             m3u8file = os.path.normpath(os.path.abspath(content)) if isinstance(content, str) else None
             if m3u8file and os.path.isfile(m3u8file):
                 with open(m3u8file, "r", encoding="utf-8") as read_fileobj:
                     content = read_fileobj.read()
                     if not self._is_m3u8_content(content):
                         self._console.print("[red b]m3u8 content is not available![/]")
-                        return
+                        return None
             else:
                 self._console.print("[red b]m3u8 content is not available![/]")
-                return
+                return None
         # 解析m3u8
         return self.start_parse(content=content, url=url)
 
     def start_parse(self, content: str, url: Optional[str]):
         """开始解析m3u8内容
 
         :param content: m3u8 内容
@@ -188,23 +188,22 @@
         live = _rich_live.Live(panel, console=self._console)
         with live:
             Downloader.run(
                 m3obj=self,
                 m3u8keys=m3u8parse["m3u8keys"],
                 segments=m3u8parse["segments"],
                 progress=progress,
-                download=download,
+                download=download
             )
         # 删除m3u8文件
-        if not self._reserve:
-            import shlex
-            import subprocess
-            args = shlex.split(f"rm -rf {self._temp_file}")
-            subprocess.run(args, check=True)
-
+        if not self._reserve and self._temp_file:
+            import shutil
+            if os.path.isdir(self._temp_file):
+                shutil.rmtree(self._temp_file)
+            
     def get_m3u8_content(
         self, url: Optional[str], *, is_m3u8key: bool = False
     ) -> Union[str, bytes]:
         """获取m3u8内容
 
         :param url: url
         :param is_m3u8key: m3u8 key(type: bool)
```

### Comparing `pyxk-0.6.1/pyxk/requests/api.py` & `pyxk-0.6.2/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.1/pyxk/requests/entry_point.py` & `pyxk-0.6.2/pyxk/requests/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.1/pyxk/requests/sessions.py` & `pyxk-0.6.2/pyxk/requests/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 _rich_live = LazyLoader("_rich_live", globals(), "rich.live")
 _rich_panel = LazyLoader("_rich_panel", globals(), "rich.panel")
 _rich_table = LazyLoader("_rich_table", globals(), "rich.table")
 _rich_console = LazyLoader("_rich_console", globals(), "rich.console")
 
 
 class Session(_Session):
+    """重构 requests.Session"""
 
     def __init__(
         self,
         *,
         headers: Optional[Union[CIDict, dict]] = None,
         base_url: Optional[str] = None,
         user_agent: Optional[str] = None
```

### Comparing `pyxk-0.6.1/pyxk/utils.py` & `pyxk-0.6.2/pyxk/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,16 @@
     "download_column",
     "progress_column",
     "chardet"
 ]
 
 
 class LazyLoader(ModuleType):
-    """模块延迟加载
+    """模块延迟加载"""
 
-    :param local_name: 模块引用名称
-    :param module_life_cycle: 模块生命周期(建议使用全局变量 globals)
-    :param import_name: 导入模块名称
-    """
     def __init__(self, local_name, module_life_cycle, import_name=None):
         """模块延迟加载
 
         :param local_name: 模块引用名称
         :param module_life_cycle: 模块生命周期(建议使用全局变量 globals)
         :param import_name: 导入模块名称
         """
```

### Comparing `pyxk-0.6.1/pyxk.egg-info/SOURCES.txt` & `pyxk-0.6.2/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.1/setup.py` & `pyxk-0.6.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pyxk",
-    version="0.6.1",
+    version="0.6.2",
     author="pengke",
     install_requires=[
         "requests",
         "pycryptodome",
         "rich",
         "m3u8",
         "aiohttp",
```

