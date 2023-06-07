# Comparing `tmp/mikro_napari-0.1.51.tar.gz` & `tmp/mikro_napari-0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikro_napari-0.1.51.tar", max compression
+gzip compressed data, was "mikro_napari-0.1.52.tar", max compression
```

## Comparing `mikro_napari-0.1.51.tar` & `mikro_napari-0.1.52.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1318 2023-05-05 21:12:55.597194 mikro_napari-0.1.51/README.md
--rw-r--r--   0        0        0        0 2023-05-08 18:04:36.280895 mikro_napari-0.1.51/mikro_napari/__init__.py
--rw-r--r--   0        0        0    99909 2023-05-08 18:04:36.281344 mikro_napari-0.1.51/mikro_napari/api/schema.py
--rw-r--r--   0        0        0      480 2023-05-05 21:12:55.598314 mikro_napari-0.1.51/mikro_napari/api/structures.py
--rw-r--r--   0        0        0        0 2023-05-05 21:12:55.598358 mikro_napari-0.1.51/mikro_napari/container/__init__.py
--rw-r--r--   0        0        0      299 2023-05-05 21:12:55.598412 mikro_napari-0.1.51/mikro_napari/container/base.py
--rw-r--r--   0        0        0    25874 2023-05-08 18:33:40.432878 mikro_napari-0.1.51/mikro_napari/models/representation.py
--rw-r--r--   0        0        0      289 2023-05-05 21:12:55.598590 mikro_napari-0.1.51/mikro_napari/napari.yaml
--rw-r--r--   0        0        0      497 2023-05-08 20:13:38.943805 mikro_napari-0.1.51/mikro_napari/plugin.py
--rw-r--r--   0        0        0     1028 2023-05-05 21:12:55.598699 mikro_napari-0.1.51/mikro_napari/run.py
--rw-r--r--   0        0        0      701 2023-05-05 21:12:55.598752 mikro_napari-0.1.51/mikro_napari/utils.py
--rw-r--r--   0        0        0        0 2023-05-05 21:12:55.598837 mikro_napari-0.1.51/mikro_napari/widgets/dialogs/__init__.py
--rw-r--r--   0        0        0     2680 2023-05-05 21:12:55.598902 mikro_napari-0.1.51/mikro_napari/widgets/dialogs/open_image.py
--rw-r--r--   0        0        0        0 2023-05-05 21:12:55.598924 mikro_napari-0.1.51/mikro_napari/widgets/dialogs/show_roi.py
--rw-r--r--   0        0        0     8437 2023-05-08 18:04:36.281814 mikro_napari-0.1.51/mikro_napari/widgets/main_widget.py
--rw-r--r--   0        0        0        0 2023-05-05 21:12:55.599062 mikro_napari-0.1.51/mikro_napari/widgets/sidebar/__init__.py
--rw-r--r--   0        0        0     5926 2023-05-08 18:04:36.281970 mikro_napari-0.1.51/mikro_napari/widgets/sidebar/sidebar.py
--rw-r--r--   0        0        0     1921 2023-05-08 20:19:30.440575 mikro_napari-0.1.51/pyproject.toml
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 mikro_napari-0.1.51/PKG-INFO
+-rw-r--r--   0        0        0     1318 2022-10-11 12:19:03.583911 mikro_napari-0.1.52/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 10:02:21.299344 mikro_napari-0.1.52/mikro_napari/__init__.py
+-rw-r--r--   0        0        0    99999 2023-05-22 14:58:22.576682 mikro_napari-0.1.52/mikro_napari/api/schema.py
+-rw-r--r--   0        0        0      480 2022-10-11 12:19:03.583911 mikro_napari-0.1.52/mikro_napari/api/structures.py
+-rw-r--r--   0        0        0        0 2022-10-11 12:19:03.587911 mikro_napari-0.1.52/mikro_napari/container/__init__.py
+-rw-r--r--   0        0        0      299 2023-03-04 18:17:50.027023 mikro_napari-0.1.52/mikro_napari/container/base.py
+-rw-r--r--   0        0        0      175 2023-06-07 14:54:39.966032 mikro_napari-0.1.52/mikro_napari/manifest.py
+-rw-r--r--   0        0        0    25979 2023-06-07 08:06:31.794483 mikro_napari-0.1.52/mikro_napari/models/representation.py
+-rw-r--r--   0        0        0      289 2023-02-15 17:47:06.550532 mikro_napari-0.1.52/mikro_napari/napari.yaml
+-rw-r--r--   0        0        0      447 2023-06-07 14:55:48.790493 mikro_napari-0.1.52/mikro_napari/plugin.py
+-rw-r--r--   0        0        0     1025 2023-06-07 14:55:17.462284 mikro_napari-0.1.52/mikro_napari/run.py
+-rw-r--r--   0        0        0      701 2022-10-11 12:19:03.587911 mikro_napari-0.1.52/mikro_napari/utils.py
+-rw-r--r--   0        0        0        0 2022-03-25 12:04:03.354310 mikro_napari-0.1.52/mikro_napari/widgets/dialogs/__init__.py
+-rw-r--r--   0        0        0     2680 2022-03-28 15:11:00.264225 mikro_napari-0.1.52/mikro_napari/widgets/dialogs/open_image.py
+-rw-r--r--   0        0        0        0 2022-10-11 12:19:03.587911 mikro_napari-0.1.52/mikro_napari/widgets/dialogs/show_roi.py
+-rw-r--r--   0        0        0     7816 2023-05-17 14:28:58.546388 mikro_napari-0.1.52/mikro_napari/widgets/main_widget.py
+-rw-r--r--   0        0        0        0 2022-10-11 12:19:03.587911 mikro_napari-0.1.52/mikro_napari/widgets/sidebar/__init__.py
+-rw-r--r--   0        0        0     5926 2023-05-08 15:52:59.131693 mikro_napari-0.1.52/mikro_napari/widgets/sidebar/sidebar.py
+-rw-r--r--   0        0        0     1915 2023-06-07 15:00:58.104483 mikro_napari-0.1.52/pyproject.toml
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 mikro_napari-0.1.52/PKG-INFO
```

### Comparing `mikro_napari-0.1.51/README.md` & `mikro_napari-0.1.52/README.md`

 * *Files identical despite different names*

### Comparing `mikro_napari-0.1.51/mikro_napari/api/schema.py` & `mikro_napari-0.1.52/mikro_napari/api/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from mikro.scalars import Store, AffineMatrix, AssignationID, FeatureValue, MetricValue
-from datetime import datetime
-from mikro.funcs import aexecute, asubscribe, subscribe, execute
-from mikro.rath import MikroRath
-from pydantic import Field, BaseModel
-from typing import Iterator, Tuple, Dict, Literal, AsyncIterator, List, Optional
+from rath.scalars import ID
 from mikro.traits import (
-    Vectorizable,
-    PhysicalSize,
-    Stage,
     Position,
-    Omero,
-    ROI,
+    Stage,
+    PhysicalSize,
+    Vectorizable,
     Representation,
+    ROI,
+    Omero,
 )
