# Comparing `tmp/mvtech-plugin-1.0.3.tar.gz` & `tmp/mvtech-plugin-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mvtech-plugin-1.0.3.tar", last modified: Wed Jun  7 01:37:31 2023, max compression
+gzip compressed data, was "dist\mvtech-plugin-1.0.4.tar", last modified: Wed Jun  7 03:09:58 2023, max compression
```

## Comparing `mvtech-plugin-1.0.3.tar` & `mvtech-plugin-1.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 01:37:31.640863 mvtech-plugin-1.0.3/
--rw-rw-rw-   0        0        0       31 2023-03-27 00:54:56.000000 mvtech-plugin-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2365 2023-06-07 01:37:31.640863 mvtech-plugin-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2086 2023-03-27 00:49:39.000000 mvtech-plugin-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 01:37:31.621914 mvtech-plugin-1.0.3/core/
--rw-rw-rw-   0        0        0       21 2023-06-07 01:37:28.000000 mvtech-plugin-1.0.3/core/__init__.py
--rw-rw-rw-   0        0        0    10018 2023-06-05 09:44:22.000000 mvtech-plugin-1.0.3/core/cli_methods.py
--rw-rw-rw-   0        0        0    14501 2023-06-05 09:56:41.000000 mvtech-plugin-1.0.3/core/config.py
--rw-rw-rw-   0        0        0     1637 2023-03-27 01:06:38.000000 mvtech-plugin-1.0.3/core/main.py
-drwxrwxrwx   0        0        0        0 2023-06-07 01:37:31.623909 mvtech-plugin-1.0.3/core/res/
-drwxrwxrwx   0        0        0        0 2023-06-07 01:37:31.634881 mvtech-plugin-1.0.3/core/res/SDK/
--rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.3/core/res/SDK/__init__.py
--rw-rw-rw-   0        0        0     7829 2023-02-15 05:39:36.000000 mvtech-plugin-1.0.3/core/res/SDK/base.py
--rw-rw-rw-   0        0        0     2132 2023-06-05 07:27:02.000000 mvtech-plugin-1.0.3/core/res/SDK/cli.py
--rw-rw-rw-   0        0        0     4643 2023-03-27 00:56:18.000000 mvtech-plugin-1.0.3/core/res/SDK/http_run.py
--rw-rw-rw-   0        0        0      162 2023-03-27 00:44:29.000000 mvtech-plugin-1.0.3/core/res/SDK/models.py
--rw-rw-rw-   0        0        0      463 2023-03-27 01:09:02.000000 mvtech-plugin-1.0.3/core/res/SDK/plugin.py
--rw-rw-rw-   0        0        0    12776 2023-06-05 09:23:34.000000 mvtech-plugin-1.0.3/core/res/SDK/run_define.py
--rw-rw-rw-   0        0        0     1719 2023-02-20 08:33:11.000000 mvtech-plugin-1.0.3/core/res/SDK/service_stop.py
--rw-rw-rw-   0        0        0     5323 2023-06-05 09:24:15.000000 mvtech-plugin-1.0.3/core/res/SDK/web.py
--rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.3/core/res/__init__.py
--rw-rw-rw-   0        0        0    37636 2023-06-06 01:54:59.000000 mvtech-plugin-1.0.3/core/res/project.tar.gz
--rw-rw-rw-   0        0        0     3473 2023-02-03 02:21:28.000000 mvtech-plugin-1.0.3/core/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-07 01:37:31.639867 mvtech-plugin-1.0.3/mvtech_plugin.egg-info/
--rw-rw-rw-   0        0        0     2365 2023-06-07 01:37:31.000000 mvtech-plugin-1.0.3/mvtech_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      601 2023-06-07 01:37:31.000000 mvtech-plugin-1.0.3/mvtech_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 01:37:31.000000 mvtech-plugin-1.0.3/mvtech_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-07 01:37:31.000000 mvtech-plugin-1.0.3/mvtech_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2023-06-07 01:37:31.000000 mvtech-plugin-1.0.3/mvtech_plugin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-07 01:37:31.000000 mvtech-plugin-1.0.3/mvtech_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 01:37:31.641864 mvtech-plugin-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1236 2023-02-03 03:01:22.000000 mvtech-plugin-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:09:58.899163 mvtech-plugin-1.0.4/
+-rw-rw-rw-   0        0        0       31 2023-03-27 00:54:56.000000 mvtech-plugin-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2630 2023-06-07 03:09:58.899163 mvtech-plugin-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2353 2023-06-07 02:22:15.000000 mvtech-plugin-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 03:09:58.881211 mvtech-plugin-1.0.4/core/
+-rw-rw-rw-   0        0        0       21 2023-06-07 03:08:31.000000 mvtech-plugin-1.0.4/core/__init__.py
+-rw-rw-rw-   0        0        0    10018 2023-06-05 09:44:22.000000 mvtech-plugin-1.0.4/core/cli_methods.py
+-rw-rw-rw-   0        0        0    14631 2023-06-07 03:06:20.000000 mvtech-plugin-1.0.4/core/config.py
+-rw-rw-rw-   0        0        0     1637 2023-03-27 01:06:38.000000 mvtech-plugin-1.0.4/core/main.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:09:58.883206 mvtech-plugin-1.0.4/core/res/
+drwxrwxrwx   0        0        0        0 2023-06-07 03:09:58.893180 mvtech-plugin-1.0.4/core/res/SDK/
+-rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.4/core/res/SDK/__init__.py
+-rw-rw-rw-   0        0        0     7829 2023-02-15 05:39:36.000000 mvtech-plugin-1.0.4/core/res/SDK/base.py
+-rw-rw-rw-   0        0        0     2132 2023-06-05 07:27:02.000000 mvtech-plugin-1.0.4/core/res/SDK/cli.py
+-rw-rw-rw-   0        0        0     4643 2023-03-27 00:56:18.000000 mvtech-plugin-1.0.4/core/res/SDK/http_run.py
+-rw-rw-rw-   0        0        0      162 2023-03-27 00:44:29.000000 mvtech-plugin-1.0.4/core/res/SDK/models.py
+-rw-rw-rw-   0        0        0      463 2023-03-27 01:09:02.000000 mvtech-plugin-1.0.4/core/res/SDK/plugin.py
+-rw-rw-rw-   0        0        0    12776 2023-06-05 09:23:34.000000 mvtech-plugin-1.0.4/core/res/SDK/run_define.py
+-rw-rw-rw-   0        0        0     1719 2023-02-20 08:33:11.000000 mvtech-plugin-1.0.4/core/res/SDK/service_stop.py
+-rw-rw-rw-   0        0        0     5323 2023-06-05 09:24:15.000000 mvtech-plugin-1.0.4/core/res/SDK/web.py
+-rw-rw-rw-   0        0        0        0 2023-01-29 09:23:09.000000 mvtech-plugin-1.0.4/core/res/__init__.py
+-rw-rw-rw-   0        0        0    37636 2023-06-06 01:54:59.000000 mvtech-plugin-1.0.4/core/res/project.tar.gz
+-rw-rw-rw-   0        0        0     3473 2023-02-03 02:21:28.000000 mvtech-plugin-1.0.4/core/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-07 03:09:58.898167 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/
+-rw-rw-rw-   0        0        0     2630 2023-06-07 03:09:58.000000 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2023-06-07 03:09:58.000000 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 03:09:58.000000 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-07 03:09:58.000000 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2023-06-07 03:09:58.000000 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-07 03:09:58.000000 mvtech-plugin-1.0.4/mvtech_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 03:09:58.900291 mvtech-plugin-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1236 2023-02-03 03:01:22.000000 mvtech-plugin-1.0.4/setup.py
```

### Comparing `mvtech-plugin-1.0.3/PKG-INFO` & `mvtech-plugin-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: mvtech-plugin
-Version: 1.0.3
+Version: 1.0.4
 Summary: 插件生成等功能...
 Home-page: https://www.mvtech.cn/market/introduction
 Author: sandy
 Author-email: tong@mvtech.com.cn
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 ### mvtech_plugin
 
 ---
 
 #### 简介
