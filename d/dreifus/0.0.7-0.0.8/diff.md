# Comparing `tmp/dreifus-0.0.7.tar.gz` & `tmp/dreifus-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-qc7pkx08/dreifus-0.0.7.tar", last modified: Fri Jun  2 08:59:47 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-gdlwbtsm/dreifus-0.0.8.tar", last modified: Tue Jun  6 22:51:02 2023, max compression
```

## Comparing `dreifus-0.0.7.tar` & `dreifus-0.0.8.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:47.645101 dreifus-0.0.7/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-06-02 08:59:47.637962 dreifus-0.0.7/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       10 2023-02-13 11:32:40.000000 dreifus-0.0.7/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1087 2023-06-02 08:58:21.000000 dreifus-0.0.7/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-06-02 08:59:47.646656 dreifus-0.0.7/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.0.7/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:46.481742 dreifus-0.0.7/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:46.788377 dreifus-0.0.7/src/dreifus/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.0.7/src/dreifus/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.0.7/src/dreifus/camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5078 2023-04-11 17:41:05.000000 dreifus-0.0.7/src/dreifus/camera_bundle.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1483 2023-02-24 11:10:52.000000 dreifus-0.0.7/src/dreifus/graphics.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:47.258176 dreifus-0.0.7/src/dreifus/matrix/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      251 2023-04-11 16:52:12.000000 dreifus-0.0.7/src/dreifus/matrix/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5852 2023-02-23 11:03:29.000000 dreifus-0.0.7/src/dreifus/matrix/intrinsics_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.0.7/src/dreifus/matrix/intrinsics_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1315 2023-02-13 11:10:42.000000 dreifus-0.0.7/src/dreifus/matrix/pose_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    17557 2023-04-19 21:54:10.000000 dreifus-0.0.7/src/dreifus/matrix/pose_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.0.7/src/dreifus/matrix/pose_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1329 2023-03-08 15:24:39.000000 dreifus-0.0.7/src/dreifus/matrix/transform_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     9414 2023-04-19 22:07:01.000000 dreifus-0.0.7/src/dreifus/pyvista.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3441 2023-05-22 13:04:13.000000 dreifus-0.0.7/src/dreifus/trajectory.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:47.322200 dreifus-0.0.7/src/dreifus/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.0.7/src/dreifus/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.0.7/src/dreifus/util/typing.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:47.493856 dreifus-0.0.7/src/dreifus/vector/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.0.7/src/dreifus/vector/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.0.7/src/dreifus/vector/vector_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5740 2023-05-22 13:07:11.000000 dreifus-0.0.7/src/dreifus/vector/vector_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.0.7/src/dreifus/vector/vector_torch.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:46.965796 dreifus-0.0.7/src/dreifus.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-06-02 08:59:46.000000 dreifus-0.0.7/src/dreifus.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      873 2023-06-02 08:59:46.000000 dreifus-0.0.7/src/dreifus.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-06-02 08:59:46.000000 dreifus-0.0.7/src/dreifus.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       63 2023-06-02 08:59:46.000000 dreifus-0.0.7/src/dreifus.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-06-02 08:59:46.000000 dreifus-0.0.7/src/dreifus.egg-info/top_level.txt
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:47.608820 dreifus-0.0.7/test/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.0.7/test/test_camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.0.7/test/test_intrinsics.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.0.7/test/test_pose.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3677 2023-02-13 11:26:58.000000 dreifus-0.0.7/test/test_vector.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.625413 dreifus-0.0.8/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-06-06 22:51:02.621402 dreifus-0.0.8/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       10 2023-02-13 11:32:40.000000 dreifus-0.0.8/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1087 2023-06-06 22:50:08.000000 dreifus-0.0.8/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-06-06 22:51:02.625413 dreifus-0.0.8/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.0.8/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:01.695326 dreifus-0.0.8/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.029315 dreifus-0.0.8/src/dreifus/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.0.8/src/dreifus/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.0.8/src/dreifus/camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5926 2023-06-06 18:50:08.000000 dreifus-0.0.8/src/dreifus/camera_bundle.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1550 2023-06-06 21:52:50.000000 dreifus-0.0.8/src/dreifus/graphics.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.324371 dreifus-0.0.8/src/dreifus/matrix/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      285 2023-06-06 17:30:54.000000 dreifus-0.0.8/src/dreifus/matrix/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5852 2023-02-23 11:03:29.000000 dreifus-0.0.8/src/dreifus/matrix/intrinsics_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.0.8/src/dreifus/matrix/intrinsics_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1315 2023-02-13 11:10:42.000000 dreifus-0.0.8/src/dreifus/matrix/pose_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    17626 2023-06-06 18:45:27.000000 dreifus-0.0.8/src/dreifus/matrix/pose_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.0.8/src/dreifus/matrix/pose_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4824 2023-06-06 17:53:09.000000 dreifus-0.0.8/src/dreifus/matrix/transform_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     9414 2023-04-19 22:07:01.000000 dreifus-0.0.8/src/dreifus/pyvista.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      952 2023-06-06 21:55:22.000000 dreifus-0.0.8/src/dreifus/render.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3441 2023-05-22 13:04:13.000000 dreifus-0.0.8/src/dreifus/trajectory.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.379828 dreifus-0.0.8/src/dreifus/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.0.8/src/dreifus/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.0.8/src/dreifus/util/typing.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.494097 dreifus-0.0.8/src/dreifus/vector/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.0.8/src/dreifus/vector/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.0.8/src/dreifus/vector/vector_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5740 2023-05-22 13:07:11.000000 dreifus-0.0.8/src/dreifus/vector/vector_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.0.8/src/dreifus/vector/vector_torch.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.134255 dreifus-0.0.8/src/dreifus.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-06-06 22:51:01.000000 dreifus-0.0.8/src/dreifus.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      922 2023-06-06 22:51:01.000000 dreifus-0.0.8/src/dreifus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-06-06 22:51:01.000000 dreifus-0.0.8/src/dreifus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       63 2023-06-06 22:51:01.000000 dreifus-0.0.8/src/dreifus.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-06-06 22:51:01.000000 dreifus-0.0.8/src/dreifus.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.599897 dreifus-0.0.8/test/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.0.8/test/test_camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1398 2023-06-06 18:46:31.000000 dreifus-0.0.8/test/test_camera_bundle.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.0.8/test/test_intrinsics.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.0.8/test/test_pose.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3677 2023-02-13 11:26:58.000000 dreifus-0.0.8/test/test_vector.py
```

### Comparing `dreifus-0.0.7/pyproject.toml` & `dreifus-0.0.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dreifus"
-version = "0.0.7"
+version = "0.0.8"
 description = "dreifus lifts your 3D camera experience and facilitates computer vision applications"
 authors = [
     { name = "Tobias Kirschstein", email = "tobias.kirschstein@gmail.com" },
 ]
 readme = "README.md"
 license = { text = "Apache 2.0" }
 requires-python = ">=3.8.0"