-from rath.scalars import ID
+from typing import AsyncIterator, Literal, List, Optional, Iterator, Dict, Tuple
+from mikro.funcs import aexecute, execute, asubscribe, subscribe
+from mikro.scalars import AffineMatrix, MetricValue, FeatureValue, AssignationID, Store
 from enum import Enum
+from pydantic import Field, BaseModel
+from mikro.rath import MikroRath
+from datetime import datetime
 
 
 class CommentableModels(str, Enum):
     GRUNNLAG_USERMETA = "GRUNNLAG_USERMETA"
     GRUNNLAG_ANTIBODY = "GRUNNLAG_ANTIBODY"
     GRUNNLAG_OBJECTIVE = "GRUNNLAG_OBJECTIVE"
     GRUNNLAG_INSTRUMENT = "GRUNNLAG_INSTRUMENT"
@@ -44,14 +44,15 @@
     GRUNNLAG_METRIC = "GRUNNLAG_METRIC"
     GRUNNLAG_THUMBNAIL = "GRUNNLAG_THUMBNAIL"
     GRUNNLAG_VIDEO = "GRUNNLAG_VIDEO"
     GRUNNLAG_ROI = "GRUNNLAG_ROI"
     GRUNNLAG_LABEL = "GRUNNLAG_LABEL"
     GRUNNLAG_FEATURE = "GRUNNLAG_FEATURE"
     BORD_TABLE = "BORD_TABLE"
