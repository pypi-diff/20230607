# Comparing `tmp/nonebot_plugin_bilichat-2.4.0.tar.gz` & `tmp/nonebot_plugin_bilichat-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.4.0.tar", last modified: Tue Jun  6 06:36:35 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.4.1.tar", last modified: Wed Jun  7 08:38:33 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.4.0.tar` & `nonebot_plugin_bilichat-2.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-06-06 06:36:19.199038 nonebot_plugin_bilichat-2.4.0/LICENSE
--rw-r--r--   0        0        0    12555 2023-06-06 06:36:19.199038 nonebot_plugin_bilichat-2.4.0/README.md
--rw-r--r--   0        0        0     8870 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4882 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6439 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1363 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5904 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2343 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-06 06:36:19.207038 nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1499 2023-06-06 06:36:35.352341 nonebot_plugin_bilichat-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    13996 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-07 08:38:24.283974 nonebot_plugin_bilichat-2.4.1/LICENSE
+-rw-r--r--   0        0        0    12555 2023-06-07 08:38:24.283974 nonebot_plugin_bilichat-2.4.1/README.md
+-rw-r--r--   0        0        0     8790 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4914 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6439 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3812 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1363 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5904 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2363 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1499 2023-06-07 08:38:33.092092 nonebot_plugin_bilichat-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0    13996 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.4.0/LICENSE` & `nonebot_plugin_bilichat-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/README.md` & `nonebot_plugin_bilichat-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     event: MESSAGE_EVENT,
     state: T_State,
     matcher: Matcher,
     options: Options = Depends(get_args),
 ):
     # sourcery skip: raise-from-previous-error, use-fstring-for-concatenation
     DISABLE_REPLY = isinstance(bot, Mirai_Bot)  # 部分平台Reply暂不可用
-    DISABLE_LINK = isinstance(bot, QG_Bot) and plugin_config.bilichat_basic_info_url  # 部分平台发送链接都要审核
+    DISABLE_LINK = isinstance(bot, QG_Bot) or not plugin_config.bilichat_basic_info_url  # 部分平台发送链接都要审核
     SEND_IMAGE_SEPARATELY = isinstance(bot, QG_Bot)  # 部分平台无法一次性发送多张图片，或无法与其他消息组合发出
     reply = "" if DISABLE_REPLY else await SegmentBuilder.reply()
     # basic info
     bili_number, uid = state["bili_number"], state["_uid_"]
     if bili_number[:2] in ["BV", "bv", "av"]:
         msg, img, info = await get_video_basic(bili_number, uid)
         if not msg or not info:
@@ -206,34 +206,30 @@
         raise FinishedException
 
     # wordcloud
     wc_image = ""
     if plugin_config.bilichat_word_cloud:
         if image := await wordcloud(cache=cache, cid=str(info.cid)):
             wc_image = await SegmentBuilder.image(image=image)
+            if SEND_IMAGE_SEPARATELY:
+                await matcher.send(wc_image)
         else:
             if plugin_config.bilichat_show_error_msg:
                 await matcher.finish(reply + "视频无有效字幕")
             raise FinishedException
 
     # summary
     summary = ""
     if ENABLE_SUMMARY:
         if summary := await summarization(cache=cache, cid=str(info.cid)):
+            # if summary is image
             if isinstance(summary, bytes):
                 summary = await SegmentBuilder.image(image=summary)
+            if SEND_IMAGE_SEPARATELY:
+                await matcher.finish(summary)
         else:
             if plugin_config.bilichat_show_error_msg:
                 await matcher.finish(reply + "视频无有效字幕")
             raise FinishedException
 
-    if wc_image:
-        if SEND_IMAGE_SEPARATELY:
-            await matcher.send(wc_image)
-            if summary:
-                await matcher.finish(summary)
-        await matcher.finish(reply + wc_image + summary)  # type: ignore
-
-    elif summary:
-        if SEND_IMAGE_SEPARATELY:
-            await matcher.finish(summary)
-        await matcher.finish(reply + wc_image + summary)  # type: ignore
+    if (not SEND_IMAGE_SEPARATELY) and (wc_image or summary):
+        await matcher.finish(reply + wc_image + summary)
```

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,20 +51,20 @@
     bilichat_newbing_token_limit: int = 0
     bilichat_newbing_preprocess: bool = True
     bilichat_openai_token: Optional[str]
     bilichat_openai_proxy: Optional[str]
     bilichat_openai_model: Literal["gpt-3.5-turbo-0301", "gpt-4-0314", "gpt-4-32k-0314"] = "gpt-3.5-turbo-0301"
     bilichat_openai_token_limit: int = 3500
 
-    @validator("bilichat_openai_proxy")
+    @validator("bilichat_openai_proxy",always=True,pre=True)
     def check_openai_proxy(cls, v, values):
         if not (values["bilichat_openai_token"] or values["bilichat_newbing_cookie"]):
             return v
         if v is None:
-            logger.warning("you have enabled openai summary without a proxy, this may cause request failure.")
+            logger.warning("you have enabled openai or newbing summary without a proxy, this may cause request failure.")
         return v
 
     @validator("bilichat_openai_token_limit")
     def check_token_limit(cls, v, values):
         if values["bilichat_openai_token"] is None:
             return v
         if not isinstance(v, int):
```

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     try:
         loop = asyncio.get_event_loop()
         if loop.is_closed():
             raise RuntimeError
     except RuntimeError:
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
-    return asyncio.run(get_font(font))
+    return loop.run_until_complete(get_font(font))
 
 
 def font_init():
     font_url = (
         "https://mirrors.bfsu.edu.cn/pypi/web/packages/ad/97/"
         "03cd0a15291c6c193260d97586c4adf37a7277d8ae4507d68566c5757a6a/"
         "bbot_fonts-0.1.1-py3-none-any.whl"
```

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 raise ValueError(f"Illegal Video(Column) types {cache.id}")
 
             if ai_summary.response:
                 cache.episodes[cid].openai = ai_summary.response
                 cache.save()
             else:
                 logger.warning(f"Video(Column) {cache.id} summary failure: {ai_summary.raw}")
-                return f"视频(专栏) {cache.id} 总结失败: {ai_summary.raw}"
+                return f"视频(专栏) {cache.id} 总结失败: 响应内容异常\n{ai_summary.raw}"
         if img := await rich_text2image(cache.episodes[cid].openai or "视频无法总结", plugin_config.bilichat_openai_model):
             return img
         else:
             return f"总结图片生成失败, 直接发送原文:\n{cache.episodes[cid].openai}"
     except AbortError as e:
         logger.exception(f"Video(Column) {cache.id} summary aborted: {e}")
         return f"视频(专栏) {cache.id} 总结中止: {e}"
```

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.0/pyproject.toml` & `nonebot_plugin_bilichat-2.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.4.0"
+version = "2.4.1"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
```

### Comparing `nonebot_plugin_bilichat-2.4.0/PKG-INFO` & `nonebot_plugin_bilichat-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.4.0
+Version: 2.4.1
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.4.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.4.1 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
```

