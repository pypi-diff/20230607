# Comparing `tmp/mvtech-plugin-1.0.5.tar.gz` & `tmp/mvtech-plugin-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mvtech-plugin-1.0.5.tar", last modified: Wed Jun  7 03:18:40 2023, max compression
+gzip compressed data, was "dist\mvtech-plugin-1.0.6.tar", last modified: Wed Jun  7 07:55:42 2023, max compression
```

## Comparing `mvtech-plugin-1.0.5.tar` & `mvtech-plugin-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 03:18:40.690667 mvtech-plugin-1.0.5/
--rw-rw-rw-   0        0        0       31 2023-03-27 00:54:56.000000 mvtech-plugin-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2630 2023-06-07 03:18:40.690667 mvtech-plugin-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2353 2023-06-07 02:22:15.000000 mvtech-plugin-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 03:18:40.663584 mvtech-plugin-1.0.5/core/
--rw-rw-rw-   0        0        0       21 2023-06-07 03:18:37.000000 mvtech-plugin-1.0.5/core/__init__.py
--rw-rw-rw-   0        0        0    10018 2023-06-05 09:44:22.000000 mvtech-plugin-1.0.5/core/cli_methods.py
--rw-rw-rw-   0        0        0    14631 2023-06-07 03:06:20.000000 mvtech-plugin-1.0.5/core/config.py
--rw-rw-rw-   0        0        0     1637 2023-03-27 01:06:38.000000 mvtech-plugin-1.0.5/core/main.py
-drwxrwxrwx   0        0        0        0 2023-06-07 03:18:40.665580 mvtech-plugin-1.0.5/core/res/
-drwxrwxrwx   0        0        0        0 2023-06-07 03:18:40.681693 mvtech-plugin-1.0.5/core/res/SDK/
--rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.5/core/res/SDK/__init__.py
--rw-rw-rw-   0        0        0     7829 2023-02-15 05:39:36.000000 mvtech-plugin-1.0.5/core/res/SDK/base.py
--rw-rw-rw-   0        0        0     2126 2023-06-07 03:13:07.000000 mvtech-plugin-1.0.5/core/res/SDK/cli.py
--rw-rw-rw-   0        0        0     4643 2023-03-27 00:56:18.000000 mvtech-plugin-1.0.5/core/res/SDK/http_run.py
--rw-rw-rw-   0        0        0      162 2023-03-27 00:44:29.000000 mvtech-plugin-1.0.5/core/res/SDK/models.py
--rw-rw-rw-   0        0        0      463 2023-03-27 01:09:02.000000 mvtech-plugin-1.0.5/core/res/SDK/plugin.py
--rw-rw-rw-   0        0        0    12776 2023-06-05 09:23:34.000000 mvtech-plugin-1.0.5/core/res/SDK/run_define.py
--rw-rw-rw-   0        0        0     1719 2023-02-20 08:33:11.000000 mvtech-plugin-1.0.5/core/res/SDK/service_stop.py
--rw-rw-rw-   0        0        0     5323 2023-06-05 09:24:15.000000 mvtech-plugin-1.0.5/core/res/SDK/web.py
--rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.5/core/res/__init__.py
--rw-rw-rw-   0        0        0    37636 2023-06-06 01:54:59.000000 mvtech-plugin-1.0.5/core/res/project.tar.gz
--rw-rw-rw-   0        0        0     3473 2023-02-03 02:21:28.000000 mvtech-plugin-1.0.5/core/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-07 03:18:40.689681 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/
--rw-rw-rw-   0        0        0     2630 2023-06-07 03:18:40.000000 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      601 2023-06-07 03:18:40.000000 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 03:18:40.000000 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-07 03:18:40.000000 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2023-06-07 03:18:40.000000 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-07 03:18:40.000000 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 03:18:40.691667 mvtech-plugin-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1236 2023-02-03 03:01:22.000000 mvtech-plugin-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:55:42.502571 mvtech-plugin-1.0.6/
+-rw-rw-rw-   0        0        0       31 2023-03-27 00:54:56.000000 mvtech-plugin-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2630 2023-06-07 07:55:42.503568 mvtech-plugin-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2353 2023-06-07 02:22:15.000000 mvtech-plugin-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 07:55:42.481782 mvtech-plugin-1.0.6/core/
+-rw-rw-rw-   0        0        0       21 2023-06-07 07:54:18.000000 mvtech-plugin-1.0.6/core/__init__.py
+-rw-rw-rw-   0        0        0    10018 2023-06-05 09:44:22.000000 mvtech-plugin-1.0.6/core/cli_methods.py
+-rw-rw-rw-   0        0        0    14629 2023-06-07 07:38:51.000000 mvtech-plugin-1.0.6/core/config.py
+-rw-rw-rw-   0        0        0     1637 2023-03-27 01:06:38.000000 mvtech-plugin-1.0.6/core/main.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:55:42.483776 mvtech-plugin-1.0.6/core/res/
+drwxrwxrwx   0        0        0        0 2023-06-07 07:55:42.493750 mvtech-plugin-1.0.6/core/res/SDK/
+-rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.6/core/res/SDK/__init__.py
+-rw-rw-rw-   0        0        0     7829 2023-02-15 05:39:36.000000 mvtech-plugin-1.0.6/core/res/SDK/base.py
+-rw-rw-rw-   0        0        0     2126 2023-06-07 03:13:07.000000 mvtech-plugin-1.0.6/core/res/SDK/cli.py
+-rw-rw-rw-   0        0        0     4643 2023-03-27 00:56:18.000000 mvtech-plugin-1.0.6/core/res/SDK/http_run.py
+-rw-rw-rw-   0        0        0      162 2023-03-27 00:44:29.000000 mvtech-plugin-1.0.6/core/res/SDK/models.py
+-rw-rw-rw-   0        0        0      463 2023-03-27 01:09:02.000000 mvtech-plugin-1.0.6/core/res/SDK/plugin.py
+-rw-rw-rw-   0        0        0    12776 2023-06-05 09:23:34.000000 mvtech-plugin-1.0.6/core/res/SDK/run_define.py
+-rw-rw-rw-   0        0        0     1719 2023-02-20 08:33:11.000000 mvtech-plugin-1.0.6/core/res/SDK/service_stop.py
+-rw-rw-rw-   0        0        0     5323 2023-06-05 09:24:15.000000 mvtech-plugin-1.0.6/core/res/SDK/web.py
+-rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.6/core/res/__init__.py
+-rw-rw-rw-   0        0        0    37636 2023-06-06 01:54:59.000000 mvtech-plugin-1.0.6/core/res/project.tar.gz
+-rw-rw-rw-   0        0        0     3473 2023-02-03 02:21:28.000000 mvtech-plugin-1.0.6/core/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:55:42.502571 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/
+-rw-rw-rw-   0        0        0     2630 2023-06-07 07:55:42.000000 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2023-06-07 07:55:42.000000 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 07:55:42.000000 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-07 07:55:42.000000 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2023-06-07 07:55:42.000000 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-07 07:55:42.000000 mvtech-plugin-1.0.6/mvtech_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 07:55:42.503763 mvtech-plugin-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1236 2023-02-03 03:01:22.000000 mvtech-plugin-1.0.6/setup.py
```

### Comparing `mvtech-plugin-1.0.5/PKG-INFO` & `mvtech-plugin-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvtech-plugin
-Version: 1.0.5
+Version: 1.0.6
 Summary: 插件生成等功能...
 Home-page: https://www.mvtech.cn/market/introduction
 Author: sandy
 Author-email: tong@mvtech.com.cn
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `mvtech-plugin-1.0.5/README.md` & `mvtech-plugin-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.5/core/cli_methods.py` & `mvtech-plugin-1.0.6/core/cli_methods.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.5/core/config.py` & `mvtech-plugin-1.0.6/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 '''
 test_server = FastAPI(title="MVTECH-Plugin Test Server", version="1.0.0", description=desc)
 {% for name, className in init_list %}
 @test_server.post("/actions/{{ name }}",response_model={{ className }}().outputModel,tags=["动作"])
 def action_{{ name }}(action_name:str="{{ name }}",
                       adapter_data:{{ className }}().adapMdl=None,
-                      baseRunModel:ENCODE_STR_ACTION().baseRunModel=None,
+                      baseRunModel:{{ className }}().baseRunModel=None,
                       input_data:{{ className }}().inputModel=None):
     
     clearLog()
 
     adapter_data = adapter_data.dict()
 
     baseRunModel = baseRunModel.dict()
```

