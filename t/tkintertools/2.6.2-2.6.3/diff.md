# Comparing `tmp/tkintertools-2.6.2.tar.gz` & `tmp/tkintertools-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.2.tar", last modified: Tue May 30 05:03:42 2023, max compression
+gzip compressed data, was "tkintertools-2.6.3.tar", last modified: Wed Jun  7 04:03:31 2023, max compression
```

## Comparing `tkintertools-2.6.2.tar` & `tkintertools-2.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 05:03:42.315983 tkintertools-2.6.2/
--rw-rw-rw-   0        0        0     7548 2023-05-27 20:59:02.000000 tkintertools-2.6.2/LICENSE
--rw-rw-rw-   0        0        0    28242 2023-05-30 05:03:42.314979 tkintertools-2.6.2/PKG-INFO
--rw-rw-rw-   0        0        0    27737 2023-05-30 05:02:43.000000 tkintertools-2.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-30 05:03:42.315983 tkintertools-2.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1206 2023-05-30 05:00:07.000000 tkintertools-2.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:03:42.307980 tkintertools-2.6.2/tkintertools/
--rw-rw-rw-   0        0        0     1852 2023-05-29 13:41:50.000000 tkintertools-2.6.2/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    60774 2023-05-29 12:50:33.000000 tkintertools-2.6.2/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     1359 2023-05-29 16:01:56.000000 tkintertools-2.6.2/tkintertools/constants.py
--rw-rw-rw-   0        0        0    14044 2023-05-30 03:03:47.000000 tkintertools-2.6.2/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:03:42.312981 tkintertools-2.6.2/tkintertools.egg-info/
--rw-rw-rw-   0        0        0    28242 2023-05-30 05:03:42.000000 tkintertools-2.6.2/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-05-30 05:03:42.000000 tkintertools-2.6.2/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 05:03:42.000000 tkintertools-2.6.2/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-30 05:03:42.000000 tkintertools-2.6.2/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 04:03:31.396749 tkintertools-2.6.3/
+-rw-rw-rw-   0        0        0     7548 2023-05-27 20:59:02.000000 tkintertools-2.6.3/LICENSE
+-rw-rw-rw-   0        0        0    28315 2023-06-07 04:03:31.395748 tkintertools-2.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0    27814 2023-06-06 17:55:42.000000 tkintertools-2.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 04:03:31.396749 tkintertools-2.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1212 2023-06-06 18:02:17.000000 tkintertools-2.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:03:31.381897 tkintertools-2.6.3/tkintertools/
+-rw-rw-rw-   0        0        0     2352 2023-06-06 07:56:16.000000 tkintertools-2.6.3/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    62722 2023-06-06 09:57:09.000000 tkintertools-2.6.3/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     2066 2023-06-06 07:55:51.000000 tkintertools-2.6.3/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    14823 2023-06-06 17:59:15.000000 tkintertools-2.6.3/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:03:31.392751 tkintertools-2.6.3/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0    28315 2023-06-07 04:03:31.000000 tkintertools-2.6.3/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-06-07 04:03:31.000000 tkintertools-2.6.3/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 04:03:31.000000 tkintertools-2.6.3/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-07 04:03:31.000000 tkintertools-2.6.3/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.2/LICENSE` & `tkintertools-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.2/PKG-INFO` & `tkintertools-2.6.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,112 +1,98 @@
-Metadata-Version: 2.1
-Name: tkintertools
-Version: 2.6.2
-Summary: An auxiliary module of the tkinder module
-Home-page: https://gitcode.net/weixin_62651706/tkintertools
-Author: Xiaokang2022
-Author-email: 2951256653@qq.com
-License: MulanPSL-2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
-        src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/tkintertools.png" />
+        src="tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
-        <a href="./tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.2-blue" alt="latest version" />
+        <a href="tkintertools/__init__.py">
+            <img src="https://img.shields.io/badge/Version-2.6.3-blue" alt="latest version" />
         </a>
-        <a href="./LICENSE">
+        <a href="LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
-        <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/05/30-orange" alt="ChangeLog" />
+        <a href="CHANGELOG.md">
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/07-orange" alt="ChangeLog" />
         </a>
-        <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-13-yellow" alt="ToDos" />
+        <a href="TODO.md">
+            <img src="https://img.shields.io/badge/ToDos-14-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
-            <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
+            <img src="https://img.shields.io/badge/Downloads-4k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
             <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
         </a>
         <a href="https://xiaokang2022.blog.csdn.net">
             <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
         </a>
-        <a href="https://gitcode.net/weixin_62651706">
+        <a href="https://github.com/Xiaokang2022">
             <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
         </a>
     </p>
 </div>
 
 Installation/模块安装
------------------------
+--------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.2
-* Release Date/发布日期 : 2023/05/30
+* Version/版本 : 2.6.3
+* Release Date/发布日期 : 2023/06/07
 
 ```
-pip install tkintertools==2.6.2
+pip install tkintertools==2.6.3
 ```
 或者
 ```
 pip install tkintertools
 ```
 
 这个是目前的最新稳定版，比较稳定，bug 没有那么多，推荐使用这个。  
 稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.2
-* Release Date/发布日期 : 2023/05/26
+* Version/版本 : 2.6.3
+* Release Date/发布日期 : 2023/06/06
 
 ```
-pip install tkintertools-dev==2.6.2
+pip install tkintertools-dev==2.6.3
 ```
 
-这个是作者正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
+这个是我正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
 开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
 
 News/最新功能
 ------------
 
-最新版的`tkintertools`为`2.6.2`，新增一项极为强大的功能：3d绘图！  
+最新版的tkintertools新增一项极为强大的功能：3d绘图！  
 同时修复一些bug，优化了一部分代码，提升了一部分性能。
 
 通过以下代码来使用3d绘图功能：
 
 ```python
 from tkintertools import tools_3d as t3d
 import tkintertools.tools_3d as t3d
 # 两种引入方式都可以
 ```
 
-子模块: [tools_3d.py](./tkintertools/tools_3d.py)
+子模块: [tools_3d.py](tkintertools/tools_3d.py)
 
 目前3d绘图功能还比较简陋，仅能绘制点、线、面以及直边的空间几何体，对于曲边的空间几何体还在开发中！  
 以下是一个使用3d绘图的示例：
 
 在这个示例中，按住鼠标左键可以旋转几何体，按住鼠标右键可以平移几何体，滚动鼠标滚轮可以缩放几何体！  
 x、y 和 z 轴分别是红色、绿色和蓝色的线。
 
-![3d绘图](./docs/images/3d.png)
+![3d绘图](docs/images/3d.png)
 
 <details><summary><b>源代码</b></summary>
 
 ```python
 import random
 import tkinter
 
@@ -183,15 +169,15 @@
 root.bind('<B3-Motion>', translate)
 root.bind('<MouseWheel>', scale)
 root.mainloop()
 ```
 
 </details>
 
-更多更新信息请见：[CHANGELOG.md](./CHANGELOG.md)
+更多更新信息请见：[CHANGELOG.md](CHANGELOG.md)
 
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
@@ -219,15 +205,15 @@
 
 ### Customizable widgets/可自定义的控件
 
 tkintertools 模块的控件拥有许多参数供我们设置，比如圆角的半径、文本和边框以及控件内部的颜色，关联事件等等。  
 这里要说明的是，每个控件可以设置的关联事件不止一种，在鼠标经过控件时可以绑定事件，鼠标点击控件也可以，鼠标点击后松开也行等等。  
 文本和边框以及控件的填充色也是类似的，在鼠标经过控件、点击控件、点击后松开都可以设定颜色。  
 文本类控件还能够从右边逐步输入文本，文本输入提示符也可以不是单调无趣的竖线，可以是其他的，比如下划线等。  
-最后，大家可以看一下 [test.py](./test.py) 文件里面的示例，这个示例展示了 tkintertools 模块的绝大部分功能，示例中更有隐藏的 “多彩变幻” 彩蛋哦！
+最后，大家可以看一下 [test.py](test.py) 文件里面的示例，这个示例展示了 tkintertools 模块的绝大部分功能，示例中更有隐藏的 “多彩变幻” 彩蛋哦！
 
 ### Automatically control size/自动控制大小
 
 tkintertools 中的控件，其大小和形状可以随着窗口的变化而成比例地变化，不仅仅是控件中的文本，Canvas 绘制的图形也会随之变动，更让人兴奋的是，png 类型的图片也会随之成比例地缩放！当然，你也可以设定参数让其不随之变动，也可以设定参数使其在缩放的时候保持横纵方向的比例。  
 总之，很方便，很舒适！
 
 ### Easily move widgets/轻松移动控件
@@ -249,22 +235,26 @@
 
 ![type_hint.png](docs/images/type_hint_vscode.png)
 
 在 VSCode 编辑器中，当鼠标移至类或者函数的名字上面时，会自动显示该类或者函数的注释文档。通过这种方式，不需要看太多的帮助文档和资料就能熟练地使用 tkintertools 模块！
 
 ### Across Platforms/跨平台
 
-[test.py](./test.py) 在 Windows 系统（Windows10）上运行的界面如下：
+[test.py](test.py) 在 Windows 系统（**Windows10**）上运行的界面如下：
 
-![test_win32.png](docs/images/test_win32.png)
+![test_windows10.png](docs/images/test_windows10.png)
 
-[test.py](./test.py) 在 Linux 系统（Ubuntu22.04）上运行的界面如下：
+[test.py](test.py) 在 Linux 系统（**Ubuntu22.04**）上运行的界面如下：
 
 ![test_linux.png](docs/images/test_linux.png)
 
+[test.py](test.py) 在 Windows 系统（**Windows11**）上运行的界面如下(智能控制圆角半径)：
+
+![test_windows11.png](docs/images/test_windows11.png)
+
 Contents/模块内容
 -------------------
 
 Each non internal class and function in the module will be described in detail here  
 这里会详细说明模块中的每个非内部类和函数
 
 ### Container Widget/容器控件
@@ -692,14 +682,14 @@
 
 More/更多
 ---------
 
 > GitHub:  
 > https://github.com/Xiaokang2022/tkintertools
 
-> GitCode(Mirror/镜像):  
-> https://gitcode.net/weixin_62651706/tkintertools
-
 > Gitee(Mirror/镜像):  
 > https://gitee.com/xiaokang-2022/tkintertools
 
