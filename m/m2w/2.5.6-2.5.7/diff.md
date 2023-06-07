# Comparing `tmp/m2w-2.5.6.tar.gz` & `tmp/m2w-2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m2w-2.5.6.tar", last modified: Tue Jun  6 11:39:12 2023, max compression
+gzip compressed data, was "m2w-2.5.7.tar", last modified: Wed Jun  7 01:25:38 2023, max compression
```

## Comparing `m2w-2.5.6.tar` & `m2w-2.5.7.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 11:39:12.324732 m2w-2.5.6/
--rw-rw-rw-   0        0        0     9202 2023-06-06 11:39:12.323732 m2w-2.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     8662 2023-06-06 10:37:28.000000 m2w-2.5.6/README.md
--rw-rw-rw-   0        0        0     1091 2022-12-04 08:15:05.000000 m2w-2.5.6/license.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 11:39:12.297726 m2w-2.5.6/m2w/
--rw-rw-rw-   0        0        0      127 2023-02-15 16:04:18.000000 m2w-2.5.6/m2w/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:39:12.309729 m2w-2.5.6/m2w/config/
--rw-rw-rw-   0        0        0      200 2023-04-23 10:06:12.000000 m2w-2.5.6/m2w/config/__init__.py
--rw-rw-rw-   0        0        0     2556 2023-06-05 04:00:39.000000 m2w-2.5.6/m2w/config/config.py
--rw-rw-rw-   0        0        0      496 2023-04-23 10:06:12.000000 m2w-2.5.6/m2w/json2.py
--rw-rw-rw-   0        0        0     1070 2023-02-15 16:04:18.000000 m2w-2.5.6/m2w/md5.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:39:12.321731 m2w-2.5.6/m2w/rest_api/
--rw-rw-rw-   0        0        0      180 2023-04-23 10:06:12.000000 m2w-2.5.6/m2w/rest_api/__init__.py
--rw-rw-rw-   0        0        0     1385 2023-06-05 02:18:13.000000 m2w-2.5.6/m2w/rest_api/articles.py
--rw-rw-rw-   0        0        0     2091 2023-06-05 02:16:44.000000 m2w-2.5.6/m2w/rest_api/categories.py
--rw-rw-rw-   0        0        0     2637 2023-06-06 10:59:07.000000 m2w-2.5.6/m2w/rest_api/create.py
--rw-rw-rw-   0        0        0     4432 2023-06-06 11:30:13.000000 m2w-2.5.6/m2w/rest_api/rest_api.py
--rw-rw-rw-   0        0        0     2030 2023-06-05 02:17:51.000000 m2w-2.5.6/m2w/rest_api/tags.py
--rw-rw-rw-   0        0        0     2949 2023-06-06 11:31:44.000000 m2w-2.5.6/m2w/rest_api/update.py
--rw-rw-rw-   0        0        0     9666 2023-02-15 16:04:18.000000 m2w-2.5.6/m2w/up.py
--rw-rw-rw-   0        0        0     3254 2023-06-06 11:18:01.000000 m2w-2.5.6/m2w/update.py
--rw-rw-rw-   0        0        0     3709 2023-02-15 16:04:18.000000 m2w-2.5.6/m2w/upload.py
--rw-rw-rw-   0        0        0      892 2023-02-15 16:04:18.000000 m2w-2.5.6/m2w/wp.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:39:12.306727 m2w-2.5.6/m2w.egg-info/
--rw-rw-rw-   0        0        0     9202 2023-06-06 11:39:12.000000 m2w-2.5.6/m2w.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-06-06 11:39:12.000000 m2w-2.5.6/m2w.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 11:39:12.000000 m2w-2.5.6/m2w.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-06-06 11:39:12.000000 m2w-2.5.6/m2w.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-06 11:39:12.000000 m2w-2.5.6/m2w.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 11:39:12.324732 m2w-2.5.6/setup.cfg
--rw-rw-rw-   0        0        0     2898 2023-06-06 11:15:31.000000 m2w-2.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 01:25:38.480287 m2w-2.5.7/
+-rw-rw-rw-   0        0        0     9202 2023-06-07 01:25:38.479286 m2w-2.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8662 2023-06-06 10:37:28.000000 m2w-2.5.7/README.md
+-rw-rw-rw-   0        0        0     1091 2022-12-04 08:15:05.000000 m2w-2.5.7/license.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 01:25:38.451288 m2w-2.5.7/m2w/
+-rw-rw-rw-   0        0        0      152 2023-06-06 15:56:02.000000 m2w-2.5.7/m2w/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 01:25:38.463457 m2w-2.5.7/m2w/config/
+-rw-rw-rw-   0        0        0      200 2023-04-23 10:06:12.000000 m2w-2.5.7/m2w/config/__init__.py
+-rw-rw-rw-   0        0        0     2556 2023-06-05 04:00:39.000000 m2w-2.5.7/m2w/config/config.py
+-rw-rw-rw-   0        0        0      496 2023-04-23 10:06:12.000000 m2w-2.5.7/m2w/json2.py
+-rw-rw-rw-   0        0        0     1070 2023-02-15 16:04:18.000000 m2w-2.5.7/m2w/md5.py
+drwxrwxrwx   0        0        0        0 2023-06-07 01:25:38.476281 m2w-2.5.7/m2w/rest_api/
+-rw-rw-rw-   0        0        0      180 2023-04-23 10:06:12.000000 m2w-2.5.7/m2w/rest_api/__init__.py
+-rw-rw-rw-   0        0        0     1385 2023-06-05 02:18:13.000000 m2w-2.5.7/m2w/rest_api/articles.py
+-rw-rw-rw-   0        0        0     2091 2023-06-05 02:16:44.000000 m2w-2.5.7/m2w/rest_api/categories.py
+-rw-rw-rw-   0        0        0     2637 2023-06-06 10:59:07.000000 m2w-2.5.7/m2w/rest_api/create.py
+-rw-rw-rw-   0        0        0     4432 2023-06-06 11:30:13.000000 m2w-2.5.7/m2w/rest_api/rest_api.py
+-rw-rw-rw-   0        0        0     2030 2023-06-05 02:17:51.000000 m2w-2.5.7/m2w/rest_api/tags.py
+-rw-rw-rw-   0        0        0     2949 2023-06-06 11:31:44.000000 m2w-2.5.7/m2w/rest_api/update.py
+-rw-rw-rw-   0        0        0     5221 2023-06-07 01:12:34.000000 m2w-2.5.7/m2w/up.py
+-rw-rw-rw-   0        0        0     9675 2023-06-06 15:23:34.000000 m2w-2.5.7/m2w/up_password.py
+-rw-rw-rw-   0        0        0     3254 2023-06-06 11:18:01.000000 m2w-2.5.7/m2w/update.py
+-rw-rw-rw-   0        0        0     3709 2023-02-15 16:04:18.000000 m2w-2.5.7/m2w/upload.py
+-rw-rw-rw-   0        0        0      892 2023-02-15 16:04:18.000000 m2w-2.5.7/m2w/wp.py
+drwxrwxrwx   0        0        0        0 2023-06-07 01:25:38.459456 m2w-2.5.7/m2w.egg-info/
+-rw-rw-rw-   0        0        0     9202 2023-06-07 01:25:38.000000 m2w-2.5.7/m2w.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-06-07 01:25:38.000000 m2w-2.5.7/m2w.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 01:25:38.000000 m2w-2.5.7/m2w.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-07 01:25:38.000000 m2w-2.5.7/m2w.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-07 01:25:38.000000 m2w-2.5.7/m2w.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 01:25:38.480287 m2w-2.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     2971 2023-06-07 01:25:06.000000 m2w-2.5.7/setup.py
```

### Comparing `m2w-2.5.6/PKG-INFO` & `m2w-2.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: m2w
-Version: 2.5.6
-Summary: 2.5.6: Optimize organization of m2w configuration. Both password and REST API supported!
+Version: 2.5.7
+Summary: 2.5.7: Optimize organization of m2w configuration. Both password and REST API supported!
 Home-page: https://github.com/huangwb8/m2w
 Author: ['Bensz', 'FoxSuzuran']
 Author-email: hwb2012@qq.com
 Keywords: markdown,wordpress,xmlrpc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: m2w Version: 2.5.6 Summary: 2.5.6: Optimize
