# Comparing `tmp/pysimflow-0.0.40.tar.gz` & `tmp/pysimflow-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysimflow-0.0.40.tar", last modified: Wed May 24 11:17:34 2023, max compression
+gzip compressed data, was "pysimflow-0.0.42.tar", last modified: Wed Jun  7 02:41:30 2023, max compression
```

## Comparing `pysimflow-0.0.40.tar` & `pysimflow-0.0.42.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:17:34.535807 pysimflow-0.0.40/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-24 11:17:34.536807 pysimflow-0.0.40/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    29351 2023-05-24 04:24:44.000000 pysimflow-0.0.40/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:17:34.535807 pysimflow-0.0.40/digitaltwin/
--rw-r--r--   0 root         (0) root         (0)      384 2023-05-24 11:13:44.000000 pysimflow-0.0.40/digitaltwin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-05-24 09:06:06.000000 pysimflow-0.0.40/digitaltwin/active_obj.py
--rw-r--r--   0 root         (0) root         (0)    16452 2023-05-24 03:11:27.000000 pysimflow-0.0.40/digitaltwin/camera.py
--rw-r--r--   0 root         (0) root         (0)     3934 2023-05-24 08:31:10.000000 pysimflow-0.0.40/digitaltwin/editor.py
--rw-r--r--   0 root         (0) root         (0)     2663 2023-05-24 07:12:44.000000 pysimflow-0.0.40/digitaltwin/placer.py
--rw-r--r--   0 root         (0) root         (0)    10083 2023-03-15 13:18:59.000000 pysimflow-0.0.40/digitaltwin/printer.py
--rw-r--r--   0 root         (0) root         (0)     3554 2023-05-12 09:18:14.000000 pysimflow-0.0.40/digitaltwin/render.py
--rw-r--r--   0 root         (0) root         (0)    20135 2023-05-24 06:06:28.000000 pysimflow-0.0.40/digitaltwin/robot.py
--rw-r--r--   0 root         (0) root         (0)     6143 2023-05-24 06:42:20.000000 pysimflow-0.0.40/digitaltwin/scene.py
--rw-r--r--   0 root         (0) root         (0)     2592 2023-05-24 07:57:44.000000 pysimflow-0.0.40/digitaltwin/stacker.py
--rw-r--r--   0 root         (0) root         (0)     6296 2023-05-24 01:54:30.000000 pysimflow-0.0.40/digitaltwin/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:17:34.535807 pysimflow-0.0.40/digitaltwin_data/
--rw-r--r--   0 root         (0) root         (0)       99 2023-05-24 11:15:22.000000 pysimflow-0.0.40/digitaltwin_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:17:34.535807 pysimflow-0.0.40/pysimflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-24 11:17:34.000000 pysimflow-0.0.40/pysimflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      471 2023-05-24 11:17:34.000000 pysimflow-0.0.40/pysimflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 11:17:34.000000 pysimflow-0.0.40/pysimflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-24 11:17:34.000000 pysimflow-0.0.40/pysimflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 11:17:34.000000 pysimflow-0.0.40/pysimflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-05-24 11:17:34.536807 pysimflow-0.0.40/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-24 11:17:28.000000 pysimflow-0.0.40/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 02:41:30.293341 pysimflow-0.0.42/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-07 02:41:30.293341 pysimflow-0.0.42/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    26999 2023-06-07 02:03:31.000000 pysimflow-0.0.42/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 02:41:30.292342 pysimflow-0.0.42/digitaltwin/
+-rw-r--r--   0 root         (0) root         (0)      493 2023-06-05 06:58:11.000000 pysimflow-0.0.42/digitaltwin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2023-05-29 08:58:34.000000 pysimflow-0.0.42/digitaltwin/active_obj.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-06-05 08:48:15.000000 pysimflow-0.0.42/digitaltwin/box.py
+-rw-r--r--   0 root         (0) root         (0)    16516 2023-05-30 11:24:25.000000 pysimflow-0.0.42/digitaltwin/camera.py
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-06-05 06:50:25.000000 pysimflow-0.0.42/digitaltwin/cube.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-05 06:56:29.000000 pysimflow-0.0.42/digitaltwin/cylinder.py
+-rw-r--r--   0 root         (0) root         (0)     4392 2023-06-05 09:24:58.000000 pysimflow-0.0.42/digitaltwin/editor.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-05-25 09:07:12.000000 pysimflow-0.0.42/digitaltwin/placer.py
+-rw-r--r--   0 root         (0) root         (0)    10083 2023-03-15 13:18:59.000000 pysimflow-0.0.42/digitaltwin/printer.py
+-rw-r--r--   0 root         (0) root         (0)     3554 2023-05-12 09:18:14.000000 pysimflow-0.0.42/digitaltwin/render.py
+-rw-r--r--   0 root         (0) root         (0)    22619 2023-06-05 09:46:39.000000 pysimflow-0.0.42/digitaltwin/robot.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-05-30 11:28:51.000000 pysimflow-0.0.42/digitaltwin/scene.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-06-02 01:48:36.000000 pysimflow-0.0.42/digitaltwin/stacker.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2023-06-05 04:04:34.000000 pysimflow-0.0.42/digitaltwin/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 02:41:30.292342 pysimflow-0.0.42/digitaltwin_data/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-25 02:54:55.000000 pysimflow-0.0.42/digitaltwin_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 02:41:30.293341 pysimflow-0.0.42/pysimflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-07 02:41:30.000000 pysimflow-0.0.42/pysimflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      534 2023-06-07 02:41:30.000000 pysimflow-0.0.42/pysimflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 02:41:30.000000 pysimflow-0.0.42/pysimflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-07 02:41:30.000000 pysimflow-0.0.42/pysimflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-07 02:41:30.000000 pysimflow-0.0.42/pysimflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-07 02:41:30.293341 pysimflow-0.0.42/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      368 2023-06-07 02:37:57.000000 pysimflow-0.0.42/setup.py
```

### Comparing `pysimflow-0.0.40/README.md` & `pysimflow-0.0.42/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 [TOC]
 
 <div style="page-break-after: always;" ></div>
 
 # 1 概述
 
-        本文的目标在于梳理并定义前端业务接口规范，用于避免SDK开发者在不完全了解前端业务的情况下开发出不兼容的接口。 
+        一套简易的机械臂仿真工作流测试框架。
 
 ## 1.1 安装
 
-下载源代码：`pip3 install pysimflow`
+`pip3 install pysimflow`
 
-## 1.2 快速开始
 
 
+## 1.2 示例工作流
 
 获取一堆工件的深度图：`python3 test.py`
 
 获取一堆工件的姿态数据：`python3 test0.py`
 
 混合拆垛演示：`python3 test1.py`
 
@@ -26,72 +26,55 @@
 
 虚拟相机拍摄点云：`python3 test3.py`
 
 标定： `python3 test5.py`
 
 # 2 工作计划
 