```

### Comparing `dreifus-0.0.7/src/dreifus/camera.py` & `dreifus-0.0.8/src/dreifus/camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/src/dreifus/camera_bundle.py` & `dreifus-0.0.8/src/dreifus/camera_bundle.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Union, Tuple
 
 import numpy as np
 from dreifus.camera import PoseType
 
 from dreifus.matrix import Pose
 from dreifus.vector import Vec3, rotation_matrix_between_vectors, offset_vector_between_line_and_point, \
     angle_between_vectors
@@ -33,15 +33,16 @@
 
 
 def align_poses(world_to_cam_poses: List[Pose],
                 up: Optional[Vec3] = Vec3(0, 1, 0),
                 look: Optional[Vec3] = Vec3(0, 0, -1),
                 look_center: Optional[Vec3] = Vec3(0, 0, 0),
                 cam_to_world: bool = False,
-                inplace: bool = False) -> List[Pose]:
+                inplace: bool = False,
+                return_transformation: bool = False) -> Union[List[Pose], Tuple[List[Pose], Pose]]:
     """
     Calibration poses can be arbitrarily aligned. This method provides a utility to transform a set of camera poses
     such that their up/look directions and look center correspond to the specified values.
     calibration poses are expected in world_to_cam format and OpenCV coordinate convention
     (i.e., x -> right, y -> down, z -> forward).
     Per default, the set of camera poses will be transformed to look at the center in an OpenGL world
     (i.e., x -> right, y -> up, z -> backward).
@@ -49,43 +50,51 @@
     Parameters
     ----------
         world_to_cam_poses: the poses to transform
         up: where the up direction should point to
         look: where the look direction should point to
         look_center: where the look center of all cameras should fall into
         cam_to_world: whether the provided poses are already cam_to_world
+        return_transformation:
+            If specified, a 4x4 transformation matrix is returned that transforms the cam_to_world_poses into
+            aligned space exactly as align_poses() would do. Apply as:
+                transformation @ world_to_cam_poses[i].invert()
 
     Returns
     -------
         the re-aligned camera poses
     """
 
     if not inplace:
         world_to_cam_poses = [pose.copy() for pose in world_to_cam_poses]
 
     if cam_to_world:
         cam_to_world_poses = world_to_cam_poses
     else:
         cam_to_world_poses = [cam_pose.invert() for cam_pose in world_to_cam_poses]
 