+Metadata-Version: 2.1 Name: m2w Version: 2.5.7 Summary: 2.5.7: Optimize
 organization of m2w configuration. Both password and REST API supported! Home-
 page: https://github.com/huangwb8/m2w Author: ['Bensz', 'FoxSuzuran'] Author-
 email: hwb2012@qq.com Keywords: markdown,wordpress,xmlrpc Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7.6
 Description-Content-Type: text/markdown License-File: license.txt ### [English]
 (https://github.com/huangwb8/m2w) | [ç®ä½ä¸­æ](https://github.com/huangwb8/
```

### Comparing `m2w-2.5.6/README.md` & `m2w-2.5.7/README.md`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/license.txt` & `m2w-2.5.7/license.txt`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/m2w/config/config.py` & `m2w-2.5.7/m2w/config/config.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/m2w/md5.py` & `m2w-2.5.7/m2w/md5.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/m2w/rest_api/articles.py` & `m2w-2.5.7/m2w/rest_api/articles.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/m2w/rest_api/categories.py` & `m2w-2.5.7/m2w/rest_api/categories.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/m2w/rest_api/create.py` & `m2w-2.5.7/m2w/rest_api/create.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/m2w/rest_api/rest_api.py` & `m2w-2.5.7/m2w/rest_api/rest_api.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/m2w/rest_api/tags.py` & `m2w-2.5.7/m2w/rest_api/tags.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/m2w/rest_api/update.py` & `m2w-2.5.7/m2w/rest_api/update.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/m2w/up.py` & `m2w-2.5.7/m2w/up_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 print('No changed legacy markdown files. Ignored.')
 
         # Output
         result = {"new": list(new), "legacy": list(md5_filter.keys())}  #
         return result
 
 
-def up(client, md_upload, md_update, post_metadata, force_upload=False, verbose=True):
+def up_password(client, md_upload, md_update, post_metadata, force_upload=False, verbose=True):
     """
     ### Description
     Upload or update markdown files to your WordPress site.
 
     ### Parameters
     + client: The return of m2w.wp.wp_xmlrpc.
     + md_upload: String. The path of new markdown files.
```

### Comparing `m2w-2.5.6/m2w/update.py` & `m2w-2.5.7/m2w/update.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/m2w/upload.py` & `m2w-2.5.7/m2w/upload.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/m2w/wp.py` & `m2w-2.5.7/m2w/wp.py`

 * *Files identical despite different names*

### Comparing `m2w-2.5.6/m2w.egg-info/PKG-INFO` & `m2w-2.5.7/m2w.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: m2w
-Version: 2.5.6
-Summary: 2.5.6: Optimize organization of m2w configuration. Both password and REST API supported!
+Version: 2.5.7
+Summary: 2.5.7: Optimize organization of m2w configuration. Both password and REST API supported!
 Home-page: https://github.com/huangwb8/m2w
 Author: ['Bensz', 'FoxSuzuran']
 Author-email: hwb2012@qq.com
 Keywords: markdown,wordpress,xmlrpc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: m2w Version: 2.5.6 Summary: 2.5.6: Optimize
+Metadata-Version: 2.1 Name: m2w Version: 2.5.7 Summary: 2.5.7: Optimize
 organization of m2w configuration. Both password and REST API supported! Home-
 page: https://github.com/huangwb8/m2w Author: ['Bensz', 'FoxSuzuran'] Author-
 email: hwb2012@qq.com Keywords: markdown,wordpress,xmlrpc Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7.6
 Description-Content-Type: text/markdown License-File: license.txt ### [English]
 (https://github.com/huangwb8/m2w) | [ç®ä½ä¸­æ](https://github.com/huangwb8/
```

### Comparing `m2w-2.5.6/setup.py` & `m2w-2.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
 + 其次，你需要在PyPi上注册一个账号，并登录。
 
 + 接下来，打开命令行界面，进入到你的项目根目录。
 
 + 输入"pip install twine"来安装twine工具。 必要时可更新工具包：pip install --upgrade twine setuptools wheel
 
-+ 使用"python setup.py sdist"命令来生成项目的源代码包。 如果要测试该包，可运行类似命令： python setup.py sdist; pip install .\dist\m2w-2.5.6.tar.gz
++ 使用"python setup.py sdist"命令来生成项目的源代码包。 如果要测试该包，可运行类似命令： python setup.py sdist; pip install .\dist\m2w-2.5.7.tar.gz
 
 + 使用"python setup.py bdist_wheel"命令来生成项目的长描述。
 
-+ 输入"twine upload dist/* --verbose"来上传项目的源代码包。
++ 先完成Github仓库的更新和加tag。最后再上传至PyPi。输入"twine upload dist/*2.5.7* --verbose"来上传项目的源代码包。
 
 + 在上传过程中，你需要输入你在PyPi上注册的用户名和密码。
 
 一旦上传完成，你的项目就已经成功发布到了PyPi上。你可以在PyPi的网站上搜索你的项目名称，找到你的项目，并查看它的安装和使用说明。
 
 ### My environment
 
@@ -41,15 +41,15 @@
 ### How to install
 + pip install --upgrade -i https://pypi.org/simple m2w 
 + pip install -i https://pypi.org/simple m2w==2.2.11
 + pip install m2w 
 
 """
 
-VERSION = "2.5.6"
+VERSION = "2.5.7"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="m2w",
     version=VERSION,
```