-| 目标                | 任务                    | 问题                             | 备注                          |
-| ----------------- | --------------------- | ------------------------------ | --------------------------- |
-| 接口定义              | 场景查看                  | 载入/重置                          |                             |
-|                   |                       | 获取物体标识                         |                             |
-|                   |                       | 获取场景画面                         |                             |
-|                   |                       | 暂停/继续仿真                        |                             |
-|                   |                       | 平移/旋转/缩放/焦点                    |                             |
-|                   |                       | 视图切换-前后左右                      |                             |
-|                   |                       | 绘制原点/碰撞点                       | 实现较为复杂                      |
-|                   |                       | 关闭场景                           |                             |
-|                   | 场景编辑                  | 坐标检测                           |                             |
-|                   |                       | 选择/添加/删除/保存                    |                             |
-|                   |                       | 透明化                            |                             |
-|                   |                       | 移动/旋转/缩放                       |                             |
-|                   | 物体                    | 位置/姿态                          |                             |
-|                   |                       | 标识                             |                             |
-|                   |                       | 模型更换                           |                             |
-|                   |                       | 纹理更换                           |                             |
-|                   | 物体.机械臂                | 获取/设置末端执行器                     |                             |
-|                   |                       | 获取/设置末端执行器姿态                   |                             |
-|                   |                       | 获取/设置末端执行器位置                   |                             |
-|                   |                       | 设置末端执行器数字输出                    |                             |
-|                   |                       | 获取关节数                          |                             |
-|                   |                       | 获取/设置关节位置                      |                             |
-|                   |                       | 获取/设置速度                        |                             |
-|                   |                       | 设置当前位置为休息点                     |                             |
-|                   |                       | 前往休息点                          |                             |
-|                   | 物体.相机                 | 获取相机画面                         |                             |
-|                   |                       | 获取/设置标定参数                      |                             |
-|                   |                       | 设置/清除点云                        |                             |
-|                   | 物体.码垛器                | 区域参数                           |                             |
-|                   |                       | 工件更换                           |                             |
-|                   | 物体.放置器                | 区域参数                           |                             |
-|                   |                       | 获取/设置工件                        |                             |
-|                   |                       | 获取/设置工件纹理                      |                             |
-|                   |                       | 获取/设置放置点                       |                             |
-|                   |                       | 获取/设置总计工件数                     |                             |
-|                   |                       | 获取/设置缩放因子                      |                             |
-|                   |                       | 获取/设置放置模式                      |                             |
-|                   | 工作流                   | 获取可用节点                         |                             |
-|                   |                       | 设置/获取                          |                             |
-|                   |                       | 启动/停止                          | 结束后崩溃                       |
-|                   | ..................... | .............................. |                             |
-| SimEngine<br/>陈君辉 | 验收要求                  | 载入物体的示例                        | 可以调节位置和姿态，并且与地面发生物理交互，如碰撞   |
-|                   |                       | 获取RGBD图的示例                     | 显示RGB图，深度图展现为灰度图的形式         |
-|                   |                       | 获取物体姿态的示例                      | 通过射线检测物体的存在，然后把该物体的姿态轴画出来即可 |
-|                   |                       | 吸盘吸附物体的示例                      | 对力的控制功能                     |
-|                   |                       | 夹爪拾取物体的示例                      | 对摩擦的控制功能                    |
-|                   |                       | 控制一个关节的运动，使另一个关节进行同步运动         | 对关节同步的控制功能                  |
-|                   | ..................... |                                |                             |
-| DexSim<br/>李瑶     | 验收要求                  | 一堆工件生成的示例                      |                             |
-|                   |                       | 一堆工件的深度图示例                     |                             |
-|                   |                       | 一堆工件的姿态示例                      |                             |
-|                   |                       | 控制机械臂+吸盘去拾取工件                  |                             |
-|                   |                       | 控制机械臂+夹爪去拾取工件                  |                             |
-|                   |                       |                                |                             |
+| 目标     | 任务     | 问题               | 备注  |
+| ------ | ------ | ---------------- | --- |
+| 前端接口实现 | 场景查看   | 载入/重置            |     |
+|        |        | 获取物体标识           |     |
+|        |        | 获取场景画面           |     |
+|        |        | 暂停/继续仿真          |     |
+|        |        | 平移/旋转/缩放/焦点      |     |
+|        |        | 视图切换-前后左右        |     |
+|        |        | 绘制原点/碰撞点         |     |
+|        |        | 关闭场景             |     |
+|        | 场景编辑   | 坐标检测             |     |
+|        |        | 选择/添加/删除/保存      |     |
+|        |        | 透明化              |     |
+|        |        | 移动/旋转/缩放         |     |
+|        | 物体     | 位置/姿态            |     |
+|        |        | 标识               |     |
+|        |        | 模型更换             |     |
+|        |        | 纹理更换             |     |
+|        | 物体.机械臂 | 获取/设置末端执行器       |     |
+|        |        | 获取/设置末端执行器-位置/姿态 |     |
+|        |        | 设置末端执行器数字输出      |     |
+|        |        | 获取/设置关节位置        |     |
+|        |        | 获取/设置速度          |     |
+|        |        | 设置/前往休息点         |     |
+|        | 物体.相机  | 获取相机画面           |     |
+|        |        | 获取/设置标定参数        |     |
+|        |        | 设置/清除点云          |     |
+|        | 物体.码垛器 | 区域参数             |     |
+|        |        | 工件更换             |     |
+|        | 物体.放置器 | 区域参数             |     |
+|        |        | 获取/设置工件          |     |
+|        |        | 获取/设置工件纹理        |     |
+|        |        | 获取/设置放置点         |     |
+|        |        | 获取/设置总计工件数       |     |
+|        |        | 获取/设置缩放因子        |     |
+|        |        | 获取/设置放置模式        |     |
+|        | 工作流    | 获取可用节点           |     |
+|        |        | 设置/获取            |     |
+|        |        | 启动/停止            |     |
 
-# 3 业务流程
+# 3 功能接口
 
 ## 3.1 场景-载入场景并获取画面
 
         通过解析一个场景文件并加载其定义的物体到分拣场景中，通过渲染到纹理技术获取场景画面到前端显示。  
 
         文件定义如下：
 
@@ -149,14 +132,41 @@
     ui->>scene: 获取场景画面()
     scene->>bullet: 获取相机图片
     note left of bullet: 相关函数：getCameraImage
     scene-->>ui: 返回场景相机的画面纹理，以RGBA格式的一维数组形式
     ui->ui: 将纹理绘制到窗口上
 ```
 
+### Python
+
+```python
+import os
+from digitaltwin import Scene
+import digitaltwin_data
+
+data_dir = digitaltwin_data.get_data_path()
+scene = Scene(1024,768,data_dir)
+scene.load(os.path.join(data_dir,'scenes/空.json'))
+
+rgba = scene.rtt()
+```
+
+### C++
+
+```cpp
+#include "digitaltwin.hpp"
+using namespace digitaltwin; 
+
+auto scene = make_shared<Scene>(1024,768,"./digitaltwin","./digitaltwin_data");
+scene->load("./digitaltwin_data/scenes/空.json"); 
+
+Texture texture;
+scene->rtt(texture); 
+```
+
 ## 3.2 场景-启动/停止
 
         当场景布置完毕后，执行启动即可持续进行物理运算。停止则暂停物理运算。
 
 ```mermaid
 sequenceDiagram
     participant ui as 前端
@@ -164,14 +174,51 @@
     ui->>scene: 启动()
     scene->>bullet: 创建一个循环执行场景更新的任务
     note left of bullet: 相关函数：stepSimulation
     ui->>scene: 停止()
     scene->scene: 停止场景更新的任务
 ```
 
+### Python
+
+```python
+from threading import Thread
+from digitaltwin import Scene,Workflow,Editor
+import digitaltwin_data
+
+data_dir = digitaltwin_data.get_data_path()
+scene = Scene(1024,768,data_dir)
+scene.load(os.path.join(data_dir,'scenes/空.json'))
+
+def updating():
+    import time
+    while True:
+        scene.update_for_tick(1/180.)
+        time.sleep(1/180.)
+
+t = Thread(target=updating)
+t.start()
+```
+
+### C++
+
+```cpp
+#include "digitaltwin.hpp"
+using namespace digitaltwin; 
+
+auto scene = make_shared<Scene>(1024,768,"./digitaltwin","./digitaltwin_data");
+scene->load("./digitaltwin_data/scenes/空.json"); 
+
+scene->play(false);
+
+//做些什么...
+
+scene->play();
+```
+
 ## 3.3 场景-视口控制
 
         用户会经常使用鼠标或者手势进行镜头控制。
 
 ```mermaid
 sequenceDiagram
     participant ui as 前端
@@ -186,14 +233,33 @@
     note left of bullet: 相关函数：resetDebugVisualizerCamera
     ui->>scene: 缩放(缩放百分比)
     scene->scene: 计算相机位置相对于焦点位置的距离
     scene->bullet: 重新设置相机的位置
     note left of bullet: 相关函数：resetDebugVisualizerCamera
 ```
 
+### Python
+
+```python
+
+```
+
+### C++
+
+```cpp
+#include "digitaltwin.hpp"
+using namespace digitaltwin; 
+
+auto scene = make_shared<Scene>(1024,768,"./digitaltwin","./digitaltwin_data");
+scene->load("./digitaltwin_data/scenes/空.json"); 
+
+scene->rotate(0.1,0.0); 
+scene->pan(0.1,0.0);
+```
+
 ## 3.4 场景-获取选中物体的信息
 
         用户在布置场景的时候会通过鼠标获取物体的各种信息。
 
 ```mermaid
 sequenceDiagram
     participant ui as 前端