-还有更多内容请在 [源代码](./tkintertools/) 中探索！
+> GitCode(Mirror/镜像):  
+> https://gitcode.net/weixin_62651706/tkintertools
+
+还有更多内容请在 [源代码](tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,43 +1,35 @@
-Metadata-Version: 2.1 Name: tkintertools Version: 2.6.2 Summary: An auxiliary
-module of the tkinder module Home-page: https://gitcode.net/weixin_62651706/
-tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com License:
-MulanPSL-2.0 Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
-Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
-Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/30
-``` pip install tkintertools==2.6.2 ``` æè ``` pip install tkintertools ```
+Installation/æ¨¡åå®è£ -------------------- ### Stable version/ç¨³å®çæ¬
+* Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/07 ``` pip
+install tkintertools==2.6.3 ``` æè ``` pip install tkintertools ```
 è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
 æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
 issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/26
-``` pip install tkintertools-dev==2.6.2 ```
-è¿ä¸ªæ¯ä½èæ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
+å¼åçæ¬ * Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/06
+``` pip install tkintertools-dev==2.6.3 ```
+è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
 å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
 ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
 News/ææ°åè½ -----------
--
-ææ°çç`tkintertools`ä¸º`2.6.2`ï¼æ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
+- ææ°ççtkintertoolsæ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
 åæ¶ä¿®å¤ä¸äºbugï¼ä¼åäºä¸é¨åä»£ç ï¼æåäºä¸é¨åæ§è½ã
 éè¿ä»¥ä¸ä»£ç æ¥ä½¿ç¨3dç»å¾åè½ï¼ ```python from tkintertools import
 tools_3d as t3d import tkintertools.tools_3d as t3d #
-ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](./tkintertools/
+ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](tkintertools/
 tools_3d.py)
 ç®å3dç»å¾åè½è¿æ¯è¾ç®éï¼ä»è½ç»å¶ç¹ãçº¿ãé¢ä»¥åç´è¾¹çç©ºé´å ä½ä½ï¼å¯¹äºæ²è¾¹çç©ºé´å ä½ä½è¿å¨å¼åä¸­ï¼
 ä»¥ä¸æ¯ä¸ä¸ªä½¿ç¨3dç»å¾çç¤ºä¾ï¼
 å¨è¿ä¸ªç¤ºä¾ä¸­ï¼æä½é¼ æ å·¦é®å¯ä»¥æè½¬å ä½ä½ï¼æä½é¼ æ å³é®å¯ä»¥å¹³ç§»å ä½ä½ï¼æ»å¨é¼ æ æ»è½®å¯ä»¥ç¼©æ¾å ä½ä½ï¼
-xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](./docs/
+xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](docs/
 images/3d.png) æºä»£ç  ```python import random import tkinter import
 tkintertools as tkt from tkintertools import tools_3d as t3d root = tkt.Tk
 ('tools_3d', 1280, 720) canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0) geos = []
 # type: list[t3d.Geometry] origin = t3d.Point(canvas, [0, 0, 0], size=5) #
 åç¹ axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'), #
 åå»ºåæ è½´ t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3,
 fill='green'), t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
@@ -58,15 +50,15 @@
 axes: axis.rotate(0, 6*dx, 6*dy, center=origin.coords) axis.update() for geo in
 geos: geo.rotate(0, dx, dy, center=origin.coords) geo.update() def scale
 (event): # type: (tkinter.Event) -> None """ ç¼©æ¾äºä»¶ """ k = 1.01 if
 event.delta > 0 else 0.99 for geo in geos: geo.scale(k, k, k) geo.update()
 root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
 root.bind('', lambda event: translate(event, True)) root.bind('', translate)
 root.bind('', scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼
-[CHANGELOG.md](./CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
+[CHANGELOG.md](CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
 - tkintertools æ¯ä¸æ¬¾åºäº tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
@@ -82,15 +74,15 @@
 Provides/æ¨¡ååè½ ------------------- Here, only the more distinctive
 features will be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ###
 Customizable widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
 æ¨¡åçæ§ä»¶æ¥æè®¸å¤åæ°ä¾æä»¬è®¾ç½®ï¼æ¯å¦åè§çåå¾ãææ¬åè¾¹æ¡ä»¥åæ§ä»¶åé¨çé¢è²ï¼å³èäºä»¶ç­ç­ã
 è¿éè¦è¯´æçæ¯ï¼æ¯ä¸ªæ§ä»¶å¯ä»¥è®¾ç½®çå³èäºä»¶ä¸æ­¢ä¸ç§ï¼å¨é¼ æ ç»è¿æ§ä»¶æ¶å¯ä»¥ç»å®äºä»¶ï¼é¼ æ ç¹å»æ§ä»¶ä¹å¯ä»¥ï¼é¼ æ ç¹å»åæ¾å¼ä¹è¡ç­ç­ã
 ææ¬åè¾¹æ¡ä»¥åæ§ä»¶çå¡«åè²ä¹æ¯ç±»ä¼¼çï¼å¨é¼ æ ç»è¿æ§ä»¶ãç¹å»æ§ä»¶ãç¹å»åæ¾å¼é½å¯ä»¥è®¾å®é¢è²ã
 ææ¬ç±»æ§ä»¶è¿è½å¤ä»å³è¾¹éæ­¥è¾å¥ææ¬ï¼ææ¬è¾å¥æç¤ºç¬¦ä¹å¯ä»¥ä¸æ¯åè°æ è¶£çç«çº¿ï¼å¯ä»¥æ¯å¶ä»çï¼æ¯å¦ä¸åçº¿ç­ã
-æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](./test.py)
+æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](test.py)
 æä»¶éé¢çç¤ºä¾ï¼è¿ä¸ªç¤ºä¾å±ç¤ºäº tkintertools
 æ¨¡åçç»å¤§é¨ååè½ï¼ç¤ºä¾ä¸­æ´æéèç âå¤å½©åå¹»â
 å½©èå¦ï¼ ### Automatically control size/èªå¨æ§å¶å¤§å° tkintertools
 ä¸­çæ§ä»¶ï¼å¶å¤§å°åå½¢ç¶å¯ä»¥éççªå£çååèææ¯ä¾å°ååï¼ä¸ä»ä»æ¯æ§ä»¶ä¸­çææ¬ï¼Canvas
 ç»å¶çå¾å½¢ä¹ä¼éä¹åå¨ï¼æ´è®©äººå´å¥çæ¯ï¼png
 ç±»åçå¾çä¹ä¼éä¹ææ¯ä¾å°ç¼©æ¾ï¼å½ç¶ï¼ä½ ä¹å¯ä»¥è®¾å®åæ°è®©å¶ä¸éä¹åå¨ï¼ä¹å¯ä»¥è®¾å®åæ°ä½¿å¶å¨ç¼©æ¾çæ¶åä¿ææ¨ªçºµæ¹åçæ¯ä¾ã
 æ»ä¹ï¼å¾æ¹ä¾¿ï¼å¾èéï¼ ### Easily move widgets/è½»æ¾ç§»å¨æ§ä»¶
@@ -101,20 +93,23 @@
 peps.python.org/pep-0586/)ã[PEP 604](https://peps.python.org/pep-0604/) å
 [PEP 612](https://peps.python.org/pep-0612/
 )ï¼æéç¨äºæå¼å®¹çæ¹å¼å»å®ç°è¯¦ç»çç±»åæç¤ºï¼å¯éç¨
 IDE æ VScodeãPycharm ç­ã
 é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼ !
 [type_hint.png](docs/images/type_hint_vscode.png) å¨ VSCode
 ç¼è¾å¨ä¸­ï¼å½é¼ æ ç§»è³ç±»æèå½æ°çåå­ä¸é¢æ¶ï¼ä¼èªå¨æ¾ç¤ºè¯¥ç±»æèå½æ°çæ³¨éææ¡£ãéè¿è¿ç§æ¹å¼ï¼ä¸éè¦çå¤ªå¤çå¸®å©ææ¡£åèµæå°±è½çç»å°ä½¿ç¨
-tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](./test.py) å¨
-Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_win32.png]
-(docs/images/test_win32.png) [test.py](./test.py) å¨ Linux
-ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png](docs/
-images/test_linux.png) Contents/æ¨¡ååå®¹ ------------------- Each non
-internal class and function in the module will be described in detail here
+tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](test.py) å¨
+Windows ç³»ç»ï¼**Windows10**ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ !
+[test_windows10.png](docs/images/test_windows10.png) [test.py](test.py) å¨
+Linux ç³»ç»ï¼**Ubuntu22.04**ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png]
+(docs/images/test_linux.png) [test.py](test.py) å¨ Windows
+ç³»ç»ï¼**Windows11**ï¼ä¸è¿è¡ççé¢å¦ä¸(æºè½æ§å¶åè§åå¾)ï¼
+![test_windows11.png](docs/images/test_windows11.png) Contents/æ¨¡ååå®¹ ---
+---------------- Each non internal class and function in the module will be
+described in detail here
 è¿éä¼è¯¦ç»è¯´ææ¨¡åä¸­çæ¯ä¸ªéåé¨ç±»åå½æ° ### Container
 Widget/å®¹å¨æ§ä»¶ 1. `Tk`: çªå£ç±»
 ç»§æ¿äº`tkinter.Tk`ï¼å¨ç»§æ¿äº`tkinter`æ¨¡åå`Tk`çåºç¡ä¸ï¼åå å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¹¶å å¥äºæ£æµçªå£å¤§å°æ¯å¦ç¼©æ¾çæºå¶ï¼ä»¥ä½¿å¾å¶å­`Canvas`åè½æ­£ç¡®å°è¿è¡ç¼©æ¾
 2. `Toplevel`: é¡¶çº§çªå£ç±»
 ç»§æ¿äº`tkinter.Toplevel`å`Tk`ï¼å å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¶ä½åä¸`Tk`ä¸æ ·
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
@@ -295,11 +290,11 @@
 ### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
 ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
 æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
 examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
