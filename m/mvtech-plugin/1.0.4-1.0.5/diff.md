# Comparing `tmp/mvtech-plugin-1.0.4.tar.gz` & `tmp/mvtech-plugin-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mvtech-plugin-1.0.4.tar", last modified: Wed Jun  7 03:09:58 2023, max compression
+gzip compressed data, was "dist\mvtech-plugin-1.0.5.tar", last modified: Wed Jun  7 03:18:40 2023, max compression
```

## Comparing `mvtech-plugin-1.0.4.tar` & `mvtech-plugin-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 03:09:58.899163 mvtech-plugin-1.0.4/
--rw-rw-rw-   0        0        0       31 2023-03-27 00:54:56.000000 mvtech-plugin-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2630 2023-06-07 03:09:58.899163 mvtech-plugin-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2353 2023-06-07 02:22:15.000000 mvtech-plugin-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 03:09:58.881211 mvtech-plugin-1.0.4/core/
--rw-rw-rw-   0        0        0       21 2023-06-07 03:08:31.000000 mvtech-plugin-1.0.4/core/__init__.py
--rw-rw-rw-   0        0        0    10018 2023-06-05 09:44:22.000000 mvtech-plugin-1.0.4/core/cli_methods.py
--rw-rw-rw-   0        0        0    14631 2023-06-07 03:06:20.000000 mvtech-plugin-1.0.4/core/config.py
--rw-rw-rw-   0        0        0     1637 2023-03-27 01:06:38.000000 mvtech-plugin-1.0.4/core/main.py
-drwxrwxrwx   0        0        0        0 2023-06-07 03:09:58.883206 mvtech-plugin-1.0.4/core/res/
-drwxrwxrwx   0        0        0        0 2023-06-07 03:09:58.893180 mvtech-plugin-1.0.4/core/res/SDK/
--rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.4/core/res/SDK/__init__.py
--rw-rw-rw-   0        0        0     7829 2023-02-15 05:39:36.000000 mvtech-plugin-1.0.4/core/res/SDK/base.py
--rw-rw-rw-   0        0        0     2132 2023-06-05 07:27:02.000000 mvtech-plugin-1.0.4/core/res/SDK/cli.py
--rw-rw-rw-   0        0        0     4643 2023-03-27 00:56:18.000000 mvtech-plugin-1.0.4/core/res/SDK/http_run.py
--rw-rw-rw-   0        0        0      162 2023-03-27 00:44:29.000000 mvtech-plugin-1.0.4/core/res/SDK/models.py
--rw-rw-rw-   0        0        0      463 2023-03-27 01:09:02.000000 mvtech-plugin-1.0.4/core/res/SDK/plugin.py
--rw-rw-rw-   0        0        0    12776 2023-06-05 09:23:34.000000 mvtech-plugin-1.0.4/core/res/SDK/run_define.py
--rw-rw-rw-   0        0        0     1719 2023-02-20 08:33:11.000000 mvtech-plugin-1.0.4/core/res/SDK/service_stop.py
--rw-rw-rw-   0        0        0     5323 2023-06-05 09:24:15.000000 mvtech-plugin-1.0.4/core/res/SDK/web.py
--rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.4/core/res/__init__.py
--rw-rw-rw-   0        0        0    37636 2023-06-06 01:54:59.000000 mvtech-plugin-1.0.4/core/res/project.tar.gz
--rw-rw-rw-   0        0        0     3473 2023-02-03 02:21:28.000000 mvtech-plugin-1.0.4/core/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-07 03:09:58.898167 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/
--rw-rw-rw-   0        0        0     2630 2023-06-07 03:09:58.000000 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      601 2023-06-07 03:09:58.000000 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 03:09:58.000000 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-07 03:09:58.000000 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2023-06-07 03:09:58.000000 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-07 03:09:58.000000 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 03:09:58.900291 mvtech-plugin-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1236 2023-02-03 03:01:22.000000 mvtech-plugin-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:18:40.690667 mvtech-plugin-1.0.5/
+-rw-rw-rw-   0        0        0       31 2023-03-27 00:54:56.000000 mvtech-plugin-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2630 2023-06-07 03:18:40.690667 mvtech-plugin-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2353 2023-06-07 02:22:15.000000 mvtech-plugin-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 03:18:40.663584 mvtech-plugin-1.0.5/core/
+-rw-rw-rw-   0        0        0       21 2023-06-07 03:18:37.000000 mvtech-plugin-1.0.5/core/__init__.py
+-rw-rw-rw-   0        0        0    10018 2023-06-05 09:44:22.000000 mvtech-plugin-1.0.5/core/cli_methods.py
+-rw-rw-rw-   0        0        0    14631 2023-06-07 03:06:20.000000 mvtech-plugin-1.0.5/core/config.py
+-rw-rw-rw-   0        0        0     1637 2023-03-27 01:06:38.000000 mvtech-plugin-1.0.5/core/main.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:18:40.665580 mvtech-plugin-1.0.5/core/res/
+drwxrwxrwx   0        0        0        0 2023-06-07 03:18:40.681693 mvtech-plugin-1.0.5/core/res/SDK/
+-rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.5/core/res/SDK/__init__.py
+-rw-rw-rw-   0        0        0     7829 2023-02-15 05:39:36.000000 mvtech-plugin-1.0.5/core/res/SDK/base.py
+-rw-rw-rw-   0        0        0     2126 2023-06-07 03:13:07.000000 mvtech-plugin-1.0.5/core/res/SDK/cli.py
+-rw-rw-rw-   0        0        0     4643 2023-03-27 00:56:18.000000 mvtech-plugin-1.0.5/core/res/SDK/http_run.py
+-rw-rw-rw-   0        0        0      162 2023-03-27 00:44:29.000000 mvtech-plugin-1.0.5/core/res/SDK/models.py
+-rw-rw-rw-   0        0        0      463 2023-03-27 01:09:02.000000 mvtech-plugin-1.0.5/core/res/SDK/plugin.py
+-rw-rw-rw-   0        0        0    12776 2023-06-05 09:23:34.000000 mvtech-plugin-1.0.5/core/res/SDK/run_define.py
+-rw-rw-rw-   0        0        0     1719 2023-02-20 08:33:11.000000 mvtech-plugin-1.0.5/core/res/SDK/service_stop.py
+-rw-rw-rw-   0        0        0     5323 2023-06-05 09:24:15.000000 mvtech-plugin-1.0.5/core/res/SDK/web.py
+-rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.5/core/res/__init__.py
+-rw-rw-rw-   0        0        0    37636 2023-06-06 01:54:59.000000 mvtech-plugin-1.0.5/core/res/project.tar.gz
+-rw-rw-rw-   0        0        0     3473 2023-02-03 02:21:28.000000 mvtech-plugin-1.0.5/core/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:18:40.689681 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/
+-rw-rw-rw-   0        0        0     2630 2023-06-07 03:18:40.000000 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2023-06-07 03:18:40.000000 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 03:18:40.000000 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-07 03:18:40.000000 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2023-06-07 03:18:40.000000 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-07 03:18:40.000000 mvtech-plugin-1.0.5/mvtech_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 03:18:40.691667 mvtech-plugin-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1236 2023-02-03 03:01:22.000000 mvtech-plugin-1.0.5/setup.py
```

### Comparing `mvtech-plugin-1.0.4/PKG-INFO` & `mvtech-plugin-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvtech-plugin
-Version: 1.0.4
+Version: 1.0.5
 Summary: 插件生成等功能...
 Home-page: https://www.mvtech.cn/market/introduction
 Author: sandy
 Author-email: tong@mvtech.com.cn
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `mvtech-plugin-1.0.4/README.md` & `mvtech-plugin-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.4/core/cli_methods.py` & `mvtech-plugin-1.0.5/core/cli_methods.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.4/core/config.py` & `mvtech-plugin-1.0.5/core/config.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.4/core/main.py` & `mvtech-plugin-1.0.5/core/main.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.4/core/res/SDK/base.py` & `mvtech-plugin-1.0.5/core/res/SDK/base.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.4/core/res/SDK/cli.py` & `mvtech-plugin-1.0.5/core/res/SDK/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         log("error", "未知的命令：{}".format(command))
         return
 
 
 def getData() -> dict:
     """
     #   此方法用于获取需要的运行数据
-    #   在千乘系统中，可能并不会传入json数据文件的路径，而是会直接传入json数据或字典数据，此时输入cmd指令长度不足（输入数据不计长度）
+    #   在系统中，可能并不会传入json数据文件的路径，而是会直接传入json数据或字典数据，此时输入cmd指令长度不足（输入数据不计长度）
     #   所以使用sys.stdin.read()读取可能存在的数据
     """
     if len(sys.argv) >= 3:
         testfile_path = sys.argv[2]
         data = loadData(testfile_path)
     else:
         data = sys.stdin.read()
```