@@ -221,17 +287,66 @@
     end
     opt 物体.堆叠器
         scene-->>ui: 额外的属性(区域大小,工件)
     end
     ui->ui: 显示物体属性
 ```
 
+### Python
+
+```python
+
+```
+
+### C++
+
+```cpp
+#include "digitaltwin.hpp"
+using namespace digitaltwin; 
+
+auto scene = make_shared<Scene>(1024,768,"./digitaltwin","./digitaltwin_data");
+auto editor = make_shared<Editor>(scene.get());
+scene->load("./digitaltwin_data/scenes/标定测试.json"); 
+
+RayInfo hit;
+editor->ray(0.5,0.5,hit);
+
+auto objs = scene->get_active_objs();
+auto obj = objs[hit.name];
+cout << obj.get_name() << endl;
+
+
+```
+
 ## 3.5 场景-保存
 
-        当对场景进行了编辑之后，调用此函数来进行保存。
+        当对场景的物体进行修改之后，调用此函数来进行保存。
+
+### C++
+
+```cpp
+#include "digitaltwin.hpp"
+using namespace digitaltwin; 
+
+auto scene = make_shared<Scene>(1024,768,"./digitaltwin","./digitaltwin_data");
+auto editor = make_shared<Editor>(scene.get());
+scene->load("./digitaltwin_data/scenes/标定测试.json"); 
+
+RayInfo hit;
+editor->ray(0.5,0.5,hit);
+
+auto objs = scene->get_active_objs();
+auto obj = objs[hit.name];
+obj.set_pos({0,0,1});
+scene.save();
+
+
+```
+
+
 
 ## 3.5 物体-更换模型
 
         用户布置场景的时候会对模型进行替换。
 
 ```mermaid
 sequenceDiagram
@@ -243,14 +358,28 @@
     ui->>obj: 更换模型(模型路径)
     obj->bullet: 删除场景已有的模型
     note left of bullet: 相关函数：removeBody
     obj->bullet: 解析模型路径，读取模型到场景
     note left of bullet: 相关函数：loadURDF
 ```
 
+### C++
+
+```cpp
+#include "digitaltwin.hpp"
+using namespace digitaltwin; 
+
+auto scene = make_shared<Scene>(1024,768,"./digitaltwin","./digitaltwin_data");
+auto editor = make_shared<Editor>(scene.get());
+scene->load("./digitaltwin_data/scenes/标定测试.json"); 
+
+
+
+```
+
 ## 3.6 物体.机器人-更换抓手
 
         用户在为不同工件采用不同的机器人抓手。
 
 ```mermaid
 sequenceDiagram
     participant ui as 前端
@@ -669,7 +798,11 @@
 ## 3.12 工作流-获取/设置
 
         前端要去绘制一个场景的工作流程时，首先要去调用获取函数得到流程信息（中文翻译由前端完成）。修改完流程后调用设置函数去保存工作流程信息。
 
 ## 3.13 工作流-启动/停止
 
         让整个场景工作起来，调用启动函数。需要突然终止则调用停止函数。
+
+## 3.14 工作流-移动节点
+
+3.1
```

### Comparing `pysimflow-0.0.40/digitaltwin/active_obj.py` & `pysimflow-0.0.42/digitaltwin/active_obj.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         self.scale = self.profile['scale']
         self.user_data = self.profile['user_data'] if 'user_data' in self.profile else ''
 
         self.set_base(self.base)
         pass
 
     def __del__(self):
+        self.actions.clear()
         if 'id' in vars(self): p.removeBody(self.id)
         pass
  
     def properties(self):
         return dict(kind='ActiveObject',name=self.name,base=self.base,pos=self.pos,rot=self.rot,scale=self.scale,user_data=self.user_data if 'user_data' in vars(self) else '')
     
     def update(self,dt):
```

### Comparing `pysimflow-0.0.40/digitaltwin/camera.py` & `pysimflow-0.0.42/digitaltwin/camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,18 @@
         self.sensor_h = np.tan(self.fov / 2) * self.focal * 2
         self.intrinsics = self.get_intrinsics()
         self.extrinsics = self.get_extrinsics()
 
         self.point_ids = list()
         self.rgb_pixels = bytes()
         self.depth_pixels = bytes()
+
+    def __del__(self):
+        self.clear_point_cloud()
+        super().__del__()
     
     def properties(self):
         properties = super().properties()
         properties.update(kind='Camera3DReal',focal=self.focal,
                           fov=self.fov,
                           pixels_w=self.pixels_w,
                           pixels_h=self.pixels_h,
@@ -292,15 +296,15 @@
         self.clear_point_cloud()
         pass
 
     def rtt(self):
         self.signal_capture()
         
     def signal_check(self,*args,**kwargs):
-        self.result = None,self.profile['eye_to_hand_transform']
+        self.result = None,self.extrinsics
 
     def signal_capture(self,*args,**kwargs):
         try:
             sk = s.socket(s.AF_UNIX,s.SOCK_STREAM)
             sock_path = os.path.join(self.scene.tmp_dir,self.profile['name'] + '.sock')
             sk.connect(sock_path)
             width = int.from_bytes(sk.recv(4),'little')
@@ -409,29 +413,28 @@
         while beg < end:
             offset = end - beg
             if offset > 10000: offset = 10000
             point_id = p.addUserDebugPoints(point_cloud[beg:beg+offset],point_cloud_color[beg:beg+offset,0:3],1,lifeTime=0)
             self.point_ids.append(point_id)
             beg += offset
 
-
     def draw_point_cloud(self,vertexes,colors):
         R = Rotation.from_euler('xyz',self.rot)
         T = self.pos
         
         if len(vertexes) > len(colors): colors.extend([0,0,0]*(len(vertexes)-len(colors)))
         vertexes = R.apply(vertexes) + T
         
         beg = 0; end = len(vertexes)
         while beg < end:
             offset = end - beg
             if offset > 10000: offset = 10000
             point_id = p.addUserDebugPoints(vertexes[beg:beg+offset],colors[beg:beg+offset],1,lifeTime=0)
             self.point_ids.append(point_id)
-        beg += offset
+            beg += offset
         pass
 
     def clear_point_cloud(self):
         for point_id in self.point_ids: p.removeUserDebugItem(point_id)
         pass
```

### Comparing `pysimflow-0.0.40/digitaltwin/placer.py` & `pysimflow-0.0.42/digitaltwin/placer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pybullet as p
 import numpy as np
 import random
 import py3dbp as bp
 import random
-from .active_obj import ActiveObject
+import os
+from digitaltwin.active_obj import ActiveObject
 
 class Placer(ActiveObject):
     def __init__(self,scene,**kwargs):
         if 'workpiece_texture' not in kwargs: kwargs['workpiece_texture'] = '' 
         if 'workpiece' not in kwargs: kwargs['workpiece'] = 'workpieces/lego/lego.urdf' 
         if 'center' not in kwargs: kwargs['center'] = [0,0,0]
         if 'interval' not in kwargs: kwargs['interval'] = 1
@@ -54,17 +55,17 @@
 
     def set_interval(self,seconds):
         self.interval = seconds
 
     def signal_generate(self,*args,**kwargs):
         def task():
             rot = np.array([random.randint(0,314),random.randint(0,314),random.randint(0,314)]) / 100.
-            self.objs.append(p.loadURDF(self.profile['workpiece'],self.profile['center'],p.getQuaternionFromEuler(rot)))
+            self.objs.append(p.loadURDF(os.path.join(self.scene.data_dir,self.workpiece),self.center,p.getQuaternionFromEuler(rot)))
         
-        for i in range(self.profile['amount']): self.actions.append((task, ()))
+        for i in range(self.amount): self.actions.append((task, ()))
 
         def task1():
             num = 0 
             for o in self.objs:
                 linear,angular = p.getBaseVelocity(o)
                 n = np.linalg.norm(linear) + np.linalg.norm(angular)
                 if n > num: num = n
```

### Comparing `pysimflow-0.0.40/digitaltwin/printer.py` & `pysimflow-0.0.42/digitaltwin/printer.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.40/digitaltwin/render.py` & `pysimflow-0.0.42/digitaltwin/render.py`

 * *Files identical despite different names*

### Comparing `pysimflow-0.0.40/digitaltwin/robot.py` & `pysimflow-0.0.42/digitaltwin/robot.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,45 +20,50 @@
         
         super().__init__(scene, **kwargs)
         self.pickup = False
         pass
     
     def properties(self):
         properties = super().properties()
+        
+        x,y,z,rx,ry,rz = self.get_end_effector_pose()
         properties.update(kind='Robot',speed=self.speed,
                           end_effector=self.end_effector,
                           joint_damping=self.joint_damping,
                           current_joint_poses=self.current_joint_poses,
-                          reset_joint_poses=self.reset_joint_poses)
+                          reset_joint_poses=self.reset_joint_poses,
+                          end_effector_pos=[x,y,z],end_effector_rot=[rx,ry,rz])
         return properties
 
     def update(self,dt):
         super().update(dt)
         if self.end_effector_obj:
             self.end_effector_obj.update(dt)
             if not self.end_effector_obj.idle: self.actions.append((lambda *args:None,()))
         pass
 
     def restore(self):
         super().restore()
