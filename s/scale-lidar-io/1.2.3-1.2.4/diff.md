# Comparing `tmp/scale_lidar_io-1.2.3.tar.gz` & `tmp/scale_lidar_io-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_lidar_io-1.2.3.tar", last modified: Thu Mar 16 14:04:59 2023, max compression
+gzip compressed data, was "dist/scale_lidar_io-1.2.4.tar", last modified: Wed Jun  7 14:51:10 2023, max compression
```

## Comparing `scale_lidar_io-1.2.3.tar` & `scale_lidar_io-1.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ivan.roumec   (503) staff       (20)        0 2023-03-16 14:04:59.117171 scale_lidar_io-1.2.3/
--rw-r--r--   0 ivan.roumec   (503) staff       (20)    11357 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.3/LICENSE.md
--rw-r--r--   0 ivan.roumec   (503) staff       (20)      443 2023-03-16 14:04:59.117022 scale_lidar_io-1.2.3/PKG-INFO
--rw-r--r--   0 ivan.roumec   (503) staff       (20)       30 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.3/README.md
-drwxr-xr-x   0 ivan.roumec   (503) staff       (20)        0 2023-03-16 14:04:59.115507 scale_lidar_io-1.2.3/scale_lidar_io/
--rw-r--r--   0 ivan.roumec   (503) staff       (20)      192 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.3/scale_lidar_io/__init__.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)    15951 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.3/scale_lidar_io/camera.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)     1710 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.3/scale_lidar_io/color_utils.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)     3136 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.3/scale_lidar_io/connectors.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)    20102 2023-03-16 14:03:29.000000 scale_lidar_io-1.2.3/scale_lidar_io/frame.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)     2439 2023-03-16 14:03:23.000000 scale_lidar_io-1.2.3/scale_lidar_io/helper.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)     3482 2023-03-16 14:03:23.000000 scale_lidar_io-1.2.3/scale_lidar_io/image.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)     1406 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.3/scale_lidar_io/interpolate_transforms.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)     8290 2023-03-16 14:03:29.000000 scale_lidar_io-1.2.3/scale_lidar_io/lidar_frame_1_pb2.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)    14947 2023-03-16 14:03:12.000000 scale_lidar_io-1.2.3/scale_lidar_io/nucleus_scene.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)     2723 2023-03-16 14:03:29.000000 scale_lidar_io-1.2.3/scale_lidar_io/protobuf_helper.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)    12220 2023-03-16 14:03:29.000000 scale_lidar_io-1.2.3/scale_lidar_io/scene.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)     9439 2023-03-16 14:03:29.000000 scale_lidar_io-1.2.3/scale_lidar_io/task.py
--rw-r--r--   0 ivan.roumec   (503) staff       (20)     7879 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.3/scale_lidar_io/transform.py
-drwxr-xr-x   0 ivan.roumec   (503) staff       (20)        0 2023-03-16 14:04:59.116555 scale_lidar_io-1.2.3/scale_lidar_io.egg-info/
--rw-r--r--   0 ivan.roumec   (503) staff       (20)      443 2023-03-16 14:04:59.000000 scale_lidar_io-1.2.3/scale_lidar_io.egg-info/PKG-INFO
--rw-r--r--   0 ivan.roumec   (503) staff       (20)      648 2023-03-16 14:04:59.000000 scale_lidar_io-1.2.3/scale_lidar_io.egg-info/SOURCES.txt
--rw-r--r--   0 ivan.roumec   (503) staff       (20)        1 2023-03-16 14:04:59.000000 scale_lidar_io-1.2.3/scale_lidar_io.egg-info/dependency_links.txt
--rw-r--r--   0 ivan.roumec   (503) staff       (20)      191 2023-03-16 14:04:59.000000 scale_lidar_io-1.2.3/scale_lidar_io.egg-info/requires.txt
--rw-r--r--   0 ivan.roumec   (503) staff       (20)       15 2023-03-16 14:04:59.000000 scale_lidar_io-1.2.3/scale_lidar_io.egg-info/top_level.txt
--rw-r--r--   0 ivan.roumec   (503) staff       (20)       38 2023-03-16 14:04:59.117221 scale_lidar_io-1.2.3/setup.cfg
--rw-r--r--   0 ivan.roumec   (503) staff       (20)     1071 2023-03-16 14:03:46.000000 scale_lidar_io-1.2.3/setup.py
-drwxr-xr-x   0 ivan.roumec   (503) staff       (20)        0 2023-03-16 14:04:59.116723 scale_lidar_io-1.2.3/test/
--rw-r--r--   0 ivan.roumec   (503) staff       (20)     6270 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.3/test/test_scale_lidar_io.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 14:51:10.373968 scale_lidar_io-1.2.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/LICENSE.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      443 2023-06-07 14:51:10.373968 scale_lidar_io-1.2.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 14:51:10.369967 scale_lidar_io-1.2.4/scale_lidar_io/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/scale_lidar_io/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16749 2023-06-07 14:49:18.000000 scale_lidar_io-1.2.4/scale_lidar_io/camera.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1710 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/scale_lidar_io/color_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3136 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/scale_lidar_io/connectors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20267 2023-06-07 14:49:18.000000 scale_lidar_io-1.2.4/scale_lidar_io/frame.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2439 2023-06-07 14:49:11.000000 scale_lidar_io-1.2.4/scale_lidar_io/helper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3482 2023-06-07 14:49:11.000000 scale_lidar_io-1.2.4/scale_lidar_io/image.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1406 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/scale_lidar_io/interpolate_transforms.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8290 2023-06-07 14:49:15.000000 scale_lidar_io-1.2.4/scale_lidar_io/lidar_frame_1_pb2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14947 2023-03-02 20:24:08.000000 scale_lidar_io-1.2.4/scale_lidar_io/nucleus_scene.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2723 2023-06-07 14:49:15.000000 scale_lidar_io-1.2.4/scale_lidar_io/protobuf_helper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12220 2023-06-07 14:49:15.000000 scale_lidar_io-1.2.4/scale_lidar_io/scene.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9439 2023-06-07 14:49:15.000000 scale_lidar_io-1.2.4/scale_lidar_io/task.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7879 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/scale_lidar_io/transform.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 14:51:10.373968 scale_lidar_io-1.2.4/scale_lidar_io.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      443 2023-06-07 14:51:10.000000 scale_lidar_io-1.2.4/scale_lidar_io.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-06-07 14:51:10.000000 scale_lidar_io-1.2.4/scale_lidar_io.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-07 14:51:10.000000 scale_lidar_io-1.2.4/scale_lidar_io.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      191 2023-06-07 14:51:10.000000 scale_lidar_io-1.2.4/scale_lidar_io.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-06-07 14:51:10.000000 scale_lidar_io-1.2.4/scale_lidar_io.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-07 14:51:10.373968 scale_lidar_io-1.2.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1070 2023-06-07 14:50:52.000000 scale_lidar_io-1.2.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 14:51:10.373968 scale_lidar_io-1.2.4/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6270 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/test/test_scale_lidar_io.py
```

### Comparing `scale_lidar_io-1.2.3/LICENSE.md` & `scale_lidar_io-1.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/camera.py` & `scale_lidar_io-1.2.4/scale_lidar_io/camera.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Camera object that contains all the camera information
 
     Camera properties:
         - id = camera id/Name/Identifier, type: int, str
         - pose: Camera pose/extrinsic, type: Transform
         - world_poses: World poses, this will make the camera ignore the frame poses, type: list(Transform)
         - K: Intrinsic matrix
