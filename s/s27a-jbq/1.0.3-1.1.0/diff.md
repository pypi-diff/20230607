# Comparing `tmp/s27a_jbq-1.0.3.tar.gz` & `tmp/s27a_jbq-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s27a_jbq-1.0.3.tar", last modified: Sat May 27 11:09:22 2023, max compression
+gzip compressed data, was "s27a_jbq-1.1.0.tar", last modified: Wed Jun  7 12:54:33 2023, max compression
```

## Comparing `s27a_jbq-1.0.3.tar` & `s27a_jbq-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 11:09:22.333218 s27a_jbq-1.0.3/
--rw-rw-rw-   0        0        0     1064 2023-04-16 06:28:36.000000 s27a_jbq-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     4070 2023-05-27 11:09:22.333218 s27a_jbq-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3499 2023-05-27 10:35:28.000000 s27a_jbq-1.0.3/README.md
--rw-rw-rw-   0        0        0      554 2023-05-27 11:09:02.000000 s27a_jbq-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 11:09:22.333218 s27a_jbq-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 11:09:22.308995 s27a_jbq-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 11:09:22.331640 s27a_jbq-1.0.3/src/s27a_jbq/
--rw-rw-rw-   0        0        0      177 2023-05-26 13:58:29.000000 s27a_jbq-1.0.3/src/s27a_jbq/__constants__.py
--rw-rw-rw-   0        0        0       87 2023-05-24 13:02:51.000000 s27a_jbq-1.0.3/src/s27a_jbq/__init__.py
--rw-rw-rw-   0        0        0     2188 2023-05-24 11:40:26.000000 s27a_jbq-1.0.3/src/s27a_jbq/__main__.py
--rw-rw-rw-   0        0        0     4238 2023-05-27 01:42:31.000000 s27a_jbq-1.0.3/src/s27a_jbq/extension.py
--rw-rw-rw-   0        0        0     9025 2023-05-27 10:58:01.000000 s27a_jbq-1.0.3/src/s27a_jbq/game.py
--rw-rw-rw-   0        0        0     6765 2023-05-27 02:14:40.000000 s27a_jbq-1.0.3/src/s27a_jbq/map.py
--rw-rw-rw-   0        0        0     6946 2023-05-27 10:36:44.000000 s27a_jbq-1.0.3/src/s27a_jbq/static.py
--rw-rw-rw-   0        0        0    18929 2023-05-27 02:22:25.000000 s27a_jbq-1.0.3/src/s27a_jbq/window.py
-drwxrwxrwx   0        0        0        0 2023-05-27 11:09:22.333218 s27a_jbq-1.0.3/src/s27a_jbq.egg-info/
--rw-rw-rw-   0        0        0     4070 2023-05-27 11:09:22.000000 s27a_jbq-1.0.3/src/s27a_jbq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-05-27 11:09:22.000000 s27a_jbq-1.0.3/src/s27a_jbq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:09:22.000000 s27a_jbq-1.0.3/src/s27a_jbq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 11:09:22.000000 s27a_jbq-1.0.3/src/s27a_jbq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 12:54:33.418245 s27a_jbq-1.1.0/
+-rw-rw-rw-   0        0        0     1064 2023-04-16 06:28:36.000000 s27a_jbq-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3760 2023-06-07 12:54:33.416195 s27a_jbq-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3189 2023-06-07 12:19:04.000000 s27a_jbq-1.1.0/README.md
+-rw-rw-rw-   0        0        0      554 2023-06-07 12:31:51.000000 s27a_jbq-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 12:54:33.418245 s27a_jbq-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 12:54:33.340173 s27a_jbq-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 12:54:33.365027 s27a_jbq-1.1.0/src/s27a_jbq/
+-rw-rw-rw-   0        0        0      177 2023-06-03 15:56:57.000000 s27a_jbq-1.1.0/src/s27a_jbq/__constants__.py
+-rw-rw-rw-   0        0        0       87 2023-05-24 13:02:51.000000 s27a_jbq-1.1.0/src/s27a_jbq/__init__.py
+-rw-rw-rw-   0        0        0     2662 2023-06-07 12:23:56.000000 s27a_jbq-1.1.0/src/s27a_jbq/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:54:33.398696 s27a_jbq-1.1.0/src/s27a_jbq/game/
+-rw-rw-rw-   0        0        0     5852 2023-06-07 12:14:04.000000 s27a_jbq-1.1.0/src/s27a_jbq/game/__init__.py
+-rw-rw-rw-   0        0        0     2617 2023-06-07 11:42:43.000000 s27a_jbq-1.1.0/src/s27a_jbq/game/extension.py
+-rw-rw-rw-   0        0        0     5586 2023-06-07 12:11:26.000000 s27a_jbq-1.1.0/src/s27a_jbq/game/map.py
+-rw-rw-rw-   0        0        0     2925 2023-06-06 12:19:40.000000 s27a_jbq-1.1.0/src/s27a_jbq/game/static.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:54:33.412107 s27a_jbq-1.1.0/src/s27a_jbq/window/
+-rw-rw-rw-   0        0        0    12787 2023-06-07 12:40:33.000000 s27a_jbq-1.1.0/src/s27a_jbq/window/__init__.py
+-rw-rw-rw-   0        0        0    11010 2023-06-07 12:37:23.000000 s27a_jbq-1.1.0/src/s27a_jbq/window/game_window.py
+-rw-rw-rw-   0        0        0     2578 2023-06-06 12:20:29.000000 s27a_jbq-1.1.0/src/s27a_jbq/window/setting.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:54:33.380445 s27a_jbq-1.1.0/src/s27a_jbq.egg-info/
+-rw-rw-rw-   0        0        0     3760 2023-06-07 12:54:33.000000 s27a_jbq-1.1.0/src/s27a_jbq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-06-07 12:54:33.000000 s27a_jbq-1.1.0/src/s27a_jbq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 12:54:33.000000 s27a_jbq-1.1.0/src/s27a_jbq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 12:54:33.000000 s27a_jbq-1.1.0/src/s27a_jbq.egg-info/top_level.txt
```

### Comparing `s27a_jbq-1.0.3/LICENSE` & `s27a_jbq-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `s27a_jbq-1.0.3/PKG-INFO` & `s27a_jbq-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: s27a_jbq
-Version: 1.0.3
+Version: 1.1.0
 Summary: A board game with high degrees of freedom
 Author-email: amf <xyf081202@163.com>
 Project-URL: Homepage, https://github.com/amf14151/s27a_jbq
 Project-URL: Bug Tracker, https://github.com/amf14151/s27a_jbq/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 精班棋
 
-![](https://img.shields.io/badge/release-1.0.3-blue)
-![](https://img.shields.io/badge/last%20commit-may-yellow)
+![](https://img.shields.io/badge/release-1.1.0-blue)
+![](https://img.shields.io/badge/last%20commit-june-yellow)
 ![](https://img.shields.io/badge/license-MIT-green)
 
 精班棋是一款自由度很高的棋类游戏
 
 这款游戏的最大特点就是地图的可自定义性以及对于扩展插件的高度支持
 
 运用这些，你可以在精班棋中还原出一些经典的棋类游戏
@@ -33,60 +33,47 @@
 - [使用方法](#使用方法)
 - [许可证](#许可证)
 
 # 安装
 
 [(返回目录)](#目录)
 
-您可以在[精班棋官网](https://amf14151.github.io/JBQ/)下载exe版本并获取对应的地图、扩展包，也可以按照下面的步骤安装模块并使用
+## exe版本
+
+您可以在[精班棋官网](https://amf14151.github.io/JBQ/)下载exe版本并获取对应的地图、扩展包
 
 ## 安装模块
 
 *若想通过模块的方式运行精班棋，您需要Python解释器*
 
 使用以下命令来安装模块
 
 ```
 python.exe -m pip install s27a_jbq
 ```
 
-在安装`s27a_jbq`模块后，使用以下命令来构建游戏文件夹
+在安装`s27a_jbq`模块后，使用以下命令进入精班棋面板，并按照说明生成游戏文件夹
 
 ```
