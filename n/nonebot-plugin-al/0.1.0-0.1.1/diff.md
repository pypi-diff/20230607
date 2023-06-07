# Comparing `tmp/nonebot_plugin_al-0.1.0.tar.gz` & `tmp/nonebot_plugin_al-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_al-0.1.0.tar` & `nonebot_plugin_al-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2023-05-30 02:26:50.534952 nonebot_plugin_al-0.1.0/LICENSE
--rw-r--r--   0        0        0     2156 2023-06-07 09:32:56.783348 nonebot_plugin_al-0.1.0/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0      776 2023-06-07 00:47:27.328125 nonebot_plugin_al-0.1.0/nonebot_plugin_al/api.py
--rw-r--r--   0        0        0     3338 2023-06-07 03:11:57.150498 nonebot_plugin_al-0.1.0/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0    41657 2023-06-07 07:18:35.092784 nonebot_plugin_al-0.1.0/nonebot_plugin_al/ship.json
--rw-r--r--   0        0        0     1002 2023-06-07 09:31:37.412702 nonebot_plugin_al-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1566 2023-06-07 09:33:43.971223 nonebot_plugin_al-0.1.0/README.md
--rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-05-30 14:08:53.643151 nonebot_plugin_al-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2198 2023-06-07 15:22:18.943516 nonebot_plugin_al-0.1.1/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0      776 2023-06-06 14:05:44.522832 nonebot_plugin_al-0.1.1/nonebot_plugin_al/api.py
+-rw-r--r--   0        0        0     3338 2023-06-07 15:07:11.428916 nonebot_plugin_al-0.1.1/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0    41657 2023-06-07 15:07:11.516516 nonebot_plugin_al-0.1.1/nonebot_plugin_al/ship.json
+-rw-r--r--   0        0        0     1002 2023-06-07 15:09:28.649531 nonebot_plugin_al-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1566 2023-06-07 15:07:11.098960 nonebot_plugin_al-0.1.1/README.md
+-rw-r--r--   0        0        0     2562 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.1.0/LICENSE` & `nonebot_plugin_al-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.1.0/nonebot_plugin_al/__init__.py` & `nonebot_plugin_al-0.1.1/nonebot_plugin_al/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,13 +53,14 @@
 async def _(matcher:Matcher,args:Message = CommandArg()):
     word = args.extract_plain_text()
     if word in tags:
         # 井号榜
         await matcher.finish(MessageSegment.image(await get_data(await jinghao(word))))
     elif word.startswith("角色"):
         # 舰船搜索
+        word = word.replace("角色","")
         for key, value in ships.items():
             if any(word in sublist for sublist in value):
                 await matcher.finish(MessageSegment.image(await get_ship_msg(key)))
         await matcher.finish("没有这个角色~")
     else:
         await matcher.finish()
```

### Comparing `nonebot_plugin_al-0.1.0/nonebot_plugin_al/api.py` & `nonebot_plugin_al-0.1.1/nonebot_plugin_al/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.1.0/nonebot_plugin_al/bili.py` & `nonebot_plugin_al-0.1.1/nonebot_plugin_al/bili.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.1.0/nonebot_plugin_al/ship.json` & `nonebot_plugin_al-0.1.1/nonebot_plugin_al/ship.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.1.0/pyproject.toml` & `nonebot_plugin_al-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_al"
-version = "0.1.0"
+version = "0.1.1"
 description = "Azuer L plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
 repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
 keywords = ["game", "nonebot2", "plugin","bilibili"]
```

### Comparing `nonebot_plugin_al-0.1.0/README.md` & `nonebot_plugin_al-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.1.0/PKG-INFO` & `nonebot_plugin_al-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-al
-Version: 0.1.0
+Version: 0.1.1
 Summary: Azuer L plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: GPLv3
 Keywords: game,nonebot2,plugin,bilibili
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -12,17 +12,14 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.3)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot_plugin_htmlrender (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_AL
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.1.0 Summary: Azuer L
+Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.1.1 Summary: Azuer L
 plugin for NoneBot2 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: GPLv3 Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
 Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 License :: Other/Proprietary License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.9 Requires-Dist: aiohttp (>=3.8.3) Requires-Dist: bs4
+Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.3) Requires-Dist: bs4
 (>=0.0.1,<0.0.2) Requires-Dist: nonebot-adapter-onebot (>=2.2.1) Requires-Dist:
 nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: nonebot_plugin_htmlrender
 (>=2.0.0,<3.0.0) Project-URL: Repository, https://github.com/Agnes4m/
 nonebot_plugin_AL Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
 # nonebot_plugin_AL 0.1.0 _â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨_ [GitHub_stars]
```

