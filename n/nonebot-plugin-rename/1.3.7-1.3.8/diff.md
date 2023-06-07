# Comparing `tmp/nonebot_plugin_rename-1.3.7.tar.gz` & `tmp/nonebot_plugin_rename-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.3.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.3.8.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.3.7.tar` & `nonebot_plugin_rename-1.3.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/LICENSE
--rw-r--r--   0        0        0     5286 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/README.md
--rw-r--r--   0        0        0      495 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      293 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0      903 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/gaokao_time.py
--rw-r--r--   0        0        0     1020 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/genshin_time.py
--rw-r--r--   0        0        0      689 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0      925 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      450 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0      607 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      893 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/starrail_time.py
--rw-r--r--   0        0        0      604 2023-06-02 01:25:50.922933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      377 2023-06-02 01:25:50.926933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0  1878036 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/fonts/draw.ttf
--rw-r--r--   0        0        0     8740 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      151 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      495 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      838 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0     1529 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      400 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      574 2023-06-02 01:25:50.942933 nonebot_plugin_rename-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     6191 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/LICENSE
+-rw-r--r--   0        0        0     5286 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/README.md
+-rw-r--r--   0        0        0      549 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      293 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0      903 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/gaokao_time.py
+-rw-r--r--   0        0        0     1020 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/genshin_time.py
+-rw-r--r--   0        0        0      689 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0      925 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      450 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0      607 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      893 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/starrail_time.py
+-rw-r--r--   0        0        0      604 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      468 2023-06-07 02:50:42.126917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0  1878036 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/fonts/draw.ttf
+-rw-r--r--   0        0        0     8686 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      151 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      495 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      838 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0     1529 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      400 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      574 2023-06-07 02:50:42.146917 nonebot_plugin_rename-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     6191 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.3.8/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.3.7/LICENSE` & `nonebot_plugin_rename-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.7/README.md` & `nonebot_plugin_rename-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/gaokao_time.py` & `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/gaokao_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/genshin_time.py` & `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/genshin_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/get_times.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/hot_search.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/one_word.py` & `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/one_word.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/starrail_time.py` & `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/starrail_time.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Description: 获取星穹铁道版本剩余时间
 from datetime import datetime
 
 
 def starrail_version_time() -> str:
     # 基准版本
-    Version = 1.0
+    Version = 1.1
     baseTime = (
-        datetime.strptime("2023-4-26 10:00:00", "%Y-%m-%d %H:%M:%S").timestamp() * 1000
+        datetime.strptime("2023-6-7 11:00:00", "%Y-%m-%d %H:%M:%S").timestamp() * 1000
     )
     nowTime = datetime.now().timestamp() * 1000
     # 获取持续时间
     duringTime = baseTime - nowTime
     while duringTime <= 0:
         # 版本+0.1 同时时间+42天
         duringTime += 42 * 24 * 60 * 60 * 1000
@@ -20,7 +20,8 @@
     leave1 = duringTime % (24 * 3600 * 1000)
     # 获取小时数并取整
     hours = int(leave1 / (3600 * 1000))
     leave2 = leave1 % (3600 * 1000)
     # 获取分钟数并取整
     minutes = int(leave2 / (60 * 1000))
     return f"离崩铁{Version:.1f}还有{days}天{hours}小时{minutes}分钟"
+
```

### Comparing `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/card/status.py` & `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/card/status.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/fonts/draw.ttf` & `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/fonts/draw.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,27 @@
     MessageSegment,
     PrivateMessageEvent,
 )
 from nonebot.drivers import Driver
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 
-from .config import Config
+from .config import env_config
 from .utils import (
     card_list,
     choice_card,
     generate_card_image,
     read_yaml,
     write_yaml,
 )
 
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler  # noqa
 
 driver: Driver = get_driver()
-env_config = Config.parse_obj(get_driver().config.dict())
 hour, minute = env_config.set_group_card_hour, env_config.set_group_card_minute
 if driver.config.nickname:
     NICKNAME = env_config.self_name or list(driver.config.nickname)[0]
 else:
     NICKNAME = env_config.self_name or "bot"
 yml_file = Path.cwd() / "data" / "group_card"
 permissions = SUPERUSER | GROUP_ADMIN | GROUP_OWNER
```

### Comparing `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/card_name.py` & `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/card_name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.7/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.3.8/nonebot_plugin_rename/utils/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.3.7/pyproject.toml` & `nonebot_plugin_rename-1.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-rename"
-version = "1.3.7"
+version = "1.3.8"
 description = "更改qq机器人的群名片，内置多种有趣名片"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_rename"}]
```

### Comparing `nonebot_plugin_rename-1.3.7/PKG-INFO` & `nonebot_plugin_rename-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.3.7
+Version: 1.3.8
 Summary: 更改qq机器人的群名片，内置多种有趣名片
 License: GPL-3.0
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.3.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.3.8 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-
```

