# Comparing `tmp/PyMobileProvision-1.4.3.tar.gz` & `tmp/PyMobileProvision-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyMobileProvision-1.4.3.tar", last modified: Sun Jan 16 17:44:47 2022, max compression
+gzip compressed data, was "PyMobileProvision-1.4.4.tar", last modified: Wed Jun  7 04:47:03 2023, max compression
```

## Comparing `PyMobileProvision-1.4.3.tar` & `PyMobileProvision-1.4.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2022-01-16 17:44:47.000000 PyMobileProvision-1.4.3/
--rw-r--r--   0 shaowei    (501) staff       (20)     6142 2022-01-16 17:44:47.000000 PyMobileProvision-1.4.3/PKG-INFO
-drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2022-01-16 17:44:47.000000 PyMobileProvision-1.4.3/PyMobileProvision.egg-info/
--rw-r--r--   0 shaowei    (501) staff       (20)     6142 2022-01-16 17:44:47.000000 PyMobileProvision-1.4.3/PyMobileProvision.egg-info/PKG-INFO
--rw-r--r--   0 shaowei    (501) staff       (20)      371 2022-01-16 17:44:47.000000 PyMobileProvision-1.4.3/PyMobileProvision.egg-info/SOURCES.txt
--rw-r--r--   0 shaowei    (501) staff       (20)        1 2022-01-16 17:44:47.000000 PyMobileProvision-1.4.3/PyMobileProvision.egg-info/dependency_links.txt
--rw-r--r--   0 shaowei    (501) staff       (20)       66 2022-01-16 17:44:47.000000 PyMobileProvision-1.4.3/PyMobileProvision.egg-info/entry_points.txt
--rw-r--r--   0 shaowei    (501) staff       (20)       19 2022-01-16 17:44:47.000000 PyMobileProvision-1.4.3/PyMobileProvision.egg-info/requires.txt
--rw-r--r--   0 shaowei    (501) staff       (20)       16 2022-01-16 17:44:47.000000 PyMobileProvision-1.4.3/PyMobileProvision.egg-info/top_level.txt
--rw-r--r--   0 shaowei    (501) staff       (20)     4267 2022-01-16 17:40:57.000000 PyMobileProvision-1.4.3/README.md
-drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2022-01-16 17:44:47.000000 PyMobileProvision-1.4.3/mobileprovision/
--rw-r--r--   0 shaowei    (501) staff       (20)      121 2020-03-29 09:08:29.000000 PyMobileProvision-1.4.3/mobileprovision/__init__.py
--rw-r--r--   0 shaowei    (501) staff       (20)     2992 2020-03-29 09:08:29.000000 PyMobileProvision-1.4.3/mobileprovision/command.py
--rwxr-xr-x   0 shaowei    (501) staff       (20)     9883 2022-01-04 15:54:11.000000 PyMobileProvision-1.4.3/mobileprovision/parser.py
--rw-r--r--   0 shaowei    (501) staff       (20)     2499 2020-03-29 09:08:29.000000 PyMobileProvision-1.4.3/mobileprovision/util.py
--rw-r--r--   0 shaowei    (501) staff       (20)       38 2022-01-16 17:44:47.000000 PyMobileProvision-1.4.3/setup.cfg
--rw-r--r--   0 shaowei    (501) staff       (20)     1605 2022-01-16 17:40:57.000000 PyMobileProvision-1.4.3/setup.py
+drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-06-07 04:47:03.477977 PyMobileProvision-1.4.4/
+-rw-r--r--   0 shaowei    (501) staff       (20)     1065 2019-05-17 03:04:35.000000 PyMobileProvision-1.4.4/LICENSE
+-rw-r--r--   0 shaowei    (501) staff       (20)     5257 2023-06-07 04:47:03.477780 PyMobileProvision-1.4.4/PKG-INFO
+drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-06-07 04:47:03.476199 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/
+-rw-r--r--   0 shaowei    (501) staff       (20)     5257 2023-06-07 04:47:03.000000 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/PKG-INFO
+-rw-r--r--   0 shaowei    (501) staff       (20)      379 2023-06-07 04:47:03.000000 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/SOURCES.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)        1 2023-06-07 04:47:03.000000 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/dependency_links.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)       66 2023-06-07 04:47:03.000000 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/entry_points.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)       19 2023-06-07 04:47:03.000000 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/requires.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)       16 2023-06-07 04:47:03.000000 PyMobileProvision-1.4.4/PyMobileProvision.egg-info/top_level.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)     4267 2023-06-07 04:39:55.000000 PyMobileProvision-1.4.4/README.md
+drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-06-07 04:47:03.477341 PyMobileProvision-1.4.4/mobileprovision/
+-rw-r--r--   0 shaowei    (501) staff       (20)      121 2019-11-20 12:06:23.000000 PyMobileProvision-1.4.4/mobileprovision/__init__.py
+-rw-r--r--   0 shaowei    (501) staff       (20)     2992 2019-11-21 12:23:14.000000 PyMobileProvision-1.4.4/mobileprovision/command.py
+-rwxr-xr-x   0 shaowei    (501) staff       (20)    10097 2023-06-07 04:44:55.000000 PyMobileProvision-1.4.4/mobileprovision/parser.py
+-rw-r--r--   0 shaowei    (501) staff       (20)     2499 2019-11-27 03:30:49.000000 PyMobileProvision-1.4.4/mobileprovision/util.py
+-rw-r--r--   0 shaowei    (501) staff       (20)       38 2023-06-07 04:47:03.478047 PyMobileProvision-1.4.4/setup.cfg
+-rw-r--r--   0 shaowei    (501) staff       (20)     1605 2023-06-07 04:40:01.000000 PyMobileProvision-1.4.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyMobileProvision-1.4.3/PKG-INFO` & `PyMobileProvision-1.4.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,128 +1,15 @@
 Metadata-Version: 2.1
 Name: PyMobileProvision
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python3, parse ".mobileprovision" file in MacOS System;
 Home-page: https://github.com/shede333/PyMobileProvision
 Author: shede333
 Author-email: 333wshw@163.com
 License: UNKNOWN
