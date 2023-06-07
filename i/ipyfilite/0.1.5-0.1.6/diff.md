# Comparing `tmp/ipyfilite-0.1.5.tar.gz` & `tmp/ipyfilite-0.1.6.tar.gz`

## Comparing `ipyfilite-0.1.5.tar` & `ipyfilite-0.1.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.coveragerc
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.eslintignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.npmignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.prettierignore
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.prettierrc
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/MANIFEST.in
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/babel.config.js
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/codecov.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/install.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/jest.config.js
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/package.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/setup.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/tsconfig.eslint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/tsconfig.json
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/webpack.config.js
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/css/widget.css
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/Makefile
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/environment.yml
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/make.bat
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/conf.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/develop-install.rst
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/index.rst
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/installing.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/introduction.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/_static/helper.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/examples/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/examples/introduction.nblink
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/examples/example.txt
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/examples/introduction.ipynb
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/_frontend.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/_manager.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/_version.py
--rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/http.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/upload.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/labextension/package.json
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/labextension/static/480.5228ab589234a2bdb92a.js
--rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/labextension/static/568.57321689c730e6670738.js
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/labextension/static/remoteEntry.392e4ddeb2ce5c2a11f4.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/nbextension/extension.js
--rw-r--r--   0        0        0    10768 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/nbextension/index.js
--rw-r--r--   0        0        0    28884 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/tests/__init__.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/tests/conftest.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/tests/test_upload.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/extension.ts
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/index.ts
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/plugin.ts
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/version.ts
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/widget.ts
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/__tests__/utils.ts
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/README.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/.coveragerc
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/.eslintignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/.npmignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/.prettierignore
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/.prettierrc
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/MANIFEST.in
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/babel.config.js
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/codecov.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/install.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/jest.config.js
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/package.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/setup.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/tsconfig.eslint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/tsconfig.json
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/webpack.config.js
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/css/widget.css
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/docs/Makefile
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/docs/environment.yml
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/docs/make.bat
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/docs/source/conf.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/docs/source/develop-install.rst
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/docs/source/index.rst
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/docs/source/installing.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/docs/source/introduction.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/docs/source/_static/helper.js
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/docs/source/examples/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/docs/source/examples/introduction.nblink
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/examples/example.txt
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/examples/introduction.ipynb
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/_frontend.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/_manager.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/_version.py
+-rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/http.py
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/upload.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/labextension/package.json
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/labextension/static/480.07e6f878197981be93a5.js
+-rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/labextension/static/568.775df6136673a0d7dba1.js
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/labextension/static/remoteEntry.7afaca43b1bd81f5b801.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/nbextension/extension.js
+-rw-r--r--   0        0        0    10768 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/nbextension/index.js
+-rw-r--r--   0        0        0    28884 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/tests/__init__.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/tests/conftest.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/ipyfilite/tests/test_upload.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/src/extension.ts
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/src/index.ts
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/src/plugin.ts
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/src/version.ts
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/src/widget.ts
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/src/__tests__/utils.ts
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/README.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 ipyfilite-0.1.6/PKG-INFO
```

### Comparing `ipyfilite-0.1.5/.eslintrc.js` & `ipyfilite-0.1.6/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/MANIFEST.in` & `ipyfilite-0.1.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/package.json` & `ipyfilite-0.1.6/ipyfilite/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9609375%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.7afaca43b1bd81f5b801.js'), "*

 * *                 "('extension', './extension')])}",*

 * * "'version'": "'0.1.6'"}*

```diff
@@ -44,14 +44,18 @@
     "files": [
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/juntyr/ipyfilite",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.7afaca43b1bd81f5b801.js"
+        },
         "extension": "lib/plugin",
         "outputDir": "ipyfilite/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -87,9 +91,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.5"
+    "version": "0.1.6"
 }
```

