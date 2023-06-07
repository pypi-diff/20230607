# Comparing `tmp/ipyfilite-0.1.4.tar.gz` & `tmp/ipyfilite-0.1.5.tar.gz`

## Comparing `ipyfilite-0.1.4.tar` & `ipyfilite-0.1.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.coveragerc
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.eslintignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.npmignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.prettierignore
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.prettierrc
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/MANIFEST.in
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/babel.config.js
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/codecov.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/install.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/jest.config.js
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/package.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/setup.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/tsconfig.eslint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/tsconfig.json
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/webpack.config.js
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/css/widget.css
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/Makefile
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/environment.yml
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/make.bat
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/conf.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/develop-install.rst
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/index.rst
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/installing.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/introduction.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/_static/helper.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/examples/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/examples/introduction.nblink
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/examples/example.txt
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/examples/introduction.ipynb
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/_frontend.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/_manager.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/_version.py
--rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/http.py
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/upload.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/labextension/package.json
--rw-r--r--   0        0        0    10392 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/labextension/static/480.47fe3e6cc3fce727815a.js
--rw-r--r--   0        0        0     9983 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/labextension/static/568.262a61b30c3863712d2a.js
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/labextension/static/remoteEntry.09a079dacd8ff0810e86.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/nbextension/extension.js
--rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/nbextension/index.js
--rw-r--r--   0        0        0    28799 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/tests/__init__.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/tests/conftest.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/tests/test_upload.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/extension.ts
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/index.ts
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/plugin.ts
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/version.ts
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/widget.ts
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/__tests__/utils.ts
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/README.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.coveragerc
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.eslintignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.npmignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.prettierignore
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.prettierrc
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/MANIFEST.in
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/babel.config.js
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/codecov.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/install.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/jest.config.js
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/package.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/setup.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/tsconfig.eslint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/tsconfig.json
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/webpack.config.js
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/css/widget.css
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/Makefile
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/environment.yml
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/make.bat
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/conf.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/develop-install.rst
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/index.rst
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/installing.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/introduction.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/_static/helper.js
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/examples/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/docs/source/examples/introduction.nblink
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/examples/example.txt
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/examples/introduction.ipynb
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/_frontend.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/_manager.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/_version.py
+-rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/http.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/upload.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/labextension/package.json
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/labextension/static/480.5228ab589234a2bdb92a.js
+-rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/labextension/static/568.57321689c730e6670738.js
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/labextension/static/remoteEntry.392e4ddeb2ce5c2a11f4.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/nbextension/extension.js
+-rw-r--r--   0        0        0    10768 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/nbextension/index.js
+-rw-r--r--   0        0        0    28884 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/tests/__init__.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/tests/conftest.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/ipyfilite/tests/test_upload.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/extension.ts
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/index.ts
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/plugin.ts
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/version.ts
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/widget.ts
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/src/__tests__/utils.ts
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/README.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 ipyfilite-0.1.5/PKG-INFO
```

### Comparing `ipyfilite-0.1.4/.eslintrc.js` & `ipyfilite-0.1.5/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/MANIFEST.in` & `ipyfilite-0.1.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/package.json` & `ipyfilite-0.1.5/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.1.5'"}*

```diff
@@ -87,9 +87,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.4"
+    "version": "0.1.5"
 }
```

### Comparing `ipyfilite-0.1.4/tsconfig.json` & `ipyfilite-0.1.5/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/webpack.config.js` & `ipyfilite-0.1.5/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/docs/Makefile` & `ipyfilite-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/docs/make.bat` & `ipyfilite-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/docs/source/conf.py` & `ipyfilite-0.1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/docs/source/develop-install.rst` & `ipyfilite-0.1.5/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/docs/source/index.rst` & `ipyfilite-0.1.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/docs/source/installing.rst` & `ipyfilite-0.1.5/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/examples/introduction.ipynb` & `ipyfilite-0.1.5/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/ipyfilite/__init__.py` & `ipyfilite-0.1.5/ipyfilite/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/ipyfilite/http.py` & `ipyfilite-0.1.5/ipyfilite/http.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/ipyfilite/upload.py` & `ipyfilite-0.1.5/ipyfilite/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,7 +176,10 @@
         echo_update=False,
         **_value_serialization,
     )
 
     @default("description")
     def _default_description(self):
         return "Upload"
+
+    async def next_value(self):
+        return await IpyfiliteManager.instance().wait_for_upload_value(self)
```

### Comparing `ipyfilite-0.1.4/ipyfilite/labextension/package.json` & `ipyfilite-0.1.5/ipyfilite/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9677734375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.392e4ddeb2ce5c2a11f4.js'}}",*

 * * "'version'": "'0.1.5'"}*

```diff
@@ -46,15 +46,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/juntyr/ipyfilite",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.09a079dacd8ff0810e86.js"
+            "load": "static/remoteEntry.392e4ddeb2ce5c2a11f4.js"
         },
         "extension": "lib/plugin",
         "outputDir": "ipyfilite/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -91,9 +91,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.4"
+    "version": "0.1.5"
 }
```

