# Comparing `tmp/nonebot_plugin_picstatus-0.4.2.tar.gz` & `tmp/nonebot_plugin_picstatus-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_picstatus-0.4.2.tar", last modified: Sun Jun  4 16:33:22 2023, max compression
+gzip compressed data, was "nonebot_plugin_picstatus-0.5.0.tar", last modified: Wed Jun  7 13:35:16 2023, max compression
```

## Comparing `nonebot_plugin_picstatus-0.4.2.tar` & `nonebot_plugin_picstatus-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/LICENSE
--rw-r--r--   0        0        0     6857 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/README.md
--rw-r--r--   0        0        0      932 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/__init__.py
--rw-r--r--   0        0        0     3502 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/__main__.py
--rw-r--r--   0        0        0     1251 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/config.py
--rw-r--r--   0        0        0      251 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/const.py
--rw-r--r--   0        0        0    18979 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/draw.py
--rw-r--r--   0        0        0   378600 2023-06-04 16:33:05.987925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/res/default_avatar.png
--rw-r--r--   0        0        0  1527158 2023-06-04 16:33:05.999925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/res/default_bg.png
--rw-r--r--   0        0        0     1385 2023-06-04 16:33:05.999925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/statistics.py
--rw-r--r--   0        0        0     4727 2023-06-04 16:33:05.999925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/util.py
--rw-r--r--   0        0        0       22 2023-06-04 16:33:05.999925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/version.py
--rw-r--r--   0        0        0      763 2023-06-04 16:33:22.424657 nonebot_plugin_picstatus-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     7537 1970-01-01 00:00:00.000000 nonebot_plugin_picstatus-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-07 13:35:03.242865 nonebot_plugin_picstatus-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7150 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/README.md
+-rw-r--r--   0        0        0      988 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/__init__.py
+-rw-r--r--   0        0        0     4123 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/__main__.py
+-rw-r--r--   0        0        0     1713 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/config.py
+-rw-r--r--   0        0        0      251 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/const.py
+-rw-r--r--   0        0        0    14152 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/draw.py
+-rw-r--r--   0        0        0   378600 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/res/default_avatar.png
+-rw-r--r--   0        0        0  1527158 2023-06-07 13:35:03.258866 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/res/default_bg.png
+-rw-r--r--   0        0        0     1393 2023-06-07 13:35:03.258866 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/statistics.py
+-rw-r--r--   0        0        0    12403 2023-06-07 13:35:03.258866 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/status.py
+-rw-r--r--   0        0        0     3966 2023-06-07 13:35:03.258866 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/util.py
+-rw-r--r--   0        0        0       22 2023-06-07 13:35:03.258866 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/version.py
+-rw-r--r--   0        0        0      763 2023-06-07 13:35:16.667914 nonebot_plugin_picstatus-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7830 1970-01-01 00:00:00.000000 nonebot_plugin_picstatus-0.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_picstatus-0.4.2/LICENSE` & `nonebot_plugin_picstatus-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.4.2/README.md` & `nonebot_plugin_picstatus-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,72 +37,78 @@
 不多说，直接看图！
 
 ### 效果图
 
 <details>
   <summary>点击展开</summary>
 
-![example](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/picstatus/example.png)
+![example](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/picstatus/example.jpg)
 
 </details>
 
 ## 💿 安装
 
+以下提到的方法 任选**其一** 即可
+
 <details open>
 <summary>[推荐] 使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
-    nb plugin install nonebot-plugin-picstatus
+```bash
+nb plugin install nonebot-plugin-picstatus
+```
 
 </details>
 
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
 
-    pip install nonebot-plugin-picstatus
+```bash
+pip install nonebot-plugin-picstatus
+```
 
 </details>
 <details>
 <summary>pdm</summary>
 
-    pdm add nonebot-plugin-picstatus
+```bash
+pdm add nonebot-plugin-picstatus
+```
 
 </details>
 <details>
 <summary>poetry</summary>
 
-    poetry add nonebot-plugin-picstatus
+```bash
+poetry add nonebot-plugin-picstatus
+```
 
 </details>
 <details>
 <summary>conda</summary>
 
-    conda install nonebot-plugin-picstatus
-
-</details>
-
-打开 nonebot2 项目的 `bot.py` 文件, 在其中写入
-
-    nonebot.load_plugin('nonebot_plugin_picstatus')
+```bash
+conda install nonebot-plugin-picstatus
+```
 
 </details>
 
-<details>
-<summary>从 github 安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 输入以下命令克隆此储存库
-
-    git clone https://github.com/lgc2333/nonebot-plugin-picstatus.git
-
-打开 nonebot2 项目的 `bot.py` 文件, 在其中写入
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分的 `plugins` 项里追加写入
 