### Comparing `ipyfilite-0.1.5/tsconfig.json` & `ipyfilite-0.1.6/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/webpack.config.js` & `ipyfilite-0.1.6/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/docs/Makefile` & `ipyfilite-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/docs/make.bat` & `ipyfilite-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/docs/source/conf.py` & `ipyfilite-0.1.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/docs/source/develop-install.rst` & `ipyfilite-0.1.6/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/docs/source/index.rst` & `ipyfilite-0.1.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/docs/source/installing.rst` & `ipyfilite-0.1.6/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/examples/introduction.ipynb` & `ipyfilite-0.1.6/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/ipyfilite/__init__.py` & `ipyfilite-0.1.6/ipyfilite/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/ipyfilite/_manager.py` & `ipyfilite-0.1.6/ipyfilite/_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from __future__ import annotations
 
-import asyncio
 import uuid
 import warnings
 from pathlib import Path
 
 from IPython import get_ipython
-from traitlets import Instance
+from traitlets import Bunch, Instance
 from traitlets.config import SingletonConfigurable
 
 
 class IpyfiliteManager(SingletonConfigurable):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self._session = uuid.uuid4()
-        self._upload_futures = dict()
+        self._upload_widgets = dict()
 
         try:
             import js  # noqa: F401
             import pyodide  # noqa: F401
             import pyodide_js  # noqa: F401
         except ImportError:
             warnings.warn(
@@ -46,23 +45,19 @@
                 ipyfilite_manager=Instance(
                     IpyfiliteManager, default_value=manager
                 )
             )
 
         return manager
 
-    async def wait_for_upload_value(self, widget):
-        widget_id = widget._model_id
+    def register_upload(self, widget):
+        self._upload_widgets[widget._model_id] = widget
 
-        if widget_id not in self._upload_futures:
-            self._upload_futures[widget_id] = []
-
-        future = asyncio.Future()
-        self._upload_futures[widget_id].append(future)
-        return await future
+    def unregister_upload(self, widget):
+        self._upload_widgets.pop(widget._model_id, None)
 
     def _on_file_upload(self, event):
         import js
         import pyodide
         import pyodide_js
 
         if (
@@ -73,37 +68,36 @@
             or not getattr(event.data, "widget", None)
         ):
             return
 
         if event.data.session != str(self.session):
             return
 
+        if event.data.widget not in self._upload_widgets:
+            return
+
         upload_path = Path("/uploads") / event.data.uuid
         upload_path.mkdir(parents=True, exist_ok=False)
 
         pyodide_js.FS.mount(
             pyodide_js.FS.filesystems.WORKERFS,
             pyodide.ffi.to_js(
                 {"files": event.data.files},
                 dict_converter=js.Object.fromEntries,
                 create_pyproxies=False,
             ),
             str(upload_path),
         )
 
-        futures = self._upload_futures.get(event.data.widget, [])
-
-        value = [
-            {
-                "name": file.name,
-                "type": file.type,
-                "size": file.size,
-                "last_modified": file.lastModified,
-                "path": str(upload_path / file.name),
-            }
-            for file in event.data.files
-        ]
-
-        for future in futures:
-            future.set_result(value)
-
-        self._upload_futures.pop(event.data.widget, None)
+        self._upload_widgets[event.data.widget].set_trait(
+            "value",
+            [
+                Bunch(
+                    name=file.name,
+                    type=file.type,
+                    size=file.size,
+                    last_modified=file.lastModified,
+                    path=str(upload_path / file.name),
+                )
+                for file in event.data.files
+            ],
+        )
```

### Comparing `ipyfilite-0.1.5/ipyfilite/http.py` & `ipyfilite-0.1.6/ipyfilite/http.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/ipyfilite/upload.py` & `ipyfilite-0.1.6/ipyfilite/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 """
 FileUpload class.
 
 Represents a file upload button.
 """
 
+import asyncio
 import datetime as dt
 from pathlib import Path
 
 from ipywidgets import (
     ButtonStyle,
     TypedTuple,
     ValueWidget,
@@ -177,9 +178,25 @@
         **_value_serialization,
     )
 
     @default("description")
     def _default_description(self):
         return "Upload"
 