+
 **mvtech_plugin**是MVTech插件脚手架
 
 #### 基本架构结构
+
 ```txt
 .
 ├── actions
 │   ├── __init__.py
 │   ├── ???.py     
 │   ├── models.py
 ├── Dockerfile
@@ -48,34 +50,40 @@
 - ?_plugin.yaml: 模板文件，定义插件．
 - actions/???.py: 根据模板文件定义生成动作．
 - triggers/???.py: 根据模板文件定义生成触发器．
 - actions/models.py 和 triggers/models.py: 模板文件继承pydantic
 - testAPI: FastAPI测试入口
 
 #### 环境要求
+
 - python3.+
 
 #### 安装 依赖
+
 pip install -r requirements.txt
 
 ### 脚手架离线自定义打包安装
 
 #### 脚手架打包
-    python .\setup.py sdist
 
+    python .\setup.py sdist
 
 #### 脚手架生成的压缩包解压后执行下面命令安装
+
     python setup.py install
 
 #### 脚手架卸载
+
     pip uninstall mvtech-plugin 1.0.0 -y
 
 #### 脚手架使用
+
     执行本地脚手架
     mvtech-plugin -h
+
 ```
 usage: mvtech-plugin [-h] [-v] [-g GENERATE] [-r RUN] [-hp] [-t TEST] [-tb] [-mki]
 
 插件生成器
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -83,12 +91,26 @@
   -g GENERATE, --generate GENERATE
                         插件生成
   -r RUN, --run RUN     运行action
   -hp, --http           启动api接口
   -t TEST, --test TEST  测试
   -tb, --tarball        插件打包
   -mki, --mkimg         制作成docker镜像     