### Comparing `mvtech-plugin-1.0.5/core/main.py` & `mvtech-plugin-1.0.6/core/main.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.5/core/res/SDK/base.py` & `mvtech-plugin-1.0.6/core/res/SDK/base.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.5/core/res/SDK/cli.py` & `mvtech-plugin-1.0.6/core/res/SDK/cli.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.5/core/res/SDK/http_run.py` & `mvtech-plugin-1.0.6/core/res/SDK/http_run.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.5/core/res/SDK/run_define.py` & `mvtech-plugin-1.0.6/core/res/SDK/run_define.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.5/core/res/SDK/service_stop.py` & `mvtech-plugin-1.0.6/core/res/SDK/service_stop.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.5/core/res/SDK/web.py` & `mvtech-plugin-1.0.6/core/res/SDK/web.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.5/core/res/project.tar.gz` & `mvtech-plugin-1.0.6/core/res/project.tar.gz`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.5/core/tools.py` & `mvtech-plugin-1.0.6/core/tools.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.5/mvtech_plugin.egg-info/PKG-INFO` & `mvtech-plugin-1.0.6/mvtech_plugin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvtech-plugin
-Version: 1.0.5
+Version: 1.0.6
 Summary: 插件生成等功能...
 Home-page: https://www.mvtech.cn/market/introduction
 Author: sandy
 Author-email: tong@mvtech.com.cn
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `mvtech-plugin-1.0.5/mvtech_plugin.egg-info/SOURCES.txt` & `mvtech-plugin-1.0.6/mvtech_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.5/setup.py` & `mvtech-plugin-1.0.6/setup.py`

 * *Files identical despite different names*