-    async def next_value(self):
-        return await IpyfiliteManager.instance().wait_for_upload_value(self)
+    def __init__(self):
+        super().__init__()
+        IpyfiliteManager.instance().register_upload(self)
+
+    async def request(self):
+        from IPython.display import display
+
+        display(self)
+
+        future = asyncio.Future()
+        self.observe(future.set_result, "value")
+        await future
+
+        return self.value
+
+    def __del__(self):
+        IpyfiliteManager.instance().unregister_upload(self)
+        super().__del__()
```

### Comparing `ipyfilite-0.1.5/ipyfilite/labextension/package.json` & `ipyfilite-0.1.6/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9609375%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.1.6'"}*

```diff
@@ -44,18 +44,14 @@
     "files": [
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/juntyr/ipyfilite",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.392e4ddeb2ce5c2a11f4.js"
-        },
         "extension": "lib/plugin",
         "outputDir": "ipyfilite/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -91,9 +87,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.5"
+    "version": "0.1.6"
 }
```

### Comparing `ipyfilite-0.1.5/ipyfilite/labextension/static/480.5228ab589234a2bdb92a.js` & `ipyfilite-0.1.6/ipyfilite/labextension/static/480.07e6f878197981be93a5.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -333,11 +333,11 @@
                         i = o
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.5","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.6","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyfilite-0.1.5/ipyfilite/labextension/static/568.57321689c730e6670738.js` & `ipyfilite-0.1.6/ipyfilite/labextension/static/568.775df6136673a0d7dba1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -305,11 +305,11 @@
                         i = r
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.5","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.6","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyfilite-0.1.5/ipyfilite/labextension/static/remoteEntry.392e4ddeb2ce5c2a11f4.js` & `ipyfilite-0.1.6/ipyfilite/labextension/static/remoteEntry.7afaca43b1bd81f5b801.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, i, o, a, l, f, u, s, d, p, c, h, v, g = {
+    var e, r, t, n, i, o, a, l, u, s, f, d, p, c, h, v, g = {
             229: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(829), t.e(568)]).then((() => () => t(568))),
                         "./extension": () => Promise.all([t.e(829), t.e(480)]).then((() => () => t(480)))
                     },
                     i = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -20,104 +20,104 @@
                     };
                 t.d(r, {
                     get: () => i,
                     init: () => o
                 })
             }
         },
-        m = {};
+        b = {};
 