+    BORD_GRAPH = "BORD_GRAPH"
 
 
 class SharableModels(str, Enum):
     """Sharable Models are models that can be shared amongst users and groups. They representent the models of the DB"""
 
     GRUNNLAG_USERMETA = "GRUNNLAG_USERMETA"
     GRUNNLAG_ANTIBODY = "GRUNNLAG_ANTIBODY"
@@ -79,14 +80,15 @@
     GRUNNLAG_METRIC = "GRUNNLAG_METRIC"
     GRUNNLAG_THUMBNAIL = "GRUNNLAG_THUMBNAIL"
     GRUNNLAG_VIDEO = "GRUNNLAG_VIDEO"
     GRUNNLAG_ROI = "GRUNNLAG_ROI"
     GRUNNLAG_LABEL = "GRUNNLAG_LABEL"
     GRUNNLAG_FEATURE = "GRUNNLAG_FEATURE"
     BORD_TABLE = "BORD_TABLE"
+    BORD_GRAPH = "BORD_GRAPH"
 
 
 class LokClientGrantType(str, Enum):
     """An enumeration."""
 
     CLIENT_CREDENTIALS = "CLIENT_CREDENTIALS"
     "Backend (Client Credentials)"
@@ -143,14 +145,15 @@
     GRUNNLAG_METRIC = "GRUNNLAG_METRIC"
     GRUNNLAG_THUMBNAIL = "GRUNNLAG_THUMBNAIL"
     GRUNNLAG_VIDEO = "GRUNNLAG_VIDEO"
     GRUNNLAG_ROI = "GRUNNLAG_ROI"
     GRUNNLAG_LABEL = "GRUNNLAG_LABEL"
     GRUNNLAG_FEATURE = "GRUNNLAG_FEATURE"
     BORD_TABLE = "BORD_TABLE"
+    BORD_GRAPH = "BORD_GRAPH"
     PLOTQL_PLOT = "PLOTQL_PLOT"
 
 
 class OmeroFileType(str, Enum):
     """An enumeration."""
 
     TIFF = "TIFF"
```

### Comparing `mikro_napari-0.1.51/mikro_napari/models/representation.py` & `mikro_napari-0.1.52/mikro_napari/models/representation.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     RoiTypeInput,
     Watch_roisSubscriptionRois,
     acreate_roi,
     get_representation,
     Create_roiMutation,
     aget_rois,
     awatch_rois,