-        p.setJointMotorControlArray(self.id, self.active_joint_indexes, p.POSITION_CONTROL, self.reset_joint_poses)
+        p.setJointMotorControlArray(self.id, self.used_joint_indexes, p.POSITION_CONTROL, self.reset_joint_poses)
         self.end_effector_obj.do(False)
 
     def set_base(self,base):
         base_temp = self.base = base
         
         ee_kind = ""
         mimic_name = ''
         gears = []
         with xml.parse(os.path.join(self.scene.data_dir,base)) as doc_robot:
             node_robot = doc_robot.getElementsByTagName('robot')[0]
             for mesh in node_robot.getElementsByTagName('mesh'):
                 filename = mesh.getAttribute('filename')
                 mesh.setAttribute('filename',os.path.join(self.scene.data_dir,os.path.dirname(base),filename))
 
+            num_joints = len(node_robot.getElementsByTagName('link'))
+
             if self.end_effector:
                 link_ee = node_robot.getElementsByTagName('link')[-1]
                 link_ee_name = link_ee.getAttribute('name')
                 with xml.parse(os.path.join(self.scene.data_dir,self.end_effector)) as doc_ee:
                     node_ee = doc_ee.getElementsByTagName('robot')[0]
                     ee_kind = node_ee.getAttribute("kind")
                     for mesh in node_ee.getElementsByTagName('mesh'):
@@ -71,122 +76,149 @@
                         if i == 0: joint.getElementsByTagName('parent')[0].setAttribute('link',link_ee_name)
                         node_robot.appendChild(joint)
                         node_mimics = joint.getElementsByTagName('mimic')
                         if not node_mimics: continue
                         node_mimic = node_mimics[0]
                         mimic_name = node_mimic.getAttribute('joint')
                         joint_name = joint.getAttribute('name')
-                        multiplier = int(node_mimic.getAttribute('multiplier')) if node_mimic.hasAttribute('multiplier') else 0
+                        multiplier = int(node_mimic.getAttribute('multiplier')) if node_mimic.hasAttribute('multiplier') else 1
                         offset = 0#int(node_mimic.getAttribute('offset'))
                         gears.append((mimic_name,joint_name,multiplier))
                 node_robot.removeChild(link_ee).unlink()
 
             import tempfile
             f = tempfile.NamedTemporaryFile("w",delete=False)
             base_temp = f.name
             f.write(node_robot.toxml())
             f.close()
 
         if 'id' in vars(self): p.removeBody(self.id)
-        print('robot urdf',base_temp)
+        print('robot urdf',base_temp,flush=True)
         self.id = p.loadURDF(base_temp, self.pos, p.getQuaternionFromEuler(self.rot),useFixedBase=True)
-
         if ee_kind == 'Gripper': self.end_effector_obj = Gripper(self.id,gears)
         elif ee_kind == 'Suction': self.end_effector_obj = Suction(self.id)
         else: 
-            class PlaceHolder:
+            class EndEffector:
                 def __init__(self): self.idle = True
                 def update(self,dt):pass
                 def do(self,pickup):pass
-            self.end_effector_obj = PlaceHolder()
+                def get_properties(self): return dict(king='EndEffector')
+            self.end_effector_obj = EndEffector()
             pass
 
-        num_joints = p.getNumJoints(self.id)
+        self.used_joint_indexes = []
         self.active_joint_indexes = []
-        for i in range(num_joints):
+        self.joint_velocities = []
+        for i in range(p.getNumJoints(self.id)):
+            p.setCollisionFilterPair(self.scene.plane,self.id,-1,i,0)
             ji = p.getJointInfo(self.id, i)
-            jointName,jointType = ji[1],ji[2]
+            jointName,jointType,jointVelocity = ji[1],ji[2],ji[11]
             if (jointType != p.JOINT_REVOLUTE and jointType != p.JOINT_PRISMATIC and jointType != p.JOINT_SPHERICAL): continue
-            if i < len(self.reset_joint_poses): p.resetJointState(self.id, i, self.reset_joint_poses[i])
             self.active_joint_indexes.append(i)
+            self.joint_velocities.append(jointVelocity)
+            if i < num_joints: self.used_joint_indexes.append(i)
+        
+        if len(self.active_joint_indexes) > len(self.joint_damping): self.joint_damping.extend([0]*(len(self.active_joint_indexes)-len(self.joint_damping)))
+        else: self.joint_damping = self.joint_damping[:len(self.active_joint_indexes)]
 
-        if len(self.active_joint_indexes) > len(self.joint_damping): 
-            self.joint_damping.extend([0]*(len(self.active_joint_indexes)-len(self.joint_damping)))
-            self.reset_joint_poses.extend([0]*(len(self.active_joint_indexes)-len(self.reset_joint_poses)))
-        else: 
-            self.joint_damping = self.joint_damping[:len(self.active_joint_indexes)]
-            self.reset_joint_poses = self.reset_joint_poses[:len(self.active_joint_indexes)]
+        if len(self.used_joint_indexes) > len(self.reset_joint_poses): self.reset_joint_poses.extend([0]*(len(self.used_joint_indexes)-len(self.reset_joint_poses)))
+        else: self.reset_joint_poses = self.reset_joint_poses[:len(self.used_joint_indexes)]
+
+        self.set_joints(self.reset_joint_poses)
         
-        pos,orn,_,_,_,_ = p.getLinkState(self.id,num_joints-1)
+        if 'end_effector_axis' in vars(self):
+            p.removeUserDebugItem(self.end_effector_axis[0])
+            p.removeUserDebugItem(self.end_effector_axis[1])
+            p.removeUserDebugItem(self.end_effector_axis[2])
+
+        pos,orn,_,_,_,_ = p.getLinkState(self.id,p.getNumJoints(self.id)-1)
         axis_x = Rotation.from_quat(orn).apply(np.array([0.05,0,0])) + pos
         axis_y = Rotation.from_quat(orn).apply(np.array([0,0.05,0])) + pos
         axis_z = Rotation.from_quat(orn).apply(np.array([0,0,0.05])) + pos
-        p.addUserDebugLine(pos,axis_x,[1,0,0],2,lifeTime=20)
-        p.addUserDebugLine(pos,axis_y,[0,1,0],2,lifeTime=20)
-        p.addUserDebugLine(pos,axis_z,[0,0,1],2,lifeTime=20)
+        self.end_effector_axis = p.addUserDebugLine(pos,axis_x,[1,0,0],2),p.addUserDebugLine(pos,axis_y,[0,1,0],2),p.addUserDebugLine(pos,axis_z,[0,0,1],2)
+
         self.home_pos,self.home_rot = pos,p.getEulerFromQuaternion(orn)
     
     def set_speed(self,value):
         if round(value) == 0.000: return 
         self.speed = value
-    
+     
     def get_joints(self):
-        return self.current_joint_poses
+        return self.current_joint_poses[:len(self.used_joint_indexes)]
     
     def set_joints(self,joint_poses):
-        if len(self.active_joint_indexes) > len(joint_poses): 
-            joint_poses.extend([0]*(len(self.active_joint_indexes)-len(joint_poses)))
-        else: 
-            joint_poses = joint_poses[:len(self.active_joint_indexes)]
-
-        for i in self.active_joint_indexes: p.resetJointState(self.id, i, joint_poses[i])
-        # p.setJointMotorControlArray(self.id, self.active_joint_indexes, p.POSITION_CONTROL, joint_poses)
-        self.current_joint_poses = joint_poses
+        joint_poses = joint_poses[:len(self.used_joint_indexes)]
+        for i in self.used_joint_indexes: p.resetJointState(self.id, i, joint_poses[i])
+        p.setJointMotorControlArray(self.id, self.used_joint_indexes, p.POSITION_CONTROL, joint_poses)
+        self.current_joint_poses = joint_poses[:len(self.used_joint_indexes)]
     
-    def set_end_effector_pose(self,pos,rot):
-        pass
+    def set_end_effector_pose(self,pose):
+        num_joints = p.getNumJoints(self.id)
+        ee_index = num_joints-1
+        joint_poses = p.calculateInverseKinematics(self.id, ee_index, pose[0:3], p.getQuaternionFromEuler(pose[3:6]),restPoses=self.reset_joint_poses,maxNumIterations=200)
+        self.set_joints(list(joint_poses)[:len(self.used_joint_indexes)])
 
     def get_end_effector_pose(self):
         num_joints = p.getNumJoints(self.id)
         ee_pos,ee_orn,_,_,_,_ = p.getLinkState(self.id,num_joints-1)
         ee_rot = p.getEulerFromQuaternion(ee_orn)
         return [ee_pos[0],ee_pos[1],ee_pos[2],ee_rot[0],ee_rot[1],ee_rot[2]]
 
     def set_end_effector(self,base):
         if 'id' not in vars(self): return
         self.end_effector = base
         self.set_base(self.base)
         