-python.exe -m s27a_jbq generate_game {游戏文件夹路径} {游戏运行方式}
+python.exe -m s27a_jbq
 ```
 
-其中，游戏运行方式有以下选择：
+在生成游戏文件夹中，游戏运行方式有以下选择：
 
+- `code`：代码模式（生成代码仅为示例）
 - `window`：窗口模式
 
-示例：
-
-```
-python.exe -m s27a_jbq generate_game C:/JBQ window
-```
-
-上方的代码在C盘根目录中创建名为`JBQ`的游戏文件夹
-
-您也可以在建立文件夹后直接使用以下代码构建主文件（不推荐）
-
-``` python
-from s27a_jbq.game import App
-
-def main():
-   app = App()
-   app.run()
-```
-
-在游戏文件夹中有`extensions`文件夹，该文件夹用于存储扩展，扩展具体使用方法请看[这里](#扩展)
+在窗口模式游戏文件夹中有`extensions`文件夹，该文件夹用于存储扩展，扩展具体使用方法请看[这里](#扩展)
 
 # 使用方法
 
 [(返回目录)](#目录)
 
+以下使用方法均针对窗口模式
+
 ## 游戏过程
 
 在设置好地图及扩展（具体方法请参见下文）后，点击开始游戏即可
 
 游戏中，以红方为先手，双方依次移动棋子并尝试吃掉对方棋子，以先吃掉对方的首领棋子（任意1个即可）为胜利条件
 
 每个棋子上会有可移动方向标注，在己方回合单击棋子即可查看该棋子具体可移动格子，右键棋子可以查看该棋子详细信息
@@ -97,21 +84,21 @@
 
 ## 地图
 
 地图文件是`.xlsx`文件，其中包含至少3个表，分别对应棋子、棋盘与特殊规则
 
 地图文件中可能会有其他名称的表，这些表不会被程序读取，但内部可能会有该地图的说明信息
 
-您可以在[这里](https://github.com/amf14151/s27a_jbq/tree/main/map)下载地图，也可以自定义地图（[查看帮助文档](https://amf14151.github.io/JBQ/help.html)）
+您可以在[这里](https://amf14151.github.io/JBQ/)获取地图，也可以自定义地图（[查看帮助文档](https://amf14151.github.io/JBQ/help.html)）
 
 ## 扩展
 
 扩展是`.py`文件，是用`Python`语言按照一定规则编写的一段代码块，运用扩展可以实现一些独特的行走方法及游戏规则
 
-您可以在[这里](https://github.com/amf14151/s27a_jbq/tree/main/extensions)获取扩展，也可以自行编写扩展（[查看帮助文档](https://amf14151.github.io/JBQ/help.html)）
+您可以在[这里](https://amf14151.github.io/JBQ/)获取扩展，也可以自行编写扩展（[查看帮助文档](https://amf14151.github.io/JBQ/help.html)）
 
 在游戏设置中可以导入扩展，也可以手动将扩展文件添加到游戏文件夹下的`extensions`文件夹下。扩展默认为禁用状态，可以在游戏设置中启用或禁用扩展
 
 # 许可证
 
 [(返回目录)](#目录)
```