### Comparing `ipyfilite-0.1.4/ipyfilite/labextension/static/480.47fe3e6cc3fce727815a.js` & `ipyfilite-0.1.5/ipyfilite/labextension/static/480.5228ab589234a2bdb92a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -107,15 +107,16 @@
                                 size: e.size,
                                 last_modified: e.lastModified,
                                 path: `/uploads/${t}/${e.name}`
                             })));
                         r.getBroadcastChannel().postMessage({
                             files: this.fileInput.files,
                             uuid: t,
-                            session: this.model.get("_session")
+                            session: this.model.get("_session"),
+                            widget: this.model.model_id
                         }), this.model.set({
                             value: i
                         }), this.touch()
                     })), this.listenTo(this.model, "change:button_style", this.update_button_style), this.set_button_style(), this.update()
                 }
                 update() {
                     this.el.disabled = this.model.get("disabled"), this.el.setAttribute("title", this.model.get("tooltip"));
@@ -332,11 +333,11 @@
                         i = o
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.4","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.5","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyfilite-0.1.4/ipyfilite/labextension/static/568.262a61b30c3863712d2a.js` & `ipyfilite-0.1.5/ipyfilite/labextension/static/568.57321689c730e6670738.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -79,15 +79,16 @@
                                 size: e.size,
                                 last_modified: e.lastModified,
                                 path: `/uploads/${t}/${e.name}`
                             })));
                         o.getBroadcastChannel().postMessage({
                             files: this.fileInput.files,
                             uuid: t,
-                            session: this.model.get("_session")
+                            session: this.model.get("_session"),
+                            widget: this.model.model_id
                         }), this.model.set({
                             value: i
                         }), this.touch()
                     })), this.listenTo(this.model, "change:button_style", this.update_button_style), this.set_button_style(), this.update()
                 }
                 update() {
                     this.el.disabled = this.model.get("disabled"), this.el.setAttribute("title", this.model.get("tooltip"));
@@ -304,11 +305,11 @@
                         i = r
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.4","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.5","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyfilite-0.1.4/ipyfilite/labextension/static/remoteEntry.09a079dacd8ff0810e86.js` & `ipyfilite-0.1.5/ipyfilite/labextension/static/remoteEntry.392e4ddeb2ce5c2a11f4.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, i, o, a, f, l, u, s, p, d, c, h, v, g = {
+    var e, r, t, n, i, o, a, l, f, u, s, d, p, c, h, v, g = {
             229: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(829), t.e(568)]).then((() => () => t(568))),
                         "./extension": () => Promise.all([t.e(829), t.e(480)]).then((() => () => t(480)))
                     },
                     i = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -37,74 +37,74 @@
     }
     b.m = g, b.c = m, b.d = (e, r) => {
         for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
-        480: "47fe3e6cc3fce727815a",
-        568: "262a61b30c3863712d2a",
-        829: "989f6f56f2a9f465e0c8"
+        480: "5228ab589234a2bdb92a",
+        568: "57321689c730e6670738",
+        829: "eddb7a59a74d60740eb9"
     } [e] + ".js?v=" + {
-        480: "47fe3e6cc3fce727815a",
-        568: "262a61b30c3863712d2a",
-        829: "989f6f56f2a9f465e0c8"
+        480: "5228ab589234a2bdb92a",
+        568: "57321689c730e6670738",
+        829: "eddb7a59a74d60740eb9"
     } [e], b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyfilite:", b.l = (t, n, i, o) => {
         if (e[t]) e[t].push(n);
         else {
-            var a, f;
+            var a, l;
             if (void 0 !== i)
-                for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
-                    var s = l[u];
+                for (var f = document.getElementsByTagName("script"), u = 0; u < f.length; u++) {
+                    var s = f[u];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + i) {
                         a = s;
                         break
                     }
                 }