-        - D: Camera distortion coefficients [k1,k2,p1,p2,k3,k4], default all set to ``0``
+        - D: Camera distortion coefficients [k1,k2,p1,p2,k3,k4,k5,k6,lx,ly,xi], default all set to ``0``
         - model: Camera model, default ``brown_conrady``
         - scale_factor: Camera scale factor, default ``1``
         - skew: Camera scale factor, default ``0``
 
     Usefull extra documentation to understand better how this object works:
     https://docs.opencv.org/3.4/d9/d0c/group__calib3d.html
 
@@ -189,22 +189,25 @@
           world_poses (list(Transform)):  World poses, this will make the camera ignore the frame poses
 
         Keyword Args:
           fx (str): Focal length in X
           fy (str): Focal length in Y
           cx (str): Center point in X
           cy (str): Center point in Y
-          k1 (double): Distortion value k1
-          k2 (double): Distortion value k2
-          k3 (double): Distortion value k3
-          k4 (double): Distortion value k4
-          k5 (double): Distortion value k5
-          k6 (double): Distortion value k6
-          p1 (double): Distortion value p1
-          p2 (double): Distortion value p2
+          k1 (double): Radial distortion param k1
+          k2 (double): Radial distortion param k2
+          k3 (double): Radial distortion param k3
+          k4 (double): Radial distortion param k4
+          k5 (double): Radial distortion param k5
+          k6 (double): Radial distortion param k6
+          p1 (double): Tangential distortion param p1
+          p2 (double): Tangential distortion param p2
+          lx (double): Decentering distortion param lx
+          l6 (double): Decentering distortion param ly
+          xi (double): Mirror param xi
 
         """
         if position is not None:
             self.position = position
         if rotation is not None:
             self.rotation = rotation
         if pose is not None:
@@ -247,22 +250,38 @@
         if "p2" in kwargs:
             self.D[3] = kwargs["p2"]
         if "k3" in kwargs:
             self.D[4] = kwargs["k3"]
         if "k4" in kwargs:
             self.D[5] = kwargs["k4"]
         if "k5" in kwargs:
-            self.D = np.lib.pad(self.D, (0, 1), "constant", constant_values=(0))
+            pad_count = 7 - len(self.D)
             self.D[6] = kwargs["k5"]
         if "k6" in kwargs:
-            if len(self.D) == 6:
-                self.D = np.lib.pad(self.D, (0, 2), "constant", constant_values=(0))
-            elif len(self.D) == 7:
-                self.D = np.lib.pad(self.D, (0, 1), "constant", constant_values=(0))
+            pad_count = 8 - len(self.D)
+            if pad_count > 0:
+                self.D = np.lib.pad(self.D, (0, pad_count), "constant", constant_values=(0))
             self.D[7] = kwargs["k6"]
+        if "lx" in kwargs:
+            pad_count = 9 - len(self.D)
+            if pad_count > 0:
+                self.D = np.lib.pad(self.D, (0, pad_count), "constant", constant_values=(0))
+            self.D[8] = kwargs["lx"]
+        if "ly" in kwargs:
+            pad_count = 10 - len(self.D)
+            if pad_count > 0:
+                self.D = np.lib.pad(self.D, (0, pad_count), "constant", constant_values=(0))
+            self.D[9] = kwargs["ly"]
+        if "xi" in kwargs:
+            pad_count = 11 - len(self.D)
+            if pad_count > 0:
+                self.D = np.lib.pad(self.D, (0, pad_count), "constant", constant_values=(0))
+            self.D[10] = kwargs["xi"]
+
+
 
     def apply_transform(self, transform: Transform):
         """Apply transformation to the camera (transform @ pose)
 
         :param transform: Transform to apply to the object
         :type transform: Transform
         """
```

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/color_utils.py` & `scale_lidar_io-1.2.4/scale_lidar_io/color_utils.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/connectors.py` & `scale_lidar_io-1.2.4/scale_lidar_io/connectors.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/frame.py` & `scale_lidar_io-1.2.4/scale_lidar_io/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,14 +415,17 @@
                 k2=float(D[1]),
                 p1=float(D[2]),
                 p2=float(D[3]),
                 k3=float(D[4]),
                 k4=float(D[5]),
                 k5=float(D[6]) if len(D) >= 7 else 0,
                 k6=float(D[7]) if len(D) >= 8 else 0,
+                lx=float(D[8]) if len(D) >= 9 else 0,
+                ly=float(D[9]) if len(D) >= 10 else 0,
+                xi=float(D[10]) if len(D) >= 11 else 0,
                 scale_factor=camera.scale_factor,
             )
             if image.metadata:
                 result["metadata"] = image.metadata
             if image.timestamp:
                 result["timestamp"] = image.timestamp
             return result
```

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/helper.py` & `scale_lidar_io-1.2.4/scale_lidar_io/helper.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/image.py` & `scale_lidar_io-1.2.4/scale_lidar_io/image.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/interpolate_transforms.py` & `scale_lidar_io-1.2.4/scale_lidar_io/interpolate_transforms.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/lidar_frame_1_pb2.py` & `scale_lidar_io-1.2.4/scale_lidar_io/lidar_frame_1_pb2.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/nucleus_scene.py` & `scale_lidar_io-1.2.4/scale_lidar_io/nucleus_scene.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/protobuf_helper.py` & `scale_lidar_io-1.2.4/scale_lidar_io/protobuf_helper.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/scene.py` & `scale_lidar_io-1.2.4/scale_lidar_io/scene.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/task.py` & `scale_lidar_io-1.2.4/scale_lidar_io/task.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io/transform.py` & `scale_lidar_io-1.2.4/scale_lidar_io/transform.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/scale_lidar_io.egg-info/SOURCES.txt` & `scale_lidar_io-1.2.4/scale_lidar_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.3/setup.py` & `scale_lidar_io-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scale_lidar_io",
-    version="1.2.03",
+    version="1.2.4",
     author="Scale AI",
     author_email="rodrigo.belfiore@scale.com, ivan.roumec@scale.com",
     description="Lidar data conversion helpers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["scale_lidar_io"],
     install_requires=[
```

### Comparing `scale_lidar_io-1.2.3/test/test_scale_lidar_io.py` & `scale_lidar_io-1.2.4/test/test_scale_lidar_io.py`

 * *Files identical despite different names*