-```
+```  
+
+### 打包出现#!/usr/bin/env python 
+- vi 文件名
+- : set ff = unix
+- : wq
+
+### 打docker镜像包 并且下载过程
+make image
+docker save mvtech/kafka:1.0.0 -o mvtech-kafka-1.0.0.tar
+
+### 生成系统安装包
+make tarball
+
 #### 离线打Docker包
+
 - docker save <myimage>:<tag> | gzip > <myimage>_<tag>.tar.gz
 
 - docker save mvtech/rest:1.0.0 | gzip > mvtech_rest_1.0.0.tar.gz
```

### Comparing `mvtech-plugin-1.0.3/README.md` & `mvtech-plugin-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 ### mvtech_plugin
 
 ---
 
 #### 简介
+
 **mvtech_plugin**是MVTech插件脚手架
 
 #### 基本架构结构
+
 ```txt
 .
 ├── actions
 │   ├── __init__.py
 │   ├── ???.py     
 │   ├── models.py
 ├── Dockerfile
@@ -37,34 +39,40 @@
 - ?_plugin.yaml: 模板文件，定义插件．
 - actions/???.py: 根据模板文件定义生成动作．
 - triggers/???.py: 根据模板文件定义生成触发器．
 - actions/models.py 和 triggers/models.py: 模板文件继承pydantic
 - testAPI: FastAPI测试入口
 
 #### 环境要求
+
 - python3.+
 
 #### 安装 依赖
+
 pip install -r requirements.txt
 
 ### 脚手架离线自定义打包安装
 
 #### 脚手架打包
-    python .\setup.py sdist
 
+    python .\setup.py sdist
 
 #### 脚手架生成的压缩包解压后执行下面命令安装
+
     python setup.py install
 
 #### 脚手架卸载
+
     pip uninstall mvtech-plugin 1.0.0 -y
 
 #### 脚手架使用
+
     执行本地脚手架
     mvtech-plugin -h
+
 ```
 usage: mvtech-plugin [-h] [-v] [-g GENERATE] [-r RUN] [-hp] [-t TEST] [-tb] [-mki]
 
 插件生成器
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -72,12 +80,26 @@
   -g GENERATE, --generate GENERATE
                         插件生成
   -r RUN, --run RUN     运行action
   -hp, --http           启动api接口
   -t TEST, --test TEST  测试
   -tb, --tarball        插件打包
   -mki, --mkimg         制作成docker镜像     
-```
+```  
+
+### 打包出现#!/usr/bin/env python 
+- vi 文件名
+- : set ff = unix
+- : wq
+
+### 打docker镜像包 并且下载过程
+make image
+docker save mvtech/kafka:1.0.0 -o mvtech-kafka-1.0.0.tar
+
+### 生成系统安装包
+make tarball
+
 #### 离线打Docker包
+
 - docker save <myimage>:<tag> | gzip > <myimage>_<tag>.tar.gz
 
