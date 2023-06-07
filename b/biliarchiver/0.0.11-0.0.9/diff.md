# Comparing `tmp/biliarchiver-0.0.11.tar.gz` & `tmp/biliarchiver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biliarchiver-0.0.11.tar", max compression
+gzip compressed data, was "biliarchiver-0.0.9.tar", max compression
```

## Comparing `biliarchiver-0.0.11.tar` & `biliarchiver-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      429 2023-06-06 20:05:41.529385 biliarchiver-0.0.11/README.md
--rw-r--r--   0        0        0     7575 2023-06-07 12:25:53.093261 biliarchiver-0.0.11/biliarchiver/_biliarchiver_upload_bvid.py
--rw-r--r--   0        0        0     7157 2023-06-06 19:12:07.431306 biliarchiver-0.0.11/biliarchiver/archive_bvid.py
--rw-r--r--   0        0        0     4839 2023-06-07 07:19:17.062795 biliarchiver-0.0.11/biliarchiver/bili_archive_bvids.py
--rw-r--r--   0        0        0     4133 2023-06-06 19:45:06.489235 biliarchiver-0.0.11/biliarchiver/bili_get_bvids.py
--rw-r--r--   0        0        0     1490 2023-06-07 12:25:53.093261 biliarchiver-0.0.11/biliarchiver/bili_upload.py
--rw-r--r--   0        0        0     2018 2023-06-06 19:20:55.302758 biliarchiver-0.0.11/biliarchiver/config.py
--rw-r--r--   0        0        0     2724 2023-06-06 05:53:18.324384 biliarchiver-0.0.11/biliarchiver/utils/dirLock.py
--rw-r--r--   0        0        0      237 2023-06-07 06:29:29.311341 biliarchiver-0.0.11/biliarchiver/utils/ffmpeg.py
--rw-r--r--   0        0        0     1278 2023-06-05 16:41:54.082484 biliarchiver-0.0.11/biliarchiver/utils/string.py
--rw-r--r--   0        0        0       32 2023-06-07 06:32:05.907925 biliarchiver-0.0.11/biliarchiver/version.py
--rw-r--r--   0        0        0      529 2023-06-07 08:35:32.732728 biliarchiver-0.0.11/pyproject.toml
--rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 biliarchiver-0.0.11/setup.py
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 biliarchiver-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-06-06 20:05:41.529385 biliarchiver-0.0.9/README.md
+-rw-r--r--   0        0        0     7575 2023-06-06 19:48:46.123664 biliarchiver-0.0.9/biliarchiver/_biliarchiver_upload_bvid.py
+-rw-r--r--   0        0        0     7157 2023-06-06 19:12:07.431306 biliarchiver-0.0.9/biliarchiver/archive_bvid.py
+-rw-r--r--   0        0        0     4734 2023-06-07 04:48:33.598085 biliarchiver-0.0.9/biliarchiver/bili_archive_bvids.py
+-rw-r--r--   0        0        0     4133 2023-06-06 19:45:06.489235 biliarchiver-0.0.9/biliarchiver/bili_get_bvids.py
+-rw-r--r--   0        0        0     1490 2023-06-07 04:52:11.184454 biliarchiver-0.0.9/biliarchiver/bili_uploade.py
+-rw-r--r--   0        0        0     2018 2023-06-06 19:20:55.302758 biliarchiver-0.0.9/biliarchiver/config.py
+-rw-r--r--   0        0        0     2724 2023-06-06 05:53:18.324384 biliarchiver-0.0.9/biliarchiver/utils/dirLock.py
+-rw-r--r--   0        0        0     1278 2023-06-05 16:41:54.082484 biliarchiver-0.0.9/biliarchiver/utils/string.py
+-rw-r--r--   0        0        0       31 2023-06-06 19:35:41.648702 biliarchiver-0.0.9/biliarchiver/version.py
+-rw-r--r--   0        0        0      530 2023-06-07 04:58:02.482737 biliarchiver-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 biliarchiver-0.0.9/setup.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 biliarchiver-0.0.9/PKG-INFO
```

### Comparing `biliarchiver-0.0.11/biliarchiver/_biliarchiver_upload_bvid.py` & `biliarchiver-0.0.9/biliarchiver/_biliarchiver_upload_bvid.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.11/biliarchiver/archive_bvid.py` & `biliarchiver-0.0.9/biliarchiver/archive_bvid.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.11/biliarchiver/bili_archive_bvids.py` & `biliarchiver-0.0.9/biliarchiver/bili_archive_bvids.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 from biliarchiver.archive_bvid import archive_bvid
 from biliarchiver.config import Config
 
 from bilix.sites.bilibili.downloader import DownloaderBilibili
 from rich.console import Console
 from httpx import AsyncClient, Client
 from rich.traceback import install