-    function b(e) {
-        var r = m[e];
+    function m(e) {
+        var r = b[e];
         if (void 0 !== r) return r.exports;
-        var t = m[e] = {
+        var t = b[e] = {
             id: e,
             exports: {}
         };
-        return g[e].call(t.exports, t, t.exports, b), t.exports
+        return g[e].call(t.exports, t, t.exports, m), t.exports
     }
-    b.m = g, b.c = m, b.d = (e, r) => {
-        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
+    m.m = g, m.c = b, m.d = (e, r) => {
+        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
-        480: "5228ab589234a2bdb92a",
-        568: "57321689c730e6670738",
+    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
+        480: "07e6f878197981be93a5",
+        568: "775df6136673a0d7dba1",
         829: "eddb7a59a74d60740eb9"
     } [e] + ".js?v=" + {
-        480: "5228ab589234a2bdb92a",
-        568: "57321689c730e6670738",
+        480: "07e6f878197981be93a5",
+        568: "775df6136673a0d7dba1",
         829: "eddb7a59a74d60740eb9"
-    } [e], b.g = function() {
+    } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyfilite:", b.l = (t, n, i, o) => {
+    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyfilite:", m.l = (t, n, i, o) => {
         if (e[t]) e[t].push(n);
         else {
             var a, l;
             if (void 0 !== i)
-                for (var f = document.getElementsByTagName("script"), u = 0; u < f.length; u++) {
-                    var s = f[u];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + i) {
-                        a = s;
+                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
+                    var f = u[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + i) {
+                        a = f;
                         break
                     }
                 }
-            a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, b.nc && a.setAttribute("nonce", b.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
+            a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, m.nc && a.setAttribute("nonce", m.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
             var d = (r, n) => {
                     a.onerror = a.onload = null, clearTimeout(p);
                     var i = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), i && i.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
             a.onerror = d.bind(null, a.onerror), a.onload = d.bind(null, a.onload), l && document.head.appendChild(a)
         }
     }, (() => {
-        b.S = {};
+        m.S = {};
         var e = {},
             r = {};
-        b.I = (t, n) => {
+        m.I = (t, n) => {
             n || (n = []);
             var i = r[t];
             if (i || (i = r[t] = {}), !(n.indexOf(i) >= 0)) {
                 if (n.push(i), e[t]) return e[t];
-                b.o(b.S, t) || (b.S[t] = {});
-                var o = b.S[t],
+                m.o(m.S, t) || (m.S[t] = {});
+                var o = m.S[t],
                     a = "ipyfilite",
                     l = [];
                 return "default" === t && ((e, r, t, n) => {
                     var i = o[e] = o[e] || {},
                         l = i[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : a > l.from)) && (i[r] = {
-                        get: () => Promise.all([b.e(829), b.e(568)]).then((() => () => b(568))),
+                        get: () => Promise.all([m.e(829), m.e(568)]).then((() => () => m(568))),
                         from: a,
                         eager: !1
                     })
-                })("ipyfilite", "0.1.5"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("ipyfilite", "0.1.6"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        b.g.importScripts && (e = b.g.location + "");
-        var r = b.g.document;
+        m.g.importScripts && (e = m.g.location + "");
+        var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
                 for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -140,131 +140,131 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var a = [];
         for (o = 1; o < e.length; o++) {
             var l = e[o];
-            a.push(0 === l ? "not(" + f() + ")" : 1 === l ? "(" + f() + " || " + f() + ")" : 2 === l ? a.pop() + " " + a.pop() : i(l))
+            a.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? a.pop() + " " + a.pop() : i(l))
         }
-        return f();
+        return u();
 
-        function f() {
+        function u() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 i = n < 0;
             i && (n = -n - 1);
-            for (var a = 0, l = 1, f = !0;; l++, a++) {
-                var u, s, d = l < e.length ? (typeof e[l])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(u = r[a]))[0])) return !f || ("u" == d ? l > n && !i : "" == d != i);
-                if ("u" == s) {
-                    if (!f || "u" != d) return !1
-                } else if (f)
-                    if (d == s)
+            for (var a = 0, l = 1, u = !0;; l++, a++) {
+                var s, f, d = l < e.length ? (typeof e[l])[0] : "";
+                if (a >= r.length || "o" == (f = (typeof(s = r[a]))[0])) return !u || ("u" == d ? l > n && !i : "" == d != i);
+                if ("u" == f) {
+                    if (!u || "u" != d) return !1
+                } else if (u)
+                    if (d == f)
                         if (l <= n) {
-                            if (u != e[l]) return !1
+                            if (s != e[l]) return !1
                         } else {
-                            if (i ? u > e[l] : u < e[l]) return !1;
-                            u != e[l] && (f = !1)
+                            if (i ? s > e[l] : s < e[l]) return !1;
+                            s != e[l] && (u = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (i || l <= n) return !1;
-                    f = !1, l--
+                    u = !1, l--
                 } else {
-                    if (l <= n || s < d != i) return !1;
-                    f = !1
-                } else "s" != d && "n" != d && (f = !1, l--)
+                    if (l <= n || f < d != i) return !1;
+                    u = !1
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, a = (e, r) => {
-        var t = b.S[e];
-        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = m.S[e];
+        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", u = (e, r, t, n) => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", s = (e, r, t, n) => {
         var i = l(e, t);
-        return o(n, i) || s(f(e, t, i, n)), d(e[t][i])
-    }, s = e => {
+        return o(n, i) || f(u(e, t, i, n)), d(e[t][i])
+    }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, i) {
-        var o = b.I(r);
-        return o && o.then ? o.then(e.bind(e, r, b.S[r], t, n, i)) : e(r, b.S[r], t, n)
-    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), c = {}, h = {
+        var o = m.I(r);
+        return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, i)) : e(r, m.S[r], t, n)
+    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), c = {}, h = {
         829: () => p("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1, 1, 1
         ])
     }, v = {
         829: [829]
-    }, b.f.consumes = (e, r) => {
-        b.o(v, e) && v[e].forEach((e => {
-            if (b.o(c, e)) return r.push(c[e]);
+    }, m.f.consumes = (e, r) => {
+        m.o(v, e) && v[e].forEach((e => {
+            if (m.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    c[e] = 0, b.m[e] = t => {
-                        delete b.c[e], t.exports = r()
+                    c[e] = 0, m.m[e] = t => {
+                        delete m.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete c[e], b.m[e] = t => {
-                        throw delete b.c[e], r
+                    delete c[e], m.m[e] = t => {
+                        throw delete m.c[e], r
                     }
                 };
             try {
                 var i = h[e]();
                 i.then ? r.push(c[e] = i.then(t).catch(n)) : t(i)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             430: 0
         };
-        b.f.j = (r, t) => {
-            var n = b.o(e, r) ? e[r] : void 0;
+        m.f.j = (r, t) => {
+            var n = m.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (829 != r) {
                 var i = new Promise(((t, i) => n = e[r] = [t, i]));
                 t.push(n[2] = i);
-                var o = b.p + b.u(r),
+                var o = m.p + m.u(r),
                     a = new Error;
-                b.l(o, (t => {
-                    if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                m.l(o, (t => {
+                    if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                         var i = t && ("load" === t.type ? "missing" : t.type),
                             o = t && t.target && t.target.src;
                         a.message = "Loading chunk " + r + " failed.\n(" + i + ": " + o + ")", a.name = "ChunkLoadError", a.type = i, a.request = o, n[1](a)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
                 var n, i, [o, a, l] = t,
-                    f = 0;
+                    u = 0;
                 if (o.some((r => 0 !== e[r]))) {
-                    for (n in a) b.o(a, n) && (b.m[n] = a[n]);
-                    l && l(b)
+                    for (n in a) m.o(a, n) && (m.m[n] = a[n]);
+                    l && l(m)
                 }
-                for (r && r(t); f < o.length; f++) i = o[f], b.o(e, i) && e[i] && e[i][0](), e[i] = 0
+                for (r && r(t); u < o.length; u++) i = o[u], m.o(e, i) && e[i] && e[i][0](), e[i] = 0
             },
             t = self.webpackChunkipyfilite = self.webpackChunkipyfilite || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), b.nc = void 0;
-    var y = b(229);
+    })(), m.nc = void 0;
+    var y = m(229);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipyfilite = y
 })();
```

### Comparing `ipyfilite-0.1.5/ipyfilite/labextension/static/third-party-licenses.json` & `ipyfilite-0.1.6/ipyfilite/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/ipyfilite/nbextension/index.js` & `ipyfilite-0.1.6/ipyfilite/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -328,15 +328,15 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.5","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.6","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         i = {};
 
     function n(e) {
         var s = i[e];
         if (void 0 !== s) return s.exports;
```

### Comparing `ipyfilite-0.1.5/ipyfilite/nbextension/index.js.map` & `ipyfilite-0.1.6/ipyfilite/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/ipyfilite/tests/conftest.py` & `ipyfilite-0.1.6/ipyfilite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/src/extension.ts` & `ipyfilite-0.1.6/src/extension.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/src/plugin.ts` & `ipyfilite-0.1.6/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/src/version.ts` & `ipyfilite-0.1.6/src/version.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/src/widget.ts` & `ipyfilite-0.1.6/src/widget.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/src/__tests__/index.spec.ts` & `ipyfilite-0.1.6/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/src/__tests__/utils.ts` & `ipyfilite-0.1.6/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/.gitignore` & `ipyfilite-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/LICENSE.txt` & `ipyfilite-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/README.md` & `ipyfilite-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.5/pyproject.toml` & `ipyfilite-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.0.0",
 ]
-version = "0.1.5"
+version = "0.1.6"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
@@ -101,15 +101,15 @@
 ]
 file = [
     { src = "pyproject.toml", version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\"" },
     { src = "ipyfilite/_version.py" },
 ]
 
 [tool.tbump.version]
-current = "0.1.5"
+current = "0.1.6"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [tool.black]
```

### Comparing `ipyfilite-0.1.5/PKG-INFO` & `ipyfilite-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyfilite
-Version: 0.1.5
+Version: 0.1.6
 Summary: File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.
 Project-URL: Homepage, https://github.com/juntyr/ipyfilite
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 License: Copyright (c) 2023 Juniper Tyree
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

