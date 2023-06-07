# Comparing `tmp/napari-label-focus-0.0.2.tar.gz` & `tmp/napari-label-focus-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-label-focus-0.0.2.tar", last modified: Mon Jun  5 10:07:14 2023, max compression
+gzip compressed data, was "napari-label-focus-0.0.3.tar", last modified: Wed Jun  7 07:52:31 2023, max compression
```

## Comparing `napari-label-focus-0.0.2.tar` & `napari-label-focus-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1490 2023-05-24 09:58:04.000000 napari-label-focus-0.0.2/LICENSE
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       96 2023-05-24 09:58:04.000000 napari-label-focus-0.0.2/MANIFEST.in
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     2651 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/PKG-INFO
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1702 2023-06-01 14:15:18.000000 napari-label-focus-0.0.2/README.md
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      178 2023-06-01 14:12:18.000000 napari-label-focus-0.0.2/pyproject.toml
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1457 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/setup.cfg
-drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/src/
-drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/src/napari_label_focus/
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       89 2023-05-25 16:10:58.000000 napari-label-focus-0.0.2/src/napari_label_focus/__init__.py
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     3889 2023-06-05 09:59:24.000000 napari-label-focus-0.0.2/src/napari_label_focus/_table.py
-drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/src/napari_label_focus/_tests/
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-05-24 09:58:04.000000 napari-label-focus-0.0.2/src/napari_label_focus/_tests/__init__.py
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      352 2023-06-01 14:10:17.000000 napari-label-focus-0.0.2/src/napari_label_focus/_tests/test_widget.py
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1908 2023-06-05 09:53:47.000000 napari-label-focus-0.0.2/src/napari_label_focus/_widget.py
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      276 2023-05-25 16:11:06.000000 napari-label-focus-0.0.2/src/napari_label_focus/napari.yaml
-drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-05 10:07:14.473454 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     2651 2023-06-05 10:07:14.000000 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/PKG-INFO
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      556 2023-06-05 10:07:14.000000 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/SOURCES.txt
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)        1 2023-06-05 10:07:14.000000 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/dependency_links.txt
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       70 2023-06-05 10:07:14.000000 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/entry_points.txt
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      114 2023-06-05 10:07:14.000000 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/requires.txt
--rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       19 2023-06-05 10:07:14.000000 napari-label-focus-0.0.2/src/napari_label_focus.egg-info/top_level.txt
+drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-07 07:52:31.759806 napari-label-focus-0.0.3/
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1490 2023-05-24 09:58:04.000000 napari-label-focus-0.0.3/LICENSE
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       96 2023-05-24 09:58:04.000000 napari-label-focus-0.0.3/MANIFEST.in
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     2651 2023-06-07 07:52:31.759806 napari-label-focus-0.0.3/PKG-INFO
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1702 2023-06-01 14:15:18.000000 napari-label-focus-0.0.3/README.md
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      178 2023-06-01 14:12:18.000000 napari-label-focus-0.0.3/pyproject.toml
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1457 2023-06-07 07:52:31.759806 napari-label-focus-0.0.3/setup.cfg
+drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-07 07:52:31.759806 napari-label-focus-0.0.3/src/
+drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-07 07:52:31.759806 napari-label-focus-0.0.3/src/napari_label_focus/
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       89 2023-05-25 16:10:58.000000 napari-label-focus-0.0.3/src/napari_label_focus/__init__.py
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     3953 2023-06-06 14:45:45.000000 napari-label-focus-0.0.3/src/napari_label_focus/_table.py
+drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-07 07:52:31.759806 napari-label-focus-0.0.3/src/napari_label_focus/_tests/
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-05-24 09:58:04.000000 napari-label-focus-0.0.3/src/napari_label_focus/_tests/__init__.py
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      604 2023-06-06 14:39:12.000000 napari-label-focus-0.0.3/src/napari_label_focus/_tests/test_widget.py
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     1908 2023-06-05 09:53:47.000000 napari-label-focus-0.0.3/src/napari_label_focus/_widget.py
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      276 2023-05-25 16:11:06.000000 napari-label-focus-0.0.3/src/napari_label_focus/napari.yaml
+drwxr-xr-x   0 wittwer  (127501) IMAGING-GE-unit (11027)        0 2023-06-07 07:52:31.759806 napari-label-focus-0.0.3/src/napari_label_focus.egg-info/
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)     2651 2023-06-07 07:52:31.000000 napari-label-focus-0.0.3/src/napari_label_focus.egg-info/PKG-INFO
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      556 2023-06-07 07:52:31.000000 napari-label-focus-0.0.3/src/napari_label_focus.egg-info/SOURCES.txt
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)        1 2023-06-07 07:52:31.000000 napari-label-focus-0.0.3/src/napari_label_focus.egg-info/dependency_links.txt
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       70 2023-06-07 07:52:31.000000 napari-label-focus-0.0.3/src/napari_label_focus.egg-info/entry_points.txt
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)      114 2023-06-07 07:52:31.000000 napari-label-focus-0.0.3/src/napari_label_focus.egg-info/requires.txt
+-rw-r--r--   0 wittwer  (127501) IMAGING-GE-unit (11027)       19 2023-06-07 07:52:31.000000 napari-label-focus-0.0.3/src/napari_label_focus.egg-info/top_level.txt
```

### Comparing `napari-label-focus-0.0.2/LICENSE` & `napari-label-focus-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-label-focus-0.0.2/PKG-INFO` & `napari-label-focus-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-label-focus
-Version: 0.0.2
+Version: 0.0.3
 Summary: Easily focus the view on selected elements form a Labels layer.
 Home-page: https://github.com/MalloryWittwer/napari-label-focus.git
 Author: Mallory Wittwer
 Author-email: mallory.wittwer@epfl.ch
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `napari-label-focus-0.0.2/README.md` & `napari-label-focus-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `napari-label-focus-0.0.2/setup.cfg` & `napari-label-focus-0.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-label-focus
-version = 0.0.2
+version = 0.0.3
 description = Easily focus the view on selected elements form a Labels layer.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MalloryWittwer/napari-label-focus.git
 author = Mallory Wittwer
 author_email = mallory.wittwer@epfl.ch
 license = BSD-3-Clause