-    def plan(self,origin,target,dt=1):
-        ee_pos,ee_rot = origin
-        o_pos,o_rot = target
-        o_pos = np.array(o_pos)
-        p.addUserDebugLine(ee_pos,o_pos,[0,1,0],2,lifeTime=5) 
+    def plan(self,target_pos,target_rot,s=1,mode='joint'):
+        target_orn = p.getQuaternionFromEuler(target_rot)
+        num_joints = p.getNumJoints(self.id)
+        ee_index = num_joints-1
 
+        ee_pos,ee_orn,_,_,_,_ = p.getLinkState(self.id,num_joints-1)
+        ee_pos = np.array(ee_pos)
+        ee_rot = p.getEulerFromQuaternion(ee_orn)
+        
         route_poses = list()
-        while np.linalg.norm(o_pos - ee_pos) != 0:
-            direction = o_pos - ee_pos
-            length = abs(np.linalg.norm(direction))
-            if length < (self.scene.timestep * dt * self.speed): 
-                increment_direction = direction
-            else: 
-                increment_direction = direction / length * (self.scene.timestep * dt * self.speed)
-            ee_pos += increment_direction
 
-            num_joints = p.getNumJoints(self.id)
-            ee_index = num_joints-1
-            ee_orn = p.getQuaternionFromEuler(o_rot)
-            ll = [-7]*len(self.active_joint_indexes)
-            ul = [7]*len(self.active_joint_indexes)
-            jr = [7]*len(self.active_joint_indexes)
-            
-            poses = p.calculateInverseKinematics(self.id, ee_index, ee_pos, ee_orn,
-                                                lowerLimits=ll,upperLimits=ul,jointRanges=jr,restPoses=self.reset_joint_poses,
-                                                jointDamping=self.joint_damping,maxNumIterations=200)
-            route_poses.append(poses)
+        if mode=='joint':
+            end_poses = p.calculateInverseKinematics(self.id, ee_index, target_pos, target_orn, restPoses=self.reset_joint_poses, maxNumIterations=200)
+            end_poses = list(end_poses)[:len(self.used_joint_indexes)]
+            num = int(1 / s / self.scene.timestep) + 1
+            for n in range(num):
+                poses = []
+                t = n / num
+                for i in range(len(self.current_joint_poses)):
+                    poses.append(np.interp(t,[0,1],[self.current_joint_poses[i],end_poses[i]]))
+                route_poses.append(poses[:len(self.used_joint_indexes)])
+        else:
+            num = int(1 / s / self.scene.timestep) + 1
+            for n in range(num):
+                poses = []
+                t = n / num
+                x = np.interp(t,[0,1],[ee_pos[0],target_pos[0]])
+                y = np.interp(t,[0,1],[ee_pos[1],target_pos[1]])
+                z = np.interp(t,[0,1],[ee_pos[2],target_pos[2]])
+                pos = [x,y,z]
+
+                q1 = np.array(ee_orn)
+                q2 = np.array(target_orn)
+                q_dot = q1.dot(q2)
+    
+                if (np.abs(q_dot) < 1e-5):
+                    orn = q1
+                else:
+                    if q_dot < 0:
+                        q2 = -q2
+                    
+                    orn = (1 - t) * q1 + t * q2
+                    orn = orn / np.linalg.norm(orn)
+
+                poses = p.calculateInverseKinematics(self.id, ee_index, pos, orn, restPoses=self.reset_joint_poses, maxNumIterations=200)
+                route_poses.append(list(poses)[:len(self.used_joint_indexes)])
+
         return route_poses
 
     def signal_pick_plan(self,*args,**kwargs):
         objs, = args
         def near_obj(o):
             e_pos,e_orn,_,_,_,_ = p.getLinkState(self.id,p.getNumJoints(self.id)-1)
             o_pos,e_pos = np.array(o[0]),np.array(e_pos)
@@ -234,37 +266,26 @@
         self.actions.append((output,()))
 
     def signal_plan_move(self,*args,**kwargs):
         num_joints = p.getNumJoints(self.id)
         ee_index = num_joints-1
 
         def task(*poses):
-            p.setJointMotorControlArray(self.id, self.active_joint_indexes, p.POSITION_CONTROL, poses)
+            p.setJointMotorControlArray(self.id, self.used_joint_indexes, p.POSITION_CONTROL, poses)
             self.current_joint_poses = poses
-            pos,orn,_,_,_,_ = p.getLinkState(self.id,ee_index)
-            # axis_x = Rotation.from_quat(orn).apply([0.05,0,0]) + pos
-            # axis_y = Rotation.from_quat(orn).apply([0,0.05,0]) + pos
-            # axis_z = Rotation.from_quat(orn).apply([0,0,0.05]) + pos
-            # p.addUserDebugLine(pos,axis_x,[1,0,0],2,lifeTime=0.1)
-            # p.addUserDebugLine(pos,axis_y,[0,1,0],2,lifeTime=0.1)
-            # p.addUserDebugLine(pos,axis_z,[0,0,1],2,lifeTime=0.1)
 
         def task2(*point):
             num_joints = p.getNumJoints(self.id)
             ee_index = num_joints-1
-            ll = [-7]*len(self.active_joint_indexes)
-            ul = [7]*len(self.active_joint_indexes)
-            jr = [7]*len(self.active_joint_indexes)
             
             poses = p.calculateInverseKinematics(self.id, ee_index, point, p.getQuaternionFromEuler([0,0,0]),
-                                                lowerLimits=ll,upperLimits=ul,jointRanges=jr,restPoses=self.self.current_joint_poses,
-                                                jointDamping=self.joint_damping,maxNumIterations=200)
-            p.setJointMotorControlArray(self.id, self.active_joint_indexes, p.POSITION_CONTROL, poses)
+                                                restPoses=self.current_joint_poses,jointDamping=self.joint_damping,maxNumIterations=200)[:len(self.used_joint_indexes)]
+            p.setJointMotorControlArray(self.id, self.used_joint_indexes, p.POSITION_CONTROL, poses)
 
-            self.current_joint_poses = poses
+            self.current_joint_poses = list(poses)
             p.addUserDebugPoints([point],[[1,1,1]],2,lifeTime=5)
 
         route_poses,route_points = args
         if route_poses:
             for poses in route_poses: self.actions.append((task,poses))
         else:
             for point in route_points: self.actions.append((task2,point))
@@ -275,177 +296,231 @@
             if round(last_pos - pos,6) != 0.000000:
                 self.actions.append((output,(pos,)))
                 return
             self.result = None,
         self.actions.append((output,(0,)))
         pass
 
-    def signal_pick_move(self,pick_points,**kwargs):
+    def signal_pick_move(self,*args,**kwargs):
+        if not args: 
+            active_plugins = kwargs['plugins']
+            picklight = active_plugins['PickLight']
+            _,pickpose = picklight.result
+            args = pickpose,
+        
         num_joints = p.getNumJoints(self.id)
         ee_index = num_joints-1
-
-        ee_pos,ee_orn,_,_,_,_ = p.getLinkState(self.id,num_joints-1)
+        ee_pos,ee_orn,_,_,_,_ = p.getLinkState(self.id,ee_index)
         ee_pos = np.array(ee_pos)
         ee_rot = p.getEulerFromQuaternion(ee_orn)
 
-        if not pick_points: 
-            self.result = 'failed', 
+        if 'speed' not in kwargs: kwargs['speed'] = 1
+        speed = kwargs['speed']
+        if speed == 0: 
+            if 'pickup' in kwargs: self.end_effector_obj.do(kwargs['pickup'])
+            self.result = None,[ee_pos[0],ee_pos[1],ee_pos[2],ee_rot[0],ee_rot[1],ee_rot[2]]
             return
 
-        pick_pos,pick_rot = pick_points[0]
-        route_poses = self.plan( (ee_pos,pick_rot), (pick_pos, pick_rot))
+        if 'mode' not in kwargs: kwargs['mode'] = 'joint'
+        mode = kwargs['mode']
+
+        pick_pose = args[0]
+        pick_pos,pick_rot = pick_pose[0:3],pick_pose[3:6]
+        pick_orn = p.getQuaternionFromEuler(pick_rot)
+        route_poses = self.plan( pick_pos, pick_rot, speed, mode)
+
+        if 'axis' in vars(self):
+            p.removeUserDebugItem(self.axis[0])
+            p.removeUserDebugItem(self.axis[1])
+            p.removeUserDebugItem(self.axis[2])
+        
+        axis_x = Rotation.from_euler('xyz',pick_rot).apply([0.05,0,0]) + pick_pos
+        axis_y = Rotation.from_euler('xyz',pick_rot).apply([0,0.05,0]) + pick_pos
+        axis_z = Rotation.from_euler('xyz',pick_rot).apply([0,0,0.05]) + pick_pos
+        self.axis = [
+            p.addUserDebugLine(pick_pos,axis_x,[1,0,0],2),
+            p.addUserDebugLine(pick_pos,axis_y,[0,1,0],2),
+            p.addUserDebugLine(pick_pos,axis_z,[0,0,1],2)
+        ]
 
         def task(*poses):
