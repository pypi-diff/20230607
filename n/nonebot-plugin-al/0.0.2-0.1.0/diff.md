# Comparing `tmp/nonebot_plugin_al-0.0.2.tar.gz` & `tmp/nonebot_plugin_al-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.1.0.tar", max compression
```

## Comparing `nonebot_plugin_al-0.0.2.tar` & `nonebot_plugin_al-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1091 2023-05-30 02:26:50.534952 nonebot_plugin_al-0.0.2/LICENSE
--rw-r--r--   0        0        0     1546 2023-06-02 07:19:07.918501 nonebot_plugin_al-0.0.2/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0     2361 2023-05-30 05:06:38.896053 nonebot_plugin_al-0.0.2/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0      964 2023-06-02 07:19:44.389387 nonebot_plugin_al-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1570 2023-06-02 06:46:21.539695 nonebot_plugin_al-0.0.2/README.md
--rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-05-30 02:26:50.534952 nonebot_plugin_al-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2156 2023-06-07 09:32:56.783348 nonebot_plugin_al-0.1.0/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0      776 2023-06-07 00:47:27.328125 nonebot_plugin_al-0.1.0/nonebot_plugin_al/api.py
+-rw-r--r--   0        0        0     3338 2023-06-07 03:11:57.150498 nonebot_plugin_al-0.1.0/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0    41657 2023-06-07 07:18:35.092784 nonebot_plugin_al-0.1.0/nonebot_plugin_al/ship.json
+-rw-r--r--   0        0        0     1002 2023-06-07 09:31:37.412702 nonebot_plugin_al-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1566 2023-06-07 09:33:43.971223 nonebot_plugin_al-0.1.0/README.md
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.0.2/LICENSE` & `nonebot_plugin_al-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.0.2/nonebot_plugin_al/__init__.py` & `nonebot_plugin_al-0.1.0/nonebot_plugin_al/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-import aiohttp
 
 from nonebot import on_command
 from nonebot.params import CommandArg
 from nonebot.matcher import Matcher
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters.onebot.v11 import (
     Message,
     MessageSegment
 )
-from .bili import jinghao,get_data
 
-__version__ = "0.0.1"
+from pathlib import Path
+try:
+    import ujson as json
+except:
+    import json
+
+from .bili import jinghao,get_data, get_ship_msg
+
+__version__ = "0.1.0"
 __plugin_meta__ = PluginMetadata(
     name="碧蓝航线攻略",
     description='碧蓝航线井号榜等等攻略',
     usage='碧蓝航线攻略',
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_AL",
     supported_adapters={"~onebot.v11"},
@@ -24,24 +30,36 @@
     },
 )
 
 al_command = on_command('al',aliases={'碧蓝'},priority=30,block=True)
 tag_ser = on_command('alhelp',aliases={'碧蓝指令','碧蓝帮助'},priority=30,block=True)
 tags = ['强度榜','装备榜','金部件榜','萌新榜','兵器榜','专武榜',
         '兑换榜','研发榜','改造榜','跨队榜','pt榜','氪金榜','打捞主线榜','打捞作战榜']
+with open((Path(__file__).parent.joinpath("ship.json")),
+          mode='r',encoding='utf-8')as f:
+    ships = json.load(f)
 
 @tag_ser.handle()
 async def _(matcher:Matcher):
-    msg = '碧蓝帮助指令\n'
+    msg = '指令:碧蓝+\n----------'
     data:str = ''
     for one in tags:
         data += f'{one} | '
     msg += data
+    msg += "----------"
+    msg += "碧蓝角色【角色名称】"
     await matcher.finish(msg)
 
 @al_command.handle()
 async def _(matcher:Matcher,args:Message = CommandArg()):
     word = args.extract_plain_text()
     if word in tags:
+        # 井号榜
         await matcher.finish(MessageSegment.image(await get_data(await jinghao(word))))
+    elif word.startswith("角色"):
+        # 舰船搜索
+        for key, value in ships.items():
+            if any(word in sublist for sublist in value):
+                await matcher.finish(MessageSegment.image(await get_ship_msg(key)))
+        await matcher.finish("没有这个角色~")
     else:
         await matcher.finish()
```

### Comparing `nonebot_plugin_al-0.0.2/pyproject.toml` & `nonebot_plugin_al-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_al"
-version = "0.0.2"
+version = "0.1.0"
 description = "Azuer L plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
 repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
 keywords = ["game", "nonebot2", "plugin","bilibili"]
