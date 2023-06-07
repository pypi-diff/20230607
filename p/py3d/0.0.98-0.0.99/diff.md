# Comparing `tmp/py3d-0.0.98.tar.gz` & `tmp/py3d-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.0.98.tar", last modified: Tue Jun  6 15:39:23 2023, max compression
+gzip compressed data, was "py3d-0.0.99.tar", last modified: Wed Jun  7 15:17:26 2023, max compression
```

## Comparing `py3d-0.0.98.tar` & `py3d-0.0.99.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:39:23.944769 py3d-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-06 15:39:23.944769 py3d-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-06 15:39:02.000000 py3d-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:39:23.940769 py3d-0.0.98/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-06 15:38:18.000000 py3d-0.0.98/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28362 2023-06-06 15:38:18.000000 py3d-0.0.98/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22635 2023-06-06 15:38:18.000000 py3d-0.0.98/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:39:23.940769 py3d-0.0.98/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-06 15:39:23.000000 py3d-0.0.98/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-06 15:39:23.000000 py3d-0.0.98/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 15:39:23.000000 py3d-0.0.98/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-06 15:39:23.000000 py3d-0.0.98/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-06 15:39:23.000000 py3d-0.0.98/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 15:39:23.944769 py3d-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-06 15:38:18.000000 py3d-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:17:26.029535 py3d-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-07 15:17:26.029535 py3d-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-07 15:17:04.000000 py3d-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:17:26.029535 py3d-0.0.99/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-07 15:16:21.000000 py3d-0.0.99/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28362 2023-06-07 15:16:21.000000 py3d-0.0.99/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22638 2023-06-07 15:16:21.000000 py3d-0.0.99/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:17:26.029535 py3d-0.0.99/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-07 15:17:26.000000 py3d-0.0.99/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-07 15:17:26.000000 py3d-0.0.99/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 15:17:26.000000 py3d-0.0.99/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-07 15:17:26.000000 py3d-0.0.99/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-07 15:17:26.000000 py3d-0.0.99/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 15:17:26.029535 py3d-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-07 15:16:21.000000 py3d-0.0.99/setup.py
```

### Comparing `py3d-0.0.98/PKG-INFO` & `py3d-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.98
+Version: 0.0.99
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.98/README.md` & `py3d-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.0.98/py3d/core.py` & `py3d-0.0.99/py3d/core.py`

 * *Files identical despite different names*

### Comparing `py3d-0.0.98/py3d/viewer.html` & `py3d-0.0.99/py3d/viewer.html`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
             this.toolbar.btn_grid.onclick = (ev) => {
                 this.toolbar.btn_grid.style.background = this.toolbar.btn_grid.style.background == "grey" ? "buttonface" : "grey"
                 this.render()
             }
             this.toolbar.slider.oninput = (ev) => {
                 for (let i = 0, l = this.toolbar.ts.length; i < l; i++) {
                     let t = this.toolbar.ts[i]
-                    if (t >= this.toolbar.slider.value) {
+                    if (t - this.toolbar.slider.value > 0) {
                         this.toolbar.ti = i
                         this.toolbar.time.innerHTML = t + "/" + this.toolbar.slider.max
                         this.render()
                         return
                     }
                 }
             }
```

### Comparing `py3d-0.0.98/py3d.egg-info/PKG-INFO` & `py3d-0.0.99/py3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.98
+Version: 0.0.99
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.98/setup.py` & `py3d-0.0.99/setup.py`

 * *Files identical despite different names*