-            p.setJointMotorControlArray(self.id, self.active_joint_indexes, p.POSITION_CONTROL, poses)
+            p.setJointMotorControlArray(self.id, self.used_joint_indexes, p.POSITION_CONTROL, poses)
             self.current_joint_poses = poses
-            pos,orn,_,_,_,_ = p.getLinkState(self.id,ee_index)
-            # axis_x = Rotation.from_quat(orn).apply([0.05,0,0]) + pos
-            # axis_y = Rotation.from_quat(orn).apply([0,0.05,0]) + pos
-            # axis_z = Rotation.from_quat(orn).apply([0,0,0.05]) + pos
-            # p.addUserDebugLine(pos,axis_x,[1,0,0],2,lifeTime=0.1)
-            # p.addUserDebugLine(pos,axis_y,[0,1,0],2,lifeTime=0.1)
-            # p.addUserDebugLine(pos,axis_z,[0,0,1],2,lifeTime=0.1)
 
         for poses in route_poses: self.actions.append((task,poses))
-        
-        def output(last_pos):
-            pos,orn,_,_,_,_ = p.getLinkState(self.id,ee_index)
-            pos = np.linalg.norm(pos)
-            if round(last_pos - pos,6) != 0.000000:
-                self.actions.append((output,(pos,)))
-                return
+        def output(last_pos): 
+            if 'pickup' in kwargs: self.end_effector_obj.do(kwargs['pickup'])
             self.result = None,
-        
         self.actions.append((output,(0,)))
         pass
 
     def signal_move(self,*args,**kwargs):
-        if 'home' in kwargs:
+        if 'home' in kwargs and kwargs['home']:
             self.signal_home()
             return 
         
         num_joints = p.getNumJoints(self.id)
         ee_index = num_joints-1
         ee_pos,ee_orn,_,_,_,_ = p.getLinkState(self.id,ee_index)
         ee_pos = np.array(ee_pos)
         ee_rot = p.getEulerFromQuaternion(ee_orn)
+
+        if 'speed' not in kwargs: kwargs['speed'] = 1
+        speed = kwargs['speed']
+        if speed == 0: 
+            if 'pickup' in kwargs: self.end_effector_obj.do(kwargs['pickup'])
+            self.result = None,[ee_pos[0],ee_pos[1],ee_pos[2],ee_rot[0],ee_rot[1],ee_rot[2]]
+            return
+
         t_pos = ee_pos
         t_rot = ee_rot
-
-        if 'mode' in kwargs:
-            if 'point' == kwargs['mode']:
-                t_pos = kwargs['point'][0:3]
-                t_rot = kwargs['point'][3:6]
-                
-        def task(*poses):
-            p.setJointMotorControlArray(self.id, self.active_joint_indexes, p.POSITION_CONTROL, poses)
+        poses = []
+        
+        def task(poses):
+            p.setJointMotorControlArray(self.id, self.used_joint_indexes, p.POSITION_CONTROL, poses)
             self.current_joint_poses = poses
-            pos,orn,_,_,_,_ = p.getLinkState(self.id,ee_index)
-            # axis_x = Rotation.from_quat(orn).apply([0.05,0,0]) + pos
-            # axis_y = Rotation.from_quat(orn).apply([0,0.05,0]) + pos
-            # axis_z = Rotation.from_quat(orn).apply([0,0,0.05]) + pos
-            # p.addUserDebugLine(pos,axis_x,[1,0,0],2,lifeTime=0.1)
-            # p.addUserDebugLine(pos,axis_y,[0,1,0],2,lifeTime=0.1)
-            # p.addUserDebugLine(pos,axis_z,[0,0,1],2,lifeTime=0.1)
-    
-        route_poses = self.plan((ee_pos,ee_rot),(t_pos,t_rot))
-        for poses in route_poses: self.actions.append((task,(poses)))
         
-        def output(last_pos):
-            pos,orn,_,_,_,_ = p.getLinkState(self.id,ee_index)
-            pos = np.linalg.norm(pos)
-            if round(last_pos - pos,6) != 0.000000:
-                self.actions.append((output,(pos,)))
-                return
+        if 'mode' not in kwargs: kwargs['mode'] = 'joint'
+        mode = kwargs['mode']
 
+        if 'point' in kwargs:
+            t_pos = kwargs['point'][0:3]
+            t_rot = kwargs['point'][3:6]
+            route_poses = self.plan(t_pos,t_rot,speed,mode)
+            for poses in route_poses: self.actions.append((task,(poses,)))
+        else:
+            end_poses = kwargs['joints'][:len(self.current_joint_poses)]
+            num = int(1 / speed / self.scene.timestep)
+            route_poses = []
+            for n in range(num):
+                poses = []
+                t = n / num
+                for i in range(len(self.current_joint_poses)):
+                    poses.append(np.interp(t,[0,1],[self.current_joint_poses[i],end_poses[i]]))
+                self.actions.append((task,(poses,)))
+            
+        def output(last_pos): 
+            if 'pickup' in kwargs: self.end_effector_obj.do(kwargs['pickup'])
             self.result = None,
         self.actions.append((output,(0,)))
-        pass
+        pass    
     
     def signal_move_relatively(self,*args,**kwargs):
         num_joints = p.getNumJoints(self.id)
         ee_index = num_joints-1
         ee_pos,ee_orn,_,_,_,_ = p.getLinkState(self.id,ee_index)
-        ee_pos = np.array(ee_pos)
-        ee_rot = np.array(p.getEulerFromQuaternion(ee_orn))
+        ee_rot = p.getEulerFromQuaternion(ee_orn)
+
+        if args: 
+            pick_point = args[0]
+            ee_pos = pick_point[0:3]
+            ee_rot = pick_point[3:6]
+            ee_orn = p.getQuaternionFromEuler(ee_rot)
+
+        if 'target' not in kwargs: kwargs['target'] = 'task_current'
+        target = kwargs['target']
+
+        if target == 'task_next':
+            declare = kwargs['declare']
+            cursor = kwargs['cursor']
+            active_plugins = kwargs['plugins']
+
+            act = declare[cursor]
+            next = act['next']
+            act_next = declare[next]
+
+            if act_next['fun'] == 'move_relatively':
+                self.result = 'failed', 
+                return
+            elif act_next['fun'] == 'move':
+                move_args = act_next['args']
+                if 'point' not in move_args:
+                    self.result = 'non-suports relative to move of mode of joint!',
+                    return
+                
+                pick_point = move_args['point']
+            elif act_next['fun'] == 'pick_move':
+                picklight = active_plugins['PickLight']
+                _,pick_point = picklight.result
+
+                if not pick_point: 
+                    self.result = 'failed', 
+                    return
+                
+            ee_pos = pick_point[0:3]
+            ee_rot = pick_point[3:6]
+            ee_orn = p.getQuaternionFromEuler(ee_rot)
+
+        if 'speed' not in kwargs: kwargs['speed'] = 1
+        speed = kwargs['speed']
+        if speed == 0: 
+            if 'pickup' in kwargs: self.end_effector_obj.do(kwargs['pickup'])
+            self.result = None,[ee_pos[0],ee_pos[1],ee_pos[2],ee_rot[0],ee_rot[1],ee_rot[2]]
+            return
+
+        if 'mode' not in kwargs: kwargs['mode'] = 'joint'
+        mode = kwargs['mode']
+
         t_pos = ee_pos
         t_rot = ee_rot
 
-        if 'mode' in kwargs:
-            if 'point' == kwargs['mode']:
-                t_pos = kwargs['point'][0:3] + ee_pos
-                t_rot = kwargs['point'][3:6] + ee_rot
-            
-        def task(*poses):
-            p.setJointMotorControlArray(self.id, self.active_joint_indexes, p.POSITION_CONTROL, poses)
+        if 'point' in kwargs:
+            t_pos = kwargs['point'][0:3] + np.array(ee_pos)
+            t_rot = kwargs['point'][3:6] + np.array(ee_rot)
+        
+        route_poses = self.plan(t_pos,t_rot,speed,mode)
+
+        def task(poses):
+            p.setJointMotorControlArray(self.id, self.used_joint_indexes, p.POSITION_CONTROL, poses)
             self.current_joint_poses = poses