```

### Comparing `napari-label-focus-0.0.2/src/napari_label_focus/_table.py` & `napari-label-focus-0.0.3/src/napari_label_focus/_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     QGridLayout,
     QHBoxLayout,
     QPushButton,
     QTableWidget,
     QTableWidgetItem,
     QWidget,
 )
+from qtpy.QtCore import Qt
 
 class Table(QWidget):
     def __init__(self, layer: napari.layers.Layer = None, viewer: napari.Viewer = None):
         super().__init__()
         self._layer = layer
         self._viewer = viewer
         self._view = QTableWidget()
@@ -54,15 +55,15 @@
         cx = (x1 + x0) / 2
         cy = (y1 + y0) / 2
         cz = int((z1 + z0) / 2)
         self._viewer.camera.center = (0.0, cx, cy)
         self._viewer.camera.angles = (0.0, 0.0, 90.0)
 
         label_size = max(x1 - x0, y1 - y0)
-        self._viewer.camera.zoom = max(20 - 0.2 * label_size, 5)
+        self._viewer.camera.zoom = max(5 - 0.005 * label_size, 0.01)
 
         current_step = self._viewer.dims.current_step
         current_step = np.array(current_step)
         current_step[0] = cz
         current_step = tuple(current_step)
         self._viewer.dims.current_step = current_step
 
@@ -101,10 +102,12 @@
     def set_content(self, df: pd.DataFrame):
         self._table = df
         self._view.clear()
         self._view.setRowCount(len(self._table))
         self._view.setHorizontalHeaderItem(0, QTableWidgetItem('label'))
         self._view.setHorizontalHeaderItem(1, QTableWidgetItem('volume'))
 
-        for i, (lab, vol) in self._table[['label', 'volume']].iterrows():
-            self._view.setItem(i, 0, QTableWidgetItem(str(lab)))
-            self._view.setItem(i, 1, QTableWidgetItem(str(vol)))
+        k = 0
+        for _, (lab, vol) in self._table[['label', 'volume']].iterrows():
+            self._view.setItem(k, 0, QTableWidgetItem(str(lab)))
+            self._view.setItem(k, 1, QTableWidgetItem(str(vol)))
+            k += 1
```

### Comparing `napari-label-focus-0.0.2/src/napari_label_focus/_widget.py` & `napari-label-focus-0.0.3/src/napari_label_focus/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-label-focus-0.0.2/src/napari_label_focus.egg-info/PKG-INFO` & `napari-label-focus-0.0.3/src/napari_label_focus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-label-focus
-Version: 0.0.2
+Version: 0.0.3
 Summary: Easily focus the view on selected elements form a Labels layer.
 Home-page: https://github.com/MalloryWittwer/napari-label-focus.git
 Author: Mallory Wittwer
 Author-email: mallory.wittwer@epfl.ch
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `napari-label-focus-0.0.2/src/napari_label_focus.egg-info/SOURCES.txt` & `napari-label-focus-0.0.3/src/napari_label_focus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