-            a || (f = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, b.nc && a.setAttribute("nonce", b.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
-            var p = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(d);
+            a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, b.nc && a.setAttribute("nonce", b.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
+            var d = (r, n) => {
+                    a.onerror = a.onload = null, clearTimeout(p);
                     var i = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), i && i.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(p.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
-            a.onerror = p.bind(null, a.onerror), a.onload = p.bind(null, a.onload), f && document.head.appendChild(a)
+            a.onerror = d.bind(null, a.onerror), a.onload = d.bind(null, a.onload), l && document.head.appendChild(a)
         }
     }, (() => {
         b.S = {};
         var e = {},
             r = {};
         b.I = (t, n) => {
             n || (n = []);
             var i = r[t];
             if (i || (i = r[t] = {}), !(n.indexOf(i) >= 0)) {
                 if (n.push(i), e[t]) return e[t];
                 b.o(b.S, t) || (b.S[t] = {});
                 var o = b.S[t],
                     a = "ipyfilite",
-                    f = [];
+                    l = [];
                 return "default" === t && ((e, r, t, n) => {
                     var i = o[e] = o[e] || {},
-                        f = i[r];
-                    (!f || !f.loaded && (1 != !f.eager ? n : a > f.from)) && (i[r] = {
+                        l = i[r];
+                    (!l || !l.loaded && (1 != !l.eager ? n : a > l.from)) && (i[r] = {
                         get: () => Promise.all([b.e(829), b.e(568)]).then((() => () => b(568))),
                         from: a,
                         eager: !1
                     })
-                })("ipyfilite", "0.1.4"), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
+                })("ipyfilite", "0.1.5"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         b.g.importScripts && (e = b.g.location + "");
         var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -123,90 +123,90 @@
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var i = e[n],
                 o = (typeof i)[0];
             if (n >= r.length) return "u" == o;
             var a = r[n],
-                f = (typeof a)[0];
-            if (o != f) return "o" == o && "n" == f || "s" == f || "u" == o;
+                l = (typeof a)[0];
+            if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
             if ("o" != o && "u" != o && i != a) return i < a;
             n++
         }
     }, i = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(f = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, f);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var a = [];
         for (o = 1; o < e.length; o++) {
-            var f = e[o];
-            a.push(0 === f ? "not(" + l() + ")" : 1 === f ? "(" + l() + " || " + l() + ")" : 2 === f ? a.pop() + " " + a.pop() : i(f))
+            var l = e[o];
+            a.push(0 === l ? "not(" + f() + ")" : 1 === l ? "(" + f() + " || " + f() + ")" : 2 === l ? a.pop() + " " + a.pop() : i(l))
         }
-        return l();
+        return f();
 
-        function l() {
+        function f() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 i = n < 0;
             i && (n = -n - 1);
-            for (var a = 0, f = 1, l = !0;; f++, a++) {
-                var u, s, p = f < e.length ? (typeof e[f])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(u = r[a]))[0])) return !l || ("u" == p ? f > n && !i : "" == p != i);
+            for (var a = 0, l = 1, f = !0;; l++, a++) {
+                var u, s, d = l < e.length ? (typeof e[l])[0] : "";
+                if (a >= r.length || "o" == (s = (typeof(u = r[a]))[0])) return !f || ("u" == d ? l > n && !i : "" == d != i);
                 if ("u" == s) {
-                    if (!l || "u" != p) return !1
-                } else if (l)
-                    if (p == s)
-                        if (f <= n) {
-                            if (u != e[f]) return !1
+                    if (!f || "u" != d) return !1
+                } else if (f)
+                    if (d == s)
+                        if (l <= n) {
+                            if (u != e[l]) return !1
                         } else {
-                            if (i ? u > e[f] : u < e[f]) return !1;
-                            u != e[f] && (l = !1)
+                            if (i ? u > e[l] : u < e[l]) return !1;
+                            u != e[l] && (f = !1)
                         }
-                else if ("s" != p && "n" != p) {
-                    if (i || f <= n) return !1;
-                    l = !1, f--
+                else if ("s" != d && "n" != d) {
+                    if (i || l <= n) return !1;
+                    f = !1, l--
                 } else {
-                    if (f <= n || s < p != i) return !1;
-                    l = !1
-                } else "s" != p && "n" != p && (l = !1, f--)
+                    if (l <= n || s < d != i) return !1;
+                    f = !1
+                } else "s" != d && "n" != d && (f = !1, l--)
             }
         }
-        var d = [],
-            c = d.pop.bind(d);
+        var p = [],
+            c = p.pop.bind(p);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
-            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, a = (e, r) => {
         var t = b.S[e];
         if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, f = (e, r) => {
+    }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", u = (e, r, t, n) => {
-        var i = f(e, t);
-        return o(n, i) || s(l(e, t, i, n)), p(e[t][i])
+    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", u = (e, r, t, n) => {
+        var i = l(e, t);
+        return o(n, i) || s(f(e, t, i, n)), d(e[t][i])
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, i) {
+    }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, i) {
         var o = b.I(r);
         return o && o.then ? o.then(e.bind(e, r, b.S[r], t, n, i)) : e(r, b.S[r], t, n)
     })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), c = {}, h = {
-        829: () => d("default", "@jupyter-widgets/base", [, [1, 6],
+        829: () => p("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1, 1, 1
         ])
     }, v = {
@@ -250,21 +250,21 @@
                             o = t && t.target && t.target.src;
                         a.message = "Loading chunk " + r + " failed.\n(" + i + ": " + o + ")", a.name = "ChunkLoadError", a.type = i, a.request = o, n[1](a)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, i, [o, a, f] = t,
-                    l = 0;
+                var n, i, [o, a, l] = t,
+                    f = 0;
                 if (o.some((r => 0 !== e[r]))) {
                     for (n in a) b.o(a, n) && (b.m[n] = a[n]);
-                    f && f(b)
+                    l && l(b)
                 }
-                for (r && r(t); l < o.length; l++) i = o[l], b.o(e, i) && e[i] && e[i][0](), e[i] = 0
+                for (r && r(t); f < o.length; f++) i = o[f], b.o(e, i) && e[i] && e[i][0](), e[i] = 0
             },
             t = self.webpackChunkipyfilite = self.webpackChunkipyfilite || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), b.nc = void 0;
     var y = b(229);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipyfilite = y
 })();
```

### Comparing `ipyfilite-0.1.4/ipyfilite/labextension/static/third-party-licenses.json` & `ipyfilite-0.1.5/ipyfilite/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/ipyfilite/nbextension/index.js` & `ipyfilite-0.1.5/ipyfilite/nbextension/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -79,27 +79,27 @@
                         } return t
                 }
 
                 function o(e, t) {
                     for (var i = {}, n = [], s = 0; s < e.length; s++) {
                         var o = e[s],
                             l = t.base ? o[0] + t.base : o[0],
-                            u = i[l] || 0,
-                            d = "".concat(l, " ").concat(u);
-                        i[l] = u + 1;
-                        var c = a(d),
+                            d = i[l] || 0,
+                            u = "".concat(l, " ").concat(d);
+                        i[l] = d + 1;
+                        var c = a(u),
                             p = {
                                 css: o[1],
                                 media: o[2],
                                 sourceMap: o[3]
                             }; - 1 !== c ? (r[c].references++, r[c].updater(p)) : r.push({
-                            identifier: d,
+                            identifier: u,
                             updater: m(p, t),
                             references: 1
-                        }), n.push(d)
+                        }), n.push(u)
                     }
                     return n
                 }
 
                 function l(e) {
                     var t = document.createElement("style"),
                         n = e.attributes || {};
@@ -113,21 +113,21 @@
                     else {
                         var a = s(e.insert || "head");
                         if (!a) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                         a.appendChild(t)
                     }
                     return t
                 }
