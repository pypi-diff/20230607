# Comparing `tmp/pytest-yaml-yoyo-1.2.4.tar.gz` & `tmp/pytest-yaml-yoyo-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.4.tar", last modified: Tue May 30 00:50:39 2023, max compression
+gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.5.tar", last modified: Wed Jun  7 14:33:02 2023, max compression
```

## Comparing `pytest-yaml-yoyo-1.2.4.tar` & `pytest-yaml-yoyo-1.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 00:50:39.469094 pytest-yaml-yoyo-1.2.4/
--rw-rw-rw-   0        0        0    24830 2023-05-30 00:50:39.468098 pytest-yaml-yoyo-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    24331 2023-05-30 00:38:17.000000 pytest-yaml-yoyo-1.2.4/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-30 00:50:39.469094 pytest-yaml-yoyo-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1347 2023-05-30 00:16:46.000000 pytest-yaml-yoyo-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 00:50:39.431172 pytest-yaml-yoyo-1.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 00:50:39.457126 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/
--rw-rw-rw-   0        0        0        0 2022-11-23 03:54:21.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/__init__.py
--rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/create_funtion.py
--rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/db.py
--rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/exceptions.py
--rw-rw-rw-   0        0        0     4113 2023-05-30 00:16:10.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/extract.py
--rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/http_session.py
--rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/log.py
--rw-rw-rw-   0        0        0     2734 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/my_builtins.py
--rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/parser.py
--rw-rw-rw-   0        0        0     9720 2023-05-29 07:10:40.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/plugin.py
--rw-rw-rw-   0        0        0     4966 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/render_template_obj.py
--rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/report_notify.py
--rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/request_session.py
--rw-rw-rw-   0        0        0    28695 2023-05-30 00:24:02.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/runner.py
--rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/swagger_parser.py
--rw-rw-rw-   0        0        0     3666 2023-05-22 13:47:47.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/validate.py
-drwxrwxrwx   0        0        0        0 2023-05-30 00:50:39.467099 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/
--rw-rw-rw-   0        0        0    24830 2023-05-30 00:50:39.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      839 2023-05-30 00:50:39.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 00:50:39.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-30 00:50:39.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2023-05-30 00:50:39.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-30 00:50:39.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 14:33:02.808215 pytest-yaml-yoyo-1.2.5/
+-rw-rw-rw-   0        0        0    24946 2023-06-07 14:33:02.808215 pytest-yaml-yoyo-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    24447 2023-06-07 14:32:57.000000 pytest-yaml-yoyo-1.2.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-07 14:33:02.809212 pytest-yaml-yoyo-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1347 2023-06-07 14:31:06.000000 pytest-yaml-yoyo-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:33:02.756354 pytest-yaml-yoyo-1.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 14:33:02.796248 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/
+-rw-rw-rw-   0        0        0       20 2023-06-07 14:28:14.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/__init__.py
+-rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/create_funtion.py
+-rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/db.py
+-rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/exceptions.py
+-rw-rw-rw-   0        0        0     4113 2023-05-30 00:16:10.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/extract.py
+-rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/http_session.py
+-rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/log.py
+-rw-rw-rw-   0        0        0     3063 2023-06-07 14:30:58.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/my_builtins.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/parser.py
+-rw-rw-rw-   0        0        0     9783 2023-06-07 14:28:48.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/plugin.py
+-rw-rw-rw-   0        0        0     4966 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/render_template_obj.py
+-rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/report_notify.py
+-rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/request_session.py
+-rw-rw-rw-   0        0        0    28695 2023-05-30 00:24:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/runner.py
+-rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/swagger_parser.py
+-rw-rw-rw-   0        0        0     3666 2023-05-22 13:47:47.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:33:02.806220 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/
+-rw-rw-rw-   0        0        0    24946 2023-06-07 14:33:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2023-06-07 14:33:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:33:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-07 14:33:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2023-06-07 14:33:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-07 14:33:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/top_level.txt
```

### Comparing `pytest-yaml-yoyo-1.2.4/PKG-INFO` & `pytest-yaml-yoyo-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.4
+Version: 1.2.5
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
@@ -206,14 +206,19 @@
 优化以下问题
 
 - 1.解决用例全部 skip 报错问题
 - 2.解决文件上传参数全部传 files 不生效问题
 - 3.数据库配置支持 DB_INFO 参数传字典类型
 - 4.jmespath 表达式支持 length 等函数的提取
 
+v1.2.5 发布 2023-06-07
+
+优化以下问题
+
+- 1.优化参数化路径读取，以项目根路径拼接路径
 
 Installation / 安装
 --------------------------
 最佳环境体验
 
 - Python 3.8, 3.9. 3.10 版本
 - Pytest 7.2.0+