------- > GitHub: > https://github.com/Xiaokang2022/tkintertools > GitCode
-(Mirror/éå): > https://gitcode.net/weixin_62651706/tkintertools > Gitee
-(Mirror/éå): > https://gitee.com/xiaokang-2022/tkintertools
-è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
+------ > GitHub: > https://github.com/Xiaokang2022/tkintertools > Gitee(Mirror/
+éå): > https://gitee.com/xiaokang-2022/tkintertools > GitCode(Mirror/
+éå): > https://gitcode.net/weixin_62651706/tkintertools
+è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](tkintertools/) ä¸­æ¢ç´¢ï¼
```

### Comparing `tkintertools-2.6.2/README.md` & `tkintertools-2.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,98 +1,112 @@
+Metadata-Version: 2.1
+Name: tkintertools
+Version: 2.6.3
+Summary: An auxiliary module of the tkinder module
+Home-page: https://github.com/Xiaokang2022/tkintertools
+Author: Xiaokang2022
+Author-email: 2951256653@qq.com
+License: MulanPSL-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
-        src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/tkintertools.png" />
+        src="tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
-        <a href="./tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.2-blue" alt="latest version" />
+        <a href="tkintertools/__init__.py">
+            <img src="https://img.shields.io/badge/Version-2.6.3-blue" alt="latest version" />
         </a>
-        <a href="./LICENSE">
+        <a href="LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
-        <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/05/30-orange" alt="ChangeLog" />
+        <a href="CHANGELOG.md">
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/07-orange" alt="ChangeLog" />
         </a>
-        <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-13-yellow" alt="ToDos" />
+        <a href="TODO.md">
+            <img src="https://img.shields.io/badge/ToDos-14-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
-            <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
+            <img src="https://img.shields.io/badge/Downloads-4k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
             <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
         </a>
         <a href="https://xiaokang2022.blog.csdn.net">
             <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
         </a>
-        <a href="https://gitcode.net/weixin_62651706">
+        <a href="https://github.com/Xiaokang2022">
             <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
         </a>
     </p>
 </div>
 
 Installation/模块安装
------------------------
+--------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.2
-* Release Date/发布日期 : 2023/05/30
+* Version/版本 : 2.6.3
+* Release Date/发布日期 : 2023/06/07
 
 ```
-pip install tkintertools==2.6.2
+pip install tkintertools==2.6.3
 ```
 或者
 ```
 pip install tkintertools
 ```
 
 这个是目前的最新稳定版，比较稳定，bug 没有那么多，推荐使用这个。  
 稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.2
-* Release Date/发布日期 : 2023/05/26
+* Version/版本 : 2.6.3
+* Release Date/发布日期 : 2023/06/06
 
 ```
-pip install tkintertools-dev==2.6.2
+pip install tkintertools-dev==2.6.3
 ```
 
-这个是作者正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
+这个是我正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
 开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
 
 News/最新功能
 ------------
 
-最新版的`tkintertools`为`2.6.2`，新增一项极为强大的功能：3d绘图！  
+最新版的tkintertools新增一项极为强大的功能：3d绘图！  
 同时修复一些bug，优化了一部分代码，提升了一部分性能。
 
 通过以下代码来使用3d绘图功能：
 
 ```python
 from tkintertools import tools_3d as t3d
 import tkintertools.tools_3d as t3d
 # 两种引入方式都可以
 ```
 
-子模块: [tools_3d.py](./tkintertools/tools_3d.py)
+子模块: [tools_3d.py](tkintertools/tools_3d.py)
 
 目前3d绘图功能还比较简陋，仅能绘制点、线、面以及直边的空间几何体，对于曲边的空间几何体还在开发中！  
 以下是一个使用3d绘图的示例：
 
 在这个示例中，按住鼠标左键可以旋转几何体，按住鼠标右键可以平移几何体，滚动鼠标滚轮可以缩放几何体！  
 x、y 和 z 轴分别是红色、绿色和蓝色的线。
 
-![3d绘图](./docs/images/3d.png)
+![3d绘图](docs/images/3d.png)
 
 <details><summary><b>源代码</b></summary>
 
 ```python
 import random
 import tkinter
 
@@ -169,15 +183,15 @@
 root.bind('<B3-Motion>', translate)
 root.bind('<MouseWheel>', scale)
 root.mainloop()
 ```
 
 </details>
 
-更多更新信息请见：[CHANGELOG.md](./CHANGELOG.md)
+更多更新信息请见：[CHANGELOG.md](CHANGELOG.md)
 
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
@@ -205,15 +219,15 @@
 
 ### Customizable widgets/可自定义的控件
 
 tkintertools 模块的控件拥有许多参数供我们设置，比如圆角的半径、文本和边框以及控件内部的颜色，关联事件等等。  
 这里要说明的是，每个控件可以设置的关联事件不止一种，在鼠标经过控件时可以绑定事件，鼠标点击控件也可以，鼠标点击后松开也行等等。  
 文本和边框以及控件的填充色也是类似的，在鼠标经过控件、点击控件、点击后松开都可以设定颜色。  
 文本类控件还能够从右边逐步输入文本，文本输入提示符也可以不是单调无趣的竖线，可以是其他的，比如下划线等。  
-最后，大家可以看一下 [test.py](./test.py) 文件里面的示例，这个示例展示了 tkintertools 模块的绝大部分功能，示例中更有隐藏的 “多彩变幻” 彩蛋哦！
+最后，大家可以看一下 [test.py](test.py) 文件里面的示例，这个示例展示了 tkintertools 模块的绝大部分功能，示例中更有隐藏的 “多彩变幻” 彩蛋哦！
 
 ### Automatically control size/自动控制大小
 
 tkintertools 中的控件，其大小和形状可以随着窗口的变化而成比例地变化，不仅仅是控件中的文本，Canvas 绘制的图形也会随之变动，更让人兴奋的是，png 类型的图片也会随之成比例地缩放！当然，你也可以设定参数让其不随之变动，也可以设定参数使其在缩放的时候保持横纵方向的比例。  
 总之，很方便，很舒适！
 
 ### Easily move widgets/轻松移动控件
@@ -235,22 +249,26 @@
 
 ![type_hint.png](docs/images/type_hint_vscode.png)
 
 在 VSCode 编辑器中，当鼠标移至类或者函数的名字上面时，会自动显示该类或者函数的注释文档。通过这种方式，不需要看太多的帮助文档和资料就能熟练地使用 tkintertools 模块！
 
 ### Across Platforms/跨平台
 
-[test.py](./test.py) 在 Windows 系统（Windows10）上运行的界面如下：
+[test.py](test.py) 在 Windows 系统（**Windows10**）上运行的界面如下：
 
-![test_win32.png](docs/images/test_win32.png)
+![test_windows10.png](docs/images/test_windows10.png)
 
-[test.py](./test.py) 在 Linux 系统（Ubuntu22.04）上运行的界面如下：
+[test.py](test.py) 在 Linux 系统（**Ubuntu22.04**）上运行的界面如下：
 
 ![test_linux.png](docs/images/test_linux.png)
 
+[test.py](test.py) 在 Windows 系统（**Windows11**）上运行的界面如下(智能控制圆角半径)：
+
+![test_windows11.png](docs/images/test_windows11.png)
+
 Contents/模块内容
 -------------------
 
 Each non internal class and function in the module will be described in detail here  
 这里会详细说明模块中的每个非内部类和函数
 
 ### Container Widget/容器控件
@@ -678,14 +696,14 @@
 
 More/更多
 ---------
 
 > GitHub:  
 > https://github.com/Xiaokang2022/tkintertools
 
-> GitCode(Mirror/镜像):  
-> https://gitcode.net/weixin_62651706/tkintertools
-
 > Gitee(Mirror/镜像):  
 > https://gitee.com/xiaokang-2022/tkintertools
 
-还有更多内容请在 [源代码](./tkintertools/) 中探索！
+> GitCode(Mirror/镜像):  
+> https://gitcode.net/weixin_62651706/tkintertools
+
+还有更多内容请在 [源代码](tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,36 +1,42 @@
+Metadata-Version: 2.1 Name: tkintertools Version: 2.6.3 Summary: An auxiliary
+module of the tkinder module Home-page: https://github.com/Xiaokang2022/
+tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com License:
+MulanPSL-2.0 Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
+Classifier: Operating System :: OS Independent Description-Content-Type: text/
+markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
-Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/30
-``` pip install tkintertools==2.6.2 ``` æè ``` pip install tkintertools ```
+Installation/æ¨¡åå®è£ -------------------- ### Stable version/ç¨³å®çæ¬
+* Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/07 ``` pip
+install tkintertools==2.6.3 ``` æè ``` pip install tkintertools ```
 è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
 æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
 issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/26
-``` pip install tkintertools-dev==2.6.2 ```
-è¿ä¸ªæ¯ä½èæ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
+å¼åçæ¬ * Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/06
+``` pip install tkintertools-dev==2.6.3 ```
+è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
 å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
 ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
 News/ææ°åè½ -----------
--
-ææ°çç`tkintertools`ä¸º`2.6.2`ï¼æ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
+- ææ°ççtkintertoolsæ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
 åæ¶ä¿®å¤ä¸äºbugï¼ä¼åäºä¸é¨åä»£ç ï¼æåäºä¸é¨åæ§è½ã
 éè¿ä»¥ä¸ä»£ç æ¥ä½¿ç¨3dç»å¾åè½ï¼ ```python from tkintertools import
 tools_3d as t3d import tkintertools.tools_3d as t3d #
-ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](./tkintertools/
+ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](tkintertools/
 tools_3d.py)
 ç®å3dç»å¾åè½è¿æ¯è¾ç®éï¼ä»è½ç»å¶ç¹ãçº¿ãé¢ä»¥åç´è¾¹çç©ºé´å ä½ä½ï¼å¯¹äºæ²è¾¹çç©ºé´å ä½ä½è¿å¨å¼åä¸­ï¼
 ä»¥ä¸æ¯ä¸ä¸ªä½¿ç¨3dç»å¾çç¤ºä¾ï¼
 å¨è¿ä¸ªç¤ºä¾ä¸­ï¼æä½é¼ æ å·¦é®å¯ä»¥æè½¬å ä½ä½ï¼æä½é¼ æ å³é®å¯ä»¥å¹³ç§»å ä½ä½ï¼æ»å¨é¼ æ æ»è½®å¯ä»¥ç¼©æ¾å ä½ä½ï¼
-xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](./docs/
+xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](docs/
 images/3d.png) æºä»£ç  ```python import random import tkinter import
 tkintertools as tkt from tkintertools import tools_3d as t3d root = tkt.Tk
 ('tools_3d', 1280, 720) canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0) geos = []
 # type: list[t3d.Geometry] origin = t3d.Point(canvas, [0, 0, 0], size=5) #
 åç¹ axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'), #
 åå»ºåæ è½´ t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3,
 fill='green'), t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