+    transformation = np.eye(4)
+
     # Align up direction
     if up is not None:
         up_directions = [cam_pose.get_up_direction() for cam_pose in cam_to_world_poses]
         average_up_direction = np.mean(up_directions, axis=0)
         align_up_rotation = rotation_matrix_between_vectors(average_up_direction, up)
         rotator_up = Pose(align_up_rotation, Vec3(), pose_type=PoseType.CAM_2_CAM)
         cam_to_world_poses = [rotator_up @ cam_pose for cam_pose in cam_to_world_poses]
+        transformation = rotator_up
 
     # Align the look direction
     if look is not None:
         look_directions = [cam_pose.get_look_direction() for cam_pose in cam_to_world_poses]
         average_look_direction = np.mean(look_directions, axis=0)
         align_look_rotation = rotation_matrix_between_vectors(average_look_direction, look)
         rotator_look = Pose(align_look_rotation, Vec3(), pose_type=PoseType.CAM_2_CAM)
         cam_to_world_poses = [rotator_look @ cam_pose for cam_pose in cam_to_world_poses]
+        transformation = rotator_look @ transformation
 
     # Align the look center
     if look_center is not None:
         original_look_center = calculate_look_center(cam_to_world_poses)
         offset_vector = look_center - original_look_center
 
         # look_directions = [cam_pose.get_look_direction() for cam_pose in cam_to_world_poses]
@@ -93,18 +102,27 @@
         # average_look_direction = np.mean(look_directions, axis=0)
         # # TODO: This won't move cameras much if cameras_center is already at look_center
         # #   Would have to somehow find the point that is closest to all camera rays
         # offset_vector = offset_vector_between_line_and_point(cameras_center, average_look_direction, look_center)
         for cam_pose in cam_to_world_poses:
             cam_pose.move(offset_vector)
 
+        mover = np.eye(4)
+        mover[:3, 3] = offset_vector
+        transformation = mover @ transformation
+
     if up is not None:
         # Aligning the look direction might mess up the up direction again
         up_directions = [cam_pose.get_up_direction() for cam_pose in cam_to_world_poses]
         average_up_direction = np.mean(up_directions, axis=0)
         angle = angle_between_vectors(average_up_direction, up)
 
         # TODO: Here we assume that look direction should be z axis. Correct would be to rotate around look direction
         rotator = Pose.from_euler(Vec3(0, 0, -angle), pose_type=PoseType.CAM_2_CAM)
         cam_to_world_poses = [rotator @ cam_pose for cam_pose in cam_to_world_poses]
+        transformation = rotator @ transformation
 
