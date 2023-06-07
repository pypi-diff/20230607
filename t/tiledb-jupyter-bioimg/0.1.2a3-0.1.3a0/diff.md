# Comparing `tmp/tiledb_jupyter_bioimg-0.1.2a3.tar.gz` & `tmp/tiledb_jupyter_bioimg-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb_jupyter_bioimg-0.1.2a3.tar", last modified: Tue Jun  6 12:02:37 2023, max compression
+gzip compressed data, was "tiledb_jupyter_bioimg-0.1.3a0.tar", last modified: Wed Jun  7 13:57:13 2023, max compression
```

## Comparing `tiledb_jupyter_bioimg-0.1.2a3.tar` & `tiledb_jupyter_bioimg-0.1.3a0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:37.992256 tiledb_jupyter_bioimg-0.1.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-06 12:02:37.992256 tiledb_jupyter_bioimg-0.1.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-06 12:00:10.000000 tiledb_jupyter_bioimg-0.1.2a3/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:02:37.992256 tiledb_jupyter_bioimg-0.1.2a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:37.988257 tiledb_jupyter_bioimg-0.1.2a3/src/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/src/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:37.988257 tiledb_jupyter_bioimg-0.1.2a3/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:37.988257 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:37.988257 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-06 12:02:36.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:37.992256 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-06-06 12:02:36.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-06 12:02:36.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/241.7a42393c28911f92f6c6.js
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-06 12:02:36.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
--rw-r--r--   0 runner    (1001) docker     (123)   516688 2023-06-06 12:02:36.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-06 12:02:36.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-06 12:02:36.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/744.83657870ab57005727cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-06 12:02:36.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
--rw-r--r--   0 runner    (1001) docker     (123)   756074 2023-06-06 12:02:36.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/774.3d92675aa1721b861046.js
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-06 12:02:36.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/774.3d92675aa1721b861046.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-06-06 12:02:36.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/remoteEntry.97aa55da34c5f332490c.js
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-06 12:02:08.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    85216 2023-06-06 12:02:36.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:37.988257 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-06 12:02:37.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-06 12:02:37.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:02:37.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:01:19.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-06 12:02:37.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 12:02:37.000000 tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-06 11:57:51.000000 tiledb_jupyter_bioimg-0.1.2a3/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.395265 tiledb_jupyter_bioimg-0.1.3a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-07 13:57:13.395265 tiledb_jupyter_bioimg-0.1.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-07 13:55:06.000000 tiledb_jupyter_bioimg-0.1.3a0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:57:13.395265 tiledb_jupyter_bioimg-0.1.3a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.391265 tiledb_jupyter_bioimg-0.1.3a0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/src/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.391265 tiledb_jupyter_bioimg-0.1.3a0/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.391265 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.391265 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.395265 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/241.3606da7606ad147cbcb2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
+-rw-r--r--   0 runner    (1001) docker     (123)   755430 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   516678 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/744.32875cac115e9f54b48d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/remoteEntry.9bb49b46696448b14690.js
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-07 13:56:47.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    85180 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.391265 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-07 13:57:13.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-07 13:57:13.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:57:13.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:56:05.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 13:57:13.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 13:57:13.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/tsconfig.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/LICENSE` & `tiledb_jupyter_bioimg-0.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb_jupyter_bioimg
-Version: 0.1.2a3
+Version: 0.1.3a0
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/README.md` & `tiledb_jupyter_bioimg-0.1.3a0/README.md`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/package.json` & `tiledb_jupyter_bioimg-0.1.3a0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9708333333333332%*

 * *Differences: {"'dependencies'": "{'@tiledb-inc/bioimage-viewer': '^0.1.1-beta.2'}",*

 * * "'version'": "'0.1.3-alpha.0'"}*

```diff
@@ -2,15 +2,15 @@
     "author": "TileDB",
     "bugs": {
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
         "@jupyterlab/application": "^3.4.5",
-        "@tiledb-inc/bioimage-viewer": "^0.1.1-beta.1"
+        "@tiledb-inc/bioimage-viewer": "^0.1.1-beta.2"
     },
     "description": "A jupyterlab extension to visualize bioimages in TileDB format",
     "devDependencies": {
         "@jupyterlab/builder": "^3.1.0",
         "@typescript-eslint/eslint-plugin": "^2.27.0",
         "@typescript-eslint/parser": "^2.27.0",
         "eslint": "^7.5.0",
@@ -93,9 +93,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.2-alpha.3"
+    "version": "0.1.3-alpha.0"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/setup.py` & `tiledb_jupyter_bioimg-0.1.3a0/setup.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/src/index.ts` & `tiledb_jupyter_bioimg-0.1.3a0/src/index.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/src/version.ts` & `tiledb_jupyter_bioimg-0.1.3a0/src/version.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/src/widget.ts` & `tiledb_jupyter_bioimg-0.1.3a0/src/widget.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/_version.py` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/_version.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/package.json` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9704166666666666%*

 * *Differences: {"'dependencies'": "{'@tiledb-inc/bioimage-viewer': '^0.1.1-beta.2'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9bb49b46696448b14690.js'}}",*

 * * "'version'": "'0.1.3-alpha.0'"}*

```diff
@@ -2,15 +2,15 @@
     "author": "TileDB",
     "bugs": {
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
         "@jupyterlab/application": "^3.4.5",
-        "@tiledb-inc/bioimage-viewer": "^0.1.1-beta.1"
+        "@tiledb-inc/bioimage-viewer": "^0.1.1-beta.2"
     },
     "description": "A jupyterlab extension to visualize bioimages in TileDB format",
     "devDependencies": {
         "@jupyterlab/builder": "^3.1.0",
         "@typescript-eslint/eslint-plugin": "^2.27.0",
         "@typescript-eslint/parser": "^2.27.0",
         "eslint": "^7.5.0",
@@ -27,15 +27,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.97aa55da34c5f332490c.js",
+            "load": "static/remoteEntry.9bb49b46696448b14690.js",
             "style": "./style"
         },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
@@ -98,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.2-alpha.3"
+    "version": "0.1.3-alpha.0"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/241.7a42393c28911f92f6c6.js` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/241.3606da7606ad147cbcb2.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -101,20 +101,20 @@
                         a = e.data.levelRecord.dimensions[e.data.levelRecord.axes.indexOf("X")],
                         s = e.data.levelRecord.dimensions[e.data.levelRecord.axes.indexOf("Y")],
                         h = e.data.levelRecord.downsample,
                         p = e.data.index.x,
                         g = e.data.index.y,
                         d = e.data.tileSize,
                         y = e.data.attribute.type.toLowerCase(),
-                        x = e.data.levelRecord.axesMapping,
-                        A = new i(e.data.levelRecord.arrayAxes.map((t => e.data.levelRecord.axesMapping.get(t))).flat(), ["C", "Y", "X"]),
-                        b = new Array(A.baseAxes.length);
-                    for (let e = 0; e < A.baseAxes.length; ++e) {
-                        const t = A.baseAxes[e];
-                        b[e] = "X" === t || "Y" === t ? h : 1
+                        b = e.data.levelRecord.axesMapping,
+                        x = new i(e.data.levelRecord.arrayAxes.map((t => e.data.levelRecord.axesMapping.get(t))).flat(), ["C", "Y", "X"]),
+                        A = new Array(x.baseAxes.length);
+                    for (let e = 0; e < x.baseAxes.length; ++e) {
+                        const t = x.baseAxes[e];
+                        A[e] = "X" === t || "Y" === t ? h : 1
                     }
                     const m = new Map;
                     m.set("C", e.data.channelRanges), m.set("Y", [g * d * h, Math.min((g + 1) * d * h, s) - 1]), m.set("X", [p * d * h, Math.min((p + 1) * d * h, a) - 1]);
                     const E = ~~((m.get("X")[1] - m.get("X")[0] + 1) / h),
                         v = ~~((m.get("Y")[1] - m.get("Y")[0] + 1) / h);
                     let R = 0;
                     for (let e = 0; e < m.get("C").length; e += 2) R += m.get("C")[e + 1] - m.get("C")[e] + 1;
@@ -137,44 +137,44 @@
                                         a = n.get(e);
                                     for (let e = 0; e < a.length; e += 2) t.push(a[e + 1] - a[e] + 1), r.push(a[e]);
                                     h.push(t), p.push(r)
                                 }
                                 const g = f(...h),
                                     d = f(...p),
                                     y = [],
-                                    x = [];
+                                    b = [];
                                 for (const e of d) {
                                     let t = 0;
                                     for (let r = 0; r < e.length; ++r) t += e[r] * c[r];
                                     y.push(t)
                                 }
                                 for (const e of g) {
                                     const t = new Array(i.length + 1).fill(Number.MAX_SAFE_INTEGER, 0, 1).fill(1, 1);
                                     for (let r = 0; r < e.length; ++r)
                                         for (let a = r + 1; a < e.length; ++a) t[r + 1] *= e[a];
-                                    x.push(t)
+                                    b.push(t)
                                 }
-                                let A = 0;
-                                const b = new Array(i.length),
+                                let x = 0;
+                                const A = new Array(i.length),
                                     m = [],
                                     E = o[r.indexOf(l)];
                                 for (let e = 0; e < g.length; ++e) {
                                     const t = g[e].reduce(((e, t) => e * t), 1);
                                     for (let r = 0; r < t; ++r) {
-                                        A = y[e];
-                                        for (let t = 0; t < x[e].length - 1; ++t) b[t] = ~~(r % x[e][t] / x[e][t + 1]), A += b[t] * c[t];
-                                        if (A >= E) return console.error("OOB"), [];
-                                        m.push(A)
+                                        x = y[e];
+                                        for (let t = 0; t < b[e].length - 1; ++t) A[t] = ~~(r % b[e][t] / b[e][t + 1]), x += A[t] * c[t];
+                                        if (x >= E) return console.error("OOB"), [];
+                                        m.push(x)
                                     }
                                 }
                                 m.sort(((e, t) => e - t)), s.push(u(m))
                             }
                         }
                         return s
-                    }(e.data.levelRecord.dimensions, e.data.levelRecord.axes, e.data.levelRecord.arrayAxes, x, m, e.data.levelRecord.arrayExtends);
+                    }(e.data.levelRecord.dimensions, e.data.levelRecord.axes, e.data.levelRecord.arrayAxes, b, m, e.data.levelRecord.arrayExtends);
                     if (0 === w.length) return;
                     const S = {
                             layout: o.Layout.RowMajor,
                             ranges: w,
                             bufferSize: 12e7,
                             attributes: [e.data.attribute.name],
                             returnRawBuffers: !0
@@ -207,15 +207,15 @@
                             h = new Array(t.baseAxes.length);
                         for (let r = 0; r < e.length; ++r) {
                             f = 0;
                             for (let e = 0; e < i.length - 1; ++e) h[e] = ~~(r % i[e] / i[e + 1]), f += ~~(h[e] / o[t.permutationMatrix[e]]) * c[t.permutationMatrix[e]];
                             l[f] += e[r] / u
                         }
                         return l
-                    }(T, A, O, b);
+                    }(T, x, O, A);
                     self.postMessage({
                         data: M,
                         width: E,
                         height: v,
                         channels: R
                     }, [M.buffer])
                 }
@@ -258,15 +258,15 @@
             a: t
         }), t
     }, n.d = (e, t) => {
         for (var r in t) n.o(t, r) && !n.o(e, r) && Object.defineProperty(e, r, {
             enumerable: !0,
             get: t[r]
         })
-    }, n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, r) => (n.f[r](e, t), t)), [])), n.u = e => e + ".b2bedc962bcd82714540.js?v=b2bedc962bcd82714540", n.g = function() {
+    }, n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, r) => (n.f[r](e, t), t)), [])), n.u = e => e + ".a03dea4f48d4a0dc1e4c.js?v=a03dea4f48d4a0dc1e4c", n.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), n.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), n.r = e => {
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 635.b2bedc962bcd82714540.js.LICENSE.txt */
+/*! For license information please see 635.a03dea4f48d4a0dc1e4c.js.LICENSE.txt */
 (self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || []).push([
     [635], {
         9757: (t, e, r) => {
             "use strict";
             r.d(e, {
                 Z: () => i
             });
@@ -723,15 +723,15 @@
                 value: !0
             });
             const s = i(r(2437));
             e.default = s.default
         },
         7342: function(t, e, r) {
             "use strict";
-            var i = r(4155),
+            var i = r(46),
                 s = this && this.__awaiter || function(t, e, r, i) {
                     return new(r || (r = Promise))((function(s, n) {
                         function a(t) {
                             try {
                                 c(i.next(t))
                             } catch (t) {
                                 n(t)
@@ -12503,15 +12503,15 @@
                 return i.forEach(r, (function(r) {
                     t = r.call(n, t, e)
                 })), t
             }
         },
         5655: (t, e, r) => {
             "use strict";
-            var i = r(4155),
+            var i = r(46),
                 s = r(4867),
                 n = r(6016),
                 a = r(481),
                 o = {
                     "Content-Type": "application/x-www-form-urlencoded"
                 };
 
@@ -15402,15 +15402,15 @@
             }, i.default.formatters.a = function(t) {
                 return "0x" + o(t.toString(16), 8)
             }, i.default.formatters.X = function(t) {
                 return "0x" + t.toString(16).toUpperCase()
             }
         },
         3834: (t, e, r) => {
-            var i = r(4155);
+            var i = r(46);
 
             function s() {
                 var t;
                 try {
                     t = e.storage.debug
                 } catch (t) {}
                 return !t && void 0 !== i && "env" in i && (t = i.env.DEBUG), t
@@ -15721,15 +15721,15 @@
                     data: t
                 }))
             }, s.prototype.terminate = function() {
                 this.process.kill()
             }, t.exports = s
         },
         6549: (t, e, r) => {
-            var i = r(4155);
+            var i = r(46);
             ! function() {
                 const e = t.exports,
                     s = void 0 !== i && i.release && "node" === i.release.name;
                 var n = n || function(t) {
                     setTimeout(t, 0)
                 };
                 const a = s ? r(5820) : self.Worker,
@@ -15909,15 +15909,15 @@
                             const s = e(t);
                             void 0 !== s && (r.data = s), i.resolve(null, r.data)
                         } else i.resolve(null, t)
                     })), this.operation = i, this
                 }, e ? t.exports = l : self.Parallel = l
             }()
         },