@@ -51,15 +57,15 @@
 axes: axis.rotate(0, 6*dx, 6*dy, center=origin.coords) axis.update() for geo in
 geos: geo.rotate(0, dx, dy, center=origin.coords) geo.update() def scale
 (event): # type: (tkinter.Event) -> None """ ç¼©æ¾äºä»¶ """ k = 1.01 if
 event.delta > 0 else 0.99 for geo in geos: geo.scale(k, k, k) geo.update()
 root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
 root.bind('', lambda event: translate(event, True)) root.bind('', translate)
 root.bind('', scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼
-[CHANGELOG.md](./CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
+[CHANGELOG.md](CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
 - tkintertools æ¯ä¸æ¬¾åºäº tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
@@ -75,15 +81,15 @@
 Provides/æ¨¡ååè½ ------------------- Here, only the more distinctive
 features will be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ###
 Customizable widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
 æ¨¡åçæ§ä»¶æ¥æè®¸å¤åæ°ä¾æä»¬è®¾ç½®ï¼æ¯å¦åè§çåå¾ãææ¬åè¾¹æ¡ä»¥åæ§ä»¶åé¨çé¢è²ï¼å³èäºä»¶ç­ç­ã
 è¿éè¦è¯´æçæ¯ï¼æ¯ä¸ªæ§ä»¶å¯ä»¥è®¾ç½®çå³èäºä»¶ä¸æ­¢ä¸ç§ï¼å¨é¼ æ ç»è¿æ§ä»¶æ¶å¯ä»¥ç»å®äºä»¶ï¼é¼ æ ç¹å»æ§ä»¶ä¹å¯ä»¥ï¼é¼ æ ç¹å»åæ¾å¼ä¹è¡ç­ç­ã
 ææ¬åè¾¹æ¡ä»¥åæ§ä»¶çå¡«åè²ä¹æ¯ç±»ä¼¼çï¼å¨é¼ æ ç»è¿æ§ä»¶ãç¹å»æ§ä»¶ãç¹å»åæ¾å¼é½å¯ä»¥è®¾å®é¢è²ã
 ææ¬ç±»æ§ä»¶è¿è½å¤ä»å³è¾¹éæ­¥è¾å¥ææ¬ï¼ææ¬è¾å¥æç¤ºç¬¦ä¹å¯ä»¥ä¸æ¯åè°æ è¶£çç«çº¿ï¼å¯ä»¥æ¯å¶ä»çï¼æ¯å¦ä¸åçº¿ç­ã
-æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](./test.py)
+æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](test.py)
 æä»¶éé¢çç¤ºä¾ï¼è¿ä¸ªç¤ºä¾å±ç¤ºäº tkintertools
 æ¨¡åçç»å¤§é¨ååè½ï¼ç¤ºä¾ä¸­æ´æéèç âå¤å½©åå¹»â
 å½©èå¦ï¼ ### Automatically control size/èªå¨æ§å¶å¤§å° tkintertools
 ä¸­çæ§ä»¶ï¼å¶å¤§å°åå½¢ç¶å¯ä»¥éççªå£çååèææ¯ä¾å°ååï¼ä¸ä»ä»æ¯æ§ä»¶ä¸­çææ¬ï¼Canvas
 ç»å¶çå¾å½¢ä¹ä¼éä¹åå¨ï¼æ´è®©äººå´å¥çæ¯ï¼png
 ç±»åçå¾çä¹ä¼éä¹ææ¯ä¾å°ç¼©æ¾ï¼å½ç¶ï¼ä½ ä¹å¯ä»¥è®¾å®åæ°è®©å¶ä¸éä¹åå¨ï¼ä¹å¯ä»¥è®¾å®åæ°ä½¿å¶å¨ç¼©æ¾çæ¶åä¿ææ¨ªçºµæ¹åçæ¯ä¾ã
 æ»ä¹ï¼å¾æ¹ä¾¿ï¼å¾èéï¼ ### Easily move widgets/è½»æ¾ç§»å¨æ§ä»¶
@@ -94,20 +100,23 @@
 peps.python.org/pep-0586/)ã[PEP 604](https://peps.python.org/pep-0604/) å
 [PEP 612](https://peps.python.org/pep-0612/
 )ï¼æéç¨äºæå¼å®¹çæ¹å¼å»å®ç°è¯¦ç»çç±»åæç¤ºï¼å¯éç¨
 IDE æ VScodeãPycharm ç­ã
 é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼ !
 [type_hint.png](docs/images/type_hint_vscode.png) å¨ VSCode
 ç¼è¾å¨ä¸­ï¼å½é¼ æ ç§»è³ç±»æèå½æ°çåå­ä¸é¢æ¶ï¼ä¼èªå¨æ¾ç¤ºè¯¥ç±»æèå½æ°çæ³¨éææ¡£ãéè¿è¿ç§æ¹å¼ï¼ä¸éè¦çå¤ªå¤çå¸®å©ææ¡£åèµæå°±è½çç»å°ä½¿ç¨
-tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](./test.py) å¨
-Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_win32.png]
-(docs/images/test_win32.png) [test.py](./test.py) å¨ Linux
-ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png](docs/
-images/test_linux.png) Contents/æ¨¡ååå®¹ ------------------- Each non
-internal class and function in the module will be described in detail here
+tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](test.py) å¨
+Windows ç³»ç»ï¼**Windows10**ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ !
+[test_windows10.png](docs/images/test_windows10.png) [test.py](test.py) å¨
+Linux ç³»ç»ï¼**Ubuntu22.04**ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png]
+(docs/images/test_linux.png) [test.py](test.py) å¨ Windows
+ç³»ç»ï¼**Windows11**ï¼ä¸è¿è¡ççé¢å¦ä¸(æºè½æ§å¶åè§åå¾)ï¼
+![test_windows11.png](docs/images/test_windows11.png) Contents/æ¨¡ååå®¹ ---
+---------------- Each non internal class and function in the module will be
+described in detail here
 è¿éä¼è¯¦ç»è¯´ææ¨¡åä¸­çæ¯ä¸ªéåé¨ç±»åå½æ° ### Container
 Widget/å®¹å¨æ§ä»¶ 1. `Tk`: çªå£ç±»
 ç»§æ¿äº`tkinter.Tk`ï¼å¨ç»§æ¿äº`tkinter`æ¨¡åå`Tk`çåºç¡ä¸ï¼åå å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¹¶å å¥äºæ£æµçªå£å¤§å°æ¯å¦ç¼©æ¾çæºå¶ï¼ä»¥ä½¿å¾å¶å­`Canvas`åè½æ­£ç¡®å°è¿è¡ç¼©æ¾
 2. `Toplevel`: é¡¶çº§çªå£ç±»
 ç»§æ¿äº`tkinter.Toplevel`å`Tk`ï¼å å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¶ä½åä¸`Tk`ä¸æ ·
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
@@ -288,11 +297,11 @@
 ### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
 ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
 æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
 examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
------- > GitHub: > https://github.com/Xiaokang2022/tkintertools > GitCode
-(Mirror/éå): > https://gitcode.net/weixin_62651706/tkintertools > Gitee
-(Mirror/éå): > https://gitee.com/xiaokang-2022/tkintertools
-è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
+------ > GitHub: > https://github.com/Xiaokang2022/tkintertools > Gitee(Mirror/
+éå): > https://gitee.com/xiaokang-2022/tkintertools > GitCode(Mirror/
+éå): > https://gitcode.net/weixin_62651706/tkintertools
+è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](tkintertools/) ä¸­æ¢ç´¢ï¼
```

### Comparing `tkintertools-2.6.2/setup.py` & `tkintertools-2.6.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """ 上传 pypi """
 
 import setuptools
 
 
 setuptools.setup(
     name='tkintertools',
-    version="2.6.2",
+    version="2.6.3",
     author='Xiaokang2022',
     license='MulanPSL-2.0',
     author_email='2951256653@qq.com',
     description='An auxiliary module of the tkinder module',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
-    url='https://gitcode.net/weixin_62651706/tkintertools',
+    url='https://github.com/Xiaokang2022/tkintertools',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)',
         'Operating System :: OS Independent',
     ],
 )
 
 # python -m pip install --user --upgrade setuptools wheel [检查更新]
 
 # python setup.py sdist bdist_wheel [打包]
-# twine upload dist/* [上传]
+# python -m twine upload dist/* [上传]
 
 # pip install -U pypistats [数据分析]
 # pip install socksio [数据分析]
 
 # pypistats overall tkintertools [数据分析]
 # pypistats recent tkintertools
 # pypistats system tkintertools
```

### Comparing `tkintertools-2.6.2/tkintertools/__init__.py` & `tkintertools-2.6.3/tkintertools/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,20 +33,28 @@
 if sys.version_info < (3, 7):  # Version Check
     error_info = '\n\033[31mOperation Requirements: \033[32m\nPython version shall not be less than\033[33m 3.7.0 !\033[0m'
     raise RuntimeError(error_info)
 
 from .__main__ import (Button, Canvas, CheckButton, Entry, Label, PhotoImage,
                        Progressbar, SetProcessDpiAwareness, Singleton, Text,
                        Tk, Toplevel, askfont, color, move, text)
+from .constants import *
 
 __author__ = 'Xiaokang2022<2951256653@qq.com>'
-__version__ = '2.6.2'
+__version__ = '2.6.3'
 __all__ = [
     # Container Widgets
     'Tk', 'Toplevel', 'Canvas',
     # Virtual Canvas Widgets
     'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar',
     # Tool Classes
     'PhotoImage', 'Singleton',
     # Tool Functions
     'move', 'text', 'color', 'askfont', 'SetProcessDpiAwareness',
+    # Constants
+    'SYSTEM', 'PROCESS_SYSTEM_DPI_AWARE', 'COLOR_BUTTON_FILL', 'COLOR_BUTTON_OUTLINE',
+    'COLOR_TEXT_FILL', 'COLOR_TEXT_OUTLINE', 'COLOR_TEXT', 'COLOR_NONE', 'COLOR_BAR',
+    'BACKGROUND', 'BORDERWIDTH', 'CURSOR', 'FONT', 'SIZE', 'LIMIT', 'RADIUS', 'FRAMES',
+    'TICK', 'CFG_3D', 'COLOR_POINT_FILL', 'COLOR_POINT_OUTLINE', 'COLOR_LINE_FILL',
+    'COLOR_SIDE_FILL', 'COLOR_SIDE_OUTLINE', 'POINT_SIZE', 'POINT_WIDTH', 'LINE_WDITH',
+    'SIDE_WIDTH',
 ]