-install()
 
 from biliarchiver.utils.string import human_readable_upper_part_map
-from biliarchiver.utils.ffmpeg import check_ffmpeg
+install()
 
 from biliarchiver.config import BILIBILI_IDENTIFIER_PERFIX
 
 from dataclasses import dataclass
 
 @dataclass
 class Args:
@@ -50,15 +49,14 @@
     elif r_json['code'] == 'not_available':
         return True
     else:
         raise ValueError(f'Unexpected code: {r_json["code"]}')
 
 def _main():
     args = parse_args()
-    assert check_ffmpeg() is True, 'ffmpeg 未安装'
 
     assert args.bvids is not None, '必须指定 bvids 列表的文件路径'
     with open(args.bvids, 'r', encoding='utf-8') as f:
         bvids_from_file = f.read().splitlines()
 
     config = Config()
```

### Comparing `biliarchiver-0.0.11/biliarchiver/bili_get_bvids.py` & `biliarchiver-0.0.9/biliarchiver/bili_get_bvids.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.11/biliarchiver/bili_upload.py` & `biliarchiver-0.0.9/biliarchiver/bili_uploade.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.11/biliarchiver/config.py` & `biliarchiver-0.0.9/biliarchiver/config.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.11/biliarchiver/utils/dirLock.py` & `biliarchiver-0.0.9/biliarchiver/utils/dirLock.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.11/biliarchiver/utils/string.py` & `biliarchiver-0.0.9/biliarchiver/utils/string.py`

 * *Files identical despite different names*

### Comparing `biliarchiver-0.0.11/pyproject.toml` & `biliarchiver-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "biliarchiver"
-version = "0.0.11"
+version = "0.0.9"
 description = ""
 authors = ["yzqzss <yzqzss@yandex.com>"]
 readme = "README.md"
 packages = [{include = "biliarchiver"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 bilix = "0.18.3"
 internetarchive = "^3.5.0"
 
 [tool.poetry.scripts]
 bili_archive_bvids = "biliarchiver:bili_archive_bvids.main"
-bili_upload = "biliarchiver:bili_upload.main"
+bili_uploade = "biliarchiver:bili_uploade.main"
 bili_get_bvids = "biliarchiver:bili_get_bvids.main"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `biliarchiver-0.0.11/setup.py` & `biliarchiver-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 install_requires = \
 ['bilix==0.18.3', 'internetarchive>=3.5.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['bili_archive_bvids = '
                      'biliarchiver:bili_archive_bvids.main',
                      'bili_get_bvids = biliarchiver:bili_get_bvids.main',
-                     'bili_upload = biliarchiver:bili_upload.main']}
+                     'bili_uploade = biliarchiver:bili_uploade.main']}
 
 setup_kwargs = {
     'name': 'biliarchiver',
-    'version': '0.0.11',
+    'version': '0.0.9',
     'description': '',
     'long_description': '# biliarchiver\n\n## 基于 bilix 的 BiliBili 存档工具\n\n~~ IA iteam identifier 格式兼容 tubeup ~~。  \n现在不兼容了，Tubeup 不适合存 B 站视频，它的 identifier 设计不科学，大规模存档必定会撞车。\n\n目前，我可能随时 commit 乱飞且动不动就 git push -f 这个仓库。（为了在我的 vps 和本地之间同步代码）\n\nuserscript.js 还没适配新换的 identifier 格式。\n',
     'author': 'yzqzss',
     'author_email': 'yzqzss@yandex.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `biliarchiver-0.0.11/PKG-INFO` & `biliarchiver-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biliarchiver
-Version: 0.0.11
+Version: 0.0.9
 Summary: 
 Author: yzqzss
 Author-email: yzqzss@yandex.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