-        4155: t => {
+        46: t => {
             var e, r, i = t.exports = {};
 
             function s() {
                 throw new Error("setTimeout has not been defined")
             }
 
             function n() {
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js.LICENSE.txt` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/744.83657870ab57005727cf.js` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/744.32875cac115e9f54b48d.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -12,15 +12,15 @@
                 BioImageViewerModel: () => d,
                 BioImageViewerView: () => p
             });
             var s = l(1395);
             const n = l(4147),
                 a = n.version,
                 r = n.name;
-            var o = l(8840),
+            var o = l(4155),
                 u = l.n(o);
             class d extends s.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         _model_name: d.model_name,
                         _model_module: d.model_module,
                         _model_module_version: d.model_module_version,
@@ -57,11 +57,11 @@
                         version: a,
                         exports: t
                     })
                 }
             }
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.2-alpha.3","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.1-beta.1"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.3-alpha.0","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.1-beta.2"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/774.3d92675aa1721b861046.js` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,86 +1,10 @@
-/*! For license information please see 774.3d92675aa1721b861046.js.LICENSE.txt */
+/*! For license information please see 556.f09c354898cd66a026b3.js.LICENSE.txt */
 (self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || []).push([
-    [774], {
-        597: (t, e, n) => {
-            "use strict";
-            var i, r = Object.assign || function(t) {
-                    for (var e = 1; e < arguments.length; e++) {
-                        var n = arguments[e];
-                        for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
-                    }
-                    return t
-                },
-                s = (i = n(6271)) && i.__esModule ? i : {
-                    default: i
-                };
-            e.Z = function(t) {
-                var e = t.fill,
-                    n = void 0 === e ? "currentColor" : e,
-                    i = t.width,
-                    o = void 0 === i ? 24 : i,
-                    a = t.height,
-                    l = void 0 === a ? 24 : a,
-                    c = t.style,
-                    h = void 0 === c ? {} : c,
-                    u = function(t, e) {
-                        var n = {};
-                        for (var i in t) e.indexOf(i) >= 0 || Object.prototype.hasOwnProperty.call(t, i) && (n[i] = t[i]);
-                        return n
-                    }(t, ["fill", "width", "height", "style"]);
-                return s.default.createElement("svg", r({
-                    viewBox: "0 0 24 24",
-                    style: r({
-                        fill: n,
-                        width: o,
-                        height: l
-                    }, h)
-                }, u), s.default.createElement("path", {
-                    d: "M21,7L9,19L3.5,13.5L4.91,12.09L9,16.17L19.59,5.59L21,7Z"
-                }))
-            }
-        },
-        1995: (t, e, n) => {
-            "use strict";
-            var i, r = Object.assign || function(t) {
-                    for (var e = 1; e < arguments.length; e++) {
-                        var n = arguments[e];
-                        for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
-                    }
-                    return t
-                },
-                s = (i = n(6271)) && i.__esModule ? i : {
-                    default: i
-                };
-            e.Z = function(t) {
-                var e = t.fill,
-                    n = void 0 === e ? "currentColor" : e,
-                    i = t.width,
-                    o = void 0 === i ? 24 : i,
-                    a = t.height,
-                    l = void 0 === a ? 24 : a,
-                    c = t.style,
-                    h = void 0 === c ? {} : c,
-                    u = function(t, e) {
-                        var n = {};
-                        for (var i in t) e.indexOf(i) >= 0 || Object.prototype.hasOwnProperty.call(t, i) && (n[i] = t[i]);
-                        return n
-                    }(t, ["fill", "width", "height", "style"]);
-                return s.default.createElement("svg", r({
-                    viewBox: "0 0 24 24",
-                    style: r({
-                        fill: n,
-                        width: o,
-                        height: l
-                    }, h)
-                }, u), s.default.createElement("path", {
-                    d: "M12,18.17L8.83,15L7.42,16.41L12,21L16.59,16.41L15.17,15M12,5.83L15.17,9L16.58,7.59L12,3L7.41,7.59L8.83,9L12,5.83Z"
-                }))
-            }
-        },
+    [556], {
         9296: t => {
             "use strict";
             t.exports = n, t.exports.default = n;
             var e = 1e20;
 
             function n(t, e, n, i, r, s) {
                 this.fontSize = t || 24, this.buffer = void 0 === e ? 3 : e, this.cutoff = i || .25, this.fontFamily = r || "sans-serif", this.fontWeight = s || "normal", this.radius = n || 8;
@@ -148,29 +72,29 @@
                     }
             }, n.prototype.draw = function(t) {
                 return this._draw(t, !1).data
             }, n.prototype.drawWithMetrics = function(t) {
                 return this._draw(t, !0)
             }
         },
-        3774: (t, e, n) => {
+        1556: (t, e, n) => {
             "use strict";
             n.r(e), n.d(e, {
                 default: () => pE
             });
             var i = n(3379),
                 r = n.n(i),
                 s = n(4272);
             r()(s.Z, {
                 insert: "head",
                 singleton: !1
             }), s.Z.locals;
-            var o = n(5893),
-                a = n(4456),
-                l = n.n(a),
+            var o = n(9336),
+                a = n(2700),
+                l = n(4456),
                 c = n(6271),
                 h = n.n(c),
                 u = n(3578),
                 d = n.n(u),
                 p = n(9941),
                 f = {},
                 g = function(t, e, n, i) {
@@ -672,20 +596,20 @@
                             style: i.slider
                         }))))
                     }
                 }]), e
             }(c.PureComponent || c.Component);
             var O = n(5697),
                 L = n.n(O);
-            const k = function(t, e) {
+            const R = function(t, e) {
                     return t === e || t != t && e != e
                 },
-                R = function(t, e) {
+                k = function(t, e) {
                     for (var n = t.length; n--;)
-                        if (k(t[n][0], e)) return n;
+                        if (R(t[n][0], e)) return n;
                     return -1
                 };
             var I = Array.prototype.splice;
 
             function j(t) {
                 var e = -1,
                     n = null == t ? 0 : t.length;
@@ -694,25 +618,25 @@
                     this.set(i[0], i[1])
                 }
             }
             j.prototype.clear = function() {
                 this.__data__ = [], this.size = 0
             }, j.prototype.delete = function(t) {
                 var e = this.__data__,
-                    n = R(e, t);
+                    n = k(e, t);
                 return !(n < 0 || (n == e.length - 1 ? e.pop() : I.call(e, n, 1), --this.size, 0))
             }, j.prototype.get = function(t) {
                 var e = this.__data__,
-                    n = R(e, t);
+                    n = k(e, t);
                 return n < 0 ? void 0 : e[n][1]
             }, j.prototype.has = function(t) {
-                return R(this.__data__, t) > -1
+                return k(this.__data__, t) > -1
             }, j.prototype.set = function(t, e) {
                 var n = this.__data__,
-                    i = R(n, t);
+                    i = k(n, t);
                 return i < 0 ? (++this.size, n.push([t, e])) : n[i][1] = e, this
             };
             const z = j;
             var F = n(6169);
             const B = F.Z.Symbol;
             var D = Object.prototype,
                 N = D.hasOwnProperty,
@@ -877,15 +801,15 @@
                         configurable: !0,
                         enumerable: !0,
                         value: n,
                         writable: !0
                     }) : t[e] = n
                 },
                 yt = function(t, e, n) {
-                    (void 0 !== n && !k(t[e], n) || void 0 === n && !(e in t)) && bt(t, e, n)
+                    (void 0 !== n && !R(t[e], n) || void 0 === n && !(e in t)) && bt(t, e, n)
                 },
                 _t = function(t, e, n) {
                     for (var i = -1, r = Object(t), s = n(t), o = s.length; o--;) {
                         var a = s[++i];
                         if (!1 === e(r[a], a, r)) break
                     }
                     return t
@@ -923,21 +847,21 @@
                 },
                 Ot = function(t) {
                     return null != t && "object" == typeof t
                 },
                 Lt = function(t) {
                     return Ot(t) && "[object Arguments]" == H(t)
                 };
-            var kt = Object.prototype,
-                Rt = kt.hasOwnProperty,
-                It = kt.propertyIsEnumerable;
+            var Rt = Object.prototype,
+                kt = Rt.hasOwnProperty,
+                It = Rt.propertyIsEnumerable;
             const jt = Lt(function() {
                     return arguments
                 }()) ? Lt : function(t) {
-                    return Ot(t) && Rt.call(t, "callee") && !It.call(t, "callee")
+                    return Ot(t) && kt.call(t, "callee") && !It.call(t, "callee")
                 },
                 zt = Array.isArray,
                 Ft = function(t) {
                     return "number" == typeof t && t > -1 && t % 1 == 0 && t <= 9007199254740991
                 },
                 Bt = function(t) {
                     return null != t && Ft(t.length) && !q(t)
@@ -960,15 +884,15 @@
             var Yt;
             const Kt = function(t, e) {
                 if (("constructor" !== e || "function" != typeof t[e]) && "__proto__" != e) return t[e]
             };
             var $t = Object.prototype.hasOwnProperty;
             const Jt = function(t, e, n) {
                 var i = t[e];
-                $t.call(t, e) && k(i, n) && (void 0 !== n || e in t) || bt(t, e, n)
+                $t.call(t, e) && R(i, n) && (void 0 !== n || e in t) || bt(t, e, n)
             };
             var Qt = /^(?:0|[1-9]\d*)$/;
             const te = function(t, e) {
                 var n = typeof t;
                 return !!(e = null == e ? 9007199254740991 : e) && ("number" == n || "symbol" != n && Qt.test(t)) && t > -1 && t % 1 == 0 && t < e
             };
             var ee = Object.prototype.hasOwnProperty;
@@ -1111,15 +1035,15 @@
                     var n = -1,
                         i = e.length,
                         r = i > 1 ? e[i - 1] : void 0,
                         s = i > 2 ? e[2] : void 0;
                     for (r = me.length > 3 && "function" == typeof r ? (i--, r) : void 0, s && function(t, e, n) {
                             if (!Z(n)) return !1;
                             var i = typeof e;
-                            return !!("number" == i ? Bt(n) && te(e, n.length) : "string" == i && e in n) && k(n[e], t)
+                            return !!("number" == i ? Bt(n) && te(e, n.length) : "string" == i && e in n) && R(n[e], t)
                         }(e[0], e[1], s) && (r = i < 3 ? void 0 : r, i = 1), t = Object(t); ++n < i;) {
                         var o = e[n];
                         o && me(t, o, n)
                     }
                     return t
                 })));
             var me, ve = function(t) {
@@ -1284,26 +1208,26 @@
                 }
                 return e = Ae(e) || 0, Z(n) && (h = !!n.leading, s = (u = "maxWait" in n) ? Me(Ae(n.maxWait) || 0, e) : s, d = "trailing" in n ? !!n.trailing : d), v.cancel = function() {
                     void 0 !== a && clearTimeout(a), c = 0, i = l = r = a = void 0
                 }, v.flush = function() {
                     return void 0 === a ? o : m(ye())
                 }, v
             };
-            var ke = function() {
+            var Re = function() {
                     function t(t, e) {
                         for (var n = 0; n < e.length; n++) {
                             var i = e[n];
                             i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
                         }
                     }
                     return function(e, n, i) {
                         return n && t(e.prototype, n), i && t(e, i), e
                     }
                 }(),
-                Re = function(t) {
+                ke = function(t) {
                     function e(t) {
                         ! function(t, e) {
                             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                         }(this, e);
                         var n = function(t, e) {
                             if (!t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                             return !e || "object" != typeof e && "function" != typeof e ? t : e
@@ -1353,15 +1277,15 @@
                             constructor: {
                                 value: t,
                                 enumerable: !1,
                                 writable: !0,
                                 configurable: !0
                             }
                         }), e && (Object.setPrototypeOf ? Object.setPrototypeOf(t, e) : t.__proto__ = e)
-                    }(e, t), ke(e, [{
+                    }(e, t), Re(e, [{
                         key: "componentWillUnmount",
                         value: function() {
                             this.throttle.cancel(), this.unbindEventListeners()
                         }
                     }, {
                         key: "getContainerRenderWindow",
                         value: function() {
@@ -1443,15 +1367,15 @@
                                 style: a.pointer
                             }, this.props.pointer ? h().createElement(this.props.pointer, this.props) : h().createElement("div", {
                                 style: a.circle
                             }))))
                         }
                     }]), e
                 }(c.PureComponent || c.Component);
-            const Ie = Re,
+            const Ie = ke,
                 je = function(t, e) {
                     for (var n = -1, i = null == t ? 0 : t.length; ++n < i && !1 !== e(t[n], n, t););
                     return t
                 },
                 ze = Ct(Object.keys, Object);
             var Fe = Object.prototype.hasOwnProperty;
             const Be = function(t) {
@@ -2310,27 +2234,27 @@
             var Ln = Object.assign || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
                         var n = arguments[e];
                         for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
                     }
                     return t
                 },
-                kn = function() {
+                Rn = function() {
                     function t(t, e) {
                         for (var n = 0; n < e.length; n++) {
                             var i = e[n];
                             i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
                         }
                     }
                     return function(e, n, i) {
                         return n && t(e.prototype, n), i && t(e, i), e
                     }
                 }();
 
-            function Rn(t, e) {
+            function kn(t, e) {
                 if (!t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                 return !e || "object" != typeof e && "function" != typeof e ? t : e
             }
             var In = Object.assign || function(t) {
                 for (var e = 1; e < arguments.length; e++) {
                     var n = arguments[e];
                     for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
@@ -2342,37 +2266,37 @@
                 return function(n) {
                     function i() {
                         var t, e, n;
                         ! function(t, e) {
                             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                         }(this, i);
                         for (var r = arguments.length, s = Array(r), o = 0; o < r; o++) s[o] = arguments[o];
-                        return e = n = Rn(this, (t = i.__proto__ || Object.getPrototypeOf(i)).call.apply(t, [this].concat(s))), n.state = {
+                        return e = n = kn(this, (t = i.__proto__ || Object.getPrototypeOf(i)).call.apply(t, [this].concat(s))), n.state = {
                             focus: !1
                         }, n.handleFocus = function() {
                             return n.setState({
                                 focus: !0
                             })
                         }, n.handleBlur = function() {
                             return n.setState({
                                 focus: !1
                             })
-                        }, Rn(n, e)
+                        }, kn(n, e)
                     }
                     return function(t, e) {
                         if ("function" != typeof e && null !== e) throw new TypeError("Super expression must either be null or a function, not " + typeof e);
                         t.prototype = Object.create(e && e.prototype, {
                             constructor: {
                                 value: t,
                                 enumerable: !1,
                                 writable: !0,
                                 configurable: !0
                             }
                         }), e && (Object.setPrototypeOf ? Object.setPrototypeOf(t, e) : t.__proto__ = e)
-                    }(i, n), kn(i, [{
+                    }(i, n), Rn(i, [{
                         key: "render",
                         value: function() {
                             return h().createElement(e, {
                                 onFocus: this.handleFocus,
                                 onBlur: this.handleBlur
                             }, h().createElement(t, Ln({}, this.props, this.state)))
                         }
@@ -2650,15 +2574,15 @@
                                 if (t.byteLength != e.byteLength || t.byteOffset != e.byteOffset) return !1;
                                 t = t.buffer, e = e.buffer;
                             case "[object ArrayBuffer]":
                                 return !(t.byteLength != e.byteLength || !s(new wt(t), new wt(e)));
                             case "[object Boolean]":
                             case "[object Date]":
                             case "[object Number]":
-                                return k(+t, +e);
+                                return R(+t, +e);
                             case "[object Error]":
                                 return t.name == e.name && t.message == e.message;
                             case "[object RegExp]":
                             case "[object String]":
                                 return t == e + "";
                             case "[object Map]":
                                 var a = Wn;
@@ -2794,20 +2718,20 @@
                 return e
             }((function(t) {
                 var e = [];
                 return 46 === t.charCodeAt(0) && e.push(""), t.replace(Mi, (function(t, n, i, r) {
                     e.push(i ? r.replace(Oi, "$1") : n || t)
                 })), e
             }));
-            var ki = B ? B.prototype : void 0,
-                Ri = ki ? ki.toString : void 0;
+            var Ri = B ? B.prototype : void 0,
+                ki = Ri ? Ri.toString : void 0;
             const Ii = function t(e) {
                     if ("string" == typeof e) return e;
                     if (zt(e)) return Bn(e, t) + "";
-                    if (Ee(e)) return Ri ? Ri.call(e) : "";
+                    if (Ee(e)) return ki ? ki.call(e) : "";
                     var n = e + "";
                     return "0" == n && 1 / e == -1 / 0 ? "-0" : n
                 },
                 ji = function(t) {
                     return null == t ? "" : Ii(t)
                 },
                 zi = function(t, e) {
@@ -3051,16 +2975,16 @@
                 Sr = "#03a9f4",
                 Cr = "#0288d1",
                 Tr = "#01579b",
                 Ar = "#b2ebf2",
                 Mr = "#4dd0e1",
                 Or = "#00bcd4",
                 Lr = "#0097a7",
-                kr = "#006064",
-                Rr = "#b2dfdb",
+                Rr = "#006064",
+                kr = "#b2dfdb",
                 Ir = "#4db6ac",
                 jr = "#009688",
                 zr = "#00796b",
                 Fr = "#004d40",
                 Br = "#c8e6c9",
                 Dr = "#81c784",
                 Nr = "#4caf50",
@@ -3216,16 +3140,16 @@
                 circleSpacing: 14,
                 colors: [Yi, tr, sr, hr, gr, _r, Sr, Or, jr, Nr, Wr, Yr, ts, ss, hs, gs, _s, Ss],
                 styles: {}
             }, On(Os);
             const Ls = function(t) {
                 return void 0 === t
             };
-            var ks = n(1995),
-                Rs = function() {
+            var Rs = n(746),
+                ks = function() {
                     function t(t, e) {
                         for (var n = 0; n < e.length; n++) {
                             var i = e[n];
                             i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
                         }
                     }
                     return function(e, n, i) {
@@ -3288,15 +3212,15 @@
                             constructor: {
                                 value: t,
                                 enumerable: !1,
                                 writable: !0,
                                 configurable: !0
                             }
                         }), e && (Object.setPrototypeOf ? Object.setPrototypeOf(t, e) : t.__proto__ = e)
-                    }(e, t), Rs(e, [{
+                    }(e, t), ks(e, [{
                         key: "render",
                         value: function() {
                             var t = this,
                                 e = (0, p.ZP)({
                                     default: {
                                         wrap: {
                                             paddingTop: "16px",
@@ -3478,15 +3402,15 @@
                                 style: e.toggle
                             }, h().createElement("div", {
                                 style: e.icon,
                                 onClick: this.toggleViews,
                                 ref: function(e) {
                                     return t.icon = e
                                 }
-                            }, h().createElement(ks.Z, {
+                            }, h().createElement(Rs.Z, {
                                 style: e.svg,
                                 onMouseOver: this.showHighlight,
                                 onMouseEnter: this.showHighlight,
                                 onMouseOut: this.hideHighlight
                             }))))
                         }
                     }], [{
@@ -5304,15 +5228,15 @@
                     });
                     return h().createElement("div", {
                         style: t.picker
                     })
                 },
                 styles: {}
             }, On(lo);
-            var co = n(597);
+            var co = n(9367);
             const ho = function(t) {
                     var e = t.color,
                         n = t.onClick,
                         i = void 0 === n ? function() {} : n,
                         r = t.onSwatchHover,
                         s = t.first,
                         o = t.last,
@@ -5476,16 +5400,16 @@
                     [$i, Ki, Yi, Xi, qi],
                     [nr, er, tr, Qi, Ji],
                     [ar, or, sr, rr, ir],
                     [dr, ur, hr, cr, lr],
                     [vr, mr, gr, fr, pr],
                     [wr, xr, _r, yr, br],
                     [Tr, Cr, Sr, Pr, Er],
-                    [kr, Lr, Or, Mr, Ar],
-                    [Fr, zr, jr, Ir, Rr],
+                    [Rr, Lr, Or, Mr, Ar],
+                    [Fr, zr, jr, Ir, kr],
                     ["#194D33", Vr, Nr, Dr, Br],
                     [Zr, Hr, Wr, Gr, Ur],
                     [$r, Kr, Yr, Xr, qr],
                     [ns, es, ts, Qr, Jr],
                     [as, os, ss, rs, is],
                     [ds, us, hs, cs, ls],
                     [vs, ms, gs, fs, ps],
@@ -6109,30 +6033,30 @@
                     n >= t.duration * t.repeat ? t.time = t.duration * t.rate : (t.time = Math.max(0, n) % t.duration, t.time *= t.rate)
                 }
             }
             const Co = Symbol.for("component"),
                 To = Symbol.for("asyncPropDefaults"),
                 Ao = Symbol.for("asyncPropOriginal"),
                 Mo = Symbol.for("asyncPropResolved");
-            var Oo = n(4155);
+            var Oo = n(46);
 
             function Lo(t) {
                 if ("undefined" != typeof window && "object" == typeof window.process && "renderer" === window.process.type) return !0;
                 if (void 0 !== Oo && "object" == typeof Oo.versions && Boolean(Oo.versions.electron)) return !0;
                 const e = "object" == typeof navigator && "string" == typeof navigator.userAgent && navigator.userAgent,
                     n = t || e;
                 return !!(n && n.indexOf("Electron") >= 0)
             }
-            var ko = n(4155);
+            var Ro = n(46);
 
-            function Ro() {
-                return !("object" == typeof ko && "[object process]" === String(ko) && !ko.browser) || Lo()
+            function ko() {
+                return !("object" == typeof Ro && "[object process]" === String(Ro) && !Ro.browser) || Lo()
             }
             const Io = "undefined" != typeof __VERSION__ ? __VERSION__ : "untranspiled source";
-            Ro();
+            ko();
             class jo {
                 constructor(t, e) {
                     let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "sessionStorage";
                     wo(this, "storage", void 0), wo(this, "id", void 0), wo(this, "config", void 0), this.storage = function(t) {
                         try {
                             const e = window[t],
                                 n = "__storage_test__";
@@ -6177,38 +6101,38 @@
             }
 
             function Do(t, e) {
                 if (!t) throw new Error(e || "Assertion failed")
             }! function(t) {
                 t[t.BLACK = 30] = "BLACK", t[t.RED = 31] = "RED", t[t.GREEN = 32] = "GREEN", t[t.YELLOW = 33] = "YELLOW", t[t.BLUE = 34] = "BLUE", t[t.MAGENTA = 35] = "MAGENTA", t[t.CYAN = 36] = "CYAN", t[t.WHITE = 37] = "WHITE", t[t.BRIGHT_BLACK = 90] = "BRIGHT_BLACK", t[t.BRIGHT_RED = 91] = "BRIGHT_RED", t[t.BRIGHT_GREEN = 92] = "BRIGHT_GREEN", t[t.BRIGHT_YELLOW = 93] = "BRIGHT_YELLOW", t[t.BRIGHT_BLUE = 94] = "BRIGHT_BLUE", t[t.BRIGHT_MAGENTA = 95] = "BRIGHT_MAGENTA", t[t.BRIGHT_CYAN = 96] = "BRIGHT_CYAN", t[t.BRIGHT_WHITE = 97] = "BRIGHT_WHITE"
             }(Fo || (Fo = {}));
-            var No = n(4155);
+            var No = n(46);
             const Vo = {
                     self: "undefined" != typeof self && self,
                     window: "undefined" != typeof window && window,
                     global: void 0 !== n.g && n.g,
                     document: "undefined" != typeof document && document,
                     process: "object" == typeof No && No
                 },
                 Uo = Vo.window || Vo.self || Vo.global,
                 Go = Vo.process || {};
 
             function Wo() {
                 let t;
                 var e, n;
-                if (Ro && "performance" in Uo) t = null == Uo || null === (e = Uo.performance) || void 0 === e || null === (n = e.now) || void 0 === n ? void 0 : n.call(e);
+                if (ko && "performance" in Uo) t = null == Uo || null === (e = Uo.performance) || void 0 === e || null === (n = e.now) || void 0 === n ? void 0 : n.call(e);
                 else if ("hrtime" in Go) {
                     var i;
                     const e = null == Go || null === (i = Go.hrtime) || void 0 === i ? void 0 : i.call(Go);
                     t = 1e3 * e[0] + e[1] / 1e6
                 } else t = Date.now();
                 return t
             }
             const Ho = {
-                    debug: Ro && console.debug || console.log,
+                    debug: ko && console.debug || console.log,
                     log: console.log,
                     info: console.info,
                     warn: console.warn,
                     error: console.error
                 },
                 Zo = {
                     enabled: !0,
@@ -6324,15 +6248,15 @@
                     let {
                         logLevel: e,
                         priority: n,
                         image: i,
                         message: r = "",
                         scale: s = 1
                     } = t;
-                    return this._shouldLog(e || n) ? Ro ? function(t) {
+                    return this._shouldLog(e || n) ? ko ? function(t) {
                         let {
                             image: e,
                             message: n = "",
                             scale: i = 1
                         } = t;
                         if ("string" == typeof e) {
                             const t = new Image;
@@ -6430,15 +6354,15 @@
                                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 8;
                                     const n = Math.max(e - t.length, 0);
                                     return "".concat(" ".repeat(n)).concat(t)
                                 }(function(t) {
                                     let e;
                                     return e = t < 10 ? "".concat(t.toFixed(2), "ms") : t < 100 ? "".concat(t.toFixed(1), "ms") : t < 1e3 ? "".concat(t.toFixed(0), "ms") : "".concat((t / 1e3).toFixed(2), "s"), e
                                 }(n.total)) : "";
-                                i = e = n.time ? "".concat(t, ": ").concat(o, "  ").concat(e) : "".concat(t, ": ").concat(e), r = n.color, s = n.background, Ro || "string" != typeof i || (r && (r = Bo(r), i = "[".concat(r, "m").concat(i, "[39m")), s && (r = Bo(s), i = "[".concat(s + 10, "m").concat(i, "[49m"))), e = i
+                                i = e = n.time ? "".concat(t, ": ").concat(o, "  ").concat(e) : "".concat(t, ": ").concat(e), r = n.color, s = n.background, ko || "string" != typeof i || (r && (r = Bo(r), i = "[".concat(r, "m").concat(i, "[39m")), s && (r = Bo(s), i = "[".concat(s + 10, "m").concat(i, "[49m"))), e = i
                             }
                             var i, r, s;
                             return e
                         }(this.id, r.message, r), n.bind(console, e, ...r.args)
                     }
                     return qo
                 }
@@ -6520,15 +6444,15 @@
                 const r = e.length,
                     s = i * r;
                 let o = 0;
                 for (let i = n; o < r; o++) t[i++] = e[o];
                 for (; o < s;) o < s - o ? (t.copyWithin(n + o, n, n + o), o *= 2) : (t.copyWithin(n + o, n, n + s - o), o = s);
                 return t
             }
-            var oa = n(4155);
+            var oa = n(46);
 
             function aa() {
                 let t;
                 if ("undefined" != typeof window && window.performance) t = window.performance.now();
                 else if (void 0 !== oa && oa.hrtime) {
                     const e = oa.hrtime();
                     t = 1e3 * e[0] + e[1] / 1e6
@@ -6730,35 +6654,35 @@
                 const o = new Response(t, {
                     headers: e
                 });
                 return Object.defineProperty(o, "url", {
                     value: i
                 }), o
             }
-            async function ka(t, e) {
+            async function Ra(t, e) {
                 if ("string" == typeof t) {
                     t = function(t) {
                         for (const e in Ea)
                             if (t.startsWith(e)) {
                                 const n = Ea[e];
                                 t = t.replace(e, n)
                             } return t.startsWith("http://") || t.startsWith("https://") || (t = "".concat(wa).concat(t)), t
                     }(t);
                     let n = e;
                     return null != e && e.fetch && "function" != typeof(null == e ? void 0 : e.fetch) && (n = e.fetch), await fetch(t, n)
                 }
                 return await La(t)
             }
-            var Ra = n(4155),
-                Ia = n(4155);
+            var ka = n(46),
+                Ia = n(46);
 
             function ja() {
                 return !("object" == typeof Ia && "[object process]" === String(Ia) && !Ia.browser) || function(t) {
                     if ("undefined" != typeof window && "object" == typeof window.process && "renderer" === window.process.type) return !0;
-                    if (void 0 !== Ra && "object" == typeof Ra.versions && Boolean(Ra.versions.electron)) return !0;
+                    if (void 0 !== ka && "object" == typeof ka.versions && Boolean(ka.versions.electron)) return !0;
                     const e = "object" == typeof navigator && "string" == typeof navigator.userAgent && navigator.userAgent;
                     return !!(e && e.indexOf("Electron") >= 0)
                 }()
             }
             const za = "undefined" != typeof __VERSION__ ? __VERSION__ : "untranspiled source";
             ja();
             class Fa {
@@ -7143,15 +7067,15 @@
                 warn() {
                     return () => {}
                 }
                 error() {
                     return () => {}
                 }
             }
-            var nl = n(4155);
+            var nl = n(46);
             "undefined" != typeof self && self, "undefined" != typeof window && window, void 0 !== n.g && n.g, "undefined" != typeof document && document;
             const il = Boolean("object" != typeof nl || "[object process]" !== String(nl) || nl.browser),
                 rl = void 0 !== nl && nl.version && /v([0-9]*)/.exec(nl.version),
                 sl = (rl && parseFloat(rl[1]), {
                     fetch: null,
                     mimeType: void 0,
                     nothrow: !1,
@@ -7279,21 +7203,21 @@
                         } : t[n] = e[n]
                     }
             }
 
             function pl(t, e) {
                 const n = ll(),
                     i = t || n;
-                return "function" == typeof i.fetch ? i.fetch : ua(i.fetch) ? t => ka(t, i) : null != e && e.fetch ? null == e ? void 0 : e.fetch : ka
+                return "function" == typeof i.fetch ? i.fetch : ua(i.fetch) ? t => Ra(t, i) : null != e && e.fetch ? null == e ? void 0 : e.fetch : Ra
             }
 
             function fl(t, e) {
                 if (!t) throw new Error(e || "loaders.gl assertion failed.")
             }
-            var gl = n(4155);
+            var gl = n(46);
             "undefined" != typeof self && self, "undefined" != typeof window && window, void 0 !== n.g && n.g, "undefined" != typeof document && document;
             const ml = "object" != typeof gl || "[object process]" !== String(gl) || gl.browser,
                 vl = "undefined" != typeof window && void 0 !== window.orientation,
                 bl = void 0 !== gl && gl.version && /v([0-9]*)/.exec(gl.version);
             bl && parseFloat(bl[1]);
             class yl {
                 terminate() {}
@@ -7547,24 +7471,24 @@
                         return fl(r), r
                     }(t, n),
                     a = Ml.getWorkerFarm(n).getWorkerPool({
                         name: s,
                         url: o
                     });
                 n = JSON.parse(JSON.stringify(n)), i = JSON.parse(JSON.stringify(i || {}));
-                const l = await a.startJob("process-on-worker", kl.bind(null, r));
+                const l = await a.startJob("process-on-worker", Rl.bind(null, r));
                 l.postMessage("process", {
                     input: e,
                     options: n,
                     context: i
                 });
                 const c = await l.result;
                 return await c.result
             }
-            async function kl(t, e, n, i) {
+            async function Rl(t, e, n, i) {
                 switch (n) {
                     case "done":
                         e.done(i);
                         break;
                     case "error":
                         e.error(new Error(i.error));
                         break;
@@ -7586,15 +7510,15 @@
                             })
                         }
                         break;
                     default:
                         console.warn("parse-with-worker unknown message ".concat(n))
                 }
             }
-            const Rl = 262144,
+            const kl = 262144,
                 Il = 262144,
                 jl = 1048576;
 
             function zl(t) {
                 if ((e = t) && "object" == typeof e && e.isBuffer) return t;
                 var e;
                 if (t instanceof ArrayBuffer) return t;
@@ -7661,15 +7585,15 @@
                             }(t);
                             throw new Error(e)
                         }
                     }(n), e.binary ? await n.arrayBuffer() : await n.text()
                 }
                 if (ba(t) && (t = function(t, e) {
                         if ("string" == typeof t) return function*(t, e) {
-                            const n = (null == e ? void 0 : e.chunkSize) || Rl;
+                            const n = (null == e ? void 0 : e.chunkSize) || kl;
                             let i = 0;
                             const r = new TextEncoder;
                             for (; i < t.length;) {
                                 const e = Math.min(t.length - i, n),
                                     s = t.slice(i, i + e);
                                 i += e, yield r.encode(s)
                             }
@@ -8556,44 +8480,44 @@
                 }
                 transformByQuaternion(t) {
                     return wc(this, this, t), this.check()
                 }
             }
             const Lc = new Oc;
 
-            function kc(t, e, n, i) {
+            function Rc(t, e, n, i) {
                 Lc.set(t, e, n);
                 const r = Lc.len();
                 return {
                     distance: i / r,
                     normal: new Oc(-t / r, -e / r, -n / r)
                 }
             }
-            let Rc;
+            let kc;
 
             function Ic(t, e) {
                 const {
                     size: n = 1,
                     startIndex: i = 0
                 } = e, r = void 0 !== e.endIndex ? e.endIndex : t.length, s = (r - i) / n;
-                Rc = nc.allocate(Rc, s, {
+                kc = nc.allocate(kc, s, {
                     type: Float32Array,
                     size: 2 * n
                 });
                 let o = i,
                     a = 0;
                 for (; o < r;) {
                     for (let e = 0; e < n; e++) {
                         const i = t[o++];
-                        Rc[a + e] = i, Rc[a + e + n] = (l = i) - Math.fround(l)
+                        kc[a + e] = i, kc[a + e + n] = (l = i) - Math.fround(l)
                     }
                     a += 2 * n
                 }
                 var l;
-                return Rc.subarray(0, s * n * 2)
+                return kc.subarray(0, s * n * 2)
             }
             class jc extends cc {
                 toString() {
                     let t = "[";
                     if (ic.printRowMajor) {
                         t += "row-major:";
                         for (let e = 0; e < this.RANK; ++e)
@@ -9220,16 +9144,16 @@
                         handler: "onDrag"
                     },
                     panend: {
                         handler: "onDragEnd"
                     }
                 },
                 Lh = "draw",
-                kh = "mask",
-                Rh = Math.PI / 180,
+                Rh = "mask",
+                kh = Math.PI / 180,
                 Ih = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1],
                 jh = [0, 0, 0],
                 zh = {
                     unitsPerMeter: [1, 1, 1],
                     metersPerUnit: [1, 1, 1]
                 };
             class Fh {
@@ -9306,20 +9230,20 @@
                     width: n = 1,
                     height: i = 1
                 }) {
                     return t < this.x + this.width && this.x < t + n && e < this.y + this.height && this.y < e + i
                 }
                 getFrustumPlanes() {
                     return this._frustumPlanes.near || Object.assign(this._frustumPlanes, {
-                        left: kc((t = this.viewProjectionMatrix)[3] + t[0], t[7] + t[4], t[11] + t[8], t[15] + t[12]),
-                        right: kc(t[3] - t[0], t[7] - t[4], t[11] - t[8], t[15] - t[12]),
-                        bottom: kc(t[3] + t[1], t[7] + t[5], t[11] + t[9], t[15] + t[13]),
-                        top: kc(t[3] - t[1], t[7] - t[5], t[11] - t[9], t[15] - t[13]),
-                        near: kc(t[3] + t[2], t[7] + t[6], t[11] + t[10], t[15] + t[14]),
-                        far: kc(t[3] - t[2], t[7] - t[6], t[11] - t[10], t[15] - t[14])
+                        left: Rc((t = this.viewProjectionMatrix)[3] + t[0], t[7] + t[4], t[11] + t[8], t[15] + t[12]),
+                        right: Rc(t[3] - t[0], t[7] - t[4], t[11] - t[8], t[15] - t[12]),
+                        bottom: Rc(t[3] + t[1], t[7] + t[5], t[11] + t[9], t[15] + t[13]),
+                        top: Rc(t[3] - t[1], t[7] - t[5], t[11] - t[9], t[15] - t[13]),
+                        near: Rc(t[3] + t[2], t[7] + t[6], t[11] + t[10], t[15] + t[14]),
+                        far: Rc(t[3] - t[2], t[7] - t[6], t[11] - t[10], t[15] - t[14])
                     }), this._frustumPlanes;
                     var t
                 }
                 panByPosition(t, e) {
                     return null
                 }
                 _initProps(t) {
@@ -9395,15 +9319,15 @@
                             c[8] -= 2 * a / t, c[9] += 2 * l / e
                         }
                         return c
                     }({
                         width: this.width,
                         height: this.height,
                         orthographic: i,
-                        fovyRadians: r || s * Rh,
+                        fovyRadians: r || s * kh,
                         focalDistance: c,
                         padding: l,
                         near: o,
                         far: a
                     });
                     const h = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1];
                     var u;
@@ -9888,41 +9812,41 @@
             function Ou(t) {
                 return Cu(Au(t), "Invalid WebGLRenderingContext"), t
             }
 
             function Lu(t) {
                 return Cu(Mu(t), Tu), t
             }
-            const ku = {};
-            const Ru = function t(e) {
+            const Ru = {};
+            const ku = function t(e) {
                 const n = e.gl;
                 this.ext = e, this.isAlive = !0, this.hasBeenBound = !1, this.elementArrayBuffer = null, this.attribs = new Array(e.maxVertexAttribs);
                 for (let e = 0; e < this.attribs.length; e++) {
                     const i = new t.VertexAttrib(n);
                     this.attribs[e] = i
                 }
                 this.maxAttrib = 0
             };
-            (Ru.VertexAttrib = function(t) {
+            (ku.VertexAttrib = function(t) {
                 this.enabled = !1, this.buffer = null, this.size = 4, this.type = 5126, this.normalized = !1, this.stride = 16, this.offset = 0, this.cached = "", this.recache()
             }).prototype.recache = function() {
                 this.cached = [this.size, this.type, this.normalized, this.stride, this.offset].join(":")
             };
             const Iu = function(t) {
                 const e = this;
                 this.gl = t,
                     function(t) {
                         const e = t.getError;
                         t.getError = function() {
                             let n;
                             do {
-                                n = e.apply(t), 0 !== n && (ku[n] = !0)
+                                n = e.apply(t), 0 !== n && (Ru[n] = !0)
                             } while (0 !== n);
-                            for (n in ku)
-                                if (ku[n]) return delete ku[n], parseInt(n, 10);
+                            for (n in Ru)
+                                if (Ru[n]) return delete Ru[n], parseInt(n, 10);
                             return 0
                         }
                     }(t);
                 const n = this.original = {
                     getParameter: t.getParameter,
                     enableVertexAttribArray: t.enableVertexAttribArray,
                     disableVertexAttribArray: t.disableVertexAttribArray,
@@ -9974,25 +9898,25 @@
                     globalThis.console && globalThis.console.log && globalThis.console.log("OESVertexArrayObject emulation library context restored"), e.reset_()
                 }), !0), this.reset_()
             };
             Iu.prototype.VERTEX_ARRAY_BINDING_OES = 34229, Iu.prototype.reset_ = function() {
                 if (void 0 !== this.vertexArrayObjects)
                     for (let t = 0; t < this.vertexArrayObjects.length; ++t) this.vertexArrayObjects.isAlive = !1;
                 const t = this.gl;
-                this.maxVertexAttribs = t.getParameter(34921), this.defaultVertexArrayObject = new Ru(this), this.currentVertexArrayObject = null, this.currentArrayBuffer = null, this.vertexArrayObjects = [this.defaultVertexArrayObject], this.bindVertexArrayOES(null)
+                this.maxVertexAttribs = t.getParameter(34921), this.defaultVertexArrayObject = new ku(this), this.currentVertexArrayObject = null, this.currentArrayBuffer = null, this.vertexArrayObjects = [this.defaultVertexArrayObject], this.bindVertexArrayOES(null)
             }, Iu.prototype.createVertexArrayOES = function() {
-                const t = new Ru(this);
+                const t = new ku(this);
                 return this.vertexArrayObjects.push(t), t
             }, Iu.prototype.deleteVertexArrayOES = function(t) {
                 t.isAlive = !1, this.vertexArrayObjects.splice(this.vertexArrayObjects.indexOf(t), 1), this.currentVertexArrayObject === t && this.bindVertexArrayOES(null)
             }, Iu.prototype.isVertexArrayOES = function(t) {
-                return !!(t && t instanceof Ru && t.hasBeenBound && t.ext === this)
+                return !!(t && t instanceof ku && t.hasBeenBound && t.ext === this)
             }, Iu.prototype.bindVertexArrayOES = function(t) {
                 const e = this.gl;
-                if (t && !t.isAlive) return n = "bindVertexArrayOES: attempt to bind deleted arrayObject", ku[1282] = !0, void(void 0 !== n && (i = n, globalThis.console && globalThis.console.error && globalThis.console.error(i)));
+                if (t && !t.isAlive) return n = "bindVertexArrayOES: attempt to bind deleted arrayObject", Ru[1282] = !0, void(void 0 !== n && (i = n, globalThis.console && globalThis.console.error && globalThis.console.error(i)));
                 var n, i;
                 const r = this.original,
                     s = this.currentVertexArrayObject;
                 this.currentVertexArrayObject = t || this.defaultVertexArrayObject, this.currentVertexArrayObject.hasBeenBound = !0;
                 const o = this.currentVertexArrayObject;
                 if (s === o) return;
                 s && o.elementArrayBuffer === s.elementArrayBuffer || r.bindBuffer.call(e, 34963, o.elementArrayBuffer);
@@ -10774,15 +10698,15 @@
             function dd(t, e, n) {
                 return Math.min(Math.round(t * e), n - 1)
             }
 
             function pd(t, e, n, i) {
                 return i ? Math.max(0, n - 1 - Math.round(t * e)) : Math.min(Math.round(t * e), n - 1)
             }
-            const fd = Ro(),
+            const fd = ko(),
                 gd = fd && "undefined" != typeof document,
                 md = {
                     webgl2: !0,
                     webgl1: !0,
                     throwOnError: !0,
                     manageState: !0,
                     canvas: null,
@@ -10901,15 +10825,15 @@
 
             function Pd(t, e) {
                 e = Number(e);
                 for (const n in t)
                     if (t[n] === e) return "GL.".concat(n);
                 return String(e)
             }
-            globalThis.luma || (Ro() && Su.log(1, "luma.gl ".concat(yd, " - ").concat("set luma.log.level=1 (or higher) to trace rendering"))(), globalThis.luma = globalThis.luma || {
+            globalThis.luma || (ko() && Su.log(1, "luma.gl ".concat(yd, " - ").concat("set luma.log.level=1 (or higher) to trace rendering"))(), globalThis.luma = globalThis.luma || {
                 VERSION: yd,
                 version: yd,
                 log: Su,
                 stats: xd,
                 globals: {
                     modules: {},
                     nodeIO: {}
@@ -11075,17 +10999,17 @@
                 }
                 _doTrackDeallocatedMemory() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this[Symbol.toStringTag],
                         e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : xd.get("Memory Usage");
                     e.get("GPU Memory").subtractCount(this.byteLength), e.get("".concat(t, " Memory")).subtractCount(this.byteLength), this.byteLength = 0
                 }
             }
-            const kd = "Failed to deduce GL constant from typed array";
+            const Rd = "Failed to deduce GL constant from typed array";
 
-            function Rd(t) {
+            function kd(t) {
                 switch (ArrayBuffer.isView(t) ? t.constructor : t) {
                     case Float32Array:
                         return 5126;
                     case Uint16Array:
                         return 5123;
                     case Uint32Array:
                         return 5125;
@@ -11095,15 +11019,15 @@
                     case Int8Array:
                         return 5120;
                     case Int16Array:
                         return 5122;
                     case Int32Array:
                         return 5124;
                     default:
-                        throw new Error(kd)
+                        throw new Error(Rd)
                 }
             }
 
             function Id(t) {
                 let {
                     clamped: e = !0
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
@@ -11346,15 +11270,15 @@
                 }
                 _setData(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0,
                         n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : t.byteLength + e;
                     wd(ArrayBuffer.isView(t)), this._trackDeallocatedMemory();
                     const i = this._getTarget();
                     this.gl.bindBuffer(i, this.handle), this.gl.bufferData(i, n, this.usage), this.gl.bufferSubData(i, e, t), this.gl.bindBuffer(i, null), this.debugData = t.slice(0, 10), this.bytesUsed = n, this._trackAllocatedMemory(n);
-                    const r = Rd(t);
+                    const r = kd(t);
                     return wd(r), this.setAccessor(new Dd(this.accessor, {
                         type: r
                     })), this
                 }
                 _setByteLength(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.usage;
                     wd(t >= 0), this._trackDeallocatedMemory();
@@ -11370,15 +11294,15 @@
                     const e = t / Id(this.accessor.type || 5126, {
                         clamped: !1
                     }).BYTES_PER_ELEMENT;
                     return this.getElementCount() - e
                 }
                 _inferType(t) {
                     this.accessor.type || this.setAccessor(new Dd(this.accessor, {
-                        type: Rd(t)
+                        type: kd(t)
                     }))
                 }
                 _createHandle() {
                     return this.gl.createBuffer()
                 }
                 _deleteHandle() {
                     this.gl.deleteBuffer(this.handle), this._trackDeallocatedMemory()
@@ -12329,15 +12253,15 @@
                                 case 34836:
                                     return 4;
                                 default:
                                     return wd(!1), 0
                             }
                         }(n);
                     return new s(i * r * o)
-                }(o, c, r, a, l), c = c || Rd(o);
+                }(o, c, r, a, l), c = c || kd(o);
                 const g = d.bindFramebuffer(36160, p);
                 return d.readPixels(n, i, a, l, r, c, o), d.bindFramebuffer(36160, g || null), u && h.delete(), o
             }
 
             function lp(t) {
                 let {
                     sourceAttachment: e = 36064,
@@ -12877,41 +12801,41 @@
                 }
                 _bindHandle(t) {
                     return this.gl.bindFramebuffer(36160, t)
                 }
             }
             vp.ATTACHMENT_PARAMETERS = [36049, 36048, 33296, 33298, 33299, 33300, 33301, 33302, 33303];
             const bp = {
-                    5126: kp.bind(null, "uniform1fv", Pp, 1, Rp),
-                    35664: kp.bind(null, "uniform2fv", Pp, 2, Rp),
-                    35665: kp.bind(null, "uniform3fv", Pp, 3, Rp),
-                    35666: kp.bind(null, "uniform4fv", Pp, 4, Rp),
-                    5124: kp.bind(null, "uniform1iv", Sp, 1, Rp),
-                    35667: kp.bind(null, "uniform2iv", Sp, 2, Rp),
-                    35668: kp.bind(null, "uniform3iv", Sp, 3, Rp),
-                    35669: kp.bind(null, "uniform4iv", Sp, 4, Rp),
-                    35670: kp.bind(null, "uniform1iv", Sp, 1, Rp),
-                    35671: kp.bind(null, "uniform2iv", Sp, 2, Rp),
-                    35672: kp.bind(null, "uniform3iv", Sp, 3, Rp),
-                    35673: kp.bind(null, "uniform4iv", Sp, 4, Rp),
-                    35674: kp.bind(null, "uniformMatrix2fv", Pp, 4, Ip),
-                    35675: kp.bind(null, "uniformMatrix3fv", Pp, 9, Ip),
-                    35676: kp.bind(null, "uniformMatrix4fv", Pp, 16, Ip),
+                    5126: Rp.bind(null, "uniform1fv", Pp, 1, kp),
+                    35664: Rp.bind(null, "uniform2fv", Pp, 2, kp),
+                    35665: Rp.bind(null, "uniform3fv", Pp, 3, kp),
+                    35666: Rp.bind(null, "uniform4fv", Pp, 4, kp),
+                    5124: Rp.bind(null, "uniform1iv", Sp, 1, kp),
+                    35667: Rp.bind(null, "uniform2iv", Sp, 2, kp),
+                    35668: Rp.bind(null, "uniform3iv", Sp, 3, kp),
+                    35669: Rp.bind(null, "uniform4iv", Sp, 4, kp),
+                    35670: Rp.bind(null, "uniform1iv", Sp, 1, kp),
+                    35671: Rp.bind(null, "uniform2iv", Sp, 2, kp),
+                    35672: Rp.bind(null, "uniform3iv", Sp, 3, kp),
+                    35673: Rp.bind(null, "uniform4iv", Sp, 4, kp),
+                    35674: Rp.bind(null, "uniformMatrix2fv", Pp, 4, Ip),
+                    35675: Rp.bind(null, "uniformMatrix3fv", Pp, 9, Ip),
+                    35676: Rp.bind(null, "uniformMatrix4fv", Pp, 16, Ip),
                     35678: Lp,
                     35680: Lp,
-                    5125: kp.bind(null, "uniform1uiv", Cp, 1, Rp),
-                    36294: kp.bind(null, "uniform2uiv", Cp, 2, Rp),
-                    36295: kp.bind(null, "uniform3uiv", Cp, 3, Rp),
-                    36296: kp.bind(null, "uniform4uiv", Cp, 4, Rp),
-                    35685: kp.bind(null, "uniformMatrix2x3fv", Pp, 6, Ip),
-                    35686: kp.bind(null, "uniformMatrix2x4fv", Pp, 8, Ip),
-                    35687: kp.bind(null, "uniformMatrix3x2fv", Pp, 6, Ip),
-                    35688: kp.bind(null, "uniformMatrix3x4fv", Pp, 12, Ip),
-                    35689: kp.bind(null, "uniformMatrix4x2fv", Pp, 8, Ip),
-                    35690: kp.bind(null, "uniformMatrix4x3fv", Pp, 12, Ip),
+                    5125: Rp.bind(null, "uniform1uiv", Cp, 1, kp),
+                    36294: Rp.bind(null, "uniform2uiv", Cp, 2, kp),
+                    36295: Rp.bind(null, "uniform3uiv", Cp, 3, kp),
+                    36296: Rp.bind(null, "uniform4uiv", Cp, 4, kp),
+                    35685: Rp.bind(null, "uniformMatrix2x3fv", Pp, 6, Ip),
+                    35686: Rp.bind(null, "uniformMatrix2x4fv", Pp, 8, Ip),
+                    35687: Rp.bind(null, "uniformMatrix3x2fv", Pp, 6, Ip),
+                    35688: Rp.bind(null, "uniformMatrix3x4fv", Pp, 12, Ip),
+                    35689: Rp.bind(null, "uniformMatrix4x2fv", Pp, 8, Ip),
+                    35690: Rp.bind(null, "uniformMatrix4x3fv", Pp, 12, Ip),
                     35678: Lp,
                     35680: Lp,
                     35679: Lp,
                     35682: Lp,
                     36289: Lp,
                     36292: Lp,
                     36293: Lp,
@@ -12995,15 +12919,15 @@
                 let t = null;
                 return (e, n, i) => {
                     const r = t !== i;
                     return r && (e.uniform1i(n, i), t = i), r
                 }
             }
 
-            function kp(t, e, n, i) {
+            function Rp(t, e, n, i) {
                 let r = null,
                     s = null;
                 return (o, a, l) => {
                     const c = e(l, n),
                         h = c.length;
                     let u = !1;
                     if (null === r) r = new Float32Array(h), s = h, u = !0;
@@ -13015,15 +12939,15 @@
                                 break
                             }
                     }
                     return u && (i(o, t, a, c), r.set(c)), u
                 }
             }
 
-            function Rp(t, e, n, i) {
+            function kp(t, e, n, i) {
                 t[e](n, i)
             }
 
             function Ip(t, e, n, i) {
                 t[e](n, !1, i)
             }
 
@@ -14227,18 +14151,18 @@
                         type: this.ControllerType,
                         ...t
                     } : null
                 }
             }
             const Lf = Math.PI / 180;
 
-            function kf(t) {
+            function Rf(t) {
                 return 512 / 4003e4 / Math.cos(t * Lf)
             }
-            class Rf extends Fh {
+            class kf extends Fh {
                 constructor(t = {}) {
                     const {
                         latitude: e = 0,
                         longitude: n = 0,
                         zoom: i = 0,
                         pitch: r = 0,
                         bearing: s = 0,
@@ -14334,32 +14258,32 @@
                 }
                 get subViewports() {
                     if (this._subViewports && !this._subViewports.length) {
                         const t = this.getBounds(),
                             e = Math.floor((t[0] + 180) / 360),
                             n = Math.ceil((t[2] - 180) / 360);
                         for (let t = e; t <= n; t++) {
-                            const e = t ? new Rf({
+                            const e = t ? new kf({
                                 ...this,
                                 worldOffset: t
                             }) : this;
                             this._subViewports.push(e)
                         }
                     }
                     return this._subViewports
                 }
                 projectPosition(t) {
                     if (this._pseudoMeters) return super.projectPosition(t);
                     const [e, n] = this.projectFlat(t);
-                    return [e, n, (t[2] || 0) * kf(t[1])]
+                    return [e, n, (t[2] || 0) * Rf(t[1])]
                 }
                 unprojectPosition(t) {
                     if (this._pseudoMeters) return super.unprojectPosition(t);
                     const [e, n] = this.unprojectFlat(t);
-                    return [e, n, (t[2] || 0) / kf(n)]
+                    return [e, n, (t[2] || 0) / Rf(n)]
                 }
                 addMetersToLngLat(t, e) {
                     return yh(t, e)
                 }
                 panByPosition(t, e) {
                     const n = Eh(e, this.pixelUnprojectionMatrix),
                         i = Gc([], this.projectFlat(t), Wc([], n)),
@@ -14394,24 +14318,24 @@
                         zoom: o
                     } = Ph({
                         width: n,
                         height: i,
                         bounds: t,
                         ...e
                     });
-                    return new Rf({
+                    return new kf({
                         width: n,
                         height: i,
                         longitude: r,
                         latitude: s,
                         zoom: o
                     })
                 }
             }
-            wo(Rf, "displayName", "WebMercatorViewport");
+            wo(kf, "displayName", "WebMercatorViewport");
             class If {
                 constructor(t) {
                     wo(this, "_inProgress", void 0), wo(this, "_handle", void 0), wo(this, "_timeline", void 0), wo(this, "time", void 0), wo(this, "settings", void 0), this._inProgress = !1, this._handle = null, this._timeline = t, this.time = 0, this.settings = {
                         duration: 0
                     }
                 }
                 get inProgress() {
@@ -15425,15 +15349,15 @@
                         ...t,
                         ...this.state
                     }))
                 }
             }
             class eg extends Of {
                 get ViewportType() {
-                    return Rf
+                    return kf
                 }
                 get ControllerType() {
                     return tg
                 }
             }
             wo(eg, "displayName", "MapView");
             const ng = [255, 255, 255],
@@ -15973,15 +15897,15 @@
                     }, (() => super.render({
                         ...t,
                         target: this.fbo,
                         pass: "mask"
                     })))
                 }
                 shouldDrawLayer(t) {
-                    return t.props.operation === kh
+                    return t.props.operation === Rh
                 }
                 delete() {
                     this.fbo.delete(), this.maskMap.delete()
                 }
             }
             const Sg = (new Qc).lookAt({
                 eye: [0, 0, 1]
@@ -16366,30 +16290,30 @@
                     return Tg
                 }
                 get ControllerType() {
                     return Og
                 }
             }
             wo(Lg, "displayName", "OrthographicView");
-            class kg {
+            class Rg {
                 constructor() {
                     wo(this, "id", "mask-effect"), wo(this, "props", null), wo(this, "useInPicking", !0), wo(this, "dummyMaskMap", void 0), wo(this, "channels", []), wo(this, "masks", null), wo(this, "maskPass", void 0), wo(this, "maskMap", void 0), wo(this, "lastViewport", void 0)
                 }
                 preRender(t, {
                     layers: e,
                     layerFilter: n,
                     viewports: i,
                     onViewportActive: r,
                     views: s
                 }) {
                     this.dummyMaskMap || (this.dummyMaskMap = new Kd(t, {
                         width: 1,
                         height: 1
                     }));
-                    const o = e.filter((t => t.props.visible && t.props.operation === kh));
+                    const o = e.filter((t => t.props.visible && t.props.operation === Rh));
                     if (0 === o.length) return this.masks = null, void(this.channels.length = 0);
                     this.masks = {}, this.maskPass || (this.maskPass = new Pg(t, {
                         id: "default-mask"
                     }), this.maskMap = this.maskPass.maskMap);
                     const a = this._sortMaskChannels(o),
                         l = i[0],
                         c = !this.lastViewport || !this.lastViewport.equals(l);
@@ -16440,29 +16364,29 @@
                         } = this, a = function({
                             bounds: t,
                             viewport: e,
                             width: n,
                             height: i
                         }) {
                             if (t[2] <= t[0] || t[3] <= t[1]) return null;
-                            if (n -= 2, i -= 2, e instanceof Rf) {
+                            if (n -= 2, i -= 2, e instanceof kf) {
                                 const {
                                     longitude: e,
                                     latitude: r,
                                     zoom: s
                                 } = Ph({
                                     width: n,
                                     height: i,
                                     bounds: [
                                         [t[0], t[1]],
                                         [t[2], t[3]]
                                     ],
                                     maxZoom: 20
                                 });
-                                return new Rf({
+                                return new kf({
                                     longitude: e,
                                     latitude: r,
                                     zoom: s,
                                     x: 1,
                                     y: 1,
                                     width: n,
                                     height: i
@@ -16547,15 +16471,15 @@
                         maskChannels: this.masks
                     }
                 }
                 cleanup() {
                     this.dummyMaskMap && (this.dummyMaskMap.delete(), this.dummyMaskMap = void 0), this.maskPass && (this.maskPass.delete(), this.maskPass = void 0, this.maskMap = void 0), this.lastViewport = void 0, this.masks = null, this.channels.length = 0
                 }
             }
-            const Rg = new Eg;
+            const kg = new Eg;
             class Ig {
                 constructor() {
                     wo(this, "effects", void 0), wo(this, "_internalEffects", void 0), wo(this, "_needsRedraw", void 0), this.effects = [], this._internalEffects = [], this._needsRedraw = "Initial render", this.setEffects()
                 }
                 setProps(t) {
                     "effects" in t && (t.effects.length === this.effects.length && Pf(t.effects, this.effects) || (this.setEffects(t.effects), this._needsRedraw = "effects changed"))
                 }
@@ -16568,15 +16492,15 @@
                 getEffects() {
                     return this._internalEffects
                 }
                 finalize() {
                     this.cleanup()
                 }
                 setEffects(t = []) {
-                    this.cleanup(), this.effects = t, this._internalEffects = t.slice(), this._internalEffects.push(new kg), t.some((t => t instanceof Eg)) || this._internalEffects.push(Rg)
+                    this.cleanup(), this.effects = t, this._internalEffects = t.slice(), this._internalEffects.push(new Rg), t.some((t => t instanceof Eg)) || this._internalEffects.push(kg)
                 }
                 cleanup() {
                     for (const t of this.effects) t.cleanup();
                     for (const t of this._internalEffects) t.cleanup();
                     this.effects.length = 0, this._internalEffects.length = 0
                 }
             }
@@ -17518,15 +17442,15 @@
                     premultiplyAlpha: "none"
                 }
             }]]));
             const gm = globalThis.deck,
                 mm = globalThis;
 
             function vm(t) {
-                if (!t && !Ro()) return "Node";
+                if (!t && !ko()) return "Node";
                 if (Lo(t)) return "Electron";
                 const e = "undefined" != typeof navigator ? navigator : {},
                     n = t || e.userAgent || "";
                 if (n.indexOf("Edge") > -1) return "Edge";
                 const i = -1 !== n.indexOf("MSIE "),
                     r = -1 !== n.indexOf("Trident/");
                 return i || r ? "IE" : mm.chrome ? "Chrome" : mm.safari ? "Safari" : mm.mozInnerScreenX ? "Firefox" : "Unknown"
@@ -17601,15 +17525,15 @@
                 _createHandle() {
                     return bm.isSupported(this.gl) ? this.gl2.createQuery() : null
                 }
                 _deleteHandle() {
                     this.gl2.deleteQuery(this.handle)
                 }
             }
-            const ym = Ro() && "undefined" != typeof document;
+            const ym = ko() && "undefined" != typeof document;
             let _m = 0;
             class xm {
                 constructor() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         onCreateContext: e = (t => vd(t)),
                         onAddHTML: n = null,
@@ -17953,15 +17877,15 @@
                     mouseup: "pointerup"
                 },
                 Lm = {
                     KEY_EVENTS: ["keydown", "keyup"],
                     MOUSE_EVENTS: ["mousedown", "mousemove", "mouseup", "mouseover", "mouseout", "mouseleave"],
                     WHEEL_EVENTS: ["wheel", "mousewheel"]
                 },
-                km = {
+                Rm = {
                     tap: "tap",
                     anytap: "anytap",
                     doubletap: "doubletap",
                     press: "press",
                     pinch: "pinch",
                     pinchin: "pinch",
                     pinchout: "pinch",
@@ -17994,15 +17918,15 @@
                     pancancel: "pan",
                     swipe: "swipe",
                     swipeleft: "swipe",
                     swiperight: "swipe",
                     swipeup: "swipe",
                     swipedown: "swipe"
                 },
-                Rm = {
+                km = {
                     click: "tap",
                     anyclick: "anytap",
                     dblclick: "doubletap",
                     mousedown: "pointerdown",
                     mousemove: "pointermove",
                     mouseup: "pointerup",
                     mouseover: "pointerover",
@@ -18413,26 +18337,26 @@
                         n = e;
                         for (const e in t) this._addEventHandler(e, t[e], n, i, r);
                         return
                     }
                     const {
                         manager: s,
                         events: o
-                    } = this, a = Rm[t] || t;
+                    } = this, a = km[t] || t;
                     let l = o.get(a);
-                    l || (l = new sv(this), o.set(a, l), l.recognizerName = km[a] || a, s && s.on(a, l.handleEvent)), l.add(t, e, n, i, r), l.isEmpty() || this._toggleRecognizer(l.recognizerName, !0)
+                    l || (l = new sv(this), o.set(a, l), l.recognizerName = Rm[a] || a, s && s.on(a, l.handleEvent)), l.add(t, e, n, i, r), l.isEmpty() || this._toggleRecognizer(l.recognizerName, !0)
                 }
                 _removeEventHandler(t, e) {
                     if ("string" != typeof t) {
                         for (const e in t) this._removeEventHandler(e, t[e]);
                         return
                     }
                     const {
                         events: n
-                    } = this, i = Rm[t] || t, r = n.get(i);
+                    } = this, i = km[t] || t, r = n.get(i);
                     if (r && (r.remove(t, e), r.isEmpty())) {
                         const {
                             recognizerName: t
                         } = r;
                         let e = !1;
                         for (const i of n.values())
                             if (i.recognizerName === t && !i.isEmpty()) {
@@ -19400,15 +19324,15 @@
                     size: a,
                     getData: f
                 }), t.byteLength < m.byteLength + l && t.reallocate(m.byteLength + l), t.subData({
                     data: m,
                     offset: l
                 })
             }
-            class kv extends mv {
+            class Rv extends mv {
                 constructor(t, e) {
                     super(t, e, {
                         startIndices: null,
                         lastExternalBuffer: null,
                         binaryValue: null,
                         binaryAccessor: null,
                         needsUpdate: !0,
@@ -19641,16 +19565,16 @@
                             default:
                                 n = !1
                         }
                         if (!n) throw new Error("Illegal attribute generated for ".concat(this.id))
                     }
                 }
             }
-            const Rv = "out vec4 transform_output;\nvoid main() {\n  transform_output = vec4(0);\n}",
-                Iv = "#version 300 es\n".concat(Rv);
+            const kv = "out vec4 transform_output;\nvoid main() {\n  transform_output = vec4(0);\n}",
+                Iv = "#version 300 es\n".concat(kv);
 
             function jv(t, e) {
                 e = Array.isArray(e) ? e : [e];
                 const n = t.replace(/^\s+/, "").split(/\s+/),
                     [i, r, s] = n;
                 return e.includes(i) && r && s ? {
                     qualifier: i,
@@ -19663,15 +19587,15 @@
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                 const {
                     version: e = 100,
                     input: n,
                     inputType: i,
                     output: r
                 } = t;
-                if (!n) return 300 === e ? Iv : e > 300 ? "#version ".concat(e, "\n").concat(Rv) : "void main() {gl_FragColor = vec4(0);}";
+                if (!n) return 300 === e ? Iv : e > 300 ? "#version ".concat(e, "\n").concat(kv) : "void main() {gl_FragColor = vec4(0);}";
                 const s = function(t, e) {
                     switch (e) {
                         case "float":
                             return "vec4(".concat(t, ", 0.0, 0.0, 1.0)");
                         case "vec2":
                             return "vec4(".concat(t, ", 0.0, 1.0)");
                         case "vec3":
@@ -21349,15 +21273,15 @@
             const cb = {
                 interpolation: class {
                     constructor({
                         gl: t,
                         attribute: e,
                         timeline: n
                     }) {
-                        wo(this, "gl", void 0), wo(this, "type", "interpolation"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.transition = new If(n), this.attribute = e, this.attributeInTransition = new kv(t, e.settings), this.currentStartIndices = e.startIndices, this.currentLength = 0, this.transform = function(t, e) {
+                        wo(this, "gl", void 0), wo(this, "type", "interpolation"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.transition = new If(n), this.attribute = e, this.attributeInTransition = new Rv(t, e.settings), this.currentStartIndices = e.startIndices, this.currentLength = 0, this.transform = function(t, e) {
                             const n = Av(e.size);
                             return new lb(t, {
                                 vs: "\n#define SHADER_NAME interpolation-transition-vertex-shader\n\nuniform float time;\nattribute ATTRIBUTE_TYPE aFrom;\nattribute ATTRIBUTE_TYPE aTo;\nvarying ATTRIBUTE_TYPE vCurrent;\n\nvoid main(void) {\n  vCurrent = mix(aFrom, aTo, time);\n  gl_Position = vec4(0.0);\n}\n",
                                 defines: {
                                     ATTRIBUTE_TYPE: n
                                 },
                                 varyings: ["vCurrent"]
@@ -21432,15 +21356,15 @@
                 },
                 spring: class {
                     constructor({
                         gl: t,
                         attribute: e,
                         timeline: n
                     }) {
-                        wo(this, "gl", void 0), wo(this, "type", "spring"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "texture", void 0), wo(this, "framebuffer", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.type = "spring", this.transition = new If(n), this.attribute = e, this.attributeInTransition = new kv(t, {
+                        wo(this, "gl", void 0), wo(this, "type", "spring"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "texture", void 0), wo(this, "framebuffer", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.type = "spring", this.transition = new If(n), this.attribute = e, this.attributeInTransition = new Rv(t, {
                             ...e.settings,
                             normalized: !1
                         }), this.currentStartIndices = e.startIndices, this.currentLength = 0, this.texture = function(t) {
                             return new Kd(t, {
                                 data: new Uint8Array(4),
                                 format: 6408,
                                 type: 5121,
@@ -21727,15 +21651,15 @@
                 _createAttribute(t, e, n) {
                     const i = {
                         ...e,
                         id: t,
                         size: (e.isIndexed ? 1 : e.size) || 1,
                         divisor: n.instanced ? 1 : e.divisor || 0
                     };
-                    return new kv(this.gl, i)
+                    return new Rv(this.gl, i)
                 }
                 _mapUpdateTriggersToAttributes() {
                     const t = {};
                     for (const e in this.attributes) this.attributes[e].getUpdateTriggers().forEach((n => {
                         t[n] || (t[n] = []), t[n].push(e)
                     }));
                     this.updateTriggers = t
@@ -21962,15 +21886,15 @@
                         n.inject = i
                     } else n.inject = e.inject;
                 return n
             }
 
             function Sb(t, e, n = !1) {
                 const i = e.projectPosition(t);
-                if (n && e instanceof Rf) {
+                if (n && e instanceof kf) {
                     const [n, r, s = 0] = t, o = e.getDistanceScales([n, r]);
                     i[2] = s * o.unitsPerMeter[2]
                 }
                 return i
             }
 
             function Cb(t, {
@@ -22005,26 +21929,26 @@
                         validate: (t, e) => !0,
                         equal: (t, e, n) => Boolean(t) === Boolean(e)
                     },
                     number: {
                         validate: (t, e) => Number.isFinite(t) && (!("max" in e) || t <= e.max) && (!("min" in e) || t >= e.min)
                     },
                     color: {
-                        validate: (t, e) => e.optional && !t || Rb(t) && (3 === t.length || 4 === t.length),
+                        validate: (t, e) => e.optional && !t || kb(t) && (3 === t.length || 4 === t.length),
                         equal: (t, e, n) => Ob(t, e)
                     },
                     accessor: {
                         validate(t, e) {
                             const n = Ib(t);
                             return "function" === n || n === Ib(e.value)
                         },
                         equal: (t, e, n) => "function" == typeof e || Ob(t, e)
                     },
                     array: {
-                        validate: (t, e) => e.optional && !t || Rb(t),
+                        validate: (t, e) => e.optional && !t || kb(t),
                         equal: (t, e, n) => n.compare ? Ob(t, e) : t === e
                     },
                     object: {
                         equal: (t, e, n) => n.compare ? Pf(t, e) : t === e
                     },
                     function: {
                         validate: (t, e) => e.optional && !t || "function" == typeof t,
@@ -22065,56 +21989,56 @@
                             (e = t) && e instanceof Kd && Ab[e.id] && (e.delete(), delete Ab[e.id])
                         }
                     }
                 };
 
             function Ob(t, e) {
                 if (t === e) return !0;
-                if (!Rb(t) || !Rb(e)) return !1;
+                if (!kb(t) || !kb(e)) return !1;
                 const n = t.length;
                 if (n !== e.length) return !1;
                 for (let i = 0; i < n; i++)
                     if (t[i] !== e[i]) return !1;
                 return !0
             }
 
             function Lb(t, e) {
                 switch (Ib(e)) {
                     case "object":
-                        return kb(t, e);
+                        return Rb(t, e);
                     case "array":
-                        return kb(t, {
+                        return Rb(t, {
                             type: "array",
                             value: e,
                             compare: !1
                         });
                     case "boolean":
-                        return kb(t, {
+                        return Rb(t, {
                             type: "boolean",
                             value: e
                         });
                     case "number":
-                        return kb(t, {
+                        return Rb(t, {
                             type: "number",
                             value: e
                         });
                     case "function":
-                        return kb(t, {
+                        return Rb(t, {
                             type: "function",
                             value: e,
                             compare: !0
                         });
                     default:
                         return {
                             name: t, type: "unknown", value: e
                         }
                 }
             }
 
-            function kb(t, e) {
+            function Rb(t, e) {
                 return "type" in e ? {
                     name: t,
                     ...Mb[e.type],
                     ...e
                 } : "value" in e ? {
                     name: t,
                     type: Ib(e.value),
@@ -22122,20 +22046,20 @@
                 } : {
                     name: t,
                     type: "object",
                     value: e
                 }
             }
 
-            function Rb(t) {
+            function kb(t) {
                 return Array.isArray(t) || ArrayBuffer.isView(t)
             }
 
             function Ib(t) {
-                return Rb(t) ? "array" : null === t ? "null" : typeof t
+                return kb(t) ? "array" : null === t ? "null" : typeof t
             }
 
             function jb(t) {
                 return Bb(t, "_mergedDefaultProps") || (function(t) {
                     if (!t.prototype) return;
                     const e = Object.getPrototypeOf(t),
                         n = jb(e),
@@ -23984,24 +23908,24 @@
                 for (let o = n + 1; o < i; o += e) {
                     const e = Math.abs(t[o]);
                     e > r && (r = e, s = o - 1)
                 }
                 return s
             }
 
-            function ky(t, e, n, i, r = 85.051129) {
+            function Ry(t, e, n, i, r = 85.051129) {
                 const s = t[n],
                     o = t[i - e];
                 if (Math.abs(s - o) > 180) {
                     const i = wy(t, 0, e, n);
                     i[0] += 360 * Math.round((o - s) / 360), _y(t, i), i[1] = Math.sign(i[1]) * r, _y(t, i), i[0] = s, _y(t, i)
                 }
             }
 
-            function Ry(t, e, n, i) {
+            function ky(t, e, n, i) {
                 let r, s = t[0];
                 for (let o = n; o < i; o += e) {
                     r = t[o];
                     const e = r - s;
                     (e > 180 || e < -180) && (r -= 360 * Math.round(e / 360)), t[o] = s = r
                 }
             }
@@ -24251,15 +24175,15 @@
                                 c = 0;
                             for (let r = 0; r <= e.length; r++) {
                                 const s = e[r] || t.length,
                                     h = c,
                                     u = Ly(t, i, l, s);
                                 for (let e = u; e < s; e++) o[c++] = t[e];
                                 for (let e = l; e < u; e++) o[c++] = t[e];
-                                Ry(o, i, h, c), ky(o, i, h, c, null == n ? void 0 : n.maxLatitude), l = s, a[r] = c
+                                ky(o, i, h, c), Ry(o, i, h, c, null == n ? void 0 : n.maxLatitude), l = s, a[r] = c
                             }
                             a.pop();
                             const h = Cy(o, a, {
                                 size: i,
                                 gridResolution: 360,
                                 gridOffset: [-180, -180],
                                 edgeTypes: s
@@ -24714,15 +24638,15 @@
                         }) : i ? function(t, e) {
                             const {
                                 size: n = 2,
                                 startIndex: i = 0,
                                 endIndex: r = t.length,
                                 normalize: s = !0
                             } = e || {}, o = t.slice(i, r);
-                            Ry(o, n, 0, r - i);
+                            ky(o, n, 0, r - i);
                             const a = Ey(o, {
                                 size: n,
                                 broken: !0,
                                 gridResolution: 360,
                                 gridOffset: [-180, -180]
                             });
                             if (s)
@@ -26074,17 +25998,17 @@
                 fontSize: 64,
                 buffer: 4,
                 sdf: !1,
                 cutoff: .25,
                 radius: 12,
                 smoothing: .1
             };
-            let k_ = new O_(3);
+            let R_ = new O_(3);
 
-            function R_(t, e) {
+            function k_(t, e) {
                 for (let n = 0; n < t.length; n++) e.data[4 * n + 3] = t[n]
             }
 
             function I_(t, e, n, i) {
                 t.font = "".concat(i, " ").concat(n, "px ").concat(e), t.fillStyle = "#000", t.textBaseline = "alphabetic", t.textAlign = "left"
             }
             class j_ {
@@ -26105,23 +26029,23 @@
                 setProps(t = {}) {
                     Object.assign(this.props, t);
                     const e = this._key;
                     this._key = this._getKey();
                     const n = function(t, e) {
                             let n;
                             n = "string" == typeof e ? new Set(Array.from(e)) : new Set(e);
-                            const i = k_.get(t);
+                            const i = R_.get(t);
                             if (!i) return n;
                             for (const t in i.mapping) n.has(t) && n.delete(t);
                             return n
                         }(this._key, this.props.characterSet),
-                        i = k_.get(this._key);
+                        i = R_.get(this._key);
                     if (i && 0 === n.size) return void(this._key !== e && (this._atlas = i));
                     const r = this._generateFontAtlas(this._key, n, i);
-                    this._atlas = r, k_.set(this._key, r)
+                    this._atlas = r, R_.set(this._key, r)
                 }
                 _generateFontAtlas(t, e, n) {
                     const {
                         fontFamily: i,
                         fontWeight: r,
                         fontSize: s,
                         buffer: o,
@@ -26182,15 +26106,15 @@
                     if (h.height !== p) {
                         const t = u.getImageData(0, 0, h.width, h.height);
                         h.height = p, u.putImageData(t, 0, 0)
                     }
                     if (I_(u, i, s, r), a) {
                         const t = new(w_())(s, o, l, c, i, r),
                             n = u.getImageData(0, 0, t.size, t.size);
-                        for (const i of e) R_(t.draw(i), n), u.putImageData(n, d[i].x - o, d[i].y + o)
+                        for (const i of e) k_(t.draw(i), n), u.putImageData(n, d[i].x - o, d[i].y + o)
                     } else
                         for (const t of e) u.fillText(t, d[t].x, d[t].y + .9 * s);
                     return {
                         xOffset: f,
                         yOffset: g,
                         mapping: d,
                         data: h,
@@ -26758,15 +26682,15 @@
                         numInstances: e,
                         getIconOffsets: this.getIconOffsets,
                         getIcon: n
                     })]
                 }
                 static set fontAtlasCacheLimit(t) {
                     ! function(t) {
-                        ta.assert(Number.isFinite(t) && t >= 3, "Invalid cache limit"), k_ = new O_(t)
+                        ta.assert(Number.isFinite(t) && t >= 3, "Invalid cache limit"), R_ = new O_(t)
                     }(t)
                 }
             }
             wo(U_, "defaultProps", V_), wo(U_, "layerName", "TextLayer");
             const G_ = {
                     circle: {
                         type: b_,
@@ -27854,16 +27778,16 @@
                     o = e[3],
                     a = n[0],
                     l = n[1],
                     c = n[2],
                     h = n[3];
                 return t[0] = i * h + o * a + r * c - s * l, t[1] = r * h + o * l + s * a - i * c, t[2] = s * h + o * c + i * l - r * a, t[3] = o * h - i * a - r * l - s * c, t
             }
-            var Ax, Mx, Ox, Lx, kx = Zc,
-                Rx = function(t) {
+            var Ax, Mx, Ox, Lx, Rx = Zc,
+                kx = function(t) {
                     var e = t[0],
                         n = t[1],
                         i = t[2],
                         r = t[3];
                     return Math.hypot(e, n, i, r)
                 },
                 Ix = function(t) {
@@ -27953,15 +27877,15 @@
                 get w() {
                     return this[3]
                 }
                 set w(t) {
                     this[3] = hc(t)
                 }
                 len() {
-                    return Rx(this)
+                    return kx(this)
                 }
                 lengthSquared() {
                     return Ix(this)
                 }
                 dot(t) {
                     return function(t, e) {
                         return t[0] * e[0] + t[1] * e[1] + t[2] * e[2] + t[3] * e[3]
@@ -28052,15 +27976,15 @@
                             o = e[3],
                             a = Math.sin(n),
                             l = Math.cos(n);
                         t[0] = i * l + r * a, t[1] = r * l - i * a, t[2] = s * l + o * a, t[3] = o * l - s * a
                     }(this, this, t), this.check()
                 }
                 scale(t) {
-                    return kx(this, this, t), this.check()
+                    return Rx(this, this, t), this.check()
                 }
                 slerp(t, e, n) {
                     let i, r, s;
                     switch (arguments.length) {
                         case 1:
                             ({
                                 start: i = zx,
@@ -28628,15 +28552,15 @@
                             normal: t,
                             distance: e
                         }) => new Xx(t.clone().negate(), e))),
                         o = new Jx(s),
                         a = t.distanceScales.unitsPerMeter[2],
                         l = n && n[0] * a || 0,
                         c = n && n[1] * a || 0,
-                        h = t instanceof Rf && t.pitch <= 60 ? e : 0;
+                        h = t instanceof kf && t.pitch <= 60 ? e : 0;
                     if (i) {
                         const [t, e, n, r] = i, s = mh([t, r]), o = mh([n, e]);
                         i = [s[0], mw - s[1], o[0], mw - o[1]]
                     }
                     const u = new _w(0, 0, 0),
                         d = {
                             viewport: t,
@@ -28644,15 +28568,15 @@
                             cullingVolume: o,
                             elevationBounds: [l, c],
                             minZ: h,
                             maxZ: e,
                             bounds: i,
                             offset: 0
                         };
-                    if (u.update(d), t instanceof Rf && t.subViewports && t.subViewports.length > 1) {
+                    if (u.update(d), t instanceof kf && t.subViewports && t.subViewports.length > 1) {
                         for (d.offset = -1; u.update(d) && !(--d.offset < -3););
                         for (d.offset = 1; u.update(d) && !(++d.offset > 3););
                     }
                     return u.getSelected()
                 }(t, c, i, r) : function(t, e, n, i, r) {
                     const s = function(t, e, n) {
                             let i;
@@ -28668,26 +28592,26 @@
                             x: t,
                             y: n,
                             z: e
                         });
                     return u
                 }(t, c, s, h || ww, a)
             }
-            var Lw = n(4155);
+            var Lw = n(46);
 
-            function kw() {
+            function Rw() {
                 let t;
                 if ("undefined" != typeof window && window.performance) t = window.performance.now();
                 else if (void 0 !== Lw && Lw.hrtime) {
                     const e = Lw.hrtime();
                     t = 1e3 * e[0] + e[1] / 1e6
                 } else t = Date.now();
                 return t
             }
-            class Rw {
+            class kw {
                 constructor(t, e) {
                     this.name = void 0, this.type = void 0, this.sampleSize = 1, this.time = 0, this.count = 0, this.samples = 0, this.lastTiming = 0, this.lastSampleTime = 0, this.lastSampleCount = 0, this._count = 0, this._time = 0, this._samples = 0, this._startTime = 0, this._timerPending = !1, this.name = t, this.type = e, this.reset()
                 }
                 reset() {
                     return this.time = 0, this.count = 0, this.samples = 0, this.lastTiming = 0, this.lastSampleTime = 0, this.lastSampleCount = 0, this._count = 0, this._time = 0, this._samples = 0, this._startTime = 0, this._timerPending = !1, this
                 }
                 setSampleSize(t) {
@@ -28705,18 +28629,18 @@
                 subtractCount(t) {
                     return this._count -= t, this._samples++, this._checkSampling(), this
                 }
                 addTime(t) {
                     return this._time += t, this.lastTiming = t, this._samples++, this._checkSampling(), this
                 }
                 timeStart() {
-                    return this._startTime = kw(), this._timerPending = !0, this
+                    return this._startTime = Rw(), this._timerPending = !0, this
                 }
                 timeEnd() {
-                    return this._timerPending ? (this.addTime(kw() - this._startTime), this._timerPending = !1, this._checkSampling(), this) : this
+                    return this._timerPending ? (this.addTime(Rw() - this._startTime), this._timerPending = !1, this._checkSampling(), this) : this
                 }
                 getSampleAverageCount() {
                     return this.sampleSize > 0 ? this.lastSampleCount / this.sampleSize : 0
                 }
                 getSampleAverageTime() {
                     return this.sampleSize > 0 ? this.lastSampleTime / this.sampleSize : 0
                 }
@@ -28773,15 +28697,15 @@
                 }
                 _getOrCreate(t) {
                     const {
                         name: e,
                         type: n
                     } = t;
                     let i = this.stats[e];
-                    return i || (i = t instanceof Rw ? t : new Rw(e, n), this.stats[e] = i), i
+                    return i || (i = t instanceof kw ? t : new kw(e, n), this.stats[e] = i), i
                 }
             }
             const jw = {
                 id: "request-scheduler",
                 throttleRequests: !0,
                 maxRequests: 6
             };
@@ -30342,28 +30266,155 @@
                 render() {
                     return this.state.error && this.props.errorState ? this.props.errorState(this.state.error) : this.props.children
                 }
             }
             var dE = uE,
                 pE = t => {
                     let e;
-                    e = "string" == typeof t.rootElement ? document.getElementById(t.rootElement) : t.rootElement, l().render((0, o.jsx)(dE, {
+                    e = "string" == typeof t.rootElement ? document.getElementById(t.rootElement) : t.rootElement, l.version.startsWith("18.") ? a.createRoot(e).render((0, o.jsx)(dE, {
+                        errorHandler: t.onError,
+                        children: (0, o.jsx)(hE, {
+                            apiKey: t.apiKey,
+                            groupID: t.groupID,
+                            baseGroup: t.baseGroup,
+                            namespace: t.namespace,
+                            onError: t.onError,
+                            basePath: t.basePath,
+                            onLoad: t.onLoad
+                        })
+                    })) : (0, l.render)((0, o.jsx)(dE, {
                         errorHandler: t.onError,
                         children: (0, o.jsx)(hE, {
                             apiKey: t.apiKey,
                             groupID: t.groupID,
                             baseGroup: t.baseGroup,
                             namespace: t.namespace,
                             onError: t.onError,
                             basePath: t.basePath,
                             onLoad: t.onLoad
                         })
                     }), e)
                 }
         },
+        9367: (t, e, n) => {
+            "use strict";
+            var i, r = Object.assign || function(t) {
+                    for (var e = 1; e < arguments.length; e++) {
+                        var n = arguments[e];
+                        for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
+                    }
+                    return t
+                },
+                s = (i = n(6271)) && i.__esModule ? i : {
+                    default: i
+                };
+            e.Z = function(t) {
+                var e = t.fill,
+                    n = void 0 === e ? "currentColor" : e,
+                    i = t.width,
+                    o = void 0 === i ? 24 : i,
+                    a = t.height,
+                    l = void 0 === a ? 24 : a,
+                    c = t.style,
+                    h = void 0 === c ? {} : c,
+                    u = function(t, e) {
+                        var n = {};
+                        for (var i in t) e.indexOf(i) >= 0 || Object.prototype.hasOwnProperty.call(t, i) && (n[i] = t[i]);
+                        return n
+                    }(t, ["fill", "width", "height", "style"]);
+                return s.default.createElement("svg", r({
+                    viewBox: "0 0 24 24",
+                    style: r({
+                        fill: n,
+                        width: o,
+                        height: l
+                    }, h)
+                }, u), s.default.createElement("path", {
+                    d: "M21,7L9,19L3.5,13.5L4.91,12.09L9,16.17L19.59,5.59L21,7Z"
+                }))
+            }
+        },
+        746: (t, e, n) => {
+            "use strict";
+            var i, r = Object.assign || function(t) {
+                    for (var e = 1; e < arguments.length; e++) {
+                        var n = arguments[e];
+                        for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
+                    }
+                    return t
+                },
+                s = (i = n(6271)) && i.__esModule ? i : {
+                    default: i
+                };
+            e.Z = function(t) {
+                var e = t.fill,
+                    n = void 0 === e ? "currentColor" : e,
+                    i = t.width,
+                    o = void 0 === i ? 24 : i,
+                    a = t.height,
+                    l = void 0 === a ? 24 : a,
+                    c = t.style,
+                    h = void 0 === c ? {} : c,
+                    u = function(t, e) {
+                        var n = {};
+                        for (var i in t) e.indexOf(i) >= 0 || Object.prototype.hasOwnProperty.call(t, i) && (n[i] = t[i]);
+                        return n
+                    }(t, ["fill", "width", "height", "style"]);
+                return s.default.createElement("svg", r({
+                    viewBox: "0 0 24 24",
+                    style: r({
+                        fill: n,
+                        width: o,
+                        height: l
+                    }, h)
+                }, u), s.default.createElement("path", {
+                    d: "M12,18.17L8.83,15L7.42,16.41L12,21L16.59,16.41L15.17,15M12,5.83L15.17,9L16.58,7.59L12,3L7.41,7.59L8.83,9L12,5.83Z"
+                }))
+            }
+        },
+        2700: (t, e, n) => {
+            "use strict";
+            var i = n(4456);
+            e.createRoot = i.createRoot, e.hydrateRoot = i.hydrateRoot
+        },
+        1217: (t, e, n) => {
+            "use strict";
+            var i = n(6271),
+                r = Symbol.for("react.element"),
+                s = (Symbol.for("react.fragment"), Object.prototype.hasOwnProperty),
+                o = i.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED.ReactCurrentOwner,
+                a = {
+                    key: !0,
+                    ref: !0,
+                    __self: !0,
+                    __source: !0
+                };
+
+            function l(t, e, n) {
+                var i, l = {},
+                    c = null,
+                    h = null;
+                for (i in void 0 !== n && (c = "" + n), void 0 !== e.key && (c = "" + e.key), void 0 !== e.ref && (h = e.ref), e) s.call(e, i) && !a.hasOwnProperty(i) && (l[i] = e[i]);
+                if (t && t.defaultProps)
+                    for (i in e = t.defaultProps) void 0 === l[i] && (l[i] = e[i]);
+                return {
+                    $$typeof: r,
+                    type: t,
+                    key: c,
+                    ref: h,
+                    props: l,
+                    _owner: o.current
+                }
+            }
+            e.jsx = l, e.jsxs = l
+        },
+        9336: (t, e, n) => {
+            "use strict";
+            t.exports = n(1217)
+        },
         4272: (t, e, n) => {
             "use strict";
             n.d(e, {
                 Z: () => u
             });
             var i = n(3645),
                 r = n.n(i),
@@ -30371,15 +30422,15 @@
                 o = n.n(s),
                 a = n(6362),
                 l = n.n(a),
                 c = r()((function(t) {
                     return t[1]
                 })),
                 h = o()(l());
-            c.push([t.id, '.BioImageViewer-Slider {\n  width: 320px;\n  background: #f8fafb;\n  border-radius: 12px;\n  padding: 12px 12px 20px;\n  font-family: Inter, Arial, "sans-serif";\n}\n\n.BioImageViewer-Slider__text {\n  color: #000;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 14px;\n  font-weight: 600;\n  line-height: 20px;\n}\n\n.BioImageViewer-Slider__text--light {\n  color: #000000b3;\n}\n\n.BioImageViewer-Slider__icon {\n  width: 16px;\n}\n\n.BioImageViewer-Slider__colorpicker {\n  width: 16px;\n  height: 16px;\n  border: 2px solid #fff;\n  border-radius: 50%;\n  margin-right: 12px;\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-Slider__colorpicker-backdrop {\n  position: fixed;\n  inset: 0;\n}\n\n.BioImageViewer-Slider__colorpicker-container {\n  z-index: 2;\n  position: absolute;\n}\n\n.BioImageViewer-Slider__main {\n  justify-content: space-between;\n  display: flex;\n}\n\n.BioImageViewer-Slider__left, .BioImageViewer-Slider__info {\n  align-items: center;\n  display: flex;\n}\n\n.BioImageViewer-Slider__icon-wrapper {\n  margin-left: 6px;\n  margin-right: 14px;\n}\n\n.BioImageViewer-Slider__value {\n  color: #000000de;\n  background: #fff;\n  border: 1px solid #cfd6de;\n  border-radius: 6px;\n  padding: 6px 16px;\n  font-size: 14px;\n  font-style: normal;\n  font-weight: 400;\n  line-height: 20px;\n}\n\n.BioImageViewer-Slider__range {\n  width: 100%;\n}\n\n.BioImageViewer-ControlPanel {\n  background: #fff;\n  border-radius: 12px;\n  margin-bottom: 16px;\n  padding: 26px 16px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-ControlPanel__title {\n  align-items: center;\n  margin: 0 0 26px;\n  font-size: 16px;\n  font-style: normal;\n  font-weight: 700;\n  line-height: 24px;\n  display: flex;\n}\n\n.BioImageViewer-ControlPanel__title svg {\n  margin-right: 10px;\n}\n\n.BioImageViewer-ControlPanel__list {\n  padding-left: 0;\n  list-style: none;\n}\n\n.BioImageViewer-ControlPanel__item {\n  margin-bottom: 8px;\n}\n\n.BioImageViewer-AttributePanel {\n  background: #fff;\n  border-radius: 12px;\n  margin-bottom: 16px;\n  padding: 26px 16px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-AttributePanel__title {\n  align-items: center;\n  margin: 0 0 16px;\n  font-size: 16px;\n  font-style: normal;\n  font-weight: 700;\n  line-height: 24px;\n  display: flex;\n}\n\n.BioImageViewer-AttributePanel__item {\n  flex-direction: row;\n  align-items: center;\n  display: flex;\n}\n\n.BioImageViewer-AttributePanel__radio {\n  margin: 0;\n}\n\n.BioImageViewer-AttributePanel__label {\n  margin: 6px;\n}\n\n.BIV-ZoomControls {\n  z-index: 1;\n  background-color: #fff;\n  border-radius: 8px;\n  align-items: center;\n  gap: 8px;\n  padding: 4px;\n  display: flex;\n  position: absolute;\n  top: 16px;\n  right: 16px;\n  box-shadow: 0 1px 3px #d1d5d7;\n}\n\n.BIV-ZoomControls__label {\n  color: #000000b3;\n  width: 56px;\n  text-align: center;\n  margin: 0;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 12px;\n  font-weight: 600;\n  line-height: 20px;\n}\n\n.BIV-ZoomControls__button {\n  width: 28px;\n  height: 28px;\n  background: no-repeat;\n  border: none;\n  padding: 0;\n}\n\n.BIV-ZoomControls__button:hover {\n  cursor: pointer;\n}\n\n.BIV-Tooltip {\n  position: relative;\n}\n\n.BIV-Tooltip:hover .BIV-Tooltip__content {\n  opacity: 1;\n}\n\n.BIV-Tooltip__content {\n  color: #fff;\n  opacity: 0;\n  white-space: nowrap;\n  background-color: #333f55;\n  border-radius: 4px;\n  padding: 8px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 12px;\n  font-weight: 600;\n  line-height: 20px;\n  transition: opacity .2s ease-in-out;\n  position: absolute;\n  bottom: -54px;\n  left: 50%;\n  transform: translateX(-50%);\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BIV-Tooltip__content:before {\n  content: "";\n  width: 0;\n  height: 0;\n  border: 10px solid #0000;\n  border-top: 0;\n  border-bottom-color: #333f55;\n  position: absolute;\n  top: -10px;\n  left: 50%;\n  transform: translateX(-50%);\n}\n\n.BioImageViewer-Viewer__minimap {\n  width: 100%;\n  height: 100%;\n  position: absolute;\n  box-shadow: 0 0 8px 2px #00000073;\n}\n\n.BioImageViewer__container {\n  position: relative;\n}\n\n.BioImageViewer__container #deckgl-wrapper {\n  background-image: url(' + h + ');\n  background-size: 50px;\n}\n\n.BioImageViewer__main {\n  height: 100vh;\n}\n\n.BioImageViewer__controls {\n  z-index: 1;\n  max-height: 80vh;\n  padding: 6px;\n  position: absolute;\n  top: 68px;\n  right: 16px;\n  overflow-y: auto;\n}\n\n.BioImageViewer__minimap {\n  width: 160px;\n  height: 90px;\n  border: 1px solid gray;\n  position: absolute;\n  top: 20px;\n  left: 20px;\n}\n\n.BioImageViewer__scalebar {\n  width: calc(var(--scalebar-length) * 1px);\n  height: 10px;\n  box-sizing: border-box;\n  background: linear-gradient(to right, #fff 50%, #000 50%);\n  border: 1px solid #000;\n  position: absolute;\n  bottom: 60px;\n  left: 20px;\n}\n\n.BioImageViewer__scalebar__text {\n  width: calc(var(--scalebar-length) * 1px);\n  height: 15px;\n  box-sizing: border-box;\n  text-align: center;\n  margin: 0;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 14px;\n  font-weight: 500;\n  position: absolute;\n  top: 10px;\n  left: -1px;\n}\n\n.BioImageViewer-GroupSelector {\n  background: #fff;\n  border-radius: 12px;\n  flex-direction: column;\n  margin-bottom: 16px;\n  padding: 26px 16px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  display: flex;\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-GroupSelector__title {\n  align-items: center;\n  margin: 0 0 26px;\n  font-size: 16px;\n  font-style: normal;\n  font-weight: 700;\n  line-height: 24px;\n  display: flex;\n}\n\n.BioImageViewer-GroupSelector__title svg {\n  margin-right: 10px;\n}\n\n.BioImageViewer-GroupSelector__controls {\n  justify-content: space-between;\n  align-items: center;\n  margin: 6px;\n  display: flex;\n}\n\n.BioImageViewer-GroupSelector__list {\n  padding-left: 0;\n  list-style: none;\n}\n\n.BioImageViewer-GroupSelector__value {\n  color: #000000de;\n  background: #fff;\n  border: 1px solid #cfd6de;\n  border-radius: 6px;\n  padding: 6px 16px;\n  font-size: 14px;\n  font-style: normal;\n  font-weight: 400;\n  line-height: 20px;\n}\n\n.BioImageViewer-GroupSelector__item {\n  cursor: pointer;\n  border-radius: 12px;\n  margin-bottom: 12px;\n  padding: 8px;\n  font-size: 14px;\n}\n\n.BioImageViewer-GroupSelector__item:hover {\n  background-color: #0000ff26;\n}\n\n.BioImageViewer-GroupSelector__item p {\n  margin: 0;\n}\n\n.BioImageViewer-GroupSelector__item em {\n  font-size: 12px;\n}\n', ""]);
+            c.push([t.id, '.BioImageViewer-Slider {\n  width: 320px;\n  background: #f8fafb;\n  border-radius: 12px;\n  padding: 12px 12px 20px;\n  font-family: Inter, Arial, "sans-serif";\n}\n\n.BioImageViewer-Slider__text {\n  color: #000;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 14px;\n  font-weight: 600;\n  line-height: 20px;\n}\n\n.BioImageViewer-Slider__text--light {\n  color: #000000b3;\n}\n\n.BioImageViewer-Slider__icon {\n  width: 16px;\n}\n\n.BioImageViewer-Slider__colorpicker {\n  width: 16px;\n  height: 16px;\n  border: 2px solid #fff;\n  border-radius: 50%;\n  margin-right: 12px;\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-Slider__colorpicker-backdrop {\n  position: fixed;\n  inset: 0;\n}\n\n.BioImageViewer-Slider__colorpicker-container {\n  z-index: 2;\n  position: absolute;\n}\n\n.BioImageViewer-Slider__main {\n  justify-content: space-between;\n  display: flex;\n}\n\n.BioImageViewer-Slider__left, .BioImageViewer-Slider__info {\n  align-items: center;\n  display: flex;\n}\n\n.BioImageViewer-Slider__icon-wrapper {\n  margin-left: 6px;\n  margin-right: 14px;\n}\n\n.BioImageViewer-Slider__value {\n  color: #000000de;\n  background: #fff;\n  border: 1px solid #cfd6de;\n  border-radius: 6px;\n  padding: 6px 16px;\n  font-size: 14px;\n  font-style: normal;\n  font-weight: 400;\n  line-height: 20px;\n}\n\n.BioImageViewer-Slider__range {\n  width: 100%;\n}\n\n.BioImageViewer-ControlPanel {\n  background: #fff;\n  border-radius: 12px;\n  margin-bottom: 16px;\n  padding: 26px 16px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-ControlPanel__title {\n  align-items: center;\n  margin: 0 0 26px;\n  font-size: 16px;\n  font-style: normal;\n  font-weight: 700;\n  line-height: 24px;\n  display: flex;\n}\n\n.BioImageViewer-ControlPanel__title svg {\n  margin-right: 10px;\n}\n\n.BioImageViewer-ControlPanel__list {\n  padding-left: 0;\n  list-style: none;\n}\n\n.BioImageViewer-ControlPanel__item {\n  margin-bottom: 8px;\n}\n\n.BioImageViewer-AttributePanel {\n  background: #fff;\n  border-radius: 12px;\n  margin-bottom: 16px;\n  padding: 26px 16px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-AttributePanel__title {\n  align-items: center;\n  margin: 0 0 16px;\n  font-size: 16px;\n  font-style: normal;\n  font-weight: 700;\n  line-height: 24px;\n  display: flex;\n}\n\n.BioImageViewer-AttributePanel__item {\n  flex-direction: row;\n  align-items: center;\n  display: flex;\n}\n\n.BioImageViewer-AttributePanel__radio {\n  margin: 0;\n}\n\n.BioImageViewer-AttributePanel__label {\n  margin: 6px;\n}\n\n.BIV-ZoomControls {\n  z-index: 1;\n  background-color: #fff;\n  border-radius: 8px;\n  align-items: center;\n  gap: 8px;\n  padding: 4px;\n  display: flex;\n  position: absolute;\n  top: 16px;\n  right: 16px;\n  box-shadow: 0 1px 3px #d1d5d7;\n}\n\n.BIV-ZoomControls__label {\n  color: #000000b3;\n  width: 56px;\n  text-align: center;\n  margin: 0;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 12px;\n  font-weight: 600;\n  line-height: 20px;\n}\n\n.BIV-ZoomControls__button {\n  width: 28px;\n  height: 28px;\n  background: no-repeat;\n  border: none;\n  padding: 0;\n}\n\n.BIV-ZoomControls__button:hover {\n  cursor: pointer;\n}\n\n.BIV-Tooltip {\n  position: relative;\n}\n\n.BIV-Tooltip:hover .BIV-Tooltip__content {\n  opacity: 1;\n}\n\n.BIV-Tooltip__content {\n  color: #fff;\n  opacity: 0;\n  white-space: nowrap;\n  background-color: #333f55;\n  border-radius: 4px;\n  padding: 8px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 12px;\n  font-weight: 600;\n  line-height: 20px;\n  transition: opacity .2s ease-in-out;\n  position: absolute;\n  bottom: -54px;\n  left: 50%;\n  transform: translateX(-50%);\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BIV-Tooltip__content:before {\n  content: "";\n  width: 0;\n  height: 0;\n  border: 10px solid #0000;\n  border-top: 0;\n  border-bottom-color: #333f55;\n  position: absolute;\n  top: -10px;\n  left: 50%;\n  transform: translateX(-50%);\n}\n\n.BioImageViewer-Viewer__minimap {\n  width: 100%;\n  height: 100%;\n  position: absolute;\n  box-shadow: 0 0 8px 2px #00000073;\n}\n\n.BioImageViewer__container {\n  width: 100%;\n  height: 100%;\n  position: relative;\n}\n\n.BioImageViewer__container #deckgl-wrapper {\n  background-image: url(' + h + ');\n  background-size: 50px;\n}\n\n.BioImageViewer__controls {\n  z-index: 1;\n  max-height: 80vh;\n  padding: 6px;\n  position: absolute;\n  top: 68px;\n  right: 16px;\n  overflow-y: auto;\n}\n\n.BioImageViewer__minimap {\n  width: 160px;\n  height: 90px;\n  border: 1px solid gray;\n  position: absolute;\n  top: 20px;\n  left: 20px;\n}\n\n.BioImageViewer__scalebar {\n  width: calc(var(--scalebar-length) * 1px);\n  height: 10px;\n  box-sizing: border-box;\n  background: linear-gradient(to right, #fff 50%, #000 50%);\n  border: 1px solid #000;\n  position: absolute;\n  bottom: 60px;\n  left: 20px;\n}\n\n.BioImageViewer__scalebar__text {\n  width: calc(var(--scalebar-length) * 1px);\n  height: 15px;\n  box-sizing: border-box;\n  text-align: center;\n  margin: 0;\n  font-family: Inter, Arial, "sans-serif";\n  font-size: 14px;\n  font-weight: 500;\n  position: absolute;\n  top: 10px;\n  left: -1px;\n}\n\n.BioImageViewer-GroupSelector {\n  background: #fff;\n  border-radius: 12px;\n  flex-direction: column;\n  margin-bottom: 16px;\n  padding: 26px 16px 16px;\n  font-family: Inter, Arial, "sans-serif";\n  display: flex;\n  box-shadow: 0 1px 3px #00000029;\n}\n\n.BioImageViewer-GroupSelector__title {\n  align-items: center;\n  margin: 0 0 26px;\n  font-size: 16px;\n  font-style: normal;\n  font-weight: 700;\n  line-height: 24px;\n  display: flex;\n}\n\n.BioImageViewer-GroupSelector__title svg {\n  margin-right: 10px;\n}\n\n.BioImageViewer-GroupSelector__controls {\n  justify-content: space-between;\n  align-items: center;\n  margin: 6px;\n  display: flex;\n}\n\n.BioImageViewer-GroupSelector__list {\n  padding-left: 0;\n  list-style: none;\n}\n\n.BioImageViewer-GroupSelector__value {\n  color: #000000de;\n  background: #fff;\n  border: 1px solid #cfd6de;\n  border-radius: 6px;\n  padding: 6px 16px;\n  font-size: 14px;\n  font-style: normal;\n  font-weight: 400;\n  line-height: 20px;\n}\n\n.BioImageViewer-GroupSelector__item {\n  cursor: pointer;\n  background-color: #aeaeae;\n  border-radius: 12px;\n  margin-bottom: 12px;\n  padding: 8px;\n  font-size: 14px;\n}\n\n.BioImageViewer-GroupSelector__item:hover {\n  background-color: #0000ff26;\n}\n\n.BioImageViewer-GroupSelector__item p {\n  margin: 0;\n}\n\n.BioImageViewer-GroupSelector__item em {\n  font-size: 12px;\n}\n', ""]);
             const u = c
         },
         3645: t => {
             "use strict";
             t.exports = function(t) {
                 var e = [];
                 return e.toString = function() {
@@ -30811,39 +30862,39 @@
                     return -1
                 }
 
                 function L(t) {
                     return Array.prototype.slice.call(t, 0)
                 }
 
-                function k(t, e, n) {
+                function R(t, e, n) {
                     for (var i = [], r = [], s = 0; s < t.length;) {
                         var o = e ? t[s][e] : t[s];
                         O(r, o) < 0 && i.push(t[s]), r[s] = o, s++
                     }
                     return n && (i = e ? i.sort((function(t, n) {
                         return t[e] > n[e]
                     })) : i.sort()), i
                 }
 
-                function R(t, e) {
+                function k(t, e) {
                     for (var n, i, r = e[0].toUpperCase() + e.slice(1), s = 0; s < c.length;) {
                         if ((i = (n = c[s]) ? n + r : e) in t) return i;
                         s++
                     }
                     return a
                 }
                 var I = 1;
 
                 function j(t) {
                     var e = t.ownerDocument || t;
                     return e.defaultView || e.parentWindow || r
                 }
                 var z = "ontouchstart" in r,
-                    F = R(r, "PointerEvent") !== a,
+                    F = k(r, "PointerEvent") !== a,
                     B = z && /mobile|tablet|ip(ad|hone|od)|android/i.test(navigator.userAgent),
                     D = "touch",
                     N = "mouse",
                     V = 25,
                     U = 1,
                     G = 4,
                     W = 8,
@@ -31042,15 +31093,15 @@
                 function yt() {
                     this.evTarget = "touchstart", this.evWin = "touchstart touchmove touchend touchcancel", this.started = !1, et.apply(this, arguments)
                 }
 
                 function _t(t, e) {
                     var n = L(t.touches),
                         i = L(t.changedTouches);
-                    return e & (G | W) && (n = k(n.concat(i), "identifier", !0)), [n, i]
+                    return e & (G | W) && (n = R(n.concat(i), "identifier", !0)), [n, i]
                 }
                 x(yt, et, {
                     handler: function(t) {
                         var e = bt[t.type];
                         if (e === U && (this.started = !0), this.started) {
                             var n = _t.call(this, t, e);
                             e & (G | W) && n[0].length - n[1].length == 0 && (this.started = !1), this.callback(this.manager, e, {
@@ -31082,15 +31133,15 @@
                         a = [],
                         l = this.target;
                     if (s = n.filter((function(t) {
                             return T(t.target, l)
                         })), e === U)
                         for (r = 0; r < s.length;) i[s[r].identifier] = !0, r++;
                     for (r = 0; r < o.length;) i[o[r].identifier] && a.push(o[r]), e & (G | W) && delete i[o[r].identifier], r++;
-                    return a.length ? [k(s.concat(a), "identifier", !0), a] : void 0
+                    return a.length ? [R(s.concat(a), "identifier", !0), a] : void 0
                 }
                 x(Et, et, {
                     handler: function(t) {
                         var e = xt[t.type],
                             n = Pt.call(this, t, e);
                         n && this.callback(this.manager, e, {
                             pointers: n[0],
@@ -31147,18 +31198,18 @@
                             this.callback(t, e, n)
                         }
                     },
                     destroy: function() {
                         this.touch.destroy(), this.mouse.destroy()
                     }
                 });
-                var Ot = R(h.style, "touchAction"),
+                var Ot = k(h.style, "touchAction"),
                     Lt = Ot !== a,
-                    kt = "compute",
-                    Rt = "auto",
+                    Rt = "compute",
+                    kt = "auto",
                     It = "manipulation",
                     jt = "none",
                     zt = "pan-x",
                     Ft = "pan-y",
                     Bt = function() {
                         if (!Lt) return !1;
                         var t = {},
@@ -31169,29 +31220,29 @@
                     }();
 
                 function Dt(t, e) {
                     this.manager = t, this.set(e)
                 }
                 Dt.prototype = {
                     set: function(t) {
-                        t == kt && (t = this.compute()), Lt && this.manager.element.style && Bt[t] && (this.manager.element.style[Ot] = t), this.actions = t.toLowerCase().trim()
+                        t == Rt && (t = this.compute()), Lt && this.manager.element.style && Bt[t] && (this.manager.element.style[Ot] = t), this.actions = t.toLowerCase().trim()
                     },
                     update: function() {
                         this.set(this.manager.options.touchAction)
                     },
                     compute: function() {
                         var t = [];
                         return v(this.manager.recognizers, (function(e) {
                                 E(e.options.enable, [e]) && (t = t.concat(e.getTouchAction()))
                             })),
                             function(t) {
                                 if (A(t, jt)) return jt;
                                 var e = A(t, zt),
                                     n = A(t, Ft);
-                                return e && n ? jt : e || n ? e ? zt : Ft : A(t, It) ? It : Rt
+                                return e && n ? jt : e || n ? e ? zt : Ft : A(t, It) ? It : kt
                             }(t.join(" "))
                     },
                     preventDefaults: function(t) {
                         var e = t.srcEvent,
                             n = t.offsetDirection;
                         if (this.manager.session.prevented) e.preventDefault();
                         else {
@@ -31270,15 +31321,15 @@
                         t[2] && e.recognizeWith(t[2]), t[3] && e.requireFailure(t[3])
                     }), this)
                 }
 
                 function ee(t, e) {
                     var n, i = t.element;
                     i.style && (v(t.options.cssProps, (function(r, s) {
-                        n = R(i.style, s), e ? (t.oldCssProps[n] = i.style[n], i.style[n] = r) : i.style[n] = t.oldCssProps[n] || ""
+                        n = k(i.style, s), e ? (t.oldCssProps[n] = i.style[n], i.style[n] = r) : i.style[n] = t.oldCssProps[n] || ""
                     })), e || (t.oldCssProps = {}))
                 }
                 Ut.prototype = {
                     defaults: {},
                     set: function(t) {
                         return l(this.options, t), this.manager && this.manager.touchAction.update(), this
                     },
@@ -31402,15 +31453,15 @@
                     defaults: {
                         event: "press",
                         pointers: 1,
                         time: 251,
                         threshold: 9
                     },
                     getTouchAction: function() {
-                        return [Rt]
+                        return [kt]
                     },
                     process: function(t) {
                         var e = this.options,
                             n = t.pointers.length === e.pointers,
                             i = t.distance < e.threshold,
                             r = t.deltaTime > e.time;
                         if (this._input = t, !i || !n || t.eventType & (G | W) && !r) this.reset();
@@ -31495,15 +31546,15 @@
                         clearTimeout(this._timer)
                     },
                     emit: function() {
                         8 == this.state && (this._input.tapCount = this.count, this.manager.emit(this.options.event, this._input))
                     }
                 }), Qt.VERSION = "2.0.7", Qt.defaults = {
                     domEvents: !1,
-                    touchAction: kt,
+                    touchAction: Rt,
                     enable: !0,
                     inputTarget: null,
                     inputClass: null,
                     preset: [
                         [Kt, {
                             enable: !1
                         }],
@@ -31646,15 +31697,15 @@
                     off: C,
                     each: v,
                     merge: _,
                     extend: y,
                     assign: l,
                     inherit: x,
                     bindFn: w,
-                    prefixed: R
+                    prefixed: k
                 }), (void 0 !== r ? r : "undefined" != typeof self ? self : {}).Hammer = Qt, (i = function() {
                     return Qt
                 }.call(e, n, e, t)) === a || (t.exports = i)
             }(window, document)
         },
         2896: (t, e, n) => {
             "use strict";
@@ -31944,46 +31995,46 @@
                 w = n(2928),
                 E = n(3674),
                 P = n(1704),
                 S = "[object Arguments]",
                 C = "[object Function]",
                 T = "[object Object]",
                 A = {};
-            A[S] = A["[object Array]"] = A["[object ArrayBuffer]"] = A["[object DataView]"] = A["[object Boolean]"] = A["[object Date]"] = A["[object Float32Array]"] = A["[object Float64Array]"] = A["[object Int8Array]"] = A["[object Int16Array]"] = A["[object Int32Array]"] = A["[object Map]"] = A["[object Number]"] = A[T] = A["[object RegExp]"] = A["[object Set]"] = A["[object String]"] = A["[object Symbol]"] = A["[object Uint8Array]"] = A["[object Uint8ClampedArray]"] = A["[object Uint16Array]"] = A["[object Uint32Array]"] = !0, A["[object Error]"] = A[C] = A["[object WeakMap]"] = !1, t.exports = function t(e, n, M, O, L, k) {
-                var R, I = 1 & n,
+            A[S] = A["[object Array]"] = A["[object ArrayBuffer]"] = A["[object DataView]"] = A["[object Boolean]"] = A["[object Date]"] = A["[object Float32Array]"] = A["[object Float64Array]"] = A["[object Int8Array]"] = A["[object Int16Array]"] = A["[object Int32Array]"] = A["[object Map]"] = A["[object Number]"] = A[T] = A["[object RegExp]"] = A["[object Set]"] = A["[object String]"] = A["[object Symbol]"] = A["[object Uint8Array]"] = A["[object Uint8ClampedArray]"] = A["[object Uint16Array]"] = A["[object Uint32Array]"] = !0, A["[object Error]"] = A[C] = A["[object WeakMap]"] = !1, t.exports = function t(e, n, M, O, L, R) {
+                var k, I = 1 & n,
                     j = 2 & n,
                     z = 4 & n;
-                if (M && (R = L ? M(e, O, L, k) : M(e)), void 0 !== R) return R;
+                if (M && (k = L ? M(e, O, L, R) : M(e)), void 0 !== k) return k;
                 if (!x(e)) return e;
                 var F = b(e);
                 if (F) {
-                    if (R = g(e), !I) return c(e, R)
+                    if (k = g(e), !I) return c(e, k)
                 } else {
                     var B = f(e),
                         D = B == C || "[object GeneratorFunction]" == B;
                     if (y(e)) return l(e, I);
                     if (B == T || B == S || D && !L) {
-                        if (R = j || D ? {} : v(e), !I) return j ? u(e, a(R, e)) : h(e, o(R, e))
+                        if (k = j || D ? {} : v(e), !I) return j ? u(e, a(k, e)) : h(e, o(k, e))
                     } else {
                         if (!A[B]) return L ? e : {};
-                        R = m(e, B, I)
+                        k = m(e, B, I)
                     }
                 }
-                k || (k = new i);
-                var N = k.get(e);
+                R || (R = new i);
+                var N = R.get(e);
                 if (N) return N;
-                k.set(e, R), w(e) ? e.forEach((function(i) {
-                    R.add(t(i, n, M, i, e, k))
+                R.set(e, k), w(e) ? e.forEach((function(i) {
+                    k.add(t(i, n, M, i, e, R))
                 })) : _(e) && e.forEach((function(i, r) {
-                    R.set(r, t(i, n, M, r, e, k))
+                    k.set(r, t(i, n, M, r, e, R))
                 }));
                 var V = F ? void 0 : (z ? j ? p : d : j ? P : E)(e);
                 return r(V || e, (function(i, r) {
-                    V && (i = e[r = i]), s(R, r, t(i, n, M, r, e, k))
-                })), R
+                    V && (i = e[r = i]), s(k, r, t(i, n, M, r, e, R))
+                })), k
             }
         },
         3118: (t, e, n) => {
             var i = n(3218),
                 r = Object.create,
                 s = function() {
                     function t() {}
@@ -33274,49 +33325,14 @@
         },
         9833: (t, e, n) => {
             var i = n(531);
             t.exports = function(t) {
                 return null == t ? "" : i(t)
             }
         },
-        7418: t => {
-            "use strict";
-            var e = Object.getOwnPropertySymbols,
-                n = Object.prototype.hasOwnProperty,
-                i = Object.prototype.propertyIsEnumerable;
-            t.exports = function() {
-                try {
-                    if (!Object.assign) return !1;
-                    var t = new String("abc");
-                    if (t[5] = "de", "5" === Object.getOwnPropertyNames(t)[0]) return !1;
-                    for (var e = {}, n = 0; n < 10; n++) e["_" + String.fromCharCode(n)] = n;
-                    if ("0123456789" !== Object.getOwnPropertyNames(e).map((function(t) {
-                            return e[t]
-                        })).join("")) return !1;
-                    var i = {};
-                    return "abcdefghijklmnopqrst".split("").forEach((function(t) {
-                        i[t] = t
-                    })), "abcdefghijklmnopqrst" === Object.keys(Object.assign({}, i)).join("")
-                } catch (t) {
-                    return !1
-                }
-            }() ? Object.assign : function(t, r) {
-                for (var s, o, a = function(t) {
-                        if (null == t) throw new TypeError("Object.assign cannot be called with null or undefined");
-                        return Object(t)
-                    }(t), l = 1; l < arguments.length; l++) {
-                    for (var c in s = Object(arguments[l])) n.call(s, c) && (a[c] = s[c]);
-                    if (e) {
-                        o = e(s);
-                        for (var h = 0; h < o.length; h++) i.call(s, o[h]) && (a[o[h]] = s[o[h]])
-                    }
-                }
-                return a
-            }
-        },
         2703: (t, e, n) => {
             "use strict";
             var i = n(414);
 
             function r() {}
 
             function s() {}
@@ -33361,54 +33377,14 @@
         5697: (t, e, n) => {
             t.exports = n(2703)()
         },
         414: t => {
             "use strict";
             t.exports = "SECRET_DO_NOT_PASS_THIS_OR_YOU_WILL_BE_FIRED"
         },
-        5251: (t, e, n) => {
-            "use strict";
-            n(7418);
-            var i = n(6271),
-                r = 60103;
-            if ("function" == typeof Symbol && Symbol.for) {
-                var s = Symbol.for;
-                r = s("react.element"), s("react.fragment")
-            }
-            var o = i.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED.ReactCurrentOwner,
-                a = Object.prototype.hasOwnProperty,
-                l = {
-                    key: !0,
-                    ref: !0,
-                    __self: !0,
-                    __source: !0
-                };
-
-            function c(t, e, n) {
-                var i, s = {},
-                    c = null,
-                    h = null;
-                for (i in void 0 !== n && (c = "" + n), void 0 !== e.key && (c = "" + e.key), void 0 !== e.ref && (h = e.ref), e) a.call(e, i) && !l.hasOwnProperty(i) && (s[i] = e[i]);
-                if (t && t.defaultProps)
-                    for (i in e = t.defaultProps) void 0 === s[i] && (s[i] = e[i]);
-                return {
-                    $$typeof: r,
-                    type: t,
-                    key: c,
-                    ref: h,
-                    props: s,
-                    _owner: o.current
-                }
-            }
-            e.jsx = c, e.jsxs = c
-        },
-        5893: (t, e, n) => {
-            "use strict";
-            t.exports = n(5251)
-        },
         4754: (t, e, n) => {
             "use strict";
             Object.defineProperty(e, "__esModule", {
                 value: !0
             }), e.autoprefix = void 0;
             var i, r = (i = n(2525)) && i.__esModule ? i : {
                     default: i
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/remoteEntry.97aa55da34c5f332490c.js` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/remoteEntry.9bb49b46696448b14690.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, i, o, a, l, d, u, c, f, s, p, h, v, b, m, g, y = {
+    var e, r, t, n, i, o, a, d, l, f, u, s, c, p, h, v, b, m, g, y = {
             5290: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(744).then((() => () => t(1744))),
                         "./extension": () => t.e(744).then((() => () => t(1744))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     i = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -44,27 +44,27 @@
         }), r
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        241: "7a42393c28911f92f6c6",
+        241: "3606da7606ad147cbcb2",
         446: "3bf34f45c93ace9c0f28",
-        635: "b2bedc962bcd82714540",
-        744: "83657870ab57005727cf",
-        747: "433530952542f03ebc71",
-        774: "3d92675aa1721b861046"
+        556: "f09c354898cd66a026b3",
+        635: "a03dea4f48d4a0dc1e4c",
+        744: "32875cac115e9f54b48d",
+        747: "433530952542f03ebc71"
     } [e] + ".js?v=" + {
-        241: "7a42393c28911f92f6c6",
+        241: "3606da7606ad147cbcb2",
         446: "3bf34f45c93ace9c0f28",
-        635: "b2bedc962bcd82714540",
-        744: "83657870ab57005727cf",
-        747: "433530952542f03ebc71",
-        774: "3d92675aa1721b861046"
+        556: "f09c354898cd66a026b3",
+        635: "a03dea4f48d4a0dc1e4c",
+        744: "32875cac115e9f54b48d",
+        747: "433530952542f03ebc71"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -72,34 +72,34 @@
         enumerable: !0,
         set: () => {
             throw new Error("ES Modules may not assign module.exports or exports.*, Use ESM export syntax, instead: " + e.id)
         }
     }), e), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@tiledb-inc/jupyter-bioimage-viewer:", S.l = (t, n, i, o) => {
         if (e[t]) e[t].push(n);
         else {
-            var a, l;
+            var a, d;
             if (void 0 !== i)
-                for (var d = document.getElementsByTagName("script"), u = 0; u < d.length; u++) {
-                    var c = d[u];
-                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + i) {
-                        a = c;
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var u = l[f];
+                    if (u.getAttribute("src") == t || u.getAttribute("data-webpack") == r + i) {
+                        a = u;
                         break
                     }
                 }
-            a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, S.nc && a.setAttribute("nonce", S.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
-            var f = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(s);
+            a || (d = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, S.nc && a.setAttribute("nonce", S.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
+            var s = (r, n) => {
+                    a.onerror = a.onload = null, clearTimeout(c);
                     var i = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), i && i.forEach((e => e(n))), r) return r(n)
                 },
-                s = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
-            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), l && document.head.appendChild(a)
+            a.onerror = s.bind(null, a.onerror), a.onload = s.bind(null, a.onload), d && document.head.appendChild(a)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -111,25 +111,25 @@
             n || (n = []);
             var i = r[t];
             if (i || (i = r[t] = {}), !(n.indexOf(i) >= 0)) {
                 if (n.push(i), e[t]) return e[t];
                 S.o(S.S, t) || (S.S[t] = {});
                 var o = S.S[t],
                     a = "@tiledb-inc/jupyter-bioimage-viewer",
-                    l = (e, r, t, n) => {
+                    d = (e, r, t, n) => {
                         var i = o[e] = o[e] || {},
-                            l = i[r];
-                        (!l || !l.loaded && (!n != !l.eager ? n : a > l.from)) && (i[r] = {
+                            d = i[r];
+                        (!d || !d.loaded && (!n != !d.eager ? n : a > d.from)) && (i[r] = {
                             get: t,
                             from: a,
                             eager: !!n
                         })
                     },
-                    d = [];
-                return "default" === t && (l("@tiledb-inc/bioimage-viewer", "0.1.1-beta.1", (() => Promise.all([S.e(635), S.e(774), S.e(446)]).then((() => () => S(3774))))), l("@tiledb-inc/jupyter-bioimage-viewer", "0.1.2-alpha.3", (() => S.e(744).then((() => () => S(1744)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                    l = [];
+                return "default" === t && (d("@tiledb-inc/bioimage-viewer", "0.1.1-beta.2", (() => Promise.all([S.e(635), S.e(556), S.e(446)]).then((() => () => S(1556))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.3-alpha.0", (() => S.e(744).then((() => () => S(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -148,107 +148,107 @@
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var i = e[n],
                 o = (typeof i)[0];
             if (n >= r.length) return "u" == o;
             var a = r[n],
-                l = (typeof a)[0];
-            if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
+                d = (typeof a)[0];
+            if (o != d) return "o" == o && "n" == d || "s" == d || "u" == o;
             if ("o" != o && "u" != o && i != a) return i < a;
             n++
         }
     }, i = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(d = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, d);
             return t
         }
         var a = [];
         for (o = 1; o < e.length; o++) {
-            var l = e[o];
-            a.push(0 === l ? "not(" + d() + ")" : 1 === l ? "(" + d() + " || " + d() + ")" : 2 === l ? a.pop() + " " + a.pop() : i(l))
+            var d = e[o];
+            a.push(0 === d ? "not(" + l() + ")" : 1 === d ? "(" + l() + " || " + l() + ")" : 2 === d ? a.pop() + " " + a.pop() : i(d))
         }
-        return d();
+        return l();
 
-        function d() {
+        function l() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 i = n < 0;
             i && (n = -n - 1);
-            for (var a = 0, l = 1, d = !0;; l++, a++) {
-                var u, c, f = l < e.length ? (typeof e[l])[0] : "";
-                if (a >= r.length || "o" == (c = (typeof(u = r[a]))[0])) return !d || ("u" == f ? l > n && !i : "" == f != i);
-                if ("u" == c) {
-                    if (!d || "u" != f) return !1
-                } else if (d)
-                    if (f == c)
-                        if (l <= n) {
-                            if (u != e[l]) return !1
+            for (var a = 0, d = 1, l = !0;; d++, a++) {
+                var f, u, s = d < e.length ? (typeof e[d])[0] : "";
+                if (a >= r.length || "o" == (u = (typeof(f = r[a]))[0])) return !l || ("u" == s ? d > n && !i : "" == s != i);
+                if ("u" == u) {
+                    if (!l || "u" != s) return !1
+                } else if (l)
+                    if (s == u)
+                        if (d <= n) {
+                            if (f != e[d]) return !1
                         } else {
-                            if (i ? u > e[l] : u < e[l]) return !1;
-                            u != e[l] && (d = !1)
+                            if (i ? f > e[d] : f < e[d]) return !1;
+                            f != e[d] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
-                    if (i || l <= n) return !1;
-                    d = !1, l--
+                else if ("s" != s && "n" != s) {
+                    if (i || d <= n) return !1;
+                    l = !1, d--
                 } else {
-                    if (l <= n || c < f != i) return !1;
-                    d = !1
-                } else "s" != f && "n" != f && (d = !1, l--)
+                    if (d <= n || u < s != i) return !1;
+                    l = !1
+                } else "s" != s && "n" != s && (l = !1, d--)
             }
         }
-        var s = [],
-            p = s.pop.bind(s);
+        var c = [],
+            p = c.pop.bind(c);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
-            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
         }
         return !!p()
     }, a = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, l = (e, r) => {
+    }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", u = (e, r, t, n) => {
-        var i = l(e, t);
-        return o(n, i) || f(d(e, t, i, n)), s(e[t][i])
-    }, c = (e, r, t) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", f = (e, r, t, n) => {
+        var i = d(e, t);
+        return o(n, i) || s(l(e, t, i, n)), c(e[t][i])
+    }, u = (e, r, t) => {
         var i = e[r];
         return (r = Object.keys(i).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && i[r]
-    }, f = e => {
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, s = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, i) {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, i) {
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, n, i)) : e(r, S.S[r], t, n, i)
-    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), v = p(((e, r, t, n, i) => {
-        var o = r && S.o(r, t) && c(r, t, n);
-        return o ? s(o) : i()
+    })(((e, r, t, n) => (a(e, t), f(r, 0, t, n)))), v = p(((e, r, t, n, i) => {
+        var o = r && S.o(r, t) && u(r, t, n);
+        return o ? c(o) : i()
     })), b = {}, m = {
         1395: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ]),
-        8840: () => v("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 1, , "beta", 1], (() => Promise.all([S.e(635), S.e(774), S.e(446)]).then((() => () => S(3774))))),
+        4155: () => v("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 1, , "beta", 2], (() => Promise.all([S.e(635), S.e(556), S.e(446)]).then((() => () => S(1556))))),
         4456: () => h("default", "react-dom", [1, 17, 0, 1]),
         6271: () => h("default", "react", [1, 17, 0, 1])
     }, g = {
         446: [4456, 6271],
-        744: [1395, 8840]
+        744: [1395, 4155]
     }, S.f.consumes = (e, r) => {
         S.o(g, e) && g[e].forEach((e => {
             if (S.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
@@ -285,21 +285,21 @@
                                 o = t && t.target && t.target.src;
                             a.message = "Loading chunk " + r + " failed.\n(" + i + ": " + o + ")", a.name = "ChunkLoadError", a.type = i, a.request = o, n[1](a)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, i, [o, a, l] = t,
-                    d = 0;
+                var n, i, [o, a, d] = t,
+                    l = 0;
                 if (o.some((r => 0 !== e[r]))) {
                     for (n in a) S.o(a, n) && (S.m[n] = a[n]);
-                    l && l(S)
+                    d && d(S)
                 }
-                for (r && r(t); d < o.length; d++) i = o[d], S.o(e, i) && e[i] && e[i][0](), e[i] = 0
+                for (r && r(t); l < o.length; l++) i = o[l], S.o(e, i) && e[i] && e[i][0](), e[i] = 0
             },
             t = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
     var j = S(5290);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@tiledb-inc/jupyter-bioimage-viewer"] = j
 })();
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9806034482758621%*

 * *Differences: {"'packages'": "{23: {'versionInfo': '0.1.1-beta.2'}, 46: {'versionInfo': '18.2.0'}, insert: [(48, "*

 * *               "OrderedDict([('name', 'react-dom'), ('versionInfo', '18.2.0'), ('licenseId', "*

 * *               "'MIT'), ('extractedText', 'MIT License\\n\\nCopyright (c) Facebook, Inc. and its "*

 * *               'affiliates.\\n\\nPermission is hereby granted, free of charge, to any person '*

 * *               'obtaining a copy\\nof this software and associated documentation files (the '*

 * *               '"Software"), […]*

```diff
@@ -138,15 +138,15 @@
             "name": "@probe.gl/stats",
             "versionInfo": "3.6.0"
         },
         {
             "extractedText": "",
             "licenseId": "MIT",
             "name": "@tiledb-inc/bioimage-viewer",
-            "versionInfo": "0.1.1-beta.1"
+            "versionInfo": "0.1.1-beta.2"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) 2020 TileDB, Inc.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@tiledb-inc/tiledb-cloud",
             "versionInfo": "1.0.13-alpha.0"
         },
@@ -255,20 +255,14 @@
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2016 Zeit, Inc.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "ms",
             "versionInfo": "2.0.0"
         },
         {
-            "extractedText": "The MIT License (MIT)\n\nCopyright (c) Sindre Sorhus <sindresorhus@gmail.com> (sindresorhus.com)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
-            "licenseId": "MIT",
-            "name": "object-assign",
-            "versionInfo": "4.1.1"
-        },
-        {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2017-present Parallel.js Maintainers\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "paralleljs",
             "versionInfo": "1.1.0"
         },
         {
             "extractedText": "(The MIT License)\n\nCopyright (c) 2013 Roman Shtylman <shtylman@gmail.com>\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
@@ -282,23 +276,29 @@
             "name": "prop-types",
             "versionInfo": "15.8.1"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react",
-            "versionInfo": "17.0.2"
+            "versionInfo": "18.2.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015 Case Sandberg\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react-color",
             "versionInfo": "2.19.3"
         },
         {
+            "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "react-dom",
+            "versionInfo": "18.2.0"
+        },
+        {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015 Case Sandberg\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "reactcss",
             "versionInfo": "1.2.3"
         },
         {
             "extractedText": "",
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg/render.py` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/render.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg.egg-info/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-jupyter-bioimg
-Version: 0.1.2a3
+Version: 0.1.3a0
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tiledb_jupyter_bioimg.egg-info/SOURCES.txt` & `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 tiledb_jupyter_bioimg.egg-info/SOURCES.txt
 tiledb_jupyter_bioimg.egg-info/dependency_links.txt
 tiledb_jupyter_bioimg.egg-info/not-zip-safe
 tiledb_jupyter_bioimg.egg-info/requires.txt
 tiledb_jupyter_bioimg.egg-info/top_level.txt
 tiledb_jupyter_bioimg/labextension/package.json
 tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
-tiledb_jupyter_bioimg/labextension/static/241.7a42393c28911f92f6c6.js
+tiledb_jupyter_bioimg/labextension/static/241.3606da7606ad147cbcb2.js
 tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
-tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js
-tiledb_jupyter_bioimg/labextension/static/635.b2bedc962bcd82714540.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/744.83657870ab57005727cf.js
+tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js
+tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js.LICENSE.txt
+tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js
+tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js.LICENSE.txt
+tiledb_jupyter_bioimg/labextension/static/744.32875cac115e9f54b48d.js
 tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
-tiledb_jupyter_bioimg/labextension/static/774.3d92675aa1721b861046.js
-tiledb_jupyter_bioimg/labextension/static/774.3d92675aa1721b861046.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/remoteEntry.97aa55da34c5f332490c.js
+tiledb_jupyter_bioimg/labextension/static/remoteEntry.9bb49b46696448b14690.js
 tiledb_jupyter_bioimg/labextension/static/style.js
 tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.2a3/tsconfig.json` & `tiledb_jupyter_bioimg-0.1.3a0/tsconfig.json`

 * *Files identical despite different names*