### Comparing `mvtech-plugin-1.0.4/core/res/SDK/http_run.py` & `mvtech-plugin-1.0.5/core/res/SDK/http_run.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.4/core/res/SDK/run_define.py` & `mvtech-plugin-1.0.5/core/res/SDK/run_define.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.4/core/res/SDK/service_stop.py` & `mvtech-plugin-1.0.5/core/res/SDK/service_stop.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.4/core/res/SDK/web.py` & `mvtech-plugin-1.0.5/core/res/SDK/web.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.4/core/res/project.tar.gz` & `mvtech-plugin-1.0.5/core/res/project.tar.gz`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.4/core/tools.py` & `mvtech-plugin-1.0.5/core/tools.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.4/mvtech_plugin.egg-info/PKG-INFO` & `mvtech-plugin-1.0.5/mvtech_plugin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvtech-plugin
-Version: 1.0.4
+Version: 1.0.5
 Summary: 插件生成等功能...
 Home-page: https://www.mvtech.cn/market/introduction
 Author: sandy
 Author-email: tong@mvtech.com.cn
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `mvtech-plugin-1.0.4/mvtech_plugin.egg-info/SOURCES.txt` & `mvtech-plugin-1.0.5/mvtech_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.4/setup.py` & `mvtech-plugin-1.0.5/setup.py`

 * *Files identical despite different names*