```

### Comparing `tkintertools-2.6.2/tkintertools/__main__.py` & `tkintertools-2.6.3/tkintertools/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Main File """
 
 import math  # 数学支持
 import sys  # DPI 兼容
 import tkinter  # 基础模块
 from fractions import Fraction  # 图片缩放
-from typing import Any, Callable, Generator, Iterable  # 类型提示
+from typing import Any, Callable, Generator, Iterable, overload  # 类型提示
 
 try:  # NOTE: 为了兼容 Python3.7，从 typing_extensions 引入 Literal 而不是 typing
     from typing_extensions import Literal
 except ImportError:
     pass
 
 if sys.platform == 'win32':  # 仅在 Windows 平台下支持设置 DPI 级别
@@ -45,16 +45,16 @@
         if type(self) == Tk:  # NOTE:方便后面的 Toplevel 类继承
             tkinter.Tk.__init__(self, **kw)
 
         self.width = [100, 1]  # type: list[int]  # [初始宽度, 当前宽度]
         self.height = [100, 1]  # type: list[int]  # [初始高度, 当前高度]
         self._canvas = []  # type: list[Canvas]  # 子画布列表
 
-        if width and height:
-            if x is not None and y is not None:  # BUG: 可能需要修改
+        if width is not None and height is not None:
+            if x is not None and y is not None:
                 self.geometry('%dx%d+%d+%d' % (width, height, x, y))
             else:
                 self.geometry('%dx%d' % (width, height))
 
         self.title(title if title else None)
         self.protocol('WM_DELETE_WINDOW', shutdown if shutdown else None)
         self.bind('<Configure>', lambda _: self.__zoom())  # 开启窗口缩放检测
@@ -74,15 +74,15 @@
         for canvas in self._canvas:
             if canvas.expand and canvas._lock:
                 canvas.zoom(width/self.width[1], height/self.height[1])
 
         self.width[1], self.height[1] = width, height  # 更新窗口当前的宽高值
 
     def wm_geometry(self, newGeometry=None):  # type: (str | None) -> str | None
-        # 重写: 添加修改初始宽高值的功能并兼容不同的DPI缩放
+        # override: 添加修改初始宽高值的功能并兼容不同的DPI缩放
         if newGeometry:
             width, height, _width, _height, * \
                 _ = map(int, (newGeometry+'+0+0').replace('+', 'x').split('x'))
             self.width, self.height = [width]*2, [height]*2
             geometry = '%dx%d+%d+%d' % (width, height, _width, _height)
             if not _:
                 geometry = geometry.split('+')[0]
@@ -198,19 +198,27 @@
         self.bind('<ButtonRelease-1>', self.__release)  # 绑定鼠标左键松开
         self.bind('<<Paste>>', lambda _: self.__paste())  # 绑定粘贴快捷键
 
     def widget(self):  # type: () -> tuple[BaseWidget]
         """ 返回`Canvas`类的`BaseWidget`元组 """
         return tuple(self._widget)
 
+    @overload
+    def lock(self, value):  # type: (bool) -> None
+        ...
+
+    @overload
+    def lock(self):  # type: () -> None
+        ...
+
     def lock(self, value=None):  # type: (bool | None) -> bool | None
         """
-        设置画布锁\n
+        设置或者查询画布锁\n
         ---
-        `value`: 布尔值，True则可操作，False反之，None则返回当前值\n
+        `value`: 布尔值，True则可操作，False反之，无参数或参数为None则返回当前值\n
         """
         if value is None:
             return self._lock
         self._lock = value
         if value and self.expand:
             self.zoom()
 
@@ -222,15 +230,17 @@
         `rate_y`: 纵向缩放比率，默认值同上\n
         """
         if not rate_x:
             rate_x = self.master.width[1]/self.master.width[0]/self.rx
         if not rate_y:
             rate_y = self.master.height[1]/self.master.height[0]/self.ry
 
-        if self.keep:  # 维持比例
+        rate_x_pos, rate_y_pos = rate_x, rate_y  # 避免受 keep 影响
+
+        if self.keep is True:  # 维持比例
             rx = rate_x*self.master.width[1]/self.master.width[0]/self.rx
             ry = rate_y*self.master.height[1]/self.master.height[0]/self.ry
             rate_x = rate_y = min(rx, ry)
 
         # 更新画布的位置及大小的数据
         self.width[1] *= rate_x
         self.height[1] *= rate_y
@@ -238,16 +248,16 @@
         temp_y, self.ry = self.ry, self.height[1]/self.height[0]
 
         place_info = self.place_info()
         tkinter.Canvas.place(  # 更新画布的位置及大小
             self,
             width=self.width[1],
             height=self.height[1],
-            x=float(place_info['x'])*rate_x,
-            y=float(place_info['y'])*rate_y)
+            x=float(place_info['x'])*rate_x_pos,
+            y=float(place_info['y'])*rate_y_pos)
 
         for widget in self._widget:  # 更新子画布控件的子虚拟画布控件位置数据
             widget.x1 *= rate_x
             widget.x2 *= rate_x
             widget.y1 *= rate_y
             widget.y2 *= rate_y
 
@@ -319,48 +329,48 @@
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and isinstance(widget, TextWidget):
                     if widget.paste():
                         return
 
     def create_text(self, *args, **kw):  # type: (...) -> tkinter._CanvasItemId
-        # 重写：添加对 text 类型的 _CanvasItemId 的字体大小的控制
+        # override: 添加对 text 类型的 _CanvasItemId 的字体大小的控制
         font = kw.get('font')
         if not font:
             kw['font'] = FONT, SIZE
         elif isinstance(font, str):
             kw['font'] = font, SIZE
         item = tkinter.Canvas.create_text(self, *args, **kw)
         self._font[item] = list(kw['font'])
         return item
 
     def create_image(self, *args, **kw):  # type: (...) -> tkinter._CanvasItemId
-        # 重写：添加对 image 类型的 _CanvasItemId 的图像大小的控制
+        # override: 添加对 image 类型的 _CanvasItemId 的图像大小的控制
         item = tkinter.Canvas.create_image(self, *args, **kw)
         self._image[item] = [kw.get('image'), None]
         return item
 
     def itemconfigure(
         self,
         tagOrId,  # type: str | tkinter._CanvasItemId
         **kw
     ):  # type: (...) -> dict[str, tuple[str, str, str, str, str]] | None
-        # 重写：创建空 image 的 _CanvasItemId 时漏去对图像大小的控制
+        # override: 创建空 image 的 _CanvasItemId 时漏去对图像大小的控制
         if type(kw.get('image')) == PhotoImage:
             self._image[tagOrId] = [kw.get('image'), None]
         return tkinter.Canvas.itemconfigure(self, tagOrId, **kw)
 
     def place(self, *args, **kw):  # type: (...) -> None  # BUG: 缩放就会恢复原样
-        # 重写：增加一些特定功能
+        # override: 增加一些特定功能
         self.width[0] = kw.get('wdith', self.width[0])
         self.height[0] = kw.get('height', self.height[0])
         return tkinter.Canvas.place(self, *args, **kw)
 
     def destroy(self):  # type: () -> None
-        # 重写：兼容
+        # override: 兼容
         self.master._canvas.remove(self)
         for widget in self.widget():
             widget.destroy()
         return tkinter.Canvas.destroy(self)
 
 
 class BaseWidget:
@@ -516,18 +526,27 @@
 
         if type(font) != str:
             font = list(font)
             font[1] = int(font[1]*math.sqrt(canvas.rx*canvas.ry))
             canvas._font[self.text][1] = font[1]
             canvas.itemconfigure(self.text, font=font)
 
-    # type: (Literal['normal', 'touch', 'click', 'disabled'] | None) -> None
+    @overload
+    def state(self, mode):
+        # type: (Literal['normal', 'touch', 'click', 'disabled']) -> None
+        ...
+
+    @overload
+    def state(self):  # type: () -> None
+        ...
+
     def state(self, mode=None):
+        # type: (Literal['normal', 'touch', 'click', 'disabled'] | None) -> None
         """
-        mode 参数为 None 时仅更新控件，否则改变虚拟控件的外观\n
+        mode参数为None或者无参数时仅更新控件，否则改变虚拟控件的外观\n
         ---
         `normal`: 正常状态\n
         `touch`: 鼠标触碰时的状态\n
         `click`: 鼠标按下时的状态\n
         `disabled`: 禁用状态\n
         """
         if mode:
@@ -604,14 +623,22 @@
         改变控件的位置（以控件左上角为基准）\n
         ---
         `x`: 改变到的横坐标（单位：像素）\n
         `y`: 改变到的纵坐标\n
         """
         self.move(x - self.x1, y - self.y1)
 
+    @overload
+    def configure(self, **kw):  # type: (...) -> None
+        ...
+
+    @overload
+    def configure(self, *args):  # type: (...) -> str | tuple
+        ...
+
     def configure(self, *args, **kw):  # type: (...) -> str | tuple | None
         """
         修改或查询原有参数的值，可供修改或查询的参数有\n
         1. 所有控件: `color_text`、`color_fill`、`color_outline`
         2. 非文本控件: `text`\n
         注意：颜色修改不会立即生效，可通过鼠标经过生效，或者调用 state 方法立即刷新状态！
         """
@@ -660,21 +687,29 @@
             self.master.delete(self._text)
         if isinstance(self, Progressbar):
             self.master.delete(self.bar)
 
         self.master.delete(self.image)
         self.master.delete(self.text)
 
-    def set_live(self, boolean=None):  # type: (bool | None) -> bool | None
+    @overload
+    def set_live(self, value):  # type: (bool) -> None
+        ...
+
+    @overload
+    def set_live(self):  # type: () -> bool
+        ...
+
+    def set_live(self, value=None):  # type: (bool | None) -> bool | None
         """ 设定或查询live值 """
-        if boolean is None:
+        if value is None:
             return self.live
         else:
-            self.live = boolean
-            if boolean:
+            self.live = value
+            if value:
                 self.state('normal')
             else:
                 self.state('disabled')
 
 
 class TextWidget(BaseWidget):
     """ 内部类：文本类控件基类 """
@@ -1014,15 +1049,15 @@
                 self._value[0] = self._value[0][1:]
                 self.master.itemconfigure(self.text, text=self._value[0])
             else:
                 break
 
 
 class Text(TextWidget):
-    """ 创建一个透明的虚拟文本框，用于输入多行文本和显示多行文本（只读模式）"""
+    """ 创建一个透明的虚拟文本框，用于输入多行文本和显示多行文本 """
 
     def __init__(
         self,
         canvas,  # type: Canvas
         x,  # type: int
         y,  # type: int
         width,  # type: int
@@ -1335,23 +1370,55 @@
 
     def __new__(cls, *args, **kw):
         if not cls._instance:
             cls._instance = object.__new__(cls)
         return cls._instance
 
 
+@overload
+def move(
+    master,  # type: Tk | Canvas | tkinter.Misc | tkinter.BaseWidget | None
+    widget,  # type: Canvas | BaseWidget | tkinter.BaseWidget
+    dx,  # type: int
+    dy,  # type: int
+    times,  # type: int
+    *,
+    mode,  # type: Literal['smooth', 'rebound', 'flat']
+    frames=FRAMES,  # type: int
+    end=None,  # type: Callable | None
+    _ind=0  # type: int
+):  # type: (...) -> None
+    ...
+
+
+@overload
+def move(
+    master,  # type: Tk | Canvas | tkinter.Misc | tkinter.BaseWidget | None
+    widget,  # type: Canvas | BaseWidget | tkinter.BaseWidget
+    dx,  # type: int
+    dy,  # type: int
+    times,  # type: int
+    *,
+    mode,  # type: tuple[Callable[[float], float], float, float]
+    frames=FRAMES,  # type: int
+    end=None,  # type: Callable | None
+    _ind=0  # type: int
+):  # type: (...) -> None
+    ...
+
+
 def move(
     master,  # type: Tk | Canvas | tkinter.Misc | tkinter.BaseWidget | None
     widget,  # type: Canvas | BaseWidget | tkinter.BaseWidget
     dx,  # type: int
     dy,  # type: int
     times,  # type: int
     *,
-    # type: tuple[Callable[[float], float], float, float] | Literal['smooth', 'rebound', 'flat']  # NOTE
     mode,
+    # type: tuple[Callable[[float], float], float, float] | Literal['smooth', 'rebound', 'flat']
     frames=FRAMES,  # type: int
     end=None,  # type: Callable | None
     _ind=0  # type: int
 ):  # type: (...) -> None
     """
     ### 移动函数
     以特定方式移动由 Place 布局的某个控件或某些控件的集合或图像\n
@@ -1422,14 +1489,30 @@
     elif position == 'right':  # 靠右
         return string+length*' '
     else:  # 居中
         length, key = divmod(length, 2)
         return ' '*length+string+(length+key)*' '
 
 
+@overload
+def color(
+    color,  # type: Iterable[str]
+    proportion=1.  # type: float
+):  # type: (...) -> str
+    ...
+
+
+@overload
+def color(
+    color,  # type: str
+    proportion=1.  # type: float
+):  # type: (...) -> str
+    ...
+
+
 def color(
     color,  # type: Iterable[str] | str
     proportion=1.  # type: float
 ):  # type: (...) -> str
     """
     ### 颜色函数
     按一定比例给出已有 RGB 颜色字符串的渐变 RGB 颜色字符串，或颜色的对比色\n
```

### Comparing `tkintertools-2.6.2/tkintertools/constants.py` & `tkintertools-2.6.3/tkintertools/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """ All constants """
 
-import sys
+import platform
+
+SYSTEM = platform.system()
+""" Operating System """
 
 PROCESS_SYSTEM_DPI_AWARE = 1
 """ Default DPI aware """
 
 
 COLOR_BUTTON_FILL = '#E1E1E1', '#E5F1FB', '#CCE4F7', '#E0E0E0'
 """ Default button fill color """
@@ -33,28 +36,60 @@
 
 BORDERWIDTH = 1
 """ Default widget borderwidth """
 
 CURSOR = '│'
 """ text cursor """
 
-FONT = 'Microsoft YaHei' if sys.platform == 'win32' else 'DejaVu Sans' if sys.platform == 'linux' else 'Arial'
+FONT = 'Microsoft YaHei' if SYSTEM == 'Windows' else 'DejaVu Sans' if SYSTEM == 'linux' else 'Arial'
 """ Default font """
 
 SIZE = 20
 """ Default font size """
 
 LIMIT = -1
 """ Default widget text length limit """
 
-RADIUS = 0
+RADIUS = 0 if SYSTEM == 'Windows' and int(
+    platform.version()[-5:]) < 22000 else 4
 """ Default widget fillet radius """
 
 FRAMES = 60
 """ Default move frame rate """
 
 TICK = '✓'
 """ Default checkbox symbol """
 
 
 CFG_3D = 500, None, None
 """ Default 3D configuration """
+
+
+COLOR_POINT_FILL = '#000000'
+""" Default point fill color """
+
+COLOR_POINT_OUTLINE = '#000000'
+""" Default point outline color """
+
+COLOR_LINE_FILL = '#000000'
+""" Default line fill color """
+
+COLOR_SIDE_FILL = ''
+""" Default side fill color """
+
+COLOR_SIDE_OUTLINE = '#000000'
+""" Default side outline color """
+
+POINT_SIZE = 1
+""" Default point size """
+
+POINT_WIDTH = 1
+""" Default point width """
+
+LINE_WDITH = 1
+""" Default line width """
+
+SIDE_WIDTH = 1
+""" Default side width """
+
+
+__all__ = [name for name in globals() if name.isupper()]
```

### Comparing `tkintertools-2.6.2/tkintertools/tools_3d.py` & `tkintertools-2.6.3/tkintertools/tools_3d.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         width,  # type: int
         height,  # type: int
         x=None,  # type: int | None
         y=None,  # type: int | None
         *,
         lock=True,  # type: bool
         expand=True,  # type: bool
-        keep=False,  # type: bool
+        keep=True,  # type: bool
         cfg_3d=CFG_3D,  # type: Iterable[float, float | None, float | None]
         **kw
     ):  # type: (...) -> None
         """
         `master`: 父控件\n
         `width`: 画布宽度\n
         `height`: 画布高度\n