-    return cam_to_world_poses
+    if return_transformation:
+        transformation = Pose(transformation, pose_type=PoseType.CAM_2_CAM)
+        return cam_to_world_poses, transformation
+    else:
+        return cam_to_world_poses
```

### Comparing `dreifus-0.0.7/src/dreifus/graphics.py` & `dreifus-0.0.8/src/dreifus/graphics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from dataclasses import dataclass
 from typing import Union, Tuple, Optional
+
+import numpy as np
 from elias.config import Config
 
+from dreifus.matrix import Intrinsics, Pose
 from dreifus.vector.vector_base import unpack_nd_params
 
 
 @dataclass
 class Dimensions(Config, tuple):
     w: int
     h: int
```

### Comparing `dreifus-0.0.7/src/dreifus/matrix/intrinsics_numpy.py` & `dreifus-0.0.8/src/dreifus/matrix/intrinsics_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/src/dreifus/matrix/intrinsics_torch.py` & `dreifus-0.0.8/src/dreifus/matrix/intrinsics_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/src/dreifus/matrix/pose_base.py` & `dreifus-0.0.8/src/dreifus/matrix/pose_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/src/dreifus/matrix/pose_numpy.py` & `dreifus-0.0.8/src/dreifus/matrix/pose_numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,14 +384,17 @@
     def copy(self, order='C') -> 'Pose':
         pose = super(Pose, self).copy(order=order)
         pose.camera_coordinate_convention = self.camera_coordinate_convention
         pose.pose_type = self.pose_type
 
         return pose
 
+    def numpy(self) -> np.ndarray:
+        return np.array(self)
+
     def __repr__(self):
         representation = super(Pose, self).__repr__()
         representation = f"{representation}\n" \
                          f" > camera_coordinate_convention: {self.camera_coordinate_convention.name}\n" \
                          f" > pose_type: {self.pose_type.name}"
         return representation
```

### Comparing `dreifus-0.0.7/src/dreifus/matrix/pose_torch.py` & `dreifus-0.0.8/src/dreifus/matrix/pose_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/src/dreifus/pyvista.py` & `dreifus-0.0.8/src/dreifus/pyvista.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/src/dreifus/trajectory.py` & `dreifus-0.0.8/src/dreifus/trajectory.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/src/dreifus/vector/vector_base.py` & `dreifus-0.0.8/src/dreifus/vector/vector_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/src/dreifus/vector/vector_numpy.py` & `dreifus-0.0.8/src/dreifus/vector/vector_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/src/dreifus/vector/vector_torch.py` & `dreifus-0.0.8/src/dreifus/vector/vector_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/src/dreifus.egg-info/SOURCES.txt` & `dreifus-0.0.8/src/dreifus.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pyproject.toml
 setup.py
 src/dreifus/__init__.py
 src/dreifus/camera.py
 src/dreifus/camera_bundle.py
 src/dreifus/graphics.py
 src/dreifus/pyvista.py
+src/dreifus/render.py
 src/dreifus/trajectory.py
 src/dreifus.egg-info/PKG-INFO
 src/dreifus.egg-info/SOURCES.txt
 src/dreifus.egg-info/dependency_links.txt
 src/dreifus.egg-info/requires.txt
 src/dreifus.egg-info/top_level.txt
 src/dreifus/matrix/__init__.py
@@ -22,10 +23,11 @@
 src/dreifus/util/__init__.py
 src/dreifus/util/typing.py
 src/dreifus/vector/__init__.py
 src/dreifus/vector/vector_base.py
 src/dreifus/vector/vector_numpy.py
 src/dreifus/vector/vector_torch.py
 test/test_camera.py
+test/test_camera_bundle.py
 test/test_intrinsics.py
 test/test_pose.py
 test/test_vector.py
```

### Comparing `dreifus-0.0.7/test/test_camera.py` & `dreifus-0.0.8/test/test_camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/test/test_intrinsics.py` & `dreifus-0.0.8/test/test_intrinsics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/test/test_pose.py` & `dreifus-0.0.8/test/test_pose.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.7/test/test_vector.py` & `dreifus-0.0.8/test/test_vector.py`

 * *Files identical despite different names*