-                var u, d = (u = [], function(e, t) {
-                    return u[e] = t, u.filter(Boolean).join("\n")
+                var d, u = (d = [], function(e, t) {
+                    return d[e] = t, d.filter(Boolean).join("\n")
                 });
 
                 function c(e, t, i, n) {
                     var s = i ? "" : n.media ? "@media ".concat(n.media, " {").concat(n.css, "}") : n.css;
-                    if (e.styleSheet) e.styleSheet.cssText = d(t, s);
+                    if (e.styleSheet) e.styleSheet.cssText = u(t, s);
                     else {
                         var r = document.createTextNode(s),
                             a = e.childNodes;
                         a[t] && e.removeChild(a[t]), a.length ? e.insertBefore(r, a[t]) : e.appendChild(r)
                     }
                 }
 
@@ -168,17 +168,17 @@
                     var i = o(e = e || [], t);
                     return function(e) {
                         if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
                             for (var n = 0; n < i.length; n++) {
                                 var s = a(i[n]);
                                 r[s].references--
                             }
-                            for (var l = o(e, t), u = 0; u < i.length; u++) {
-                                var d = a(i[u]);
-                                0 === r[d].references && (r[d].updater(), r.splice(d, 1))
+                            for (var l = o(e, t), d = 0; d < i.length; d++) {
+                                var u = a(i[d]);
+                                0 === r[u].references && (r[u].updater(), r.splice(u, 1))
                             }
                             i = l
                         }
                     }
                 }
             },
             112: function(e, t, i) {
@@ -279,15 +279,16 @@
                                     size: e.size,
                                     last_modified: e.lastModified,
                                     path: `/uploads/${t}/${e.name}`
                                 })));
                             o.getBroadcastChannel().postMessage({
                                 files: this.fileInput.files,
                                 uuid: t,
-                                session: this.model.get("_session")
+                                session: this.model.get("_session"),
+                                widget: this.model.model_id
                             }), this.model.set({
                                 value: i
                             }), this.touch()
                         })), this.listenTo(this.model, "change:button_style", this.update_button_style), this.set_button_style(), this.update()
                     }
                     update() {
                         this.el.disabled = this.model.get("disabled"), this.el.setAttribute("title", this.model.get("tooltip"));
@@ -327,15 +328,15 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.4","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.5","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         i = {};
 
     function n(e) {
         var s = i[e];
         if (void 0 !== s) return s.exports;
```

### Comparing `ipyfilite-0.1.4/ipyfilite/nbextension/index.js.map` & `ipyfilite-0.1.5/ipyfilite/nbextension/index.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.916875204003917%*

 * *Differences: {"'mappings'": "'iEAEAA,EADkC,EAAQ,IAChCC,EAA4B,IAE9BC,KAAK,CAACC,EAAOC,GAAI,iFAAkF,KAE3GD,EAAOH,QAAUA,C,uBCEjBG,EAAOH,QAAU,SAAUK,GACzB,IAAIC,EAAO,GAuDX,OArDAA,EAAKC,SAAW,WACd,OAAOC,KAAKC,KAAI,SAAUC,GACxB,IAAIC,EAsDV,SAAgCD,EAAML,GACpC,IAoBiBO,EAEbC,EACAC,EAvBAH,EAAUD,EAAK,IAAM,GAErBK,EAAaL,EAAK,GAEtB,IAAKK,EACH,OAAOJ,EAGT,GAAIN,GAAgC,mBAATW,KAAqB,CAC9C,IAAIC,GAWWL,EAXeG,EAa5BF,EAASG,KAAKE,SAASC,mBAAmBC,KAAKC,UAAUT,MACzDE,EAAO,+DAA+DQ,OAAOT,GAC1E,OAAOS,OAAOR,EAAM,QAdrBS,EAAaR,EAAWS,QAAQf,KAAI,SAAUgB,GAChD,M […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "index.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "exports",
         "___CSS_LOADER_API_IMPORT___",
         "push",
         "module",
         "id",
         "useSourceMap",
@@ -174,14 +174,16 @@
         "path",
         "Private",
         "getBroadcastChannel",
         "postMessage",
         "session",
         "model",
         "get",
+        "widget",
+        "model_id",
         "set",
         "touch",
         "listenTo",
         "update_button_style",
         "set_button_style",
         "textContent",
         "update_mapped_classes",
@@ -222,15 +224,15 @@
         "// Imports\nvar ___CSS_LOADER_API_IMPORT___ = require(\"../node_modules/css-loader/dist/runtime/api.js\");\nexports = ___CSS_LOADER_API_IMPORT___(false);\n// Module\nexports.push([module.id, \".custom-widget {\\n  background-color: lightseagreen;\\n  padding: 0px 2px;\\n}\\n\", \"\"]);\n// Exports\nmodule.exports = exports;\n",
         "\"use strict\";\n\n/*\n  MIT License http://www.opensource.org/licenses/mit-license.php\n  Author Tobias Koppers @sokra\n*/\n// css base code, injected by the css-loader\n// eslint-disable-next-line func-names\nmodule.exports = function (useSourceMap) {\n  var list = []; // return the list of modules as css string\n\n  list.toString = function toString() {\n    return this.map(function (item) {\n      var content = cssWithMappingToString(item, useSourceMap);\n\n      if (item[2]) {\n        return \"@media \".concat(item[2], \" {\").concat(content, \"}\");\n      }\n\n      return content;\n    }).join('');\n  }; // import a list of modules into the list\n  // eslint-disable-next-line func-names\n\n\n  list.i = function (modules, mediaQuery, dedupe) {\n    if (typeof modules === 'string') {\n      // eslint-disable-next-line no-param-reassign\n      modules = [[null, modules, '']];\n    }\n\n    var alreadyImportedModules = {};\n\n    if (dedupe) {\n      for (var i = 0; i < this.length; i++) {\n        // eslint-disable-next-line prefer-destructuring\n        var id = this[i][0];\n\n        if (id != null) {\n          alreadyImportedModules[id] = true;\n        }\n      }\n    }\n\n    for (var _i = 0; _i < modules.length; _i++) {\n      var item = [].concat(modules[_i]);\n\n      if (dedupe && alreadyImportedModules[item[0]]) {\n        // eslint-disable-next-line no-continue\n        continue;\n      }\n\n      if (mediaQuery) {\n        if (!item[2]) {\n          item[2] = mediaQuery;\n        } else {\n          item[2] = \"\".concat(mediaQuery, \" and \").concat(item[2]);\n        }\n      }\n\n      list.push(item);\n    }\n  };\n\n  return list;\n};\n\nfunction cssWithMappingToString(item, useSourceMap) {\n  var content = item[1] || ''; // eslint-disable-next-line prefer-destructuring\n\n  var cssMapping = item[3];\n\n  if (!cssMapping) {\n    return content;\n  }\n\n  if (useSourceMap && typeof btoa === 'function') {\n    var sourceMapping = toComment(cssMapping);\n    var sourceURLs = cssMapping.sources.map(function (source) {\n      return \"/*# sourceURL=\".concat(cssMapping.sourceRoot || '').concat(source, \" */\");\n    });\n    return [content].concat(sourceURLs).concat([sourceMapping]).join('\\n');\n  }\n\n  return [content].join('\\n');\n} // Adapted from convert-source-map (MIT)\n\n\nfunction toComment(sourceMap) {\n  // eslint-disable-next-line no-undef\n  var base64 = btoa(unescape(encodeURIComponent(JSON.stringify(sourceMap))));\n  var data = \"sourceMappingURL=data:application/json;charset=utf-8;base64,\".concat(base64);\n  return \"/*# \".concat(data, \" */\");\n}",
         "var api = require(\"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\");\n            var content = require(\"!!../node_modules/css-loader/dist/cjs.js!./widget.css\");\n\n            content = content.__esModule ? content.default : content;\n\n            if (typeof content === 'string') {\n              content = [[module.id, content, '']];\n            }\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nmodule.exports = content.locals || {};",
         "\"use strict\";\n\nvar isOldIE = function isOldIE() {\n  var memo;\n  return function memorize() {\n    if (typeof memo === 'undefined') {\n      // Test for IE <= 9 as proposed by Browserhacks\n      // @see http://browserhacks.com/#hack-e71d8692f65334173fee715c222cb805\n      // Tests for existence of standard globals is to allow style-loader\n      // to operate correctly into non-standard environments\n      // @see https://github.com/webpack-contrib/style-loader/issues/177\n      memo = Boolean(window && document && document.all && !window.atob);\n    }\n\n    return memo;\n  };\n}();\n\nvar getTarget = function getTarget() {\n  var memo = {};\n  return function memorize(target) {\n    if (typeof memo[target] === 'undefined') {\n      var styleTarget = document.querySelector(target); // Special case to return head of iframe instead of iframe itself\n\n      if (window.HTMLIFrameElement && styleTarget instanceof window.HTMLIFrameElement) {\n        try {\n          // This will throw an exception if access to iframe is blocked\n          // due to cross-origin restrictions\n          styleTarget = styleTarget.contentDocument.head;\n        } catch (e) {\n          // istanbul ignore next\n          styleTarget = null;\n        }\n      }\n\n      memo[target] = styleTarget;\n    }\n\n    return memo[target];\n  };\n}();\n\nvar stylesInDom = [];\n\nfunction getIndexByIdentifier(identifier) {\n  var result = -1;\n\n  for (var i = 0; i < stylesInDom.length; i++) {\n    if (stylesInDom[i].identifier === identifier) {\n      result = i;\n      break;\n    }\n  }\n\n  return result;\n}\n\nfunction modulesToDom(list, options) {\n  var idCountMap = {};\n  var identifiers = [];\n\n  for (var i = 0; i < list.length; i++) {\n    var item = list[i];\n    var id = options.base ? item[0] + options.base : item[0];\n    var count = idCountMap[id] || 0;\n    var identifier = \"\".concat(id, \" \").concat(count);\n    idCountMap[id] = count + 1;\n    var index = getIndexByIdentifier(identifier);\n    var obj = {\n      css: item[1],\n      media: item[2],\n      sourceMap: item[3]\n    };\n\n    if (index !== -1) {\n      stylesInDom[index].references++;\n      stylesInDom[index].updater(obj);\n    } else {\n      stylesInDom.push({\n        identifier: identifier,\n        updater: addStyle(obj, options),\n        references: 1\n      });\n    }\n\n    identifiers.push(identifier);\n  }\n\n  return identifiers;\n}\n\nfunction insertStyleElement(options) {\n  var style = document.createElement('style');\n  var attributes = options.attributes || {};\n\n  if (typeof attributes.nonce === 'undefined') {\n    var nonce = typeof __webpack_nonce__ !== 'undefined' ? __webpack_nonce__ : null;\n\n    if (nonce) {\n      attributes.nonce = nonce;\n    }\n  }\n\n  Object.keys(attributes).forEach(function (key) {\n    style.setAttribute(key, attributes[key]);\n  });\n\n  if (typeof options.insert === 'function') {\n    options.insert(style);\n  } else {\n    var target = getTarget(options.insert || 'head');\n\n    if (!target) {\n      throw new Error(\"Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.\");\n    }\n\n    target.appendChild(style);\n  }\n\n  return style;\n}\n\nfunction removeStyleElement(style) {\n  // istanbul ignore if\n  if (style.parentNode === null) {\n    return false;\n  }\n\n  style.parentNode.removeChild(style);\n}\n/* istanbul ignore next  */\n\n\nvar replaceText = function replaceText() {\n  var textStore = [];\n  return function replace(index, replacement) {\n    textStore[index] = replacement;\n    return textStore.filter(Boolean).join('\\n');\n  };\n}();\n\nfunction applyToSingletonTag(style, index, remove, obj) {\n  var css = remove ? '' : obj.media ? \"@media \".concat(obj.media, \" {\").concat(obj.css, \"}\") : obj.css; // For old IE\n\n  /* istanbul ignore if  */\n\n  if (style.styleSheet) {\n    style.styleSheet.cssText = replaceText(index, css);\n  } else {\n    var cssNode = document.createTextNode(css);\n    var childNodes = style.childNodes;\n\n    if (childNodes[index]) {\n      style.removeChild(childNodes[index]);\n    }\n\n    if (childNodes.length) {\n      style.insertBefore(cssNode, childNodes[index]);\n    } else {\n      style.appendChild(cssNode);\n    }\n  }\n}\n\nfunction applyToTag(style, options, obj) {\n  var css = obj.css;\n  var media = obj.media;\n  var sourceMap = obj.sourceMap;\n\n  if (media) {\n    style.setAttribute('media', media);\n  } else {\n    style.removeAttribute('media');\n  }\n\n  if (sourceMap && typeof btoa !== 'undefined') {\n    css += \"\\n/*# sourceMappingURL=data:application/json;base64,\".concat(btoa(unescape(encodeURIComponent(JSON.stringify(sourceMap)))), \" */\");\n  } // For old IE\n\n  /* istanbul ignore if  */\n\n\n  if (style.styleSheet) {\n    style.styleSheet.cssText = css;\n  } else {\n    while (style.firstChild) {\n      style.removeChild(style.firstChild);\n    }\n\n    style.appendChild(document.createTextNode(css));\n  }\n}\n\nvar singleton = null;\nvar singletonCounter = 0;\n\nfunction addStyle(obj, options) {\n  var style;\n  var update;\n  var remove;\n\n  if (options.singleton) {\n    var styleIndex = singletonCounter++;\n    style = singleton || (singleton = insertStyleElement(options));\n    update = applyToSingletonTag.bind(null, style, styleIndex, false);\n    remove = applyToSingletonTag.bind(null, style, styleIndex, true);\n  } else {\n    style = insertStyleElement(options);\n    update = applyToTag.bind(null, style, options);\n\n    remove = function remove() {\n      removeStyleElement(style);\n    };\n  }\n\n  update(obj);\n  return function updateStyle(newObj) {\n    if (newObj) {\n      if (newObj.css === obj.css && newObj.media === obj.media && newObj.sourceMap === obj.sourceMap) {\n        return;\n      }\n\n      update(obj = newObj);\n    } else {\n      remove();\n    }\n  };\n}\n\nmodule.exports = function (list, options) {\n  options = options || {}; // Force single-tag solution on IE6-9, which has a hard limit on the # of <style>\n  // tags it will allow on a page\n\n  if (!options.singleton && typeof options.singleton !== 'boolean') {\n    options.singleton = isOldIE();\n  }\n\n  list = list || [];\n  var lastIdentifiers = modulesToDom(list, options);\n  return function update(newList) {\n    newList = newList || [];\n\n    if (Object.prototype.toString.call(newList) !== '[object Array]') {\n      return;\n    }\n\n    for (var i = 0; i < lastIdentifiers.length; i++) {\n      var identifier = lastIdentifiers[i];\n      var index = getIndexByIdentifier(identifier);\n      stylesInDom[index].references--;\n    }\n\n    var newLastIdentifiers = modulesToDom(newList, options);\n\n    for (var _i = 0; _i < lastIdentifiers.length; _i++) {\n      var _identifier = lastIdentifiers[_i];\n\n      var _index = getIndexByIdentifier(_identifier);\n\n      if (stylesInDom[_index].references === 0) {\n        stylesInDom[_index].updater();\n\n        stylesInDom.splice(_index, 1);\n      }\n    }\n\n    lastIdentifiers = newLastIdentifiers;\n  };\n};",
         "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\n\n// Entry point for the notebook bundle containing custom model definitions.\n//\n// Setup notebook base URL\n//\n// Some static assets may be required by the custom widget javascript. The base\n// url for the notebook is not known at build time and is therefore computed\n// dynamically.\n// eslint-disable-next-line @typescript-eslint/no-non-null-assertion\n(window as any).__webpack_public_path__ =\n  document.querySelector('body')!.getAttribute('data-base-url') +\n  'nbextensions/ipyfilite';\n\nexport * from './index';\n",
         "// Copyright (c) Juniper Tyree\n// Distributed under the terms of the Modified BSD License.\n\nexport * from './version';\nexport * from './widget';\n",
         "// Copyright (c) Juniper Tyree\n// Distributed under the terms of the Modified BSD License.\n\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexport const MODULE_VERSION = data.version;\n\n/*\n * The current package name.\n */\nexport const MODULE_NAME = data.name;\n",
-        "// Copyright (c) Juniper Tyree\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n  uuid as uuidv4,\n} from '@jupyter-widgets/base';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n\n// Import the CSS\nimport '../css/widget.css';\n\ninterface IFileUploaded {\n  name: string;\n  size: number;\n  type: string;\n  last_modified: number;\n  path: string;\n}\n\nexport class FileUploadLiteModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: FileUploadLiteModel.model_name,\n      _model_module: FileUploadLiteModel.model_module,\n      _model_module_version: FileUploadLiteModel.model_module_version,\n      _view_name: FileUploadLiteModel.view_name,\n      _view_module: FileUploadLiteModel.view_module,\n      _view_module_version: FileUploadLiteModel.view_module_version,\n      _session: uuidv4(),\n      accept: '',\n      description: 'Upload',\n      disabled: false,\n      icon: 'upload',\n      button_style: '',\n      multiple: false,\n      value: [], // has type Array<IFileUploaded>\n      style: null,\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // use a dummy serializer for value to circumvent the default serializer.\n    value: { serialize: <T>(x: T): T => x },\n  };\n\n  static model_name = 'FileUploadLiteModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'FileUploadLiteView';\n  static view_module = MODULE_NAME;\n  static view_module_version = MODULE_VERSION;\n}\n\nexport class FileUploadLiteView extends DOMWidgetView {\n  el: HTMLButtonElement;\n  fileInput: HTMLInputElement;\n\n  preinitialize() {\n    // Must set this before the initialize method creates the element\n    this.tagName = 'button';\n  }\n\n  render(): void {\n    super.render();\n\n    this.el.classList.add('jupyter-widgets');\n    this.el.classList.add('widget-upload-lite');\n    this.el.classList.add('jupyter-button');\n\n    this.fileInput = document.createElement('input');\n    this.fileInput.type = 'file';\n    this.fileInput.style.display = 'none';\n\n    this.el.addEventListener('click', () => {\n      this.fileInput.click();\n    });\n\n    this.fileInput.addEventListener('click', () => {\n      this.fileInput.value = '';\n    });\n\n    this.fileInput.addEventListener('change', () => {\n      const uuid: string = uuidv4();\n\n      const files: Array<IFileUploaded> = Array.from(\n        this.fileInput.files ?? []\n      ).map((file: File) => {\n        return {\n          name: file.name,\n          type: file.type,\n          size: file.size,\n          last_modified: file.lastModified,\n          path: `/uploads/${uuid}/${file.name}`,\n        };\n      });\n\n      Private.getBroadcastChannel().postMessage({\n        files: this.fileInput.files,\n        uuid,\n        session: this.model.get('_session'),\n      });\n\n      this.model.set({\n        value: files,\n      });\n      this.touch();\n    });\n\n    this.listenTo(this.model, 'change:button_style', this.update_button_style);\n    this.set_button_style();\n    this.update(); // Set defaults.\n  }\n\n  update(): void {\n    this.el.disabled = this.model.get('disabled');\n    this.el.setAttribute('title', this.model.get('tooltip'));\n\n    const value: [] = this.model.get('value');\n    const description = `${this.model.get('description')} (${value.length})`;\n    const icon = this.model.get('icon');\n\n    if (description.length || icon.length) {\n      this.el.textContent = '';\n      if (icon.length) {\n        const i = document.createElement('i');\n        i.classList.add('fa');\n        i.classList.add('fa-' + icon);\n        if (description.length === 0) {\n          i.classList.add('center');\n        }\n        this.el.appendChild(i);\n      }\n      this.el.appendChild(document.createTextNode(description));\n    }\n\n    this.fileInput.accept = this.model.get('accept');\n    this.fileInput.multiple = this.model.get('multiple');\n\n    return super.update();\n  }\n\n  update_button_style(): void {\n    this.update_mapped_classes(\n      FileUploadLiteView.class_map,\n      'button_style',\n      this.el\n    );\n  }\n\n  set_button_style(): void {\n    this.set_mapped_classes(\n      FileUploadLiteView.class_map,\n      'button_style',\n      this.el\n    );\n  }\n\n  static class_map = {\n    primary: ['mod-primary'],\n    success: ['mod-success'],\n    info: ['mod-info'],\n    warning: ['mod-warning'],\n    danger: ['mod-danger'],\n  };\n}\n\nnamespace Private {\n  const _channel = new BroadcastChannel('ipyfilite');\n\n  export function getBroadcastChannel(): BroadcastChannel {\n    return _channel;\n  }\n}\n",
+        "// Copyright (c) Juniper Tyree\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n  uuid as uuidv4,\n} from '@jupyter-widgets/base';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n\n// Import the CSS\nimport '../css/widget.css';\n\ninterface IFileUploaded {\n  name: string;\n  size: number;\n  type: string;\n  last_modified: number;\n  path: string;\n}\n\nexport class FileUploadLiteModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: FileUploadLiteModel.model_name,\n      _model_module: FileUploadLiteModel.model_module,\n      _model_module_version: FileUploadLiteModel.model_module_version,\n      _view_name: FileUploadLiteModel.view_name,\n      _view_module: FileUploadLiteModel.view_module,\n      _view_module_version: FileUploadLiteModel.view_module_version,\n      _session: uuidv4(),\n      accept: '',\n      description: 'Upload',\n      disabled: false,\n      icon: 'upload',\n      button_style: '',\n      multiple: false,\n      value: [], // has type Array<IFileUploaded>\n      style: null,\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // use a dummy serializer for value to circumvent the default serializer.\n    value: { serialize: <T>(x: T): T => x },\n  };\n\n  static model_name = 'FileUploadLiteModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'FileUploadLiteView';\n  static view_module = MODULE_NAME;\n  static view_module_version = MODULE_VERSION;\n}\n\nexport class FileUploadLiteView extends DOMWidgetView {\n  el: HTMLButtonElement;\n  fileInput: HTMLInputElement;\n\n  preinitialize() {\n    // Must set this before the initialize method creates the element\n    this.tagName = 'button';\n  }\n\n  render(): void {\n    super.render();\n\n    this.el.classList.add('jupyter-widgets');\n    this.el.classList.add('widget-upload-lite');\n    this.el.classList.add('jupyter-button');\n\n    this.fileInput = document.createElement('input');\n    this.fileInput.type = 'file';\n    this.fileInput.style.display = 'none';\n\n    this.el.addEventListener('click', () => {\n      this.fileInput.click();\n    });\n\n    this.fileInput.addEventListener('click', () => {\n      this.fileInput.value = '';\n    });\n\n    this.fileInput.addEventListener('change', () => {\n      const uuid: string = uuidv4();\n\n      const files: Array<IFileUploaded> = Array.from(\n        this.fileInput.files ?? []\n      ).map((file: File) => {\n        return {\n          name: file.name,\n          type: file.type,\n          size: file.size,\n          last_modified: file.lastModified,\n          path: `/uploads/${uuid}/${file.name}`,\n        };\n      });\n\n      Private.getBroadcastChannel().postMessage({\n        files: this.fileInput.files,\n        uuid,\n        session: this.model.get('_session'),\n        widget: this.model.model_id,\n      });\n\n      this.model.set({\n        value: files,\n      });\n      this.touch();\n    });\n\n    this.listenTo(this.model, 'change:button_style', this.update_button_style);\n    this.set_button_style();\n    this.update(); // Set defaults.\n  }\n\n  update(): void {\n    this.el.disabled = this.model.get('disabled');\n    this.el.setAttribute('title', this.model.get('tooltip'));\n\n    const value: [] = this.model.get('value');\n    const description = `${this.model.get('description')} (${value.length})`;\n    const icon = this.model.get('icon');\n\n    if (description.length || icon.length) {\n      this.el.textContent = '';\n      if (icon.length) {\n        const i = document.createElement('i');\n        i.classList.add('fa');\n        i.classList.add('fa-' + icon);\n        if (description.length === 0) {\n          i.classList.add('center');\n        }\n        this.el.appendChild(i);\n      }\n      this.el.appendChild(document.createTextNode(description));\n    }\n\n    this.fileInput.accept = this.model.get('accept');\n    this.fileInput.multiple = this.model.get('multiple');\n\n    return super.update();\n  }\n\n  update_button_style(): void {\n    this.update_mapped_classes(\n      FileUploadLiteView.class_map,\n      'button_style',\n      this.el\n    );\n  }\n\n  set_button_style(): void {\n    this.set_mapped_classes(\n      FileUploadLiteView.class_map,\n      'button_style',\n      this.el\n    );\n  }\n\n  static class_map = {\n    primary: ['mod-primary'],\n    success: ['mod-success'],\n    info: ['mod-info'],\n    warning: ['mod-warning'],\n    danger: ['mod-danger'],\n  };\n}\n\nnamespace Private {\n  const _channel = new BroadcastChannel('ipyfilite');\n\n  export function getBroadcastChannel(): BroadcastChannel {\n    return _channel;\n  }\n}\n",
         "module.exports = __WEBPACK_EXTERNAL_MODULE__146__;",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n",
         "__webpack_require__.nc = undefined;",
         "// startup\n// Load entry module and return exports\n// This entry module is referenced by other modules so it can't be inlined\nvar __webpack_exports__ = __webpack_require__(112);\n"
     ],
     "version": 3
 }
```

### Comparing `ipyfilite-0.1.4/ipyfilite/tests/conftest.py` & `ipyfilite-0.1.5/ipyfilite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/src/extension.ts` & `ipyfilite-0.1.5/src/extension.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/src/plugin.ts` & `ipyfilite-0.1.5/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/src/version.ts` & `ipyfilite-0.1.5/src/version.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/src/widget.ts` & `ipyfilite-0.1.5/src/widget.ts`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         };
       });
 
       Private.getBroadcastChannel().postMessage({
         files: this.fileInput.files,
         uuid,
         session: this.model.get('_session'),
+        widget: this.model.model_id,
       });
 
       this.model.set({
         value: files,
       });
       this.touch();
     });
```

### Comparing `ipyfilite-0.1.4/src/__tests__/index.spec.ts` & `ipyfilite-0.1.5/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/src/__tests__/utils.ts` & `ipyfilite-0.1.5/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/.gitignore` & `ipyfilite-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/LICENSE.txt` & `ipyfilite-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.4/README.md` & `ipyfilite-0.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -86,7 +86,12 @@
 By default it will also create a tag.
 
 ```bash
 pip install tbump
 tbump <new-version>
 ```
 
+## Funding
+
+`ipyfilite` has been developed as part of [ESiWACE3](https://www.esiwace.eu), the third phase of the Centre of Excellence in Simulation of Weather and Climate in Europe.
+
+Funded by the European Union. This work has received funding from the European High Performance Computing Joint Undertaking (JU) under grant agreement No 101093054.
```

### Comparing `ipyfilite-0.1.4/pyproject.toml` & `ipyfilite-0.1.5/pyproject.toml`

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
-version = "0.1.4"
+version = "0.1.5"
 
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
-current = "0.1.4"
+current = "0.1.5"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [tool.black]
```

### Comparing `ipyfilite-0.1.4/PKG-INFO` & `ipyfilite-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyfilite
-Version: 0.1.4
+Version: 0.1.5
 Summary: File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.
 Project-URL: Homepage, https://github.com/juntyr/ipyfilite
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 License: Copyright (c) 2023 Juniper Tyree
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -154,7 +154,12 @@
 By default it will also create a tag.
 
 ```bash
 pip install tbump
 tbump <new-version>
 ```
 
+## Funding
+
+`ipyfilite` has been developed as part of [ESiWACE3](https://www.esiwace.eu), the third phase of the Centre of Excellence in Simulation of Weather and Climate in Europe.
+
+Funded by the European Union. This work has received funding from the European High Performance Computing Joint Undertaking (JU) under grant agreement No 101093054.
```