```

### Comparing `pytest-yaml-yoyo-1.2.4/README.rst` & `pytest-yaml-yoyo-1.2.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,19 @@
 优化以下问题
 
 - 1.解决用例全部 skip 报错问题
 - 2.解决文件上传参数全部传 files 不生效问题
 - 3.数据库配置支持 DB_INFO 参数传字典类型
 - 4.jmespath 表达式支持 length 等函数的提取
 
+v1.2.5 发布 2023-06-07
+
+优化以下问题
+
+- 1.优化参数化路径读取，以项目根路径拼接路径
 
 Installation / 安装
 --------------------------
 最佳环境体验
 
 - Python 3.8, 3.9. 3.10 版本
 - Pytest 7.2.0+
```

### Comparing `pytest-yaml-yoyo-1.2.4/setup.py` & `pytest-yaml-yoyo-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 作者-上海悠悠 微信wx:283340479
 # blog地址 https://www.cnblogs.com/yoyoketang/
 """
 
 setup(
     name='pytest-yaml-yoyo',
     url='https://github.com/yoyoketang/pytest-yaml-yoyo',
-    version='v1.2.4',
+    version='v1.2.5',
     author="上海-悠悠",
     author_email='283340479@qq.com',
     description='http/https API run by yaml',
     long_description=open("README.rst", encoding='utf-8').read(),
     package_dir={"": "src"},
     packages=["pytest_yaml_yoyo"],
     classifiers=[
```

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/create_funtion.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/create_funtion.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/db.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/db.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/extract.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/extract.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/http_session.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/http_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/log.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/log.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/my_builtins.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/my_builtins.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,16 +55,24 @@
     :param file_path: 文件路径
     :param title: 第一行是否有title
     :return: list
     """
     f = Path(file_path)
     res = []  # 收集数据的容器
     if not f.exists():
-        log.error(f"文件路径不存在: {f}")
-        return res
+        from . import g
+        if g.get('root_path'):
+            f = g.get('root_path').joinpath(file_path)
+            if not f.exists():
+                log.error(f"文件路径不存在: {f.absolute()}")
+                return res
+        else:
+            log.error(f"文件路径不存在: {f.absolute()}")
+            return res
+    log.info(f"读取文件路径: {f.absolute()}")
     if f.suffix == '.json':
         res = json.loads(f.read_text(encoding='utf8'))
     elif f.suffix in ['.yml', '.yaml']:
         res = yaml.safe_load(f.read_text(encoding='utf8'))
     elif f.suffix in ['.txt', '.csv']:
         with f.open(mode='r', encoding="utf-8") as fp:
             if title:
```

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/plugin.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from . import runner
 from .log import set_log_format
 from .report_notify import ding_ding_notify
 from .create_funtion import import_from_file
 import os
 import platform
 import time
-
-g = {}   # 全局 g 对象，获取项目配置
+from . import g  # 全局 g 对象，获取项目配置
 
 
 @pytest.fixture(scope="session")
 def requests_session(request):
     """全局session 全部用例仅执行一次"""
     s = http_session.HttpSession()
     # max_retries=2 重试2次
@@ -159,14 +158,15 @@
         "--proxies-ip",
         action="store", default=None,
         help="proxies_ip for the  test.",
     )
 
 def pytest_configure(config):  # noqa
     # 配置日志文件和格式
+    g['root_path'] = config.rootpath  # 项目根路径
     set_log_format(config)
     config.addinivalue_line(
         "filterwarnings", "ignore::DeprecationWarning"
     )
     config.addinivalue_line(
         "filterwarnings", "ignore::urllib3.exceptions.InsecureRequestWarning"
     )
```

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/render_template_obj.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/render_template_obj.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/report_notify.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/report_notify.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/request_session.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/request_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/runner.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/runner.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/swagger_parser.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/validate.py` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/validate.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/PKG-INFO` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.4
+Version: 1.2.5
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
@@ -206,14 +206,19 @@
 优化以下问题
 
 - 1.解决用例全部 skip 报错问题
 - 2.解决文件上传参数全部传 files 不生效问题
 - 3.数据库配置支持 DB_INFO 参数传字典类型
 - 4.jmespath 表达式支持 length 等函数的提取
 
+v1.2.5 发布 2023-06-07
+
+优化以下问题
+
+- 1.优化参数化路径读取，以项目根路径拼接路径
 
 Installation / 安装
 --------------------------
 最佳环境体验
 
 - Python 3.8, 3.9. 3.10 版本
 - Pytest 7.2.0+
```

### Comparing `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/SOURCES.txt` & `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