### Comparing `s27a_jbq-1.0.3/README.md` & `s27a_jbq-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 精班棋
 
-![](https://img.shields.io/badge/release-1.0.3-blue)
-![](https://img.shields.io/badge/last%20commit-may-yellow)
+![](https://img.shields.io/badge/release-1.1.0-blue)
+![](https://img.shields.io/badge/last%20commit-june-yellow)
 ![](https://img.shields.io/badge/license-MIT-green)
 
 精班棋是一款自由度很高的棋类游戏
 
 这款游戏的最大特点就是地图的可自定义性以及对于扩展插件的高度支持
 
 运用这些，你可以在精班棋中还原出一些经典的棋类游戏
@@ -18,60 +18,47 @@
 - [使用方法](#使用方法)
 - [许可证](#许可证)
 
 # 安装
 
 [(返回目录)](#目录)
 
-您可以在[精班棋官网](https://amf14151.github.io/JBQ/)下载exe版本并获取对应的地图、扩展包，也可以按照下面的步骤安装模块并使用
+## exe版本
+
+您可以在[精班棋官网](https://amf14151.github.io/JBQ/)下载exe版本并获取对应的地图、扩展包
 
 ## 安装模块
 
 *若想通过模块的方式运行精班棋，您需要Python解释器*
 
 使用以下命令来安装模块
 
 ```
 python.exe -m pip install s27a_jbq
 ```
 
-在安装`s27a_jbq`模块后，使用以下命令来构建游戏文件夹
+在安装`s27a_jbq`模块后，使用以下命令进入精班棋面板，并按照说明生成游戏文件夹
 
 ```
-python.exe -m s27a_jbq generate_game {游戏文件夹路径} {游戏运行方式}
+python.exe -m s27a_jbq
 ```
 
-其中，游戏运行方式有以下选择：
+在生成游戏文件夹中，游戏运行方式有以下选择：
 
+- `code`：代码模式（生成代码仅为示例）
 - `window`：窗口模式
 
-示例：
-
-```
-python.exe -m s27a_jbq generate_game C:/JBQ window
-```
-
-上方的代码在C盘根目录中创建名为`JBQ`的游戏文件夹
-
-您也可以在建立文件夹后直接使用以下代码构建主文件（不推荐）
-
-``` python
-from s27a_jbq.game import App
-
-def main():
-   app = App()
-   app.run()
-```
-
-在游戏文件夹中有`extensions`文件夹，该文件夹用于存储扩展，扩展具体使用方法请看[这里](#扩展)
+在窗口模式游戏文件夹中有`extensions`文件夹，该文件夹用于存储扩展，扩展具体使用方法请看[这里](#扩展)
 
 # 使用方法
 
 [(返回目录)](#目录)
 
+以下使用方法均针对窗口模式
+
 ## 游戏过程
 
 在设置好地图及扩展（具体方法请参见下文）后，点击开始游戏即可
 
 游戏中，以红方为先手，双方依次移动棋子并尝试吃掉对方棋子，以先吃掉对方的首领棋子（任意1个即可）为胜利条件
 
 每个棋子上会有可移动方向标注，在己方回合单击棋子即可查看该棋子具体可移动格子，右键棋子可以查看该棋子详细信息
@@ -82,21 +69,21 @@
 
 ## 地图
 
 地图文件是`.xlsx`文件，其中包含至少3个表，分别对应棋子、棋盘与特殊规则
 
 地图文件中可能会有其他名称的表，这些表不会被程序读取，但内部可能会有该地图的说明信息
 
-您可以在[这里](https://github.com/amf14151/s27a_jbq/tree/main/map)下载地图，也可以自定义地图（[查看帮助文档](https://amf14151.github.io/JBQ/help.html)）
+您可以在[这里](https://amf14151.github.io/JBQ/)获取地图，也可以自定义地图（[查看帮助文档](https://amf14151.github.io/JBQ/help.html)）
 
 ## 扩展
 
 扩展是`.py`文件，是用`Python`语言按照一定规则编写的一段代码块，运用扩展可以实现一些独特的行走方法及游戏规则
 
-您可以在[这里](https://github.com/amf14151/s27a_jbq/tree/main/extensions)获取扩展，也可以自行编写扩展（[查看帮助文档](https://amf14151.github.io/JBQ/help.html)）
+您可以在[这里](https://amf14151.github.io/JBQ/)获取扩展，也可以自行编写扩展（[查看帮助文档](https://amf14151.github.io/JBQ/help.html)）
 
 在游戏设置中可以导入扩展，也可以手动将扩展文件添加到游戏文件夹下的`extensions`文件夹下。扩展默认为禁用状态，可以在游戏设置中启用或禁用扩展
 
 # 许可证
 
 [(返回目录)](#目录)
```

### Comparing `s27a_jbq-1.0.3/pyproject.toml` & `s27a_jbq-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "s27a_jbq"
-version = "1.0.3"
+version = "1.1.0"
 authors = [
   { name="amf", email="xyf081202@163.com" },
 ]
 description = "A board game with high degrees of freedom"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `s27a_jbq-1.0.3/src/s27a_jbq/__main__.py` & `s27a_jbq-1.1.0/src/s27a_jbq/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,81 @@
 import os
-import sys
 
 from .__constants__ import __version__
 
 def generate_game(game_path:str,display:str):
     import os
     if os.path.exists(game_path):
         return False
     os.mkdir(game_path)
-    if display == "window":
-        os.mkdir(os.path.join(game_path,"map"))
-        os.mkdir(os.path.join(game_path,"extensions"))
-        with open(os.path.join(game_path,"JBQ.py"),"w",encoding = "utf-8") as wfile:
-            wfile.write("from s27a_jbq.game import App\n")
-            wfile.write("\n")
-            wfile.write("""def main():
-    app = App()
+    if display == "code":
+        code = """from s27a_jbq.game import Game,MapViewer,Map,ExtensionManager
+
+def main():
+    map = Map(*MapViewer.view("[此处填写地图路径]"))
+    ext_manager = ExtensionManager()
+    ext_manager.load_extension("[此处填写扩展路径]")
+    ext_manager.load_extension("[此处填写扩展路径]") # 可导入多次
+    game = Game(map,ext_manager)
+    game.start()
+    while True:
+        game.click(arr) # arr由代码决定
+
+if __name__ == "__main__":
+    main()
+"""
+    elif display == "window":
+        code = """from s27a_jbq.window import WindowApp
+
+def main():
+    app = WindowApp()
     app.run()
 
 if __name__ == "__main__":
     main()
-""")
+"""
     else:
         return False
+    with open(os.path.join(game_path,"JBQ.py"),"w",encoding = "utf-8") as wfile:
+        wfile.write(code)
     return True
 
+commands = ["生成游戏","帮助文档","关于精班棋","退出面板"]
+
 def main():
-    try:
-        command = sys.argv[1]
-        args = sys.argv[2:]
-        if command == "help":
-            print("联网帮助请查看https://github.com/amf14151/s27a_jbq/blob/main/README.md")
-            print("")
-            print("可使用命令：")
-            print("\thelp\t\t获取帮助")
-            print("\tversion\t\t获取当前游戏版本")
-            print("\tgenerate_game\t生成游戏文件夹（详情见联网帮助）")
-        elif command == "version":
-            print(f"精班棋游戏版本：{__version__}")
-        elif command == "generate_game":
-            game_path = os.path.abspath(args[0])
-            display = args[1]
-            if display != "window":
-                print("display选项需要为以下值中的一个：")
-                print("\twindow")
-                return
-            print(f"游戏文件夹路径：{game_path}")
-            print(f"游戏运行方式：{display}")
+    print("-" * 10 + "精班棋命令行面板" + "-" * 10)
+    for i,j in enumerate(commands):
+        print(f"{i + 1} {j}")
+    while True:
+        ans = input("请输入指令:")
+        if ans == "1":
+            game_path = os.path.abspath(input("请输入游戏文件夹路径:"))
+            display = input("请输入游戏运行方式:")
+            if display not in ["code","window"]:
+                print("游戏运行方式需要为以下值中的一个：")
+                print(" code")
+                print(" window")
+                print("具体内容请查看帮助文档")
+                continue
+            print(f"游戏文件夹路径:{game_path}")
+            print(f"游戏运行方式:{display}")
             ans = input("是否确认创建文件夹？(y/n)").lower()
             if ans == "y":
                 ok = generate_game(game_path,display)
                 if ok:
                     print("创建成功")
                 else:
                     print("创建失败")
             else:
                 print("已取消创建")
-        else:
-            raise
-    except:
-        print("请输入'help'来获取帮助")
+        elif ans == "2":
+            print("联网帮助请查看https://github.com/amf14151/s27a_jbq/blob/main/README.md")
+        elif ans == "3":
+            print("关于精班棋")
+            print(f" 版本:{__version__}")
+            print(f" 发布日期:2023.6.7")
+        elif ans == "4":
+            break
 
 # 当被命令行调用时运行
 if __name__ == "__main__":
     main()
```

### Comparing `s27a_jbq-1.0.3/src/s27a_jbq/map.py` & `s27a_jbq-1.1.0/src/s27a_jbq/game/map.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import copy
 
-from tkinter.messagebox import showinfo
-
 from .static import ARR
-from .extension import ExtensionManager
 
 class Chess:
     def __init__(self,id:int,name:str,belong:int,is_captain:bool,move:list[list[tuple]],tran_con:list[tuple],tran_move:list[list[tuple]],attr:dict[str],map_data):
         self.id = id
         self.name = name
         self.belong = belong
         self.is_captain = is_captain
@@ -103,17 +100,17 @@
                 for j in i[1:]:
                     if arr[1] == get_abs_pos(j,self.cl):
                         return True
             elif command == "P": # 函数P（点）
                 for j in range(1,len(i),2):
                     if arr == (get_abs_pos(i[j],self.rl),get_abs_pos(i[j + 1],self.cl)):
                         return True
-            for j in ExtensionManager.Ext.loc_rules: # 扩展中的函数
+            for j in self.ext_manager.loc_rules: # 扩展中的函数
                 if command == j:
-                    if ExtensionManager.Ext.loc_rules[j](i[1:],arr):
+                    if self.ext_manager.loc_rules[j](i[1:],arr):
                         return True
         return False
 
     # 是否可以吃子
     def can_eat(self,chess1:Chess,chess2:Chess):
         return chess1.belong != 3 and chess2.belong != 3 and chess1.belong != chess2.belong
 
@@ -143,37 +140,10 @@
                 if not chess:
                     continue
                 if chess.is_tran:
                     continue
                 if self.is_in_position((i,j),chess.tran_con):
                     chess.is_tran = True
 
-class HistoryRecorder:
-    def __init__(self,map_data:Map):
-        self.history = list[tuple[list[list[Chess]],str]]()
-        self.history.append((self.copy_chessboard(map_data.chessboard),1)) # 初始也在其中，走完后立即add
-        self.now = 1 # 当前位置（不含）
-
-    @staticmethod
-    def copy_chessboard(chessboard:list[list[Chess]]):
-        new_chessboard = list[list[Chess]]()
-        for i in chessboard:
-            new_chessboard.append([])
-            for j in i:
-                if j:
-                    new_chessboard[-1].append(copy.copy(j))
-                else:
-                    new_chessboard[-1].append(None)
-        return new_chessboard
-
-    def add_history(self,map_data:Map,turn:str):
-        del self.history[self.now:]
-        self.history.append((self.copy_chessboard(map_data.chessboard),turn))
-        self.now += 1
-
-    def rollback(self,steps:int): # steps可以是负数（撤销）
-        if self.now - steps < 1 or self.now - steps > len(self.history):
-            showinfo("提示","操作失败")
-            return
-        self.now -= steps
-        data = self.history[self.now - 1]
-        return (self.copy_chessboard(data[0]),data[1])
+    # 添加棋子
+    def add_chess(self,id:int,arr:ARR):
+        self.chessboard[arr[0]][arr[1]] = Chess(id,*self.chesses[id - 1],self)
```

### Comparing `s27a_jbq-1.0.3/src/s27a_jbq.egg-info/PKG-INFO` & `s27a_jbq-1.1.0/src/s27a_jbq.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: s27a-jbq
-Version: 1.0.3
+Version: 1.1.0
 Summary: A board game with high degrees of freedom
 Author-email: amf <xyf081202@163.com>
 Project-URL: Homepage, https://github.com/amf14151/s27a_jbq
 Project-URL: Bug Tracker, https://github.com/amf14151/s27a_jbq/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 精班棋
 
-![](https://img.shields.io/badge/release-1.0.3-blue)
-![](https://img.shields.io/badge/last%20commit-may-yellow)
+![](https://img.shields.io/badge/release-1.1.0-blue)
+![](https://img.shields.io/badge/last%20commit-june-yellow)
 ![](https://img.shields.io/badge/license-MIT-green)
 
 精班棋是一款自由度很高的棋类游戏
 
 这款游戏的最大特点就是地图的可自定义性以及对于扩展插件的高度支持
 
 运用这些，你可以在精班棋中还原出一些经典的棋类游戏
@@ -33,60 +33,47 @@
 - [使用方法](#使用方法)
 - [许可证](#许可证)
 
 # 安装
 
 [(返回目录)](#目录)
 
-您可以在[精班棋官网](https://amf14151.github.io/JBQ/)下载exe版本并获取对应的地图、扩展包，也可以按照下面的步骤安装模块并使用
+## exe版本
+
+您可以在[精班棋官网](https://amf14151.github.io/JBQ/)下载exe版本并获取对应的地图、扩展包
 
 ## 安装模块
 
 *若想通过模块的方式运行精班棋，您需要Python解释器*
 
 使用以下命令来安装模块
 
 ```
 python.exe -m pip install s27a_jbq
 ```
 
-在安装`s27a_jbq`模块后，使用以下命令来构建游戏文件夹
+在安装`s27a_jbq`模块后，使用以下命令进入精班棋面板，并按照说明生成游戏文件夹
 
 ```
-python.exe -m s27a_jbq generate_game {游戏文件夹路径} {游戏运行方式}
+python.exe -m s27a_jbq
 ```
 
-其中，游戏运行方式有以下选择：
+在生成游戏文件夹中，游戏运行方式有以下选择：
 
+- `code`：代码模式（生成代码仅为示例）
 - `window`：窗口模式
 
-示例：
-
-```
-python.exe -m s27a_jbq generate_game C:/JBQ window
-```
-
-上方的代码在C盘根目录中创建名为`JBQ`的游戏文件夹
-
-您也可以在建立文件夹后直接使用以下代码构建主文件（不推荐）
-
-``` python
-from s27a_jbq.game import App
-
-def main():
-   app = App()
-   app.run()
-```
-
-在游戏文件夹中有`extensions`文件夹，该文件夹用于存储扩展，扩展具体使用方法请看[这里](#扩展)
+在窗口模式游戏文件夹中有`extensions`文件夹，该文件夹用于存储扩展，扩展具体使用方法请看[这里](#扩展)
 
 # 使用方法
 
 [(返回目录)](#目录)
 
+以下使用方法均针对窗口模式
+
 ## 游戏过程
 
 在设置好地图及扩展（具体方法请参见下文）后，点击开始游戏即可
 
 游戏中，以红方为先手，双方依次移动棋子并尝试吃掉对方棋子，以先吃掉对方的首领棋子（任意1个即可）为胜利条件
 
 每个棋子上会有可移动方向标注，在己方回合单击棋子即可查看该棋子具体可移动格子，右键棋子可以查看该棋子详细信息
@@ -97,21 +84,21 @@
 
 ## 地图
 
 地图文件是`.xlsx`文件，其中包含至少3个表，分别对应棋子、棋盘与特殊规则
 
 地图文件中可能会有其他名称的表，这些表不会被程序读取，但内部可能会有该地图的说明信息
 
-您可以在[这里](https://github.com/amf14151/s27a_jbq/tree/main/map)下载地图，也可以自定义地图（[查看帮助文档](https://amf14151.github.io/JBQ/help.html)）
+您可以在[这里](https://amf14151.github.io/JBQ/)获取地图，也可以自定义地图（[查看帮助文档](https://amf14151.github.io/JBQ/help.html)）
 
 ## 扩展
 
 扩展是`.py`文件，是用`Python`语言按照一定规则编写的一段代码块，运用扩展可以实现一些独特的行走方法及游戏规则
 
-您可以在[这里](https://github.com/amf14151/s27a_jbq/tree/main/extensions)获取扩展，也可以自行编写扩展（[查看帮助文档](https://amf14151.github.io/JBQ/help.html)）
+您可以在[这里](https://amf14151.github.io/JBQ/)获取扩展，也可以自行编写扩展（[查看帮助文档](https://amf14151.github.io/JBQ/help.html)）
 
 在游戏设置中可以导入扩展，也可以手动将扩展文件添加到游戏文件夹下的`extensions`文件夹下。扩展默认为禁用状态，可以在游戏设置中启用或禁用扩展
 
 # 许可证
 
 [(返回目录)](#目录)
```