-Description: # PyMobileProvision
-        
-        
-        parse ".mobileprovision" file in MacOS System;      
-        解析 MacOS 系统里，iOS和Mac开发常用到的".mobileprovision"文件，提取出里面的"plist"格式的内容
-        
-        仅支持 **Python3**，Python2版本见：[Py2MobileProvision](https://github.com/shede333/Py2MobileProvision)
-        
-        
-        ## Install
-        
-        ```
-        
-        # 注意：pip要用最新的（version>=21.0），否则，在安装cryptography依赖包时会失败
-        pip install PyMobileProvision
-        
-        ```
-        
-        ## Example Modules:
-        
-        ```python
-        
-        from mobileprovision import MobileProvisionModel
-        
-        mp_file_path = "/Users/shede333/Desktop/test.mobileprovision"
-        mp_model = MobileProvisionModel(mp_file_path)
-        
-        # 也支持直接使用mobileprovision文件内容来创建model，AppStore Connect API一般会需要这种情况：
-        # from pathlib import Path
-        # file_content = Path(mp_file_path).read_text(encoding="ascii", errors="ignore")
-        # mp_model = MobileProvisionModel(file_content)
-        
-        print(mp_model)  # 打印mobileprovision文件的详细信息
-        print(mp_model.app_id_prefix)  # appID的前缀
-        print(mp_model.app_id(is_need_prefix=True))  # app的BundleID，带app_id_prefix前缀
-        print(mp_model["name"])  # mobileprovision的"Name"属性（属性不区分大小写）
-        print(mp_model.date_is_valid())  # 现在的是否过期
-        print(mp_model.creation_timestamp)  # 证书创建时间（时间戳，int值）
-        # ......还有很多其他属性.......
-        
-        # 将int时间戳 转换为 本地日期时间
-        from datetime import datetime
-        local_dt = datetime.fromtimestamp(mp_model.creation_timestamp)
-        print(local_dt)  
-        
-        # 打印mobileprovision文件里包含的cer公钥证书信息
-        print(mp_model.developer_certificates)
-        
-        # mobileprovision文件是否包含（支持）device_id设备
-        device_id = "00008020-000XXXXXXXXXXXXXX"  # 设备的唯一ID
-        print(mp_model.contain_device_id(device_id))  
-        
-        # 转换为plist格式文件
-        dst_plist_path = "/Users/shede333/Desktop/test.plist"
-        mp_model.convert_to_plist_file(dst_plist_path)
-        
-        # 导出entitlements.plist文件信息
-        ent_dst_path = "Users/shede333/Desktop/entitlements.plist"
-        mp_model.export_entitlements_file(ent_dst_path)
-        
-        ```
-        
-        ## Example CLI:
-        
-        ```shell
-        
-        mobileprovision -h 
-        
-        输出：
-        
-        usage: OKEx工程里的多语言国际化相关的便捷操作 [-h] {import,parse,convert,entitlements} ...
-        
-        positional arguments:
-          {import,parse,convert,entitlements}
-                                支持的命令如下：
-            import              导入mobileprovision文件到系统默认路径里
-            parse               解析、打印mobileprovision文件里的内容
-            convert             转换mobileprovision文件为plist文件
-            entitlements        打印/导出 mobileprovision文件里 entitlements信息
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-        
-        
-        ```
-        
-        
-        ## 公司招聘：
-        
-        欧科云链招募新同学：  
-        可分布式`居家办公`，行业龙头，高薪资，年终奖优越，拒绝加班，**1075工作制**，公司提供团建费每人每周200元，还提供各种福利；  
-        各地同学均可在家办公（**拿北京薪资+社保，在老家工作+生活**），也可在北京公司内（海淀上地）办公；  
-        支持远程 **线上面试**；  
-        **web前端、后端、移动端**均在招人，欢迎加入团队~  
-        **简历**可发送至：<wshw333@gmail.com>  
-        微信搜索“shede333sw”咨询岗位详情；  
-        
-        移动端招聘详情如下：  
-        
-        iOS工程师任职要求：  
-        1.本科以上学历，可使用英文交流者加分；  
-        2.三年以上的iOS平台研发经验，良好的代码编写规范。有已上线App开发经验加分，有跨平台开发经验加分；  
-        3.精通Object-C/Swift语言，熟悉账户Xcode等开发佛能根据，熟练掌握使用iOS SDK，熟悉Go、Python、Ruby语言加分；  
-        4.有高性能客户端编程经验，有性能调优经历加分；  
-        5.熟悉iOS主流开源框架，并学习、研究过实现原理和源码；  
-        
-        Android工程师任职要求：  
-        1.本科以上学历，可使用英文交流者加分；  
-        2.三年以上Android开发经验；  
-        3.熟悉Android常用控件的使用并理解其原理；  
-        4.熟悉Android Framework原理，阅读过Android源代码者优先；  
-        5.对java、Kotlin、基本数据结构、计算机网络有较为深入的了解；  
-        
 Keywords: mobileprovision mobile provision MobileProvision profile profiles
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
@@ -130,7 +17,123 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyMobileProvision
+
+
+parse ".mobileprovision" file in MacOS System;      
+解析 MacOS 系统里，iOS和Mac开发常用到的".mobileprovision"文件，提取出里面的"plist"格式的内容
+
+仅支持 **Python3**，Python2版本见：[Py2MobileProvision](https://github.com/shede333/Py2MobileProvision)
+
+
+## Install
+
+```
+
+# 注意：pip要用最新的（version>=21.0），否则，在安装cryptography依赖包时会失败
+pip install PyMobileProvision
+
+```
+
+## Example Modules:
+
+```python
+
+from mobileprovision import MobileProvisionModel
+
+mp_file_path = "/Users/shede333/Desktop/test.mobileprovision"
+mp_model = MobileProvisionModel(mp_file_path)
+
+# 也支持直接使用mobileprovision文件内容来创建model，AppStore Connect API一般会需要这种情况：
+# from pathlib import Path
+# file_content = Path(mp_file_path).read_text(encoding="ascii", errors="ignore")
+# mp_model = MobileProvisionModel(file_content)
+
+print(mp_model)  # 打印mobileprovision文件的详细信息
+print(mp_model.app_id_prefix)  # appID的前缀
+print(mp_model.app_id(is_need_prefix=True))  # app的BundleID，带app_id_prefix前缀
+print(mp_model["name"])  # mobileprovision的"Name"属性（属性不区分大小写）
+print(mp_model.date_is_valid())  # 现在的是否过期
+print(mp_model.creation_timestamp)  # 证书创建时间（时间戳，int值）
+# ......还有很多其他属性.......
+
+# 将int时间戳 转换为 本地日期时间
+from datetime import datetime
+local_dt = datetime.fromtimestamp(mp_model.creation_timestamp)
+print(local_dt)  
+
+# 打印mobileprovision文件里包含的cer公钥证书信息
+print(mp_model.developer_certificates)
+
+# mobileprovision文件是否包含（支持）device_id设备
+device_id = "00008020-000XXXXXXXXXXXXXX"  # 设备的唯一ID
+print(mp_model.contain_device_id(device_id))  
+
+# 转换为plist格式文件
+dst_plist_path = "/Users/shede333/Desktop/test.plist"
+mp_model.convert_to_plist_file(dst_plist_path)
+
+# 导出entitlements.plist文件信息
+ent_dst_path = "Users/shede333/Desktop/entitlements.plist"
+mp_model.export_entitlements_file(ent_dst_path)
+
+```
+
+## Example CLI:
+
+```shell
+
+mobileprovision -h 
+
+输出：
+
+usage: OKEx工程里的多语言国际化相关的便捷操作 [-h] {import,parse,convert,entitlements} ...
+
+positional arguments:
+  {import,parse,convert,entitlements}
+                        支持的命令如下：
+    import              导入mobileprovision文件到系统默认路径里
+    parse               解析、打印mobileprovision文件里的内容
+    convert             转换mobileprovision文件为plist文件
+    entitlements        打印/导出 mobileprovision文件里 entitlements信息
+
+optional arguments:
+  -h, --help            show this help message and exit
+
+
+```
+
+
+## 公司招聘：
+
+欧科云链招募新同学：  
+可分布式`居家办公`，行业龙头，高薪资，年终奖优越，拒绝加班，**1075工作制**，公司提供团建费每人每周200元，还提供各种福利；  
+各地同学均可在家办公（**拿北京薪资+社保，在老家工作+生活**），也可在北京公司内（海淀上地）办公；  
+支持远程 **线上面试**；  
+**web前端、后端、移动端**均在招人，欢迎加入团队~  
+**简历**可发送至：<wshw333@gmail.com>  
+微信搜索“shede333sw”咨询岗位详情；  
+
+移动端招聘详情如下：  
+
+iOS工程师任职要求：  
+1.本科以上学历，可使用英文交流者加分；  
+2.三年以上的iOS平台研发经验，良好的代码编写规范。有已上线App开发经验加分，有跨平台开发经验加分；  
+3.精通Object-C/Swift语言，熟悉账户Xcode等开发佛能根据，熟练掌握使用iOS SDK，熟悉Go、Python、Ruby语言加分；  
+4.有高性能客户端编程经验，有性能调优经历加分；  
+5.熟悉iOS主流开源框架，并学习、研究过实现原理和源码；  
+
+Android工程师任职要求：  
+1.本科以上学历，可使用英文交流者加分；  
+2.三年以上Android开发经验；  
+3.熟悉Android常用控件的使用并理解其原理；  
+4.熟悉Android Framework原理，阅读过Android源代码者优先；  
+5.对java、Kotlin、基本数据结构、计算机网络有较为深入的了解；  
+
+
```

### Comparing `PyMobileProvision-1.4.3/PyMobileProvision.egg-info/PKG-INFO` & `PyMobileProvision-1.4.4/PyMobileProvision.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,128 +1,15 @@
 Metadata-Version: 2.1
 Name: PyMobileProvision
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python3, parse ".mobileprovision" file in MacOS System;
 Home-page: https://github.com/shede333/PyMobileProvision
 Author: shede333
 Author-email: 333wshw@163.com
 License: UNKNOWN
-Description: # PyMobileProvision
-        
-        
-        parse ".mobileprovision" file in MacOS System;      
-        解析 MacOS 系统里，iOS和Mac开发常用到的".mobileprovision"文件，提取出里面的"plist"格式的内容
-        
-        仅支持 **Python3**，Python2版本见：[Py2MobileProvision](https://github.com/shede333/Py2MobileProvision)
-        
-        
-        ## Install
-        
-        ```
-        
-        # 注意：pip要用最新的（version>=21.0），否则，在安装cryptography依赖包时会失败
-        pip install PyMobileProvision
-        
-        ```
-        
-        ## Example Modules:
-        
-        ```python
-        
-        from mobileprovision import MobileProvisionModel
-        
-        mp_file_path = "/Users/shede333/Desktop/test.mobileprovision"
-        mp_model = MobileProvisionModel(mp_file_path)
-        
-        # 也支持直接使用mobileprovision文件内容来创建model，AppStore Connect API一般会需要这种情况：
-        # from pathlib import Path
-        # file_content = Path(mp_file_path).read_text(encoding="ascii", errors="ignore")
-        # mp_model = MobileProvisionModel(file_content)
-        
-        print(mp_model)  # 打印mobileprovision文件的详细信息
-        print(mp_model.app_id_prefix)  # appID的前缀
-        print(mp_model.app_id(is_need_prefix=True))  # app的BundleID，带app_id_prefix前缀
-        print(mp_model["name"])  # mobileprovision的"Name"属性（属性不区分大小写）
-        print(mp_model.date_is_valid())  # 现在的是否过期
-        print(mp_model.creation_timestamp)  # 证书创建时间（时间戳，int值）
-        # ......还有很多其他属性.......
-        
-        # 将int时间戳 转换为 本地日期时间
-        from datetime import datetime
-        local_dt = datetime.fromtimestamp(mp_model.creation_timestamp)
-        print(local_dt)  
-        
-        # 打印mobileprovision文件里包含的cer公钥证书信息
-        print(mp_model.developer_certificates)
-        
-        # mobileprovision文件是否包含（支持）device_id设备
-        device_id = "00008020-000XXXXXXXXXXXXXX"  # 设备的唯一ID
-        print(mp_model.contain_device_id(device_id))  
-        
-        # 转换为plist格式文件
-        dst_plist_path = "/Users/shede333/Desktop/test.plist"
-        mp_model.convert_to_plist_file(dst_plist_path)
-        
-        # 导出entitlements.plist文件信息
-        ent_dst_path = "Users/shede333/Desktop/entitlements.plist"
-        mp_model.export_entitlements_file(ent_dst_path)
-        
-        ```
-        
-        ## Example CLI:
-        
-        ```shell
-        
-        mobileprovision -h 
-        
-        输出：
-        
-        usage: OKEx工程里的多语言国际化相关的便捷操作 [-h] {import,parse,convert,entitlements} ...
-        
-        positional arguments:
-          {import,parse,convert,entitlements}
-                                支持的命令如下：
-            import              导入mobileprovision文件到系统默认路径里
-            parse               解析、打印mobileprovision文件里的内容
-            convert             转换mobileprovision文件为plist文件
-            entitlements        打印/导出 mobileprovision文件里 entitlements信息
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-        
-        
-        ```
-        
-        
-        ## 公司招聘：
-        
-        欧科云链招募新同学：  
-        可分布式`居家办公`，行业龙头，高薪资，年终奖优越，拒绝加班，**1075工作制**，公司提供团建费每人每周200元，还提供各种福利；  
-        各地同学均可在家办公（**拿北京薪资+社保，在老家工作+生活**），也可在北京公司内（海淀上地）办公；  
-        支持远程 **线上面试**；  
-        **web前端、后端、移动端**均在招人，欢迎加入团队~  
-        **简历**可发送至：<wshw333@gmail.com>  
-        微信搜索“shede333sw”咨询岗位详情；  
-        
-        移动端招聘详情如下：  
-        
-        iOS工程师任职要求：  
-        1.本科以上学历，可使用英文交流者加分；  
-        2.三年以上的iOS平台研发经验，良好的代码编写规范。有已上线App开发经验加分，有跨平台开发经验加分；  
-        3.精通Object-C/Swift语言，熟悉账户Xcode等开发佛能根据，熟练掌握使用iOS SDK，熟悉Go、Python、Ruby语言加分；  
-        4.有高性能客户端编程经验，有性能调优经历加分；  
-        5.熟悉iOS主流开源框架，并学习、研究过实现原理和源码；  
-        
-        Android工程师任职要求：  
-        1.本科以上学历，可使用英文交流者加分；  
-        2.三年以上Android开发经验；  
-        3.熟悉Android常用控件的使用并理解其原理；  
-        4.熟悉Android Framework原理，阅读过Android源代码者优先；  
-        5.对java、Kotlin、基本数据结构、计算机网络有较为深入的了解；  
-        
 Keywords: mobileprovision mobile provision MobileProvision profile profiles
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
@@ -130,7 +17,123 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyMobileProvision
+
+
+parse ".mobileprovision" file in MacOS System;      
+解析 MacOS 系统里，iOS和Mac开发常用到的".mobileprovision"文件，提取出里面的"plist"格式的内容
+
+仅支持 **Python3**，Python2版本见：[Py2MobileProvision](https://github.com/shede333/Py2MobileProvision)
+
+
+## Install
+
+```
+
+# 注意：pip要用最新的（version>=21.0），否则，在安装cryptography依赖包时会失败
+pip install PyMobileProvision
+
+```
+
+## Example Modules:
+
+```python
+
+from mobileprovision import MobileProvisionModel
+
+mp_file_path = "/Users/shede333/Desktop/test.mobileprovision"
+mp_model = MobileProvisionModel(mp_file_path)
+
+# 也支持直接使用mobileprovision文件内容来创建model，AppStore Connect API一般会需要这种情况：
+# from pathlib import Path
+# file_content = Path(mp_file_path).read_text(encoding="ascii", errors="ignore")
+# mp_model = MobileProvisionModel(file_content)
+
+print(mp_model)  # 打印mobileprovision文件的详细信息
+print(mp_model.app_id_prefix)  # appID的前缀
+print(mp_model.app_id(is_need_prefix=True))  # app的BundleID，带app_id_prefix前缀
+print(mp_model["name"])  # mobileprovision的"Name"属性（属性不区分大小写）
+print(mp_model.date_is_valid())  # 现在的是否过期
+print(mp_model.creation_timestamp)  # 证书创建时间（时间戳，int值）
+# ......还有很多其他属性.......
+
+# 将int时间戳 转换为 本地日期时间
+from datetime import datetime
+local_dt = datetime.fromtimestamp(mp_model.creation_timestamp)
+print(local_dt)  
+
+# 打印mobileprovision文件里包含的cer公钥证书信息
+print(mp_model.developer_certificates)
+
+# mobileprovision文件是否包含（支持）device_id设备
+device_id = "00008020-000XXXXXXXXXXXXXX"  # 设备的唯一ID
+print(mp_model.contain_device_id(device_id))  
+
+# 转换为plist格式文件
+dst_plist_path = "/Users/shede333/Desktop/test.plist"
+mp_model.convert_to_plist_file(dst_plist_path)
+
+# 导出entitlements.plist文件信息
+ent_dst_path = "Users/shede333/Desktop/entitlements.plist"
+mp_model.export_entitlements_file(ent_dst_path)
+
+```
+
+## Example CLI:
+
+```shell
+
+mobileprovision -h 
+
+输出：
+
+usage: OKEx工程里的多语言国际化相关的便捷操作 [-h] {import,parse,convert,entitlements} ...
+
+positional arguments:
+  {import,parse,convert,entitlements}
+                        支持的命令如下：
+    import              导入mobileprovision文件到系统默认路径里
+    parse               解析、打印mobileprovision文件里的内容
+    convert             转换mobileprovision文件为plist文件
+    entitlements        打印/导出 mobileprovision文件里 entitlements信息
+
+optional arguments:
+  -h, --help            show this help message and exit
+
+
+```
+
+
+## 公司招聘：
+
+欧科云链招募新同学：  
+可分布式`居家办公`，行业龙头，高薪资，年终奖优越，拒绝加班，**1075工作制**，公司提供团建费每人每周200元，还提供各种福利；  
+各地同学均可在家办公（**拿北京薪资+社保，在老家工作+生活**），也可在北京公司内（海淀上地）办公；  
+支持远程 **线上面试**；  
+**web前端、后端、移动端**均在招人，欢迎加入团队~  
+**简历**可发送至：<wshw333@gmail.com>  
+微信搜索“shede333sw”咨询岗位详情；  
+
+移动端招聘详情如下：  
+
+iOS工程师任职要求：  
+1.本科以上学历，可使用英文交流者加分；  
+2.三年以上的iOS平台研发经验，良好的代码编写规范。有已上线App开发经验加分，有跨平台开发经验加分；  
+3.精通Object-C/Swift语言，熟悉账户Xcode等开发佛能根据，熟练掌握使用iOS SDK，熟悉Go、Python、Ruby语言加分；  
+4.有高性能客户端编程经验，有性能调优经历加分；  
+5.熟悉iOS主流开源框架，并学习、研究过实现原理和源码；  
+
+Android工程师任职要求：  
+1.本科以上学历，可使用英文交流者加分；  
+2.三年以上Android开发经验；  
+3.熟悉Android常用控件的使用并理解其原理；  
+4.熟悉Android Framework原理，阅读过Android源代码者优先；  
+5.对java、Kotlin、基本数据结构、计算机网络有较为深入的了解；  
+
+
```

### Comparing `PyMobileProvision-1.4.3/README.md` & `PyMobileProvision-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `PyMobileProvision-1.4.3/mobileprovision/command.py` & `PyMobileProvision-1.4.4/mobileprovision/command.py`

 * *Files identical despite different names*

### Comparing `PyMobileProvision-1.4.3/mobileprovision/parser.py` & `PyMobileProvision-1.4.4/mobileprovision/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -206,15 +206,17 @@
         return self._dev_cer_list
 
     def date_is_valid(self):
         """
         文件现在是否在有效日期范围内
         :return: 有效则返回true
         """
-        return self.creation_timestamp < datetime.utcnow().timestamp() < self.expiration_timestamp
+        # 由于本地时间和服务端时间有偏差，特别是profile刚创建完的时候，起始时间兼容 60秒 误差
+        start_is_valid = (datetime.utcnow().timestamp() - self.creation_timestamp) > -60
+        return start_is_valid and (datetime.utcnow().timestamp() < self.expiration_timestamp)
 
     def app_id(self, is_need_prefix=False):
         """
         标示App的bundleID，例如：com.apple.xcode
         :param is_need_prefix: 是否需要带上ApplicationIdentifierPrefix前缀，默认False
         :return: 标示App的ID
         """
```

### Comparing `PyMobileProvision-1.4.3/mobileprovision/util.py` & `PyMobileProvision-1.4.4/mobileprovision/util.py`

 * *Files identical despite different names*

### Comparing `PyMobileProvision-1.4.3/setup.py` & `PyMobileProvision-1.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = Path(__file__).resolve().with_name("README.md").read_text()
 
 # print("{} - {}".format("*" * 10, find_packages()))
 
 setup(
     name='PyMobileProvision',  # 包名字
-    version='1.4.3',  # 包版本
+    version='1.4.4',  # 包版本
     author='shede333',  # 作者
     author_email='333wshw@163.com',  # 作者邮箱
     keywords='mobileprovision mobile provision MobileProvision profile profiles',
     description='Python3, parse ".mobileprovision" file in MacOS System;',  # 简单描述
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/shede333/PyMobileProvision',  # 包的主页
```