@@ -38,14 +38,19 @@
         `**kw`: 与 tkinter.Canvas 类的参数相同\n
         """
         Canvas.__init__(self, master, width, height, x, y,
                         lock=lock, expand=expand, keep=keep)
         self.distance = cfg_3d[0]
         self.dx = width / 2 if cfg_3d[1] is None else cfg_3d[1]
         self.dy = height / 2 if cfg_3d[2] is None else cfg_3d[2]
+        self._items_3d = []  # type: list[Point | Line | Side | Geometry]
+
+    def items_3d(self):  # type: () -> tuple[Point | Line | Side | Geometry]
+        """ 返回`Canvas_3d`类的`items_3d`元组 """
+        return tuple(self._items_3d)
 
 
 class _Point:
     """ 点 """
 
     def __init__(self, coords):  # type: (list[float]) -> None
         self.coords = coords  # 利用列表引用
@@ -77,18 +82,18 @@
         """ 缩放 """
         for i, k in zip(range(3), (kx, ky, kz)):
             self.coords[i] += (self.coords[i] - center[i]) * (k - 1)
 
     def project(self, distance):  # type: (float) -> list[float]
         """ 投影 """
         try:
-            coefficient = distance/(distance - self.coords[0])
-        except:
+            k = distance/(distance - self.coords[0])
+        except ZeroDivisionError:
             return [distance, distance]
-        return [self.coords[1]*coefficient, self.coords[2]*coefficient]
+        return [self.coords[1]*k, self.coords[2]*k]
 
 
 class _Line:
     """ 线 """
 
     def __init__(
         self,
@@ -158,127 +163,134 @@
     """ 点 """
 
     def __init__(
         self,
         canvas,  # type: Canvas_3D
         coords,  # type: list[float]
         *,
-        size=1,  # type: float
-        width=1,  # type: float
-        fill='grey',  # type: str
-        outline='black',  # type: str
+        size=POINT_SIZE,  # type: float
+        width=POINT_WIDTH,  # type: float
+        fill=COLOR_POINT_FILL,  # type: str
+        outline=COLOR_POINT_OUTLINE,  # type: str
     ):  # type: (...) -> None
         """
         `canvas`: 父画布\n
         `coords`: 点的空间坐标\n
         `size`: 点的大小\n
         `width`: 点轮廓的宽度\n
         `fill`: 点内部的填充颜色\n
         `outline`: 点轮廓的颜色\n
         """
         _Point.__init__(self, coords)
+        canvas._items_3d.append(self)
         self.canvas = canvas
         self.size = size
         self.width = width
         self.fill = fill
         self.item = canvas.create_oval(
             -1, -1, -1, -1, fill=fill, outline=outline, width=width)
         self.update()
 
     def update(self) -> None:
         """ 更新 """
         x, y = self.project(self.canvas.distance)
+        kx, ky = self.canvas.rx, self.canvas.ry
         x += self.canvas.dx
         y += self.canvas.dy
         self.canvas.coords(
-            self.item, x-self.size, y-self.size, x+self.size, y+self.size)
+            self.item, (x-self.size)*kx, (y-self.size)*ky, (x+self.size)*kx, (y+self.size)*ky)
 
 
 class Line(_Line):
     """ 线 """
 
     def __init__(
         self,
         canvas,  # type: Canvas_3D
         point1,  # type: list[float]
         point2,  # type: list[float]
         *,
-        width=1,  # type: float
-        fill='black',  # type: str
+        width=LINE_WDITH,  # type: float
+        fill=COLOR_LINE_FILL,  # type: str
     ):  # type: (...) -> None
         """
         `canvas`: 父画布\n
         `point1`: 起点坐标\n
         `point2`: 终点坐标\n
         `width`: 线的宽度\n
         `fill`: 线的颜色\n
         """
         _Line.__init__(self, point1, point2)
+        canvas._items_3d.append(self)
         self.canvas = canvas
         self.width = width
         self.fill = fill
         self.item = canvas.create_line(-1, -1, -1, -1, width=width, fill=fill)
         self.update()
 
     def update(self) -> None:
         """ 更新 """
+        kx, ky = self.canvas.rx, self.canvas.ry
         data = self.project(self.canvas.distance)
         for point in data:
             point[0] += self.canvas.dx
             point[1] += self.canvas.dy
         self.canvas.coords(
-            self.item, *[coord for point in data for coord in point])
+            self.item, *[coord*(ky if i else kx) for point in data for i, coord in enumerate(point)])
 
 
 class Side(_Side):
     """ 面 """
 
     def __init__(
         self,
         canvas,  # type: Canvas_3D
         *points,  # type: list[float]
-        width=1,  # type: float
-        fill='',  # type: str
-        outline='black',  # type: str
+        width=SIDE_WIDTH,  # type: float
+        fill=COLOR_SIDE_FILL,  # type: str
+        outline=COLOR_SIDE_OUTLINE,  # type: str
     ):  # type: (...) -> None
         """
         `canvas`: 父画布\n
         `points`: 各点的空间坐标\n
         `width`: 面轮廓的宽度\n
         `fill`: 面内部的填充颜色\n
         `outline`: 面轮廓的颜色\n
         """
         _Side.__init__(self, *points)
+        canvas._items_3d.append(self)
         self.canvas = canvas
         self.width = width
         self.fill = fill
         self.outline = outline
         self.item = canvas.create_polygon(-1, -1, -1, -1,
                                           width=width, fill=fill, outline=outline)
         self.update()
 
     def update(self) -> None:
         """ 更新 """
+        kx, ky = self.canvas.rx, self.canvas.ry
         data = self.project(self.canvas.distance)
         for line in data:
             for point in line:
                 point[0] += self.canvas.dx
                 point[1] += self.canvas.dy
         self.canvas.coords(
-            self.item, *[coord for line in data for point in line for coord in point])
+            self.item, *[coord*(ky if i else kx) for line in data for point in line for i, coord in enumerate(point)])
 
 
 class Geometry:
     """ 几何体 """
 
     def __init__(self, canvas, *sides):  # type: (Canvas_3D, _Side) -> None
         """
         `canvas`: 显示的画布\n
         `sides`: 平面类`Side`\n
         """
+        canvas._items_3d.append(self)
         self.canvas = canvas
         self.coords = []  # type: list[list[float]]
         self.sides = []  # type: list[Side]
         if sides:
             self.append(*sides)
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
@@ -401,7 +413,10 @@
         self.coords = [list(p1), list(p2), list(p3), list(p4)]
         self.sides = [
             Side(canvas, self.coords[0], self.coords[1], self.coords[2]),
             Side(canvas, self.coords[0], self.coords[1], self.coords[3]),
             Side(canvas, self.coords[0], self.coords[2], self.coords[3]),
             Side(canvas, self.coords[1], self.coords[2], self.coords[3]),
         ]
+
+
+__all__ = [name for name in globals() if '__' not in name]
```

### Comparing `tkintertools-2.6.2/tkintertools.egg-info/PKG-INFO` & `tkintertools-2.6.3/tkintertools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,112 +1,112 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.2
+Version: 2.6.3
 Summary: An auxiliary module of the tkinder module
-Home-page: https://gitcode.net/weixin_62651706/tkintertools
+Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
-        src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/tkintertools.png" />
+        src="tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
-        <a href="./tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.2-blue" alt="latest version" />
+        <a href="tkintertools/__init__.py">
+            <img src="https://img.shields.io/badge/Version-2.6.3-blue" alt="latest version" />
         </a>
-        <a href="./LICENSE">
+        <a href="LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
-        <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/05/30-orange" alt="ChangeLog" />
+        <a href="CHANGELOG.md">
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/07-orange" alt="ChangeLog" />
         </a>
-        <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-13-yellow" alt="ToDos" />
+        <a href="TODO.md">
+            <img src="https://img.shields.io/badge/ToDos-14-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
-            <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
+            <img src="https://img.shields.io/badge/Downloads-4k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
             <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
         </a>
         <a href="https://xiaokang2022.blog.csdn.net">
             <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
         </a>
-        <a href="https://gitcode.net/weixin_62651706">
+        <a href="https://github.com/Xiaokang2022">
             <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
         </a>
     </p>
 </div>
 
 Installation/模块安装
------------------------
+--------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.2
-* Release Date/发布日期 : 2023/05/30
+* Version/版本 : 2.6.3
+* Release Date/发布日期 : 2023/06/07
 
 ```
-pip install tkintertools==2.6.2
+pip install tkintertools==2.6.3
 ```
 或者
 ```
 pip install tkintertools
 ```
 
 这个是目前的最新稳定版，比较稳定，bug 没有那么多，推荐使用这个。  
 稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.2
-* Release Date/发布日期 : 2023/05/26
+* Version/版本 : 2.6.3
+* Release Date/发布日期 : 2023/06/06
 
 ```
-pip install tkintertools-dev==2.6.2
+pip install tkintertools-dev==2.6.3
 ```
 
-这个是作者正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
+这个是我正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
 开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
 
 News/最新功能
 ------------
 
-最新版的`tkintertools`为`2.6.2`，新增一项极为强大的功能：3d绘图！  
+最新版的tkintertools新增一项极为强大的功能：3d绘图！  
 同时修复一些bug，优化了一部分代码，提升了一部分性能。
 
 通过以下代码来使用3d绘图功能：
 
 ```python
 from tkintertools import tools_3d as t3d
 import tkintertools.tools_3d as t3d
 # 两种引入方式都可以
 ```
 
-子模块: [tools_3d.py](./tkintertools/tools_3d.py)
+子模块: [tools_3d.py](tkintertools/tools_3d.py)
 
 目前3d绘图功能还比较简陋，仅能绘制点、线、面以及直边的空间几何体，对于曲边的空间几何体还在开发中！  
 以下是一个使用3d绘图的示例：
 
 在这个示例中，按住鼠标左键可以旋转几何体，按住鼠标右键可以平移几何体，滚动鼠标滚轮可以缩放几何体！  
 x、y 和 z 轴分别是红色、绿色和蓝色的线。
 
-![3d绘图](./docs/images/3d.png)
+![3d绘图](docs/images/3d.png)
 
 <details><summary><b>源代码</b></summary>
 
 ```python
 import random
 import tkinter
 
@@ -183,15 +183,15 @@
 root.bind('<B3-Motion>', translate)
 root.bind('<MouseWheel>', scale)
 root.mainloop()
 ```
 
 </details>
 
-更多更新信息请见：[CHANGELOG.md](./CHANGELOG.md)
+更多更新信息请见：[CHANGELOG.md](CHANGELOG.md)
 
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
@@ -219,15 +219,15 @@
 
 ### Customizable widgets/可自定义的控件
 
 tkintertools 模块的控件拥有许多参数供我们设置，比如圆角的半径、文本和边框以及控件内部的颜色，关联事件等等。  
 这里要说明的是，每个控件可以设置的关联事件不止一种，在鼠标经过控件时可以绑定事件，鼠标点击控件也可以，鼠标点击后松开也行等等。  
 文本和边框以及控件的填充色也是类似的，在鼠标经过控件、点击控件、点击后松开都可以设定颜色。  
 文本类控件还能够从右边逐步输入文本，文本输入提示符也可以不是单调无趣的竖线，可以是其他的，比如下划线等。  
-最后，大家可以看一下 [test.py](./test.py) 文件里面的示例，这个示例展示了 tkintertools 模块的绝大部分功能，示例中更有隐藏的 “多彩变幻” 彩蛋哦！
+最后，大家可以看一下 [test.py](test.py) 文件里面的示例，这个示例展示了 tkintertools 模块的绝大部分功能，示例中更有隐藏的 “多彩变幻” 彩蛋哦！
 
 ### Automatically control size/自动控制大小
 
 tkintertools 中的控件，其大小和形状可以随着窗口的变化而成比例地变化，不仅仅是控件中的文本，Canvas 绘制的图形也会随之变动，更让人兴奋的是，png 类型的图片也会随之成比例地缩放！当然，你也可以设定参数让其不随之变动，也可以设定参数使其在缩放的时候保持横纵方向的比例。  
 总之，很方便，很舒适！
 
 ### Easily move widgets/轻松移动控件
@@ -249,22 +249,26 @@
 
 ![type_hint.png](docs/images/type_hint_vscode.png)
 
 在 VSCode 编辑器中，当鼠标移至类或者函数的名字上面时，会自动显示该类或者函数的注释文档。通过这种方式，不需要看太多的帮助文档和资料就能熟练地使用 tkintertools 模块！
 
 ### Across Platforms/跨平台
 
-[test.py](./test.py) 在 Windows 系统（Windows10）上运行的界面如下：
+[test.py](test.py) 在 Windows 系统（**Windows10**）上运行的界面如下：
 
-![test_win32.png](docs/images/test_win32.png)
+![test_windows10.png](docs/images/test_windows10.png)
 
-[test.py](./test.py) 在 Linux 系统（Ubuntu22.04）上运行的界面如下：
+[test.py](test.py) 在 Linux 系统（**Ubuntu22.04**）上运行的界面如下：
 
 ![test_linux.png](docs/images/test_linux.png)
 
+[test.py](test.py) 在 Windows 系统（**Windows11**）上运行的界面如下(智能控制圆角半径)：
+
+![test_windows11.png](docs/images/test_windows11.png)
+
 Contents/模块内容
 -------------------
 
 Each non internal class and function in the module will be described in detail here  
 这里会详细说明模块中的每个非内部类和函数
 
 ### Container Widget/容器控件
@@ -692,14 +696,14 @@
 
 More/更多
 ---------
 
 > GitHub:  
 > https://github.com/Xiaokang2022/tkintertools
 
-> GitCode(Mirror/镜像):  
-> https://gitcode.net/weixin_62651706/tkintertools
-
 > Gitee(Mirror/镜像):  
 > https://gitee.com/xiaokang-2022/tkintertools
 
-还有更多内容请在 [源代码](./tkintertools/) 中探索！
+> GitCode(Mirror/镜像):  
+> https://gitcode.net/weixin_62651706/tkintertools
+
+还有更多内容请在 [源代码](tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,43 +1,42 @@
-Metadata-Version: 2.1 Name: tkintertools Version: 2.6.2 Summary: An auxiliary
-module of the tkinder module Home-page: https://gitcode.net/weixin_62651706/
+Metadata-Version: 2.1 Name: tkintertools Version: 2.6.3 Summary: An auxiliary
+module of the tkinder module Home-page: https://github.com/Xiaokang2022/
 tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com License:
 MulanPSL-2.0 Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
-Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/30
-``` pip install tkintertools==2.6.2 ``` æè ``` pip install tkintertools ```
+Installation/æ¨¡åå®è£ -------------------- ### Stable version/ç¨³å®çæ¬
+* Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/07 ``` pip
+install tkintertools==2.6.3 ``` æè ``` pip install tkintertools ```
 è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
 æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
 issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/26
-``` pip install tkintertools-dev==2.6.2 ```
-è¿ä¸ªæ¯ä½èæ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
+å¼åçæ¬ * Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/06
+``` pip install tkintertools-dev==2.6.3 ```
+è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
 å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
 ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
 News/ææ°åè½ -----------
--
-ææ°çç`tkintertools`ä¸º`2.6.2`ï¼æ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
+- ææ°ççtkintertoolsæ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
 åæ¶ä¿®å¤ä¸äºbugï¼ä¼åäºä¸é¨åä»£ç ï¼æåäºä¸é¨åæ§è½ã
 éè¿ä»¥ä¸ä»£ç æ¥ä½¿ç¨3dç»å¾åè½ï¼ ```python from tkintertools import
 tools_3d as t3d import tkintertools.tools_3d as t3d #
-ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](./tkintertools/
+ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](tkintertools/
 tools_3d.py)
 ç®å3dç»å¾åè½è¿æ¯è¾ç®éï¼ä»è½ç»å¶ç¹ãçº¿ãé¢ä»¥åç´è¾¹çç©ºé´å ä½ä½ï¼å¯¹äºæ²è¾¹çç©ºé´å ä½ä½è¿å¨å¼åä¸­ï¼
 ä»¥ä¸æ¯ä¸ä¸ªä½¿ç¨3dç»å¾çç¤ºä¾ï¼
 å¨è¿ä¸ªç¤ºä¾ä¸­ï¼æä½é¼ æ å·¦é®å¯ä»¥æè½¬å ä½ä½ï¼æä½é¼ æ å³é®å¯ä»¥å¹³ç§»å ä½ä½ï¼æ»å¨é¼ æ æ»è½®å¯ä»¥ç¼©æ¾å ä½ä½ï¼
-xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](./docs/
+xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](docs/
 images/3d.png) æºä»£ç  ```python import random import tkinter import
 tkintertools as tkt from tkintertools import tools_3d as t3d root = tkt.Tk
 ('tools_3d', 1280, 720) canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0) geos = []
 # type: list[t3d.Geometry] origin = t3d.Point(canvas, [0, 0, 0], size=5) #
 åç¹ axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'), #
 åå»ºåæ è½´ t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3,
 fill='green'), t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
@@ -58,15 +57,15 @@
 axes: axis.rotate(0, 6*dx, 6*dy, center=origin.coords) axis.update() for geo in
 geos: geo.rotate(0, dx, dy, center=origin.coords) geo.update() def scale
 (event): # type: (tkinter.Event) -> None """ ç¼©æ¾äºä»¶ """ k = 1.01 if
 event.delta > 0 else 0.99 for geo in geos: geo.scale(k, k, k) geo.update()
 root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
 root.bind('', lambda event: translate(event, True)) root.bind('', translate)
 root.bind('', scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼
-[CHANGELOG.md](./CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
+[CHANGELOG.md](CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
 - tkintertools æ¯ä¸æ¬¾åºäº tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
@@ -82,15 +81,15 @@
 Provides/æ¨¡ååè½ ------------------- Here, only the more distinctive
 features will be listed è¿éåªä¼åä¸¾åºæ¯è¾å·æç¹è²çåè½ ###
 Customizable widgets/å¯èªå®ä¹çæ§ä»¶ tkintertools
 æ¨¡åçæ§ä»¶æ¥æè®¸å¤åæ°ä¾æä»¬è®¾ç½®ï¼æ¯å¦åè§çåå¾ãææ¬åè¾¹æ¡ä»¥åæ§ä»¶åé¨çé¢è²ï¼å³èäºä»¶ç­ç­ã
 è¿éè¦è¯´æçæ¯ï¼æ¯ä¸ªæ§ä»¶å¯ä»¥è®¾ç½®çå³èäºä»¶ä¸æ­¢ä¸ç§ï¼å¨é¼ æ ç»è¿æ§ä»¶æ¶å¯ä»¥ç»å®äºä»¶ï¼é¼ æ ç¹å»æ§ä»¶ä¹å¯ä»¥ï¼é¼ æ ç¹å»åæ¾å¼ä¹è¡ç­ç­ã
 ææ¬åè¾¹æ¡ä»¥åæ§ä»¶çå¡«åè²ä¹æ¯ç±»ä¼¼çï¼å¨é¼ æ ç»è¿æ§ä»¶ãç¹å»æ§ä»¶ãç¹å»åæ¾å¼é½å¯ä»¥è®¾å®é¢è²ã
 ææ¬ç±»æ§ä»¶è¿è½å¤ä»å³è¾¹éæ­¥è¾å¥ææ¬ï¼ææ¬è¾å¥æç¤ºç¬¦ä¹å¯ä»¥ä¸æ¯åè°æ è¶£çç«çº¿ï¼å¯ä»¥æ¯å¶ä»çï¼æ¯å¦ä¸åçº¿ç­ã
-æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](./test.py)
+æåï¼å¤§å®¶å¯ä»¥çä¸ä¸ [test.py](test.py)
 æä»¶éé¢çç¤ºä¾ï¼è¿ä¸ªç¤ºä¾å±ç¤ºäº tkintertools
 æ¨¡åçç»å¤§é¨ååè½ï¼ç¤ºä¾ä¸­æ´æéèç âå¤å½©åå¹»â
 å½©èå¦ï¼ ### Automatically control size/èªå¨æ§å¶å¤§å° tkintertools
 ä¸­çæ§ä»¶ï¼å¶å¤§å°åå½¢ç¶å¯ä»¥éççªå£çååèææ¯ä¾å°ååï¼ä¸ä»ä»æ¯æ§ä»¶ä¸­çææ¬ï¼Canvas
 ç»å¶çå¾å½¢ä¹ä¼éä¹åå¨ï¼æ´è®©äººå´å¥çæ¯ï¼png
 ç±»åçå¾çä¹ä¼éä¹ææ¯ä¾å°ç¼©æ¾ï¼å½ç¶ï¼ä½ ä¹å¯ä»¥è®¾å®åæ°è®©å¶ä¸éä¹åå¨ï¼ä¹å¯ä»¥è®¾å®åæ°ä½¿å¶å¨ç¼©æ¾çæ¶åä¿ææ¨ªçºµæ¹åçæ¯ä¾ã
 æ»ä¹ï¼å¾æ¹ä¾¿ï¼å¾èéï¼ ### Easily move widgets/è½»æ¾ç§»å¨æ§ä»¶
@@ -101,20 +100,23 @@
 peps.python.org/pep-0586/)ã[PEP 604](https://peps.python.org/pep-0604/) å
 [PEP 612](https://peps.python.org/pep-0612/
 )ï¼æéç¨äºæå¼å®¹çæ¹å¼å»å®ç°è¯¦ç»çç±»åæç¤ºï¼å¯éç¨
 IDE æ VScodeãPycharm ç­ã
 é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼ !
 [type_hint.png](docs/images/type_hint_vscode.png) å¨ VSCode
 ç¼è¾å¨ä¸­ï¼å½é¼ æ ç§»è³ç±»æèå½æ°çåå­ä¸é¢æ¶ï¼ä¼èªå¨æ¾ç¤ºè¯¥ç±»æèå½æ°çæ³¨éææ¡£ãéè¿è¿ç§æ¹å¼ï¼ä¸éè¦çå¤ªå¤çå¸®å©ææ¡£åèµæå°±è½çç»å°ä½¿ç¨
-tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](./test.py) å¨
-Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_win32.png]
-(docs/images/test_win32.png) [test.py](./test.py) å¨ Linux
-ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png](docs/
-images/test_linux.png) Contents/æ¨¡ååå®¹ ------------------- Each non
-internal class and function in the module will be described in detail here
+tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](test.py) å¨
+Windows ç³»ç»ï¼**Windows10**ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ !
+[test_windows10.png](docs/images/test_windows10.png) [test.py](test.py) å¨
+Linux ç³»ç»ï¼**Ubuntu22.04**ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png]
+(docs/images/test_linux.png) [test.py](test.py) å¨ Windows
+ç³»ç»ï¼**Windows11**ï¼ä¸è¿è¡ççé¢å¦ä¸(æºè½æ§å¶åè§åå¾)ï¼
+![test_windows11.png](docs/images/test_windows11.png) Contents/æ¨¡ååå®¹ ---
+---------------- Each non internal class and function in the module will be
+described in detail here
 è¿éä¼è¯¦ç»è¯´ææ¨¡åä¸­çæ¯ä¸ªéåé¨ç±»åå½æ° ### Container
 Widget/å®¹å¨æ§ä»¶ 1. `Tk`: çªå£ç±»
 ç»§æ¿äº`tkinter.Tk`ï¼å¨ç»§æ¿äº`tkinter`æ¨¡åå`Tk`çåºç¡ä¸ï¼åå å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¹¶å å¥äºæ£æµçªå£å¤§å°æ¯å¦ç¼©æ¾çæºå¶ï¼ä»¥ä½¿å¾å¶å­`Canvas`åè½æ­£ç¡®å°è¿è¡ç¼©æ¾
 2. `Toplevel`: é¡¶çº§çªå£ç±»
 ç»§æ¿äº`tkinter.Toplevel`å`Tk`ï¼å å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¶ä½åä¸`Tk`ä¸æ ·
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
@@ -295,11 +297,11 @@
 ### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
 ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
 æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
 examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
------- > GitHub: > https://github.com/Xiaokang2022/tkintertools > GitCode
-(Mirror/éå): > https://gitcode.net/weixin_62651706/tkintertools > Gitee
-(Mirror/éå): > https://gitee.com/xiaokang-2022/tkintertools
-è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
+------ > GitHub: > https://github.com/Xiaokang2022/tkintertools > Gitee(Mirror/
+éå): > https://gitee.com/xiaokang-2022/tkintertools > GitCode(Mirror/
+éå): > https://gitcode.net/weixin_62651706/tkintertools
+è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](tkintertools/) ä¸­æ¢ç´¢ï¼
```