-- docker save mvtech/rest:1.0.0 | gzip > mvtech_rest_1.0.0.tar.gz
+- docker save mvtech/rest:1.0.0 | gzip > mvtech_rest_1.0.0.tar.gz
```

### Comparing `mvtech-plugin-1.0.3/core/cli_methods.py` & `mvtech-plugin-1.0.4/core/cli_methods.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.3/core/config.py` & `mvtech-plugin-1.0.4/core/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,23 +75,26 @@
 
 '''
 test_server = FastAPI(title="MVTECH-Plugin Test Server", version="1.0.0", description=desc)
 {% for name, className in init_list %}
 @test_server.post("/actions/{{ name }}",response_model={{ className }}().outputModel,tags=["动作"])
 def action_{{ name }}(action_name:str="{{ name }}",
                       adapter_data:{{ className }}().adapMdl=None,
+                      baseRunModel:ENCODE_STR_ACTION().baseRunModel=None,
                       input_data:{{ className }}().inputModel=None):
     
     clearLog()
 
     adapter_data = adapter_data.dict()
 
+    baseRunModel = baseRunModel.dict()
+
     input_data = input_data.dict()
 
-    output = {{ className }}()._run(input_data,adapter_data)
+    output = {{ className }}()._run(input_data,adapter_data,baseRunModel)
 
     if output["body"].get("error_trace"):
         raise HTTPException(500,detail=output["body"]["error_trace"])
     else:
         output_data = output["body"]["output"]
 
     return output_data
```

### Comparing `mvtech-plugin-1.0.3/core/main.py` & `mvtech-plugin-1.0.4/core/main.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.3/core/res/SDK/base.py` & `mvtech-plugin-1.0.4/core/res/SDK/base.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.3/core/res/SDK/cli.py` & `mvtech-plugin-1.0.4/core/res/SDK/cli.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.3/core/res/SDK/http_run.py` & `mvtech-plugin-1.0.4/core/res/SDK/http_run.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.3/core/res/SDK/run_define.py` & `mvtech-plugin-1.0.4/core/res/SDK/run_define.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.3/core/res/SDK/service_stop.py` & `mvtech-plugin-1.0.4/core/res/SDK/service_stop.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.3/core/res/SDK/web.py` & `mvtech-plugin-1.0.4/core/res/SDK/web.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.3/core/res/project.tar.gz` & `mvtech-plugin-1.0.4/core/res/project.tar.gz`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.3/core/tools.py` & `mvtech-plugin-1.0.4/core/tools.py`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.3/mvtech_plugin.egg-info/PKG-INFO` & `mvtech-plugin-1.0.4/mvtech_plugin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: mvtech-plugin
-Version: 1.0.3
+Version: 1.0.4
 Summary: 插件生成等功能...
 Home-page: https://www.mvtech.cn/market/introduction
 Author: sandy
 Author-email: tong@mvtech.com.cn
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 ### mvtech_plugin
 
 ---
 
 #### 简介
+
 **mvtech_plugin**是MVTech插件脚手架
 
 #### 基本架构结构
+
 ```txt
 .
 ├── actions
 │   ├── __init__.py
 │   ├── ???.py     
 │   ├── models.py
 ├── Dockerfile
@@ -48,34 +50,40 @@
 - ?_plugin.yaml: 模板文件，定义插件．
 - actions/???.py: 根据模板文件定义生成动作．
 - triggers/???.py: 根据模板文件定义生成触发器．
 - actions/models.py 和 triggers/models.py: 模板文件继承pydantic
 - testAPI: FastAPI测试入口
 
 #### 环境要求
+
 - python3.+
 
 #### 安装 依赖
+
 pip install -r requirements.txt
 
 ### 脚手架离线自定义打包安装
 
 #### 脚手架打包
-    python .\setup.py sdist
 
+    python .\setup.py sdist
 
 #### 脚手架生成的压缩包解压后执行下面命令安装
+
     python setup.py install
 
 #### 脚手架卸载
+
     pip uninstall mvtech-plugin 1.0.0 -y
 
 #### 脚手架使用
+
     执行本地脚手架
     mvtech-plugin -h
+
 ```
 usage: mvtech-plugin [-h] [-v] [-g GENERATE] [-r RUN] [-hp] [-t TEST] [-tb] [-mki]
 
 插件生成器
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -83,12 +91,26 @@
   -g GENERATE, --generate GENERATE
                         插件生成
   -r RUN, --run RUN     运行action
   -hp, --http           启动api接口
   -t TEST, --test TEST  测试
   -tb, --tarball        插件打包
   -mki, --mkimg         制作成docker镜像     
-```
+```  
+
+### 打包出现#!/usr/bin/env python 
+- vi 文件名
+- : set ff = unix
+- : wq
+
+### 打docker镜像包 并且下载过程
+make image
+docker save mvtech/kafka:1.0.0 -o mvtech-kafka-1.0.0.tar
+
+### 生成系统安装包
+make tarball
+
 #### 离线打Docker包
+
 - docker save <myimage>:<tag> | gzip > <myimage>_<tag>.tar.gz
 
 - docker save mvtech/rest:1.0.0 | gzip > mvtech_rest_1.0.0.tar.gz
```

### Comparing `mvtech-plugin-1.0.3/mvtech_plugin.egg-info/SOURCES.txt` & `mvtech-plugin-1.0.4/mvtech_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mvtech-plugin-1.0.3/setup.py` & `mvtech-plugin-1.0.4/setup.py`

 * *Files identical despite different names*