-            pos,orn,_,_,_,_ = p.getLinkState(self.id,ee_index)
-            # axis_x = Rotation.from_quat(orn).apply([0.05,0,0]) + pos
-            # axis_y = Rotation.from_quat(orn).apply([0,0.05,0]) + pos
-            # axis_z = Rotation.from_quat(orn).apply([0,0,0.05]) + pos
-            # p.addUserDebugLine(pos,axis_x,[1,0,0],2,lifeTime=0.1)
-            # p.addUserDebugLine(pos,axis_y,[0,1,0],2,lifeTime=0.1)
-            # p.addUserDebugLine(pos,axis_z,[0,0,1],2,lifeTime=0.1)
 
-        route_poses = self.plan((ee_pos,ee_rot),(t_pos,t_rot))
-        for poses in route_poses: self.actions.append((task,(poses)))
+        for poses in route_poses: self.actions.append((task,(poses,)))
         
-        def output(last_pos):
-            pos,orn,_,_,_,_ = p.getLinkState(self.id,ee_index)
-            pos = np.linalg.norm(pos)
-            if round(last_pos - pos,6) != 0.000000:
-                self.actions.append((output,(pos,)))
-                return
-
-            self.result = None,
+        def output(last_pos): 
+            if 'pickup' in kwargs: self.end_effector_obj.do(kwargs['pickup'])
+            self.result = None,[ee_pos[0],ee_pos[1],ee_pos[2],ee_rot[0],ee_rot[1],ee_rot[2]]
         self.actions.append((output,(0,)))
         pass
     
     def signal_do(self,*args,**kwargs):
-        def task(): self.end_effector_obj.do(kwargs['pickup'])
-        self.actions.append((task,()))
+        self.end_effector_obj.do(kwargs['pickup'])
         pass
 
     def signal_pick(self,*args,**kwargs):
-        def task(): self.end_effector_obj.do(True)
-        self.actions.append((task,()))
+        self.end_effector_obj.do(True)
         pass
+    
     def signal_place(self,*args,**kwargs):
-        def task(): self.end_effector_obj.do(False)
-        self.actions.append((task,()))
+        self.end_effector_obj.do(False)
         pass
     
     def signal_home(self):
         num_joints = p.getNumJoints(self.id)
         ee_index = num_joints-1
         ee_pos,ee_orn,_,_,_,_ = p.getLinkState(self.id,ee_index)
         ee_pos = np.array(ee_pos)
         ee_rot = p.getEulerFromQuaternion(ee_orn)
         
         t_pos = self.home_pos
         t_rot = self.home_rot
 
         self.reset_joint_poses
         joint_poses = []
-        for joint in self.active_joint_indexes:
+        for joint in self.used_joint_indexes:
             position,velocity,reaction_force,motor_torque = p.getJointState(self.id,joint)
             joint_poses.append(position)
 
-        def task(*poses):
-            p.setJointMotorControlArray(self.id, self.active_joint_indexes, p.POSITION_CONTROL, poses)
-            # pos,orn,_,_,_,_ = p.getLinkState(self.id,ee_index)
-            # axis_x = Rotation.from_quat(orn).apply([0.05,0,0]) + pos
-            # axis_y = Rotation.from_quat(orn).apply([0,0.05,0]) + pos
-            # axis_z = Rotation.from_quat(orn).apply([0,0,0.05]) + pos
+        def task(poses):
+            p.setJointMotorControlArray(self.id, self.used_joint_indexes, p.POSITION_CONTROL, poses)
+            self.current_joint_poses = poses
 
-        num = int(1 / self.scene.timestep) 
-        for t in range(num):
+        num = int(1 / self.speed / self.scene.timestep) + 1
+        for n in range(num):
             poses = []
-            t /= num
-            for i in range(len(self.reset_joint_poses)): 
-                pose = (1 - t) * joint_poses[i] + t * self.reset_joint_poses[i]
-                poses.append(pose)
-            self.actions.append((task,(poses)))
-        
+            t = n / num
+            for i in range(len(self.used_joint_indexes)):
+                poses.append(np.interp(t,[0,1],[self.current_joint_poses[i],self.reset_joint_poses[i]]))
+            self.actions.append((task,(poses,)))
+
         def output(): self.result = None,
         self.actions.append((output,()))
         pass
```

### Comparing `pysimflow-0.0.40/digitaltwin/scene.py` & `pysimflow-0.0.42/digitaltwin/scene.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from scipy.spatial.transform import Rotation
 from time import time,sleep
 import json
 import os
 import socket as s
 
 class Scene:
-  def __init__(self,width=1024,height=768,data_dir='./data',tmp_dir='.'):
+  def __init__(self,width=1024,height=768,data_dir='./digitaltwin_data',tmp_dir='.'):
     self.tmp_dir = tmp_dir
     self.data_dir = data_dir
 
     self.tick = time()
     self.active_objs = dict()
     self.active_objs_by_name = dict()
     self.viewport_size = width,height,4
@@ -23,69 +23,56 @@
     self.timestep = 1/180.
     self.actions = list()
     self.ground_z = 0
     
     self.id = p.connect(p.GUI,options=f'--width={width} --height={height} --headless')
     p.configureDebugVisualizer(p.COV_ENABLE_GUI,0)
     p.setPhysicsEngineParameter(erp=1,contactERP=1,frictionERP=1)
+    p.setTimeStep(self.timestep)
+    p.setGravity(0, 0, -9.81)
 
     w,h,vm,pm,up,forward,horizontal,vertical,yaw,pitch,distance,target = p.getDebugVisualizerCamera()
     p.resetDebugVisualizerCamera(3,yaw,pitch,target)
-
-    self.reset()
+    
+    self.plane = p.loadURDF(os.path.join(self.data_dir,"pybullet_objects/plane.urdf"), [0, 0, self.ground_z], useFixedBase=True)
 
   def __del__(self):
     self.play(False)
     p.resetSimulation()
     del self.active_objs
     del self.active_objs_by_name
     pass
 
   def get_profile(self):
     return self.profile
 
-  def reset(self):
-    p.resetSimulation()
-    del self.active_objs
-    del self.active_objs_by_name
-    
-    self.active_objs = dict()
-    self.active_objs_by_name = dict()
-
-    p.setGravity(0, 0, -9.81)
-    p.setTimeStep(self.timestep)
-    self.plane = p.loadURDF(os.path.join(self.data_dir,"pybullet_objects/plane.urdf"), [0, 0, self.ground_z], useFixedBase=True)
-    self.load(self.scene_path)
-    pass
-
   def load(self,scene_path):
     if not scene_path: return
 
-    p.resetSimulation()
-    p.setGravity(0, 0, -9.81)
-
     self.scene_path = scene_path
     with open(scene_path,'r') as f: self.profile = json.load(f)
 
     if 'ground_z' not in self.profile: self.profile['ground_z'] = 0
+    if 'user_data' not in self.profile: self.profile['user_data'] = ''
+    self.ground_z = self.profile['ground_z']
+    self.user_data = self.profile['user_data']
     
-    self.plane = p.loadURDF(os.path.join(self.data_dir,"pybullet_objects/plane.urdf"), [0, 0, self.profile['ground_z']], useFixedBase=True)
+    p.resetBasePositionAndOrientation(self.plane,[0,0,self.ground_z],p.getQuaternionFromEuler([0,0,0]))
+
     for object_info in self.profile['active_objects']:
       print('add object:',object_info,flush=True)
       kind = object_info['kind']
-      
       active_obj = None
       active_obj = eval(f'digitaltwin.{kind}(self,**object_info)')
       self.active_objs[active_obj.id] = active_obj
       if 'name' in object_info: self.active_objs_by_name[object_info['name']] = active_obj
 
-
   def save(self):
-      self.profile['active_objects']
       self.profile['ground_z'] = self.ground_z
+      self.profile['user_data'] = self.user_data
       active_objects = list()
       for obj in self.active_objs_by_name.values():
         obj.profile = obj.properties()
         active_objects.append(obj.profile)
       self.profile['active_objects'] = active_objects
       with open(self.scene_path,'w') as f: json.dump(self.profile,f,indent=2) 
 
@@ -187,16 +174,18 @@
   def get_active_obj_properties(self):
     objs = dict()
     for name,obj in self.active_objs_by_name.items():
       objs[name] = obj.properties()
     return objs
   
   def set_ground_z(self,z):
-    self.profile['ground_z'] = z
+    self.ground_z = z
     p.resetBasePositionAndOrientation(self.plane,[0,0,z],p.getQuaternionFromEuler([0,0,0]))
     pass
 
   def set_ground_texture(self,texture):