-    nonebot.load_plugin('src.plugins.nonebot_plugin_picstatus')
+```toml
+[tool.nonebot]
+plugins = [
+    # ...
+    "nonebot_plugin_picstatus"
+]
+```
 
 </details>
 
 ## ⚙️ 配置
 
 见[.env.example](https://github.com/lgc2333/nonebot-plugin-picstatus/blob/master/.env.example)
 
@@ -139,14 +145,21 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.5.0
+
+- 先获取状态信息再进行画图，可以获取到更精准的状态信息
+- 添加进程占用信息的展示
+- 测试网站结果状态码后面会带上 `reason`，如 `200 OK` / `404 Not Found`
+- 添加了一些配置项（`PS_SORT_PARTS`, `PS_SORT_PARTS_REVERSE`, `PS_SORT_DISK_IOS`, `PS_SORT_NETS`, `PS_SORT_SITES`, `PS_PROC_LEN`, `PS_IGNORE_PROCS`, `PS_PROC_SORT_BY`, `PS_PROC_CPU_MAX_100P`, `PS_REPLY_TARGET`, `PS_TG_MAX_FILE_SIZE`）
+
 ### 0.4.2
 
 - 添加配置项 `PS_REQ_TIMEOUT` ([#25](https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus/issues/25))
 
 ### 0.4.1
 
 - 现在默认使用 `pil_utils` 自动选择系统内支持中文的字体，删除插件内置字体
```

#### html2text {}

```diff
@@ -1,40 +1,46 @@
                                     [logo]
                                     [logo]
    # NoneBot-Plugin-PicStatus _â¨ è¿è¡ç¶æå¾çç for NoneBot2 â¨_
              [license] [pypi] [python] [pypi_download] [wakatime]
 ## ð ä»ç» ä¸å¤è¯´ï¼ç´æ¥çå¾ï¼ ### ææå¾  ç¹å»å±å¼ !
 [example](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/picstatus/
-example.png)  ## ð¿ å®è£  [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-picstatus   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot-plugin-picstatus   pdm pdm
-add nonebot-plugin-picstatus   poetry poetry add nonebot-plugin-picstatus
-conda conda install nonebot-plugin-picstatus  æå¼ nonebot2 é¡¹ç®ç
-`bot.py` æä»¶, å¨å¶ä¸­åå¥ nonebot.load_plugin
-('nonebot_plugin_picstatus')   ä» github å®è£ å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸å½ä»¤åéæ­¤å¨å­åº
-git clone https://github.com/lgc2333/nonebot-plugin-picstatus.git æå¼
-nonebot2 é¡¹ç®ç `bot.py` æä»¶, å¨å¶ä¸­åå¥ nonebot.load_plugin
-('src.plugins.nonebot_plugin_picstatus')  ## âï¸ éç½® è§[.env.example]
-(https://github.com/lgc2333/nonebot-plugin-picstatus/blob/master/.env.example)
-## ð ä½¿ç¨ ä½¿ç¨æä»¤`è¿è¡ç¶æ`ï¼æè`ç¶æ` / `zt` / `yxzt` /
+example.jpg)  ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯
+[æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
+plugin install nonebot-plugin-picstatus ```   ä½¿ç¨åç®¡çå¨å®è£ å¨
+nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
+install nonebot-plugin-picstatus ```   pdm ```bash pdm add nonebot-plugin-
+picstatus ```   poetry ```bash poetry add nonebot-plugin-picstatus ```   conda
+```bash conda install nonebot-plugin-picstatus ```  æå¼ nonebot2
+é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
+`plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
+"nonebot_plugin_picstatus" ] ```  ## âï¸ éç½® è§[.env.example](https://
+github.com/lgc2333/nonebot-plugin-picstatus/blob/master/.env.example) ## ð
+ä½¿ç¨ ä½¿ç¨æä»¤`è¿è¡ç¶æ`ï¼æè`ç¶æ` / `zt` / `yxzt` /
 `status`ï¼æ¥è§¦åæä»¶åè½
 å¯ä»¥å¨æ¶æ¯åé¢è·ä¸å¼ å¾çæèåå¤ä¸å¼ å¾çæ¥èªå®ä¹èæ¯å¾ï¼é»è®¤ä¸ºéæºèæ¯å¾
 æ´å¤èªå®ä¹é¡¹åè§ [éç½®](#ï¸-éç½®) ## ð èç³» QQï¼3076823485
 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://
 jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [ææ¢¦ API](https://api.gumengya.com) -
 éæºèæ¯å¾æ¥æº ### [LoliApi](https://docs.loliapi.com/) -
 éæºèæ¯å¾æ¥æºï¼ææ¶å¼ç¨ï¼ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.4.2 - æ·»å éç½®é¡¹
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.5.0 -
+åè·åç¶æä¿¡æ¯åè¿è¡ç»å¾ï¼å¯ä»¥è·åå°æ´ç²¾åçç¶æä¿¡æ¯
+- æ·»å è¿ç¨å ç¨ä¿¡æ¯çå±ç¤º -
+æµè¯ç½ç«ç»æç¶æç åé¢ä¼å¸¦ä¸ `reason`ï¼å¦ `200 OK` / `404 Not
+Found` - æ·»å äºä¸äºéç½®é¡¹ï¼`PS_SORT_PARTS`, `PS_SORT_PARTS_REVERSE`,
+`PS_SORT_DISK_IOS`, `PS_SORT_NETS`, `PS_SORT_SITES`, `PS_PROC_LEN`,
+`PS_IGNORE_PROCS`, `PS_PROC_SORT_BY`, `PS_PROC_CPU_MAX_100P`,
+`PS_REPLY_TARGET`, `PS_TG_MAX_FILE_SIZE`ï¼ ### 0.4.2 - æ·»å éç½®é¡¹
 `PS_REQ_TIMEOUT` ([#25](https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus/
 issues/25)) ### 0.4.1 - ç°å¨é»è®¤ä½¿ç¨ `pil_utils`
 èªå¨éæ©ç³»ç»åæ¯æä¸­æçå­ä½ï¼å é¤æä»¶åç½®å­ä½ - ä½¿ç¨
 `pil_utils` å Bot æµç§°ï¼å¯ä»¥æ¾ç¤º Emoji ç­ç¹æ®å­ç¬¦ -
 æµè¯ç½ç«åºéæ¶ä¸ä¼å¾æ¥å¿éç©éè¯¯å æ äº ### 0.4.0 - ä½¿ç¨
 [nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-
 plugin-send-anything-anywhere) å¼å®¹å¤å¹³å°åéï¼å¹¶å¯¹ OneBot V11 å
```

### Comparing `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/__init__.py` & `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 __plugin_meta__ = PluginMetadata(
     name="PicStatus",
     description="以图片形式显示当前设备的运行状态",
     usage=usage,
     type="application",
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus",
     config=Cfg,
-    supported_adapters=[
+    supported_adapters={
         "~onebot.v11",
         "~onebot.v12",
         "~telegram",
         "~kaiheila",
         "~qqguild",
-    ],
+    },
+    extra={"License": "MIT", "Author": "student_2333"},
 )
```

### Comparing `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/__main__.py` & `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,20 +68,31 @@
             msg += event.reply_to_message.message
 
         file_id = None
         if photos := msg["photo"]:
             file_id = photos[0].data["file"]
 
         elif documents := msg["document"]:
-            for doc in documents:
-                data = doc.data["document"]
-                if data["mime_type"].startswith("image/"):
-                    # if not data["file_size"] > (15 * 1024 * 1024):
+            doc = next(
+                (
+                    doc
+                    for doc in documents
+                    if doc.data["mime_type"].startswith("image/")
+                ),
+                None,
+            )
+            if doc:
+                data = doc.data
+                if data["file_size"] > (config.ps_tg_max_file_size * 1024 * 1024):
+                    logger.warning("附带图片文件过大，回退到默认行为")
+                    await MessageFactory("附带图片文件过大，将使用默认图片").send(
+                        reply=config.ps_reply_target,
+                    )
+                else:
                     file_id = data["file_id"]
-                    break
 
         if file_id:
             return await download_telegram_file(bot, file_id)
 
     return None
 
 
@@ -99,23 +110,23 @@
     matcher: Matcher,
 ):
     pic = None
     try:
         pic = await extract_msg_pic(bot, event)
     except:
         logger.exception("获取消息中附带图片失败，回退到默认行为")
+        await MessageFactory("获取消息中附带图片失败，将使用默认图片").send(reply=config.ps_reply_target)
 
     try:
         ret = await get_stat_pic(bot, pic)
     except:
         logger.exception("获取运行状态图失败")
-        await matcher.finish("获取运行状态图片失败，请检查后台输出")
+        await MessageFactory("获取运行状态图片失败，请检查后台输出").send(reply=config.ps_reply_target)
+        await matcher.finish()
 
     # 为什么 SAA 还不发版支持 TG
     # 哼哼啊啊啊啊啊啊啊啊啊啊啊啊
     if TGMessageEvent and isinstance(event, TGMessageEvent):
-        await matcher.send(File.photo(ret))
-
-    else:
-        await MessageFactory(Image(ret)).send()
+        await matcher.finish(File.photo(ret))
 
+    await MessageFactory(Image(ret)).send(reply=config.ps_reply_target)
     await matcher.finish()
```

### Comparing `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/config.py` & `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,59 @@
-from typing import List, Optional, Set, Tuple
+from typing import List, Literal, Optional, Set, Tuple
 
 from nonebot import get_driver
 from pydantic import BaseModel
 
 
 class TestSiteCfg(BaseModel):
     name: str
     url: str
     use_proxy: bool = False
 
 
+ProcSortByType = Literal["cpu", "mem"]
+
+
 class Cfg(BaseModel):
     superusers: Set[str] = set()
     nickname: Set[str] = set()
 
     proxy: Optional[str] = None
 
-    ps_only_su: bool = False
-    ps_blur_radius: int = 4
-    ps_font: Optional[str] = None
+    ps_use_env_nick: bool = False
     ps_ignore_parts: List[str] = []
     ps_ignore_bad_parts: bool = False
+    ps_sort_parts: bool = True
+    ps_sort_parts_reverse: bool = False
     ps_ignore_disk_ios: List[str] = []
-    ps_use_env_nick: bool = False
-    ps_need_at: bool = False
-    ps_mask_color: Tuple[int, int, int, int] = (255, 255, 255, 125)
-    ps_bg_color: Tuple[int, int, int, int] = (255, 255, 255, 150)
-    ps_ignore_nets: List[str] = ["^lo$", "^Loopback"]
     ps_ignore_no_io_disk: bool = False
+    ps_sort_disk_ios: bool = True
+    ps_ignore_nets: List[str] = ["^lo$", "^Loopback"]
     ps_ignore_0b_net: bool = False
-    ps_custom_bg: List[str] = []
-    ps_footer_size: int = 22
+    ps_sort_nets: bool = True
     ps_test_sites: List[TestSiteCfg] = [
-        TestSiteCfg(name="百度", url="https://baidu.com"),
-        TestSiteCfg(name="Google", url="https://google.com", use_proxy=True),
+        TestSiteCfg(name="百度", url="https://www.baidu.com/"),
+        TestSiteCfg(name="Google", url="https://www.google.com/", use_proxy=True),
     ]
+    ps_sort_sites: bool = True
+    ps_proc_len: int = 5
+    ps_ignore_procs: List[str] = ["^System Idle Process$"]
+    ps_proc_sort_by: ProcSortByType = "cpu"
+    ps_proc_cpu_max_100p: bool = False
     ps_test_timeout: int = 5
-    ps_max_text_len: int = 18
     ps_req_timeout: Optional[int] = 10
 
+    ps_font: Optional[str] = None
+    ps_custom_bg: List[str] = []
+    ps_bg_color: Tuple[int, int, int, int] = (255, 255, 255, 150)
+    ps_mask_color: Tuple[int, int, int, int] = (255, 255, 255, 125)
+    ps_blur_radius: int = 4
+    ps_footer_size: int = 22
+    ps_max_text_len: int = 18
+
+    ps_only_su: bool = False
+    ps_need_at: bool = False
+    ps_reply_target: bool = True
+    ps_tg_max_file_size: int = 15
+
 
 config: Cfg = Cfg.parse_obj(get_driver().config.dict())
```

### Comparing `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/draw.py` & `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/draw.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,123 +1,77 @@
 import asyncio
 import platform
 import random
 import time
-from datetime import datetime
 from io import BytesIO
-from typing import Dict, List, Optional, Tuple, Union, cast
+from typing import List, Optional, Union
 
-import httpx
 import nonebot
-import psutil
-from httpx import AsyncClient
 from nonebot import logger
 from nonebot.internal.adapter import Bot
 from PIL import Image, ImageDraw, ImageFilter, ImageFont
 from pil_utils import BuildImage
 from pil_utils.fonts import get_proper_font
-from psutil._common import sdiskio, sdiskusage, snetio
 
-from .config import TestSiteCfg, config
+from .config import config
 from .const import DEFAULT_BG_PATH
-from .statistics import bot_connect_time, nonebot_run_time, recv_num, send_num
+from .status import (
+    CpuMemoryStat,
+    DiskStatus,
+    DiskUsageWithExc,
+    HeaderData,
+    NetworkConnectionError,
+    NetworkStatus,
+    ProcessStatus,
+    format_freq_txt,
+    get_cpu_memory_usage,
+    get_disk_status,
+    get_header_data,
+    get_network_status,
+    get_process_status,
+    get_system_name,
+)
 from .util import (
     async_open_img,
     async_request,
     format_byte_count,
-    format_timedelta,
     get_anime_pic,
-    get_bot_avatar,
-    get_system_name,
-    match_list_regexp,
-    process_text_len,
 )
 from .version import __version__
 
-try:
-    from nonebot.adapters.onebot.v11 import Bot as OBV11Bot
-except:
-    OBV11Bot = None
-
-try:
-    from nonebot.adapters.telegram import Bot as TGBot
-except:
-    TGBot = None
-
-
 GRAY_BG_COLOR: str = "#aaaaaaaa"
 WHITE_BG_COLOR = config.ps_bg_color
 WHITE_MASK_COLOR = config.ps_mask_color
 
 FONT_PATH = config.ps_font or str(get_proper_font("国").path.resolve())
 
 
 def get_font(size: int):
     return ImageFont.truetype(FONT_PATH, size)
 
 
+font_25 = get_font(25)
+font_30 = get_font(30)
+font_40 = get_font(40)
+font_45 = get_font(45)
+font_70 = get_font(70)
+font_footer = get_font(config.ps_footer_size)
+
+
 def get_usage_color(usage: float):
     usage = round(usage)
     if usage >= 90:
         return "orangered"
     if usage >= 70:
         return "orange"
     return "lightgreen"
 
 
-async def draw_header(bot: Bot):
-    # 平台兼容处理
-    nick: Optional[str] = None
-    msg_rec: Optional[str] = None
-    msg_sent: Optional[str] = None
-
-    if OBV11Bot and isinstance(bot, OBV11Bot):
-        bot_stat = (await bot.get_status()).get("stat")
-        if bot_stat:
-            msg_rec = bot_stat.get("message_received") or bot_stat.get(
-                "MessageReceived",
-            )
-            msg_sent = bot_stat.get("message_sent") or bot_stat.get("MessageSent")
-
-        if not (config.ps_use_env_nick and config.nickname):
-            nick = (await bot.get_login_info())["nickname"]
-
-    if TGBot and isinstance(bot, TGBot):  # noqa: SIM102
-        if not (config.ps_use_env_nick and config.nickname):
-            nick = (await bot.get_me()).first_name
-
-    avatar = await get_bot_avatar(bot)
-    if not nick:
-        nick = list(config.nickname)[0] if config.nickname else "Bot"
-    if msg_rec is None:
-        num = recv_num.get(bot.self_id)
-        msg_rec = "未知" if num is None else str(num)
-    if msg_sent is None:
-        num = send_num.get(bot.self_id)
-        msg_sent = "未知" if num is None else str(num)
-
-    # 通用数据
-    bot_connected = (
-        format_timedelta(datetime.now() - t)
-        if (t := bot_connect_time.get(bot.self_id))
-        else "未知"
-    )
-    nb_run = (
-        format_timedelta(datetime.now() - nonebot_run_time)
-        if nonebot_run_time
-        else "未知"
-    )
-
-    # 系统启动时间
-    booted = format_timedelta(
-        datetime.now() - datetime.fromtimestamp(psutil.boot_time()),
-    )
-
-    font_30 = get_font(30)
-    # font_80 = get_font(80)
+async def draw_header(data: HeaderData) -> Image.Image:
+    avatar, nick, bot_connected, msg_rec, msg_sent, nb_run, booted = data
 
     bg = Image.new("RGBA", (1200, 300), WHITE_BG_COLOR)
     bg_draw = ImageDraw.Draw(bg)
 
     # 圆形遮罩
     circle_mask = Image.new("RGBA", (250, 250), "#ffffff00")
     ImageDraw.Draw(circle_mask).ellipse((0, 0, 250, 250), fill="black")
@@ -136,39 +90,31 @@
         valign="bottom",
         fontname=FONT_PATH,
     )
 
     # 详细信息
     bg_draw.multiline_text(
         (300, 160),
-        f"Bot已连接 {bot_connected} | 收 {msg_rec} | 发 {msg_sent}\nNoneBot运行 {nb_run} | 系统运行 {booted}",
+        (
+            f"Bot已连接 {bot_connected} | 收 {msg_rec} | 发 {msg_sent}\n"
+            f"NoneBot运行 {nb_run} | 系统运行 {booted}"
+        ),
         "black",
         font_30,
     )
 
     # 标题与详细信息的分隔线
     bg_draw.line((300, 150, 500, 150), GRAY_BG_COLOR, 3)
 
     return bg
 
 
-async def draw_cpu_memory_usage():
+async def draw_cpu_memory_usage(data: CpuMemoryStat) -> Image.Image:
     # 获取占用信息
-    psutil.cpu_percent()
-    await asyncio.sleep(0.1)
-    cpu_percent = psutil.cpu_percent()  # async wait
-
-    cpu_count = psutil.cpu_count(logical=False)
-    cpu_count_logical = psutil.cpu_count()
-    cpu_freq = psutil.cpu_freq()
-    ram_stat = psutil.virtual_memory()
-    swap_stat = psutil.swap_memory()
-
-    font_70 = get_font(70)
-    font_25 = get_font(25)
+    cpu_percent, cpu_count, cpu_logical_count, cpu_freq, ram_stat, swap_stat = data
 
     bg = Image.new("RGBA", (1200, 550), WHITE_BG_COLOR)
     bg_draw = ImageDraw.Draw(bg)
 
     # 背景灰色圆环
     circle_bg = Image.new("RGBA", (300, 300), "#ffffff00")
     ImageDraw.Draw(circle_bg).arc((0, 0, 300, 300), 0, 360, GRAY_BG_COLOR, 30)
@@ -213,37 +159,24 @@
         "black",
         font_70,
         "mm",
     )
 
     # 写详细信息
     # CPU
-    try:
-        if cpu_freq.max == 0:
-            if cpu_freq.current == 0:
-                freq_t = "主频未知"
-            else:
-                freq_t = f"当前 {cpu_freq.current:.0f}MHz"
-        elif cpu_freq.max == cpu_freq.current:
-            freq_t = f"最大 {cpu_freq.max:.0f}MHz"
-        else:
-            freq_t = f"{cpu_freq.current:.0f}MHz / {cpu_freq.max:.0f}MHz"
-    except AttributeError:
-        freq_t = "主频未知"
-
     bg_draw.text(
         (200, 470),
-        f"{cpu_count}核 {cpu_count_logical}线程",
+        f"{cpu_count}核 {cpu_logical_count}线程",
         "darkslategray",
         font_25,
         "ms",
     )
     bg_draw.text(
         (200, 500),
-        freq_t,
+        format_freq_txt(cpu_freq),
         "darkslategray",
         font_25,
         "ms",
     )
 
     # RAM
     bg_draw.text(
@@ -284,98 +217,46 @@
         font_25,
         "ms",
     )
 
     return bg
 
 
-async def draw_disk_usage():
-    disks = {}
-    io_rw = {}
-    left_padding = 0
-
-    font_45 = get_font(45)
-    font_40 = get_font(40)
-
-    async def get_disk_usage():
-        """获取磁盘占用，返回左边距"""
-        nonlocal left_padding
-
-        # 获取磁盘状态
-        for _d in psutil.disk_partitions():
-            # 忽略分区
-            if _r := match_list_regexp(config.ps_ignore_parts, _d.mountpoint):
-                logger.info(f"空间读取 分区 {_d.mountpoint} 匹配 {_r.re.pattern}，忽略")
-                continue
-
-            display_text = process_text_len(_d.mountpoint)
-            # 根据盘符长度计算左侧留空长度用于写字
-            s = font_45.getlength(display_text) + 25
-            if s > left_padding:
-                left_padding = s
-
-            try:
-                disks[display_text] = psutil.disk_usage(_d.mountpoint)
-            except Exception as e:
-                logger.exception(f"读取 {_d.mountpoint} 占用失败")
-                if not config.ps_ignore_bad_parts:
-                    disks[display_text] = e
-
-    async def get_disk_io():
-        """获取磁盘IO"""
-        io1: Dict[str, sdiskio] = psutil.disk_io_counters(True)
-        await asyncio.sleep(1)
-        io2: Dict[str, sdiskio] = psutil.disk_io_counters(True)
-
-        for _k, _v in io1.items():
-            # 忽略分区
-            if _r := match_list_regexp(config.ps_ignore_disk_ios, _k):
-                logger.info(f"IO统计 磁盘 {_k} 匹配 {_r.re.pattern}，忽略")
-                continue
-
-            _k = process_text_len(_k)
-            _r = io2[_k].read_bytes - _v.read_bytes
-            _w = io2[_k].write_bytes - _v.write_bytes
-
-            if _r == 0 and _w == 0 and config.ps_ignore_no_io_disk:
-                logger.info(f"IO统计 忽略无IO磁盘 {_k}")
-                continue
-
-            io_rw[_k] = (format_byte_count(_r), format_byte_count(_w))
-
-    await asyncio.gather(get_disk_usage(), get_disk_io())
+async def draw_disk_usage(data: DiskStatus) -> Optional[Image.Image]:
+    disk_usage, disk_io = data
 
     # 列表为空直接返回
-    if not (disks or io_rw):
+    if not (disk_usage and disk_io):
         return None
 
     # 计算图片高度，创建背景图
-    count = len(disks) + len(io_rw)
+    left_padding = max((font_45.getlength(x.name) + 25) for x in disk_usage)
+    count = len(disk_usage) + len(disk_io)
     bg = Image.new(
         "RGBA",
         (
             1200,
             100  # 上下边距
             + (50 * count)  # 每行磁盘/IO统计
             + (25 * (count - 1))  # 间隔
-            + (10 if disks and io_rw else 0),  # 磁盘统计与IO统计间的间距
+            + (10 if disk_usage and disk_io else 0),  # 磁盘统计与IO统计间的间距
         ),
         WHITE_BG_COLOR,
     )
     bg_draw = ImageDraw.Draw(bg)
 
     top = 50
 
     # 画分区占用列表
-    if disks:
+    if disk_usage:
         max_len = 990 - (50 + left_padding)  # 进度条长度
 
-        its = cast(List[Tuple[str, Union[sdiskusage, Exception]]], disks.items())
-        for name, usage in its:
-            fail = isinstance(usage, Exception)
+        for usage in disk_usage:
+            name = usage.name
+            fail = isinstance(usage, DiskUsageWithExc)
 
             # 进度条背景
             bg_draw.rectangle((50 + left_padding, top, 990, top + 50), GRAY_BG_COLOR)
 
             # 写盘符
             bg_draw.text((50, top + 25), name, "black", font_45, "lm")
 
@@ -412,87 +293,40 @@
                 font_40,
                 "mm",
             )
 
             top += 75
 
     # 写IO统计
-    if io_rw:
-        if disks:
+    if disk_io:
+        if disk_usage:
             # 分隔线 25+10px
             top += 10
             bg_draw.rectangle((50, top - 17, 1150, top - 15), GRAY_BG_COLOR)
 
-        for k, (r, w) in io_rw.items():
-            bg_draw.text((50, top + 25), k, "black", font_45, "lm")
-            bg_draw.text((1150, top + 25), f"读 {r}/s | 写 {w}/s", "black", font_45, "rm")
+        for name, read, write in disk_io:
+            bg_draw.text((50, top + 25), name, "black", font_45, "lm")
+            bg_draw.text(
+                (1150, top + 25),
+                f"读 {format_byte_count(read)}/s | 写 {format_byte_count(write)}/s",
+                "black",
+                font_45,
+                "rm",
+            )
             top += 75
 
     return bg
 
 
-async def draw_net_io():
-    ios = {}
-    connections: List[Tuple[str, Union[Tuple[int, float], Exception]]] = []
-
-    async def get_net_io():
-        """网络IO"""
-
-        io1: Dict[str, snetio] = psutil.net_io_counters(True)
-        await asyncio.sleep(1)
-        io2: Dict[str, snetio] = psutil.net_io_counters(True)
-
-        for k_, v in io1.items():
-            if r := match_list_regexp(config.ps_ignore_nets, k_):
-                logger.info(f"网卡 {k_} 匹配 {r.re.pattern}，忽略")
-                continue
-
-            u_ = io2[k_].bytes_sent - v.bytes_sent
-            d_ = io2[k_].bytes_recv - v.bytes_recv
-
-            if u_ == 0 and d_ == 0 and config.ps_ignore_0b_net:
-                logger.info(f"网卡 {k_} 上下行0B，忽略")
-                continue
-
-            k_ = process_text_len(k_)
-            ios[k_] = (format_byte_count(u_), format_byte_count(d_))
-
-    async def get_net_connection():
-        """网络连通性"""
-
-        tested_conn: Dict[str, Union[Tuple[int, float], Exception]] = {}
-
-        async def get_result(site: TestSiteCfg):
-            try:
-                async with AsyncClient(
-                    timeout=config.ps_test_timeout,
-                    proxies=config.proxy if site.use_proxy else None,
-                    follow_redirects=True,
-                ) as c:
-                    time1 = time.time()
-                    r = await c.get(site.url)
-                    time2 = time.time() - time1
-                    tested_conn[site.name] = (r.status_code, time2 * 1000)
-
-            except Exception as e:
-                logger.error(f"网页 {site.name}({site.url}) 访问失败: {e!r}")
-                tested_conn[site.name] = e
-
-        await asyncio.gather(*[get_result(x) for x in config.ps_test_sites])
-        connections.extend(
-            [(x.name, tested_conn[x.name]) for x in config.ps_test_sites],
-        )
-
-    await asyncio.gather(get_net_io(), get_net_connection())
+async def draw_net_io(data: NetworkStatus) -> Optional[Image.Image]:
+    ios, connections = data
 
     if not (ios and connections):
         return None
 
-    font_45 = get_font(45)
-
     # 计算图片高度并新建图片
     count = len(ios) + len(connections)
     bg = Image.new(
         "RGBA",
         (
             1200,
             100  # 上下边距
@@ -503,59 +337,87 @@
         WHITE_BG_COLOR,
     )
     draw = ImageDraw.Draw(bg)
 
     # 写字
     top = 50
     if ios:
-        for k, (u, d) in ios.items():
-            draw.text((50, top + 25), k, "black", font_45, "lm")
-            draw.text((1150, top + 25), f"↑ {u}/s | ↓ {d}/s", "black", font_45, "rm")
+        for name, sent, recv in ios:
+            draw.text((50, top + 25), name, "black", font_45, "lm")
+            draw.text(
+                (1150, top + 25),
+                f"↑ {format_byte_count(sent)}/s | ↓ {format_byte_count(recv)}/s",
+                "black",
+                font_45,
+                "rm",
+            )
             top += 75
 
     if connections:
         if ios:
             # 分隔线 25+10px
             top += 10
             draw.rectangle((50, top - 17, 1150, top - 15), GRAY_BG_COLOR)
 
-        for k, v in connections:
-            if isinstance(v, Exception):
-                if isinstance(v, httpx.ReadTimeout):
-                    tip = "超时"
-                # elif isinstance(v, ClientConnectorError):
-                #     tip = f"[{v.os_error.errno}] {v.os_error.strerror}"
-                else:
-                    tip = v.__class__.__name__
+        for conn in connections:
+            name = conn.name
+            if isinstance(conn, NetworkConnectionError):
+                tip = conn.error
             else:
-                code, latency = v
-                tip = str(code)
-                if code == 200:
-                    tip += f" | {latency:.2f}ms"
+                _, code, reason, latency = conn
+                tip = f"{code} {reason}"
+                tip = f"{tip} | {latency:.2f}ms" if code == 200 else tip
 
-            draw.text((50, top + 25), k, "black", font_45, "lm")
+            draw.text((50, top + 25), name, "black", font_45, "lm")
             draw.text((1150, top + 25), tip, "black", font_45, "rm")
             top += 75
 
     return bg
 
 
-async def draw_footer(img: Image.Image):
-    font_footer = get_font(config.ps_footer_size)
+async def draw_process_status(data: List[ProcessStatus]) -> Optional[Image.Image]:
+    if not data:
+        return None
+
+    # 计算图片高度并新建图片
+    count = len(data)
+    bg = Image.new(
+        "RGBA",
+        (1200, 100 + (50 * count) + (25 * (count - 1))),  # 高：上下边距 + 每行 + 间隔
+        WHITE_BG_COLOR,
+    )
+    draw = ImageDraw.Draw(bg)
+
+    offset = 50
+    for name, cpu, mem in data:
+        draw.text((50, offset + 25), name, "black", font_45, "lm")
+        draw.text(
+            (1150, offset + 25),
+            f"CPU {cpu:.2f}% | MEM {format_byte_count(mem)}",
+            "black",
+            font_45,
+            "rm",
+        )
+        offset += 75
+
+    return bg
+
+
+async def draw_footer(img: Image.Image, time_str: str):
     draw = ImageDraw.Draw(img)
     w, h = img.size
     padding = 15
 
     draw.text(
-        (img.size[0] / 2, h - padding),
+        (w / 2, h - padding),
         (
             f"NoneBot {nonebot.__version__} × PicStatus {__version__} | "
             f"{platform.python_implementation()} {platform.python_version()} | "
             f"{await get_system_name()} | "
-            f"{time.strftime('%Y-%m-%d %H:%M:%S')}"
+            f"{time_str}"
         ),
         "darkslategray",
         font_footer,
         "ms",
     )
 
 
@@ -587,26 +449,40 @@
     return await async_open_img(DEFAULT_BG_PATH)
 
 
 async def get_stat_pic(bot: Bot, bg_arg: Optional[bytes] = None) -> bytes:
     img_w = 1300
     img_h = 50  # 这里是上边距，留给下面代码统计图片高度
 
+    (
+        header_data,
+        cpu_memory_usage,
+        disk_stat,
+        net_stat,
+        proc_stat,
+    ) = await asyncio.gather(
+        get_header_data(bot),
+        get_cpu_memory_usage(),
+        get_disk_status(),
+        get_network_status(),
+        get_process_status(),
+    )
+    now_time = time.strftime("%Y-%m-%d %H:%M:%S")
+
     # 获取背景及各模块图片
-    ret = cast(
-        List[Optional[Image.Image]],
-        await asyncio.gather(
-            get_bg(bg_arg),
-            draw_header(bot),
-            draw_cpu_memory_usage(),
-            draw_disk_usage(),
-            draw_net_io(),
-        ),
+    ret = await asyncio.gather(
+        get_bg(bg_arg),
+        draw_header(header_data),
+        draw_cpu_memory_usage(cpu_memory_usage),
+        draw_disk_usage(disk_stat),
+        draw_net_io(net_stat),
+        draw_process_status(proc_stat),
     )
-    bg = cast(Image.Image, ret[0])
+
+    bg = ret[0]
     ret = ret[1:]
 
     # 统计图片高度
     for p in ret:
         if p:
             img_h += p.size[1] + 50
 
@@ -641,15 +517,15 @@
     h_pos = 50
     for p in ret:
         if p:
             bg.paste(p, (50, h_pos), p)
             h_pos += p.size[1] + 50
 
     # 写footer
-    await draw_footer(bg)
+    await draw_footer(bg, now_time)
 
     # 尝试解决黑底白底颜色不同问题
     bg = bg.convert("RGB")
 
     bio = BytesIO()
     bg.save(bio, "jpeg")
     return bio.getvalue()
```

### Comparing `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/res/default_avatar.png` & `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/res/default_avatar.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/res/default_bg.png` & `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/res/default_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/statistics.py` & `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/statistics.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 async def called_api(bot: Bot, exc: Optional[Exception], api: str, _, __):
     if (not exc) and method_is_send_msg(bot.adapter.get_name(), api):
         num = send_num.get(bot.self_id, 0)
         send_num[bot.self_id] = num + 1
 
 
-async def not_ob_v11_bot_rule(bot: Bot):
+async def not_ob_v11_bot_rule(bot: Bot) -> bool:
     return not (OneBotV11Bot and isinstance(bot, OneBotV11Bot))
 
 
 @driver.on_bot_connect
 async def _(bot: Bot):
     bot_id = bot.self_id
     bot_connect_time[bot_id] = datetime.now()
```

### Comparing `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/util.py` & `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
-import platform
 import re
 from datetime import timedelta
 from io import BytesIO
-from typing import Literal, Optional, cast, overload
+from typing import List, Literal, Optional, cast, overload
 
 import anyio
 from httpx import AsyncClient
 from nonebot import logger
 from nonebot.internal.adapter import Bot
 from PIL import Image
 
@@ -64,67 +63,43 @@
         follow_redirects=True,
         timeout=config.ps_req_timeout,
     ) as cli:
         res = await cli.get(url, *args, **kwargs)
         return res.text if is_text else res.content
 
 
-async def get_anime_pic():
+async def get_anime_pic() -> bytes:
     data = json.loads(
         await async_request("https://api.gumengya.com/Api/DmImg", is_text=True),
     )
     assert str(data.get("code")) == "200"
     return await async_request(data["data"]["url"])
 
 
-async def get_qq_avatar(qq):
+async def get_qq_avatar(qq) -> bytes:
     return await async_request(f"https://q2.qlogo.cn/headimg_dl?dst_uin={qq}&spec=640")
 
 
 async def async_open_img(fp, *args, **kwargs) -> Image.Image:
     async with (await anyio.open_file(fp, "rb")) as f:
         p = BytesIO(await f.read())
     return Image.open(p, *args, **kwargs)
 
 
-async def get_system_name():
-    system, _, release, version, machine, _ = platform.uname()
-    system, release, version = platform.system_alias(system, release, version)
-
-    if system == "Java":
-        _, _, _, (system, release, machine) = platform.java_ver()
-
-    if system == "Darwin":
-        return f"MacOS {platform.mac_ver()[0]} {machine}"
-    if system == "Windows":
-        return f"Windows {release} {platform.win32_edition()} {machine}"
-    if system == "Linux":
-        try:
-            v = await anyio.Path("/etc/issue").read_text()
-        except:
-            logger.exception("读取 /etc/issue 文件失败")
-            v = f"未知Linux {release}"
-        else:
-            v = v.replace(r"\n", "").replace(r"\l", "").strip()
-        return f"{v} {machine}"
-
-    return f"{system} {release}"
-
-
-def format_byte_count(b: int):
+def format_byte_count(b: int) -> str:
     if (k := b / 1024) < 1:
         return f"{b}B"
     if (m := k / 1024) < 1:
         return f"{k:.2f}K"
     if (g := m / 1024) < 1:
         return f"{m:.2f}M"
     return f"{g:.2f}G"
 
 
-def match_list_regexp(reg_list, txt):
+def match_list_regexp(reg_list: List[str], txt: str) -> Optional[re.Match]:
     for r in reg_list:
         if m := re.search(r, txt):
             return m
     return None
 
 
 def process_text_len(text: str) -> str:
```

### Comparing `nonebot_plugin_picstatus-0.4.2/pyproject.toml` & `nonebot_plugin_picstatus-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-picstatus"
-version = "0.4.2"
+version = "0.5.0"
 description = "A NoneBot2 plugin generates a picture which shows the status of current device"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "Pillow<10.0.0,>=9.2.0",
     "psutil<6.0.0,>=5.9.2",
```

### Comparing `nonebot_plugin_picstatus-0.4.2/PKG-INFO` & `nonebot_plugin_picstatus-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-picstatus
-Version: 0.4.2
+Version: 0.5.0
 Summary: A NoneBot2 plugin generates a picture which shows the status of current device
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus
 Requires-Python: <4.0,>=3.8
 Requires-Dist: Pillow<10.0.0,>=9.2.0
@@ -55,72 +55,78 @@
 不多说，直接看图！
 
 ### 效果图
 
 <details>
   <summary>点击展开</summary>
 
-![example](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/picstatus/example.png)
+![example](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/picstatus/example.jpg)
 
 </details>
 
 ## 💿 安装
 
+以下提到的方法 任选**其一** 即可
+
 <details open>
 <summary>[推荐] 使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
-    nb plugin install nonebot-plugin-picstatus
+```bash
+nb plugin install nonebot-plugin-picstatus
+```
 
 </details>
 
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
 
-    pip install nonebot-plugin-picstatus
+```bash
+pip install nonebot-plugin-picstatus
+```
 
 </details>
 <details>
 <summary>pdm</summary>
 
-    pdm add nonebot-plugin-picstatus
+```bash
+pdm add nonebot-plugin-picstatus
+```
 
 </details>
 <details>
 <summary>poetry</summary>
 
-    poetry add nonebot-plugin-picstatus
+```bash
+poetry add nonebot-plugin-picstatus
+```
 
 </details>
 <details>
 <summary>conda</summary>
 
-    conda install nonebot-plugin-picstatus
-
-</details>
-
-打开 nonebot2 项目的 `bot.py` 文件, 在其中写入
-
-    nonebot.load_plugin('nonebot_plugin_picstatus')
+```bash
+conda install nonebot-plugin-picstatus
+```
 
 </details>
 
-<details>
-<summary>从 github 安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 输入以下命令克隆此储存库
-
-    git clone https://github.com/lgc2333/nonebot-plugin-picstatus.git
-
-打开 nonebot2 项目的 `bot.py` 文件, 在其中写入
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分的 `plugins` 项里追加写入
 
-    nonebot.load_plugin('src.plugins.nonebot_plugin_picstatus')
+```toml
+[tool.nonebot]
+plugins = [
+    # ...
+    "nonebot_plugin_picstatus"
+]
+```
 
 </details>
 
 ## ⚙️ 配置
 
 见[.env.example](https://github.com/lgc2333/nonebot-plugin-picstatus/blob/master/.env.example)
 
@@ -157,14 +163,21 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.5.0
+
+- 先获取状态信息再进行画图，可以获取到更精准的状态信息
+- 添加进程占用信息的展示
+- 测试网站结果状态码后面会带上 `reason`，如 `200 OK` / `404 Not Found`
+- 添加了一些配置项（`PS_SORT_PARTS`, `PS_SORT_PARTS_REVERSE`, `PS_SORT_DISK_IOS`, `PS_SORT_NETS`, `PS_SORT_SITES`, `PS_PROC_LEN`, `PS_IGNORE_PROCS`, `PS_PROC_SORT_BY`, `PS_PROC_CPU_MAX_100P`, `PS_REPLY_TARGET`, `PS_TG_MAX_FILE_SIZE`）
+
 ### 0.4.2
 
 - 添加配置项 `PS_REQ_TIMEOUT` ([#25](https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus/issues/25))
 
 ### 0.4.1
 
 - 现在默认使用 `pil_utils` 自动选择系统内支持中文的字体，删除插件内置字体
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-picstatus Version: 0.4.2 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-picstatus Version: 0.5.0 Summary: A
 NoneBot2 plugin generates a picture which shows the status of current device
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus Author-Email:
 student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-picstatus Requires-Python: <4.0,>=3.8 Requires-Dist:
 Pillow<10.0.0,>=9.2.0 Requires-Dist: psutil<6.0.0,>=5.9.2 Requires-Dist:
 nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
@@ -10,41 +10,47 @@
 utils>=0.1.7 Description-Content-Type: text/markdown
                                     [logo]
                                     [logo]
    # NoneBot-Plugin-PicStatus _â¨ è¿è¡ç¶æå¾çç for NoneBot2 â¨_
              [license] [pypi] [python] [pypi_download] [wakatime]
 ## ð ä»ç» ä¸å¤è¯´ï¼ç´æ¥çå¾ï¼ ### ææå¾  ç¹å»å±å¼ !
 [example](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/picstatus/
-example.png)  ## ð¿ å®è£  [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-picstatus   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot-plugin-picstatus   pdm pdm
-add nonebot-plugin-picstatus   poetry poetry add nonebot-plugin-picstatus
-conda conda install nonebot-plugin-picstatus  æå¼ nonebot2 é¡¹ç®ç
-`bot.py` æä»¶, å¨å¶ä¸­åå¥ nonebot.load_plugin
-('nonebot_plugin_picstatus')   ä» github å®è£ å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸å½ä»¤åéæ­¤å¨å­åº
-git clone https://github.com/lgc2333/nonebot-plugin-picstatus.git æå¼
-nonebot2 é¡¹ç®ç `bot.py` æä»¶, å¨å¶ä¸­åå¥ nonebot.load_plugin
-('src.plugins.nonebot_plugin_picstatus')  ## âï¸ éç½® è§[.env.example]
-(https://github.com/lgc2333/nonebot-plugin-picstatus/blob/master/.env.example)
-## ð ä½¿ç¨ ä½¿ç¨æä»¤`è¿è¡ç¶æ`ï¼æè`ç¶æ` / `zt` / `yxzt` /
+example.jpg)  ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯
+[æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
+plugin install nonebot-plugin-picstatus ```   ä½¿ç¨åç®¡çå¨å®è£ å¨
+nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
+install nonebot-plugin-picstatus ```   pdm ```bash pdm add nonebot-plugin-
+picstatus ```   poetry ```bash poetry add nonebot-plugin-picstatus ```   conda
+```bash conda install nonebot-plugin-picstatus ```  æå¼ nonebot2
+é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
+`plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
+"nonebot_plugin_picstatus" ] ```  ## âï¸ éç½® è§[.env.example](https://
+github.com/lgc2333/nonebot-plugin-picstatus/blob/master/.env.example) ## ð
+ä½¿ç¨ ä½¿ç¨æä»¤`è¿è¡ç¶æ`ï¼æè`ç¶æ` / `zt` / `yxzt` /
 `status`ï¼æ¥è§¦åæä»¶åè½
 å¯ä»¥å¨æ¶æ¯åé¢è·ä¸å¼ å¾çæèåå¤ä¸å¼ å¾çæ¥èªå®ä¹èæ¯å¾ï¼é»è®¤ä¸ºéæºèæ¯å¾
 æ´å¤èªå®ä¹é¡¹åè§ [éç½®](#ï¸-éç½®) ## ð èç³» QQï¼3076823485
 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://
 jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [ææ¢¦ API](https://api.gumengya.com) -
 éæºèæ¯å¾æ¥æº ### [LoliApi](https://docs.loliapi.com/) -
 éæºèæ¯å¾æ¥æºï¼ææ¶å¼ç¨ï¼ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.4.2 - æ·»å éç½®é¡¹
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.5.0 -
+åè·åç¶æä¿¡æ¯åè¿è¡ç»å¾ï¼å¯ä»¥è·åå°æ´ç²¾åçç¶æä¿¡æ¯
+- æ·»å è¿ç¨å ç¨ä¿¡æ¯çå±ç¤º -
+æµè¯ç½ç«ç»æç¶æç åé¢ä¼å¸¦ä¸ `reason`ï¼å¦ `200 OK` / `404 Not
+Found` - æ·»å äºä¸äºéç½®é¡¹ï¼`PS_SORT_PARTS`, `PS_SORT_PARTS_REVERSE`,
+`PS_SORT_DISK_IOS`, `PS_SORT_NETS`, `PS_SORT_SITES`, `PS_PROC_LEN`,
+`PS_IGNORE_PROCS`, `PS_PROC_SORT_BY`, `PS_PROC_CPU_MAX_100P`,
+`PS_REPLY_TARGET`, `PS_TG_MAX_FILE_SIZE`ï¼ ### 0.4.2 - æ·»å éç½®é¡¹
 `PS_REQ_TIMEOUT` ([#25](https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus/
 issues/25)) ### 0.4.1 - ç°å¨é»è®¤ä½¿ç¨ `pil_utils`
 èªå¨éæ©ç³»ç»åæ¯æä¸­æçå­ä½ï¼å é¤æä»¶åç½®å­ä½ - ä½¿ç¨
 `pil_utils` å Bot æµç§°ï¼å¯ä»¥æ¾ç¤º Emoji ç­ç¹æ®å­ç¬¦ -
 æµè¯ç½ç«åºéæ¶ä¸ä¼å¾æ¥å¿éç©éè¯¯å æ äº ### 0.4.0 - ä½¿ç¨
 [nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-
 plugin-send-anything-anywhere) å¼å®¹å¤å¹³å°åéï¼å¹¶å¯¹ OneBot V11 å
```