@@ -20,13 +20,14 @@
     "LICENSE","README.md"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = ">=2.2.1"
+nonebot_plugin_htmlrender = "^2.0.0"
 aiohttp = ">=3.8.3"
 bs4 = "^0.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_al-0.0.2/README.md` & `nonebot_plugin_al-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
-# nonebot_plugin_AL 0.0.1
+# nonebot_plugin_AL 0.1.0
 
 _✨Nonebot & 碧蓝航线攻略✨_
 
 <a href="https://github.com/Agnes4m/nonebot_plugin_AL/stargazers">
         <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_AL" alt="stars">
 </a>
 <a href="https://github.com/Agnes4m/nonebot_plugin_AL/issues">
@@ -31,10 +31,11 @@
 </div>
 
 ## 指令
 
 - 碧蓝帮助 | 碧蓝指令
 - 显示的指令为【碧蓝】+xxx
 
-## 介绍
+## 功能
 
-爬取b站井号榜攻略等，在群聊展示攻略
+1、b站wiki井号榜一图流
+2、舰船图鉴
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
-# nonebot_plugin_AL 0.0.1 _â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨_ [GitHub_stars]
+# nonebot_plugin_AL 0.1.0 _â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨_ [GitHub_stars]
    [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python] [NoneBot]
 ## æä»¤ - ç¢§èå¸®å© | ç¢§èæä»¤ - æ¾ç¤ºçæä»¤ä¸ºãç¢§èã+xxx ##
-ä»ç» ç¬åbç«äºå·æ¦æ»ç¥ç­ï¼å¨ç¾¤èå±ç¤ºæ»ç¥
+åè½ 1ãbç«wikiäºå·æ¦ä¸å¾æµ 2ãè°è¹å¾é´
```

### Comparing `nonebot_plugin_al-0.0.2/PKG-INFO` & `nonebot_plugin_al-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-al
-Version: 0.0.2
+Version: 0.1.0
 Summary: Azuer L plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: GPLv3
 Keywords: game,nonebot2,plugin,bilibili
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -19,26 +19,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.3)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: nonebot_plugin_htmlrender (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_AL
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
-# nonebot_plugin_AL 0.0.1
+# nonebot_plugin_AL 0.1.0
 
 _✨Nonebot & 碧蓝航线攻略✨_
 
 <a href="https://github.com/Agnes4m/nonebot_plugin_AL/stargazers">
         <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_AL" alt="stars">
 </a>
 <a href="https://github.com/Agnes4m/nonebot_plugin_AL/issues">
@@ -59,10 +60,11 @@
 </div>
 
 ## 指令
 
 - 碧蓝帮助 | 碧蓝指令
 - 显示的指令为【碧蓝】+xxx
 
-## 介绍
+## 功能
 
-爬取b站井号榜攻略等，在群聊展示攻略
+1、b站wiki井号榜一图流
+2、舰船图鉴
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.0.2 Summary: Azuer L
+Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.1.0 Summary: Azuer L
 plugin for NoneBot2 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: GPLv3 Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
 Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 License :: Other/Proprietary License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.9 Requires-Dist: aiohttp (>=3.8.3) Requires-Dist: bs4
 (>=0.0.1,<0.0.2) Requires-Dist: nonebot-adapter-onebot (>=2.2.1) Requires-Dist:
-nonebot2 (>=2.0.0,<3.0.0) Project-URL: Repository, https://github.com/Agnes4m/
+nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: nonebot_plugin_htmlrender
+(>=2.0.0,<3.0.0) Project-URL: Repository, https://github.com/Agnes4m/
 nonebot_plugin_AL Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
-# nonebot_plugin_AL 0.0.1 _â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨_ [GitHub_stars]
+# nonebot_plugin_AL 0.1.0 _â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨_ [GitHub_stars]
    [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python] [NoneBot]
 ## æä»¤ - ç¢§èå¸®å© | ç¢§èæä»¤ - æ¾ç¤ºçæä»¤ä¸ºãç¢§èã+xxx ##
-ä»ç» ç¬åbç«äºå·æ¦æ»ç¥ç­ï¼å¨ç¾¤èå±ç¤ºæ»ç¥
+åè½ 1ãbç«wikiäºå·æ¦ä¸å¾æµ 2ãè°è¹å¾é´
```