-    self.profile['ground_texture'] = texture
+    self.ground_texture = texture
     p.changeVisualShape(self.plane,-1,textureUniqueId=p.loadTexture(texture))
     pass
 
+  def set_user_data(self,val):
+    self.user_data = val
```

### Comparing `pysimflow-0.0.40/digitaltwin/stacker.py` & `pysimflow-0.0.42/digitaltwin/stacker.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
         for idx in range(50):
             item_width = self.box_size[0] + random.randint(-self.random_factor[0]*100,self.random_factor[0]*100) / 100 * self.box_size[0] 
             item_height = self.box_size[1] + random.randint(-self.random_factor[1]*100,self.random_factor[1]*100) / 100 * self.box_size[1] 
             item_depth = self.box_size[2] + random.randint(-self.random_factor[2]*100,self.random_factor[2]*100) / 100 * self.box_size[2] 
             item_weight = 0.1
             self.packer.add_item(bp.Item('item'+str(idx), item_width, item_height, item_depth, item_weight))
-        
         self.packer.pack(bigger_first=True)
 
     def update(self, dt):
         super().update(dt)
 
     def restore(self):
         super().restore()
@@ -43,15 +42,15 @@
         self.objs.clear()
 
     def signal_generate(self):
         def task(item:bp.Item):
             item_width, item_height, item_depth = item.get_dimension()
             item_pos = self.lower_left + [float(item.position[0] + item_width / 2), float(item.position[1] + item_height / 2), float(item.position[2] + item_depth / 2)]
             item_shape = p.createCollisionShape(p.GEOM_BOX, halfExtents=[item_width/2, item_height/2, item_depth/2])
-            item_id = p.createMultiBody(item.weight, item_shape, -1, item_pos, p.getQuaternionFromEuler([0, 0, 0]))            
+            item_id = p.createMultiBody(item.weight, item_shape, -1, item_pos, p.getQuaternionFromEuler([0, 0, 0]))
             self.objs.append(item_id)
 
         for item in self.packer.bins[0].bin_fitted_items:
             self.actions.append([task,(item,)])
 
         def output(): self.result = None,
```

### Comparing `pysimflow-0.0.40/digitaltwin/workflow.py` & `pysimflow-0.0.42/digitaltwin/workflow.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,38 +5,47 @@
 
 class Workflow():
     def __init__(self,scene: Scene):
         self.scene = scene
         self.running = False
         self.nodes = [
             {'kind':'Robot','names':[],'funs':[
-                {'label':'Motion','f':'pick_move','errs':[],'args':[ #拾取移动
-                    {'name':'mode','kind':'String'}, #模式，关节：joint 点：point
-                    {'name':'speed','kind':'Flaot'}, #速度，0.0 ~ 1.0
-                    {'name':'vision_flow','kind':'String'}, #视觉流程
-                    {'name':'pickup','kind':'Bool'} #拾取设置
+                {'label':'Motion', #动作
+                 'f':'pick_move','errs':[], #拾取移动
+                 'args':[ #附加参数
+                        {'name':'mode','kind':'String'}, #运动模式，关节：joint 线：linear
+                        {'name':'speed','kind':'Flaot'}, #速度，0.0 ~ 1.0
+                        {'name':'pickup','kind':'Bool'}, #拾取设置
+                        {'name':'vision_flow','kind':'String'} #视觉流程
                     ]},
-                {'label':'Motion','f':'move','errs':[],'args':[ #移动
-                    {'name':'mode','kind':'String'}, #模式，关节：joint 点：point
+                {'label':'Motion', #动作
+                 'f':'move','errs':[], #移动
+                 'args':[ #附加参数
+                    {'name':'mode','kind':'String'}, #运动模式，关节：joint 线：linear
                     {'name':'speed','kind':'Flaot'}, #速度，值：0.0 ~ 1.0，默认：0.2
-                    {'name':'pickup','kind':'Bool'}, #拾取设置，？？
+                    {'name':'pickup','kind':'Bool'}, #拾取设置
                     {'name':'joints','kind':'List'}, #关节位置，[弧度值1,...弧度值n]
-                    {'name':'point','kind':'List'}, #点位置，[x,y,z,rx,ry,rz]
-                    {'name':'home','kind':'Bool'}, #回到home
+                    {'name':'point','kind':'List'},  #点位置，[x,y,z,rx,ry,rz] #米，弧度
+                    {'name':'home','kind':'Bool'},   #回到休息点，为true，忽略其他参数
                     ]},
-                {'label':'Motion','f':'move_relatively','errs':[],'args':[ #相对移动
-                    {'name':'mode','kind':'String'}, #模式，关节：joint 点：point
-                    {'name':'speed','kind':'Flaot'}, #速度，值：0.0 ~ 1.0，默认：0.2
-                    {'name':'pickup','kind':'Bool'}, #拾取设置，？？
-                    {'name':'joints','kind':'List'}, #关节位置，[弧度值1,...弧度值n]
-                    {'name':'point','kind':'List'}, #点位置，[x,y,z,rx,ry,rz]
-                    {'name':'target','kind':'String'}, #相对目标，当前任务：task_current，下一个任务：next，选择的任务：selected，工具坐标系：frame_end_effector，机械臂坐标系：frame_robot，全局坐标系：frame_global
+                {'label':'Motion', #动作
+                 'f':'move_relatively','errs':[], #相对移动
+                 'args':[ #附加参数
+                        {'name':'mode','kind':'String'}, #模式，关节：joint 线：linear
+                        {'name':'speed','kind':'Flaot'}, #速度，值：0.0 ~ 1.0，默认：0.2
+                        {'name':'pickup','kind':'Bool'}, #拾取设置
+                        {'name':'target','kind':'String'}, #相对目标，当前任务：task_current，下一个任务：task_next，选择的任务：selected，工具坐标系：frame_end_effector，机械臂坐标系：frame_robot，全局坐标系：frame_global
+                        {'name':'point','kind':'List'},  #点位置，[x,y,z,rx,ry,rz] #米，弧度
                     ]},
-                {'label':'EndEffector','f':'pick','errs':[],'args':[]},  #开
-                {'label':'EndEffector','f':'place','errs':[],'args':[]}  #合
+                {'label':'EndEffector',
+                 'f':'pick','errs':[], #开
+                 'args':[]}, 
+                {'label':'EndEffector',
+                 'f':'place','errs':[], #合
+                 'args':[]} 
                 ]},
             {'kind':'Camera3DReal','names':[],'funs':[  #相机
                 {'label':'Vision','f':'capture','errs':["failed"],'args':[ #拍照
                     {'name':'wait_for_seconds','kind':'Float'}] #等待时间
                 }
                 ]},
             {'kind':'Camera3D','names':[],'funs':[  #相机
@@ -91,50 +100,58 @@
                 act = declare[last]
                 name = act['name']
 
                 last_obj = self.scene.active_objs_by_name[name] if name in self.scene.active_objs_by_name else self.active_plugins_by_name[name]
                 if not last_obj.idle():
                     self.scene.actions.append((task,(last,)))
                     return
-                
+
                 res = last_obj.result
                 err,val = res[0],res[1:]
                 if 'next' in act and not err:
                     next = act['next']
                 elif 'alt' in act:
                     for opt in act['alt']:
                         if err != opt['err']: continue
                         next = opt['next']
                         break
             else:
                 next = wf["run"]
 
             if not next: 
+                if err: print('error',err,flush=True)
                 print('Workflow finished.',flush=True)
                 return
 
             try:
                 act = declare[next]
                 name = act['name']
                 fun = act['fun']
                 args = act['args'] if 'args' in act else {}
                 obj = self.scene.active_objs_by_name[name] if name in self.scene.active_objs_by_name else self.active_plugins_by_name[name]
-                
-                print('error', err,flush=True)
-                print('signal',fun,flush=True)
+
+                print('err',err,flush=True)
+                print('sig',fun,flush=True)
                 print('val',val,flush=True)
                 print('args',args,flush=True)
+
+                args['declare'] = declare
+                args['cursor'] = next
+                args['plugins'] = self.active_plugins_by_name
+
                 eval(f'obj.signal_{fun}(*val,**args)')
+                
+                del args['declare']
+                del args['cursor']
+                del args['plugins']
             except:
-                traceback.print_exc()
+                print(traceback.format_exc(),flush=True)
                 print('Workflow stopped!',flush=True)
-                return 
-
+                return
             self.scene.actions.append((task,(next,)))
-
         task(None)
 
     def stop(self):
         self.running = False
         self.scene.restore()
         pass
```