-    RepresentationFragmentOmeroPhysicalsize,
+    OmeroFragmentPhysicalsize,
     PositionFragment,
 )
 import asyncio
 from mikro_napari.api.schema import (
     DetailLabelFragment,
     aget_label_for,
     Delete_roiMutationDeleteroi,
@@ -57,15 +57,15 @@
     Mode.ADD_PATH: RoiTypeInput.PATH,
 }
 
 
 def top_left_in_view(
     position: PositionFragment,
     image: RepresentationFragment,
-    physical_size: RepresentationFragmentOmeroPhysicalsize,
+    physical_size: OmeroFragmentPhysicalsize,
 ):
     """Caluclate the top left corner of the image in world coordinates.
 
     Args:
         position (Position): _description_
         image (Representation): _description_
         physical_size (RepresentationFragmentOmeroPhysicalsize): _description_
@@ -357,14 +357,17 @@
 
     def show(self, respect_physical_size=False):
         if respect_physical_size:
             raise NotImplementedError
 
         scale = None
 
+        if self.managed_image.omero and self.managed_image.omero.physical_size:
+            scale = self.managed_image.omero.physical_size.to_scale()
+
         if self.managed_image.variety == RepresentationVariety.RGB:
             self._image_layer = self.viewer.add_image(
                 self.managed_image.data.transpose(*list("tzyxc")),
                 metadata={
                     "mikro": True,
                     "representation": self.managed_image,
                     "type": "IMAGE",
@@ -550,29 +553,33 @@
                 t_limit,
                 bottom_right_max_ceiling[0],
                 bottom_right_max_ceiling[1],
                 bottom_right_max_ceiling[2],
             )
         )
         for i, view_data in enumerate(view_datas):
-            x = view_data.sel(t=0, c=0).data
+            x = view_data.sel(t=0, c=0)
+
+            z1 = math.floor(top_left_offsets[i][0])
+            y1 = math.floor(top_left_offsets[i][1])
+            x1 = math.floor(top_left_offsets[i][2])
+
+            z2 = z1 + x.sizes["z"]
+            y2 = y1 + x.sizes["y"]
+            x2 = x1 + x.sizes["x"]
+
+            print(z1, z2, y1, y2, x1, x2)
 
             image[
                 0,
                 0,
-                math.floor(top_left_offsets[i][0]) : math.floor(
-                    bottom_right_offsets[i][0]
-                ),
-                math.floor(top_left_offsets[i][1]) : math.floor(
-                    bottom_right_offsets[i][1]
-                ),
-                math.floor(top_left_offsets[i][2]) : math.floor(
-                    bottom_right_offsets[i][2]
-                ),
-            ] = x
+                z1:z2,
+                y1:y2,
+                x1:x2,
+            ] = x.data
         image = image.compute()
 
         self.viewer.add_image(
             image,
             name="Position {pos.x}, {pos.y}, {pos.z}",
             metadata={"mikro": True, "type": "POSITION"},
         )
```

### Comparing `mikro_napari-0.1.51/mikro_napari/run.py` & `mikro_napari-0.1.52/mikro_napari/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from mikro_napari.widgets.main_widget import MikroNapariWidget
 import napari
 import argparse
 
 from mikro_napari.widgets.sidebar.sidebar import SidebarWidget
 import os
 from arkitekt.builders import publicqt
+from mikro_napari.manifest import identifier, version, logo
 
 
 def main(**kwargs):
     os.environ["NAPARI_ASYNC"] = "1"
 
-    identifier = "github.io.jhnnsrs.mikro-napari"
-    version = "latest"
-
     viewer = napari.Viewer()
 
-    app = publicqt(identifier, version, parent=viewer.window.qt_viewer)
+    app = publicqt(identifier, version, parent=viewer.window.qt_viewer, logo=logo)
 
     widget = MikroNapariWidget(viewer, app, **kwargs)
     sidebar = SidebarWidget(viewer, app, **kwargs)
     viewer.window.add_dock_widget(widget, area="left", name="Mikro")
     viewer.window.add_dock_widget(sidebar, area="right", name="Mikro")
     # viewer.add_image(astronaut(), name="astronaut")
```

### Comparing `mikro_napari-0.1.51/mikro_napari/utils.py` & `mikro_napari-0.1.52/mikro_napari/utils.py`

 * *Files identical despite different names*

### Comparing `mikro_napari-0.1.51/mikro_napari/widgets/dialogs/open_image.py` & `mikro_napari-0.1.52/mikro_napari/widgets/dialogs/open_image.py`

 * *Files identical despite different names*

### Comparing `mikro_napari-0.1.51/mikro_napari/widgets/main_widget.py` & `mikro_napari-0.1.52/mikro_napari/widgets/main_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,66 +87,57 @@
         self.mylayout.addWidget(self.magic_bar)
 
         self.setWindowTitle("My Own Title")
         self.setLayout(self.mylayout)
 
         self.viewer.layers.selection.events.active.connect(self.on_selection_changed)
 
-        self.app.rekuest.definition_registry.register(
+        self.app.rekuest.register(
             self.representation_controller.on_image_loaded,
-            self.app.rekuest.structure_registry,
             actifier=qtinloopactifier,
             parent=self,
         )
-        self.app.rekuest.definition_registry.register(
+        self.app.rekuest.register(
             self.representation_controller.open_feature,
-            self.app.rekuest.structure_registry,
             actifier=qtinloopactifier,
             parent=self,
         )
-        self.app.rekuest.definition_registry.register(
+        self.app.rekuest.register(
             self.representation_controller.open_metric,
-            self.app.rekuest.structure_registry,
             actifier=qtinloopactifier,
             parent=self,
         )
-        self.app.rekuest.definition_registry.register(
+        self.app.rekuest.register(
             self.representation_controller.open_label,
-            self.app.rekuest.structure_registry,
             actifier=qtinloopactifier,
             parent=self,
         )
 
-        self.app.rekuest.definition_registry.register(
+        self.app.rekuest.register(
             self.representation_controller.tile_images,
-            self.app.rekuest.structure_registry,
             actifier=qtinloopactifier,
             parent=self,
         )
-        self.app.rekuest.definition_registry.register(
+        self.app.rekuest.register(
             self.representation_controller.open_position,
-            self.app.rekuest.structure_registry,
             actifier=qtinloopactifier,
             parent=self,
         )
-        self.app.rekuest.definition_registry.register(
+        self.app.rekuest.register(
             self.representation_controller.open_stage,
-            self.app.rekuest.structure_registry,
             actifier=qtinloopactifier,
             parent=self,
         )
-        self.app.rekuest.definition_registry.register(
+        self.app.rekuest.register(
             self.upload_layer,
-            self.app.rekuest.structure_registry,
             actifier=qtinloopactifier,
             parent=self,
         )
-        self.app.rekuest.definition_registry.register(
+        self.app.rekuest.register(
             self.representation_controller.stream_rois,
-            self.app.rekuest.structure_registry,
         )
 
     def on_app_up(self):
         self.open_image_button.setEnabled(True)
         self.on_selection_changed()  # TRIGGER ALSO HERE
 
     def on_app_down(self):
```

### Comparing `mikro_napari-0.1.51/mikro_napari/widgets/sidebar/sidebar.py` & `mikro_napari-0.1.52/mikro_napari/widgets/sidebar/sidebar.py`

 * *Files identical despite different names*

### Comparing `mikro_napari-0.1.51/pyproject.toml` & `mikro_napari-0.1.52/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 [tool.poetry]
 name = "mikro-napari"
-version = "0.1.51"
+version = "0.1.52"
 description = "A napari plugin to interact with and provide functionality for a connected arkitekt server"
 readme = "README.md"
 repository = "https://github.com/jhnnsrs/mikro-napari"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "mikro_napari" }]
 classifiers = ["Framework :: napari"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<=3.12"
-arkitekt = "0.4.109"
+arkitekt = "0.4.122"
 numpy = "<1.24"
 koil = "0.2.14"
 
 
 [tool.poetry.scripts]
 mikro-napari = "mikro_napari.run:main"
 
 [tool.mypy]
-exclude = [
-    "venv/"
-]
+exclude = ["venv/"]
 ignore_missing_imports = true
 
 
 [tool.ruff]
 extend-select = ["ANN", "D1"]
 
 # Exclude a variety of commonly ignored directories.
```

### Comparing `mikro_napari-0.1.51/PKG-INFO` & `mikro_napari-0.1.52/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mikro-napari
-Version: 0.1.51
+Version: 0.1.52
 Summary: A napari plugin to interact with and provide functionality for a connected arkitekt server
 Home-page: https://github.com/jhnnsrs/mikro-napari
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: Framework :: napari
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: arkitekt (==0.4.109)
+Requires-Dist: arkitekt (==0.4.122)
 Requires-Dist: koil (==0.2.14)
 Requires-Dist: numpy (<1.24)
 Project-URL: Repository, https://github.com/jhnnsrs/mikro-napari
 Description-Content-Type: text/markdown
 
 # mikro-napari
```

