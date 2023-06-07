# Comparing `tmp/cf_clearance-0.29.0.tar.gz` & `tmp/cf_clearance-0.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_clearance-0.29.0.tar", max compression
+gzip compressed data, was "cf_clearance-0.29.1.tar", last modified: Wed Jun  7 07:16:06 2023, max compression
```

## Comparing `cf_clearance-0.29.0.tar` & `cf_clearance-0.29.1.tar`

### file list

```diff
@@ -1,16 +1,21 @@
--rw-r--r--   0        0        0    11357 2022-05-30 06:44:14.187456 cf_clearance-0.29.0/LICENSE
--rw-r--r--   0        0        0     5445 2023-02-27 05:47:54.327147 cf_clearance-0.29.0/README.md
--rw-r--r--   0        0        0      281 2023-02-28 06:06:57.347421 cf_clearance-0.29.0/cf_clearance/__init__.py
--rw-r--r--   0        0        0      118 2022-11-28 03:39:27.925358 cf_clearance-0.29.0/cf_clearance/errors.py
--rw-r--r--   0        0        0     1268 2022-11-28 03:39:27.925709 cf_clearance-0.29.0/cf_clearance/js/canvas.fingerprinting.js
--rw-r--r--   0        0        0     1846 2022-11-28 03:39:27.926018 cf_clearance-0.29.0/cf_clearance/js/chrome.global.js
--rw-r--r--   0        0        0     5662 2023-02-24 07:20:56.351353 cf_clearance-0.29.0/cf_clearance/js/chrome.plugin.js
--rw-r--r--   0        0        0     3575 2022-11-23 06:25:21.108178 cf_clearance-0.29.0/cf_clearance/js/chrome.runtime.js
--rw-r--r--   0        0        0       74 2022-11-28 03:39:27.926735 cf_clearance-0.29.0/cf_clearance/js/emulate.touch.js
--rw-r--r--   0        0        0     1083 2022-11-28 03:39:27.927066 cf_clearance-0.29.0/cf_clearance/js/navigator.permissions.js
--rw-r--r--   0        0        0      489 2022-12-07 10:09:49.695721 cf_clearance-0.29.0/cf_clearance/js/navigator.webdriver.js
--rw-r--r--   0        0        0     1976 2023-02-24 07:59:19.092068 cf_clearance-0.29.0/cf_clearance/retry.py
--rw-r--r--   0        0        0     3678 2022-11-28 03:39:27.927929 cf_clearance-0.29.0/cf_clearance/stealth.py
--rw-r--r--   0        0        0      684 2023-02-28 06:05:46.050717 cf_clearance-0.29.0/pyproject.toml
--rw-r--r--   0        0        0     6479 2023-02-28 06:07:07.170951 cf_clearance-0.29.0/setup.py
--rw-r--r--   0        0        0     6217 2023-02-28 06:07:07.171478 cf_clearance-0.29.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-05-30 06:44:14.187456 cf_clearance-0.29.1/LICENSE
+-rw-r--r--   0        0        0     5689 2023-06-05 08:24:29.062628 cf_clearance-0.29.1/README.md
+-rw-r--r--   0        0        0     6148 2022-05-30 06:47:41.987971 cf_clearance-0.29.1/cf_clearance/.DS_Store
+-rw-r--r--   0        0        0      281 2023-06-07 07:14:13.027584 cf_clearance-0.29.1/cf_clearance/__init__.py
+-rw-r--r--   0        0        0      118 2022-11-28 03:39:27.925358 cf_clearance-0.29.1/cf_clearance/errors.py
+-rw-r--r--   0        0        0     1268 2022-11-28 03:39:27.925709 cf_clearance-0.29.1/cf_clearance/js/canvas.fingerprinting.js
+-rw-r--r--   0        0        0     1846 2022-11-28 03:39:27.926018 cf_clearance-0.29.1/cf_clearance/js/chrome.global.js
+-rw-r--r--   0        0        0     5662 2023-02-24 07:20:56.351353 cf_clearance-0.29.1/cf_clearance/js/chrome.plugin.js
+-rw-r--r--   0        0        0     3575 2022-11-23 06:25:21.108178 cf_clearance-0.29.1/cf_clearance/js/chrome.runtime.js
+-rw-r--r--   0        0        0       74 2022-11-28 03:39:27.926735 cf_clearance-0.29.1/cf_clearance/js/emulate.touch.js
+-rw-r--r--   0        0        0     1083 2022-11-28 03:39:27.927066 cf_clearance-0.29.1/cf_clearance/js/navigator.permissions.js
+-rw-r--r--   0        0        0      489 2022-12-07 10:09:49.695721 cf_clearance-0.29.1/cf_clearance/js/navigator.webdriver.js
+-rw-r--r--   0        0        0     2058 2023-06-07 06:30:31.817778 cf_clearance-0.29.1/cf_clearance/retry.py
+-rw-r--r--   0        0        0     3678 2022-11-28 03:39:27.927929 cf_clearance-0.29.1/cf_clearance/stealth.py
+-rw-r--r--   0        0        0      772 2023-06-07 07:16:06.551887 cf_clearance-0.29.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-12-05 15:24:48.652965 cf_clearance-0.29.1/tests/__init__.py
+-rw-r--r--   0        0        0     1805 2022-11-28 03:39:27.928856 cf_clearance-0.29.1/tests/test_async_cf.py
+-rw-r--r--   0        0        0      715 2023-04-17 13:57:16.483813 cf_clearance-0.29.1/tests/test_common.py
+-rw-r--r--   0        0        0      838 2023-06-07 04:12:39.890891 cf_clearance-0.29.1/tests/test_cron_challenge.py
+-rw-r--r--   0        0        0     1660 2022-11-28 03:39:27.929569 cf_clearance-0.29.1/tests/test_sync_cf.py
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 cf_clearance-0.29.1/PKG-INFO
```

### Comparing `cf_clearance-0.29.0/LICENSE` & `cf_clearance-0.29.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.0/README.md` & `cf_clearance-0.29.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/cf_clearance.svg?color=%2334D058)](https://pypi.python.org/pypi/cf_clearance)
 [![Docker Image versions](https://img.shields.io/docker/v/vvanglro/cf-clearance?color=%2334D058&label=docker%20version)](https://hub.docker.com/r/vvanglro/cf-clearance)
 
 
 Purpose To make a cloudflare v2 challenge pass successfully, Can be use cf_clearance bypassed by cloudflare, However, with
 the cf_clearance, make sure you use the same IP and UA as when you got it.
 
+## Project Pass Challenge Status
+[![Every day cron challenge](https://github.com/vvanglro/cf-clearance/actions/workflows/every_day_cron_challenge.yml/badge.svg)](https://github.com/vvanglro/cf-clearance/actions/workflows/every_day_cron_challenge.yml)
+
 ## Warning
 
 Please use interface mode, You must add headless=False.
 If you use it on linux or docker, use XVFB.
 
 Challenge are not always successful. Please try more and handle exceptions.
 
@@ -51,15 +54,15 @@
     if '<title>Just a moment...</title>' not in res.text:
         print("cf challenge success")
 ```
 
 ## Install
 
 ```
-pip install cf-clearance==0.28.2
+pip install cf-clearance
 ```
 
 ## Usage
 
 Please make sure it is the latest package.
 
 ```
```

### Comparing `cf_clearance-0.29.0/cf_clearance/js/canvas.fingerprinting.js` & `cf_clearance-0.29.1/cf_clearance/js/canvas.fingerprinting.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.0/cf_clearance/js/chrome.global.js` & `cf_clearance-0.29.1/cf_clearance/js/chrome.global.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.0/cf_clearance/js/chrome.plugin.js` & `cf_clearance-0.29.1/cf_clearance/js/chrome.plugin.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.0/cf_clearance/js/chrome.runtime.js` & `cf_clearance-0.29.1/cf_clearance/js/chrome.runtime.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.0/cf_clearance/js/navigator.permissions.js` & `cf_clearance-0.29.1/cf_clearance/js/navigator.permissions.js`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.0/cf_clearance/retry.py` & `cf_clearance-0.29.1/cf_clearance/retry.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,55 +2,56 @@
 from playwright.async_api import Error
 from playwright.async_api import Page as AsyncPage
 from playwright.sync_api import Page as SyncPage
 
 
 async def async_cf_retry(page: AsyncPage, tries: int = 10) -> bool:
     success = False
-    while tries != 0:
+    while tries > 0:
         await page.wait_for_timeout(1500)
         try:
             success = False if await page.query_selector("#challenge-form") else True
-            click_button = await page.query_selector("#challenge-stage > div > input")
-            if click_button:
-                await click_button.click()
-            iframe = await page.query_selector(
-                "xpath=//div[@class='hcaptcha-box']/iframe"
+            if success:
+                break
+            simple_challenge = await page.query_selector(
+                "#challenge-stage > div > input[type='button']"
             )
-            if iframe:
-                switch_iframe = await iframe.content_frame()
-                iframe_button = await switch_iframe.query_selector(
-                    "xpath=//*[@id='cf-stage']//label/span"
-                )
-                if iframe_button:
-                    await iframe_button.click()
+            if simple_challenge:
+                await simple_challenge.click()
+            for target_frame in page.main_frame.child_frames:
+                if "challenge" in target_frame.url and "turnstile" in target_frame.url:
+                    click = await target_frame.query_selector(
+                        "xpath=//input[@type='checkbox']"
+                    )
+                    if click:
+                        await click.click()
         except Error:
             success = False
-        if success:
-            break
         tries -= 1
     return success
 
 
 def sync_cf_retry(page: SyncPage, tries: int = 10) -> bool:
     success = False
-    while tries != 0:
+    while tries > 0:
         page.wait_for_timeout(1500)
         try:
             success = False if page.query_selector("#challenge-form") else True
-            click_button = page.query_selector("#challenge-stage > div > input")
-            if click_button:
-                click_button.click()
-            iframe = page.query_selector("xpath=//div[@class='hcaptcha-box']/iframe")
-            if iframe:
-                iframe_button = iframe.content_frame().query_selector(
-                    "xpath=//*[@id='cf-stage']//label/span"
-                )
-                if iframe_button:
-                    iframe_button.click()
+            if success:
+                break
+            simple_challenge = page.query_selector(
+                "#challenge-stage > div > input[type='button']"
+            )
+            if simple_challenge:
+                simple_challenge.click()
+            for target_frame in page.main_frame.child_frames:
+                if "challenge" in target_frame.url and "turnstile" in target_frame.url:
+                    click = target_frame.query_selector(
+                        "xpath=//input[@type='checkbox']"
+                    )
+                    if click:
+                        click.click()
         except Error:
             success = False
-        if success:
-            break
         tries -= 1
 
     return success
```

### Comparing `cf_clearance-0.29.0/cf_clearance/stealth.py` & `cf_clearance-0.29.1/cf_clearance/stealth.py`

 * *Files identical despite different names*

### Comparing `cf_clearance-0.29.0/PKG-INFO` & `cf_clearance-0.29.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: cf-clearance
-Version: 0.29.0
+Version: 0.29.1
 Summary: Purpose To make a cloudflare v2 challenge pass successfully, Can be use cf_clearance bypassed by cloudflare, However, with the cf_clearance, make sure you use the same IP and UA as when you got it.
-Home-page: https://github.com/vvanglro/cf_clearance
-Author: vvanglro
-Author-email: you@example.com
-Requires-Python: >=3.7,<4
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: playwright
+Author-Email: vvanglro <vvanglro@gmail.com>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/vvanglro/cf_clearance
 Project-URL: Repository, https://github.com/vvanglro/cf_clearance
+Requires-Python: <4,>=3.7
+Requires-Dist: playwright>=1.34.0
 Description-Content-Type: text/markdown
 
 # cf-clearance
 
 [![OSCS Status](https://www.oscs1024.com/platform/badge/vvanglro/cf_clearance.svg?size=small)](https://www.oscs1024.com/project/vvanglro/cf_clearance?ref=badge_small)
 [![Package version](https://img.shields.io/pypi/v/cf_clearance?color=%2334D058&label=pypi%20package)](https://pypi.python.org/pypi/cf_clearance)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/cf_clearance.svg?color=%2334D058)](https://pypi.python.org/pypi/cf_clearance)
 [![Docker Image versions](https://img.shields.io/docker/v/vvanglro/cf-clearance?color=%2334D058&label=docker%20version)](https://hub.docker.com/r/vvanglro/cf-clearance)
 
 
 Purpose To make a cloudflare v2 challenge pass successfully, Can be use cf_clearance bypassed by cloudflare, However, with
 the cf_clearance, make sure you use the same IP and UA as when you got it.
 
+## Project Pass Challenge Status
+[![Every day cron challenge](https://github.com/vvanglro/cf-clearance/actions/workflows/every_day_cron_challenge.yml/badge.svg)](https://github.com/vvanglro/cf-clearance/actions/workflows/every_day_cron_challenge.yml)
+
 ## Warning
 
 Please use interface mode, You must add headless=False.
 If you use it on linux or docker, use XVFB.
 
 Challenge are not always successful. Please try more and handle exceptions.
 
@@ -68,15 +66,15 @@
     if '<title>Just a moment...</title>' not in res.text:
         print("cf challenge success")
 ```
 
 ## Install
 
 ```
-pip install cf-clearance==0.28.2
+pip install cf-clearance
 ```
 
 ## Usage
 
 Please make sure it is the latest package.
 
 ```
@@ -168,8 +166,7 @@
     res = requests.get('https://nowsecure.nl', proxies=proxies, headers=headers, cookies=cookies)
     if '<title>Just a moment...</title>' not in res.text:
         print("cf challenge success")
 
 
 asyncio.get_event_loop().run_until_complete(main())
 ```
-
```

