# Comparing `tmp/nbtools-23.4.0.tar.gz` & `tmp/nbtools-23.5.0.tar.gz`

## Comparing `nbtools-23.4.0.tar` & `nbtools-23.5.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbtools-23.4.0/.coveragerc
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nbtools-23.4.0/.eslintignore
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 nbtools-23.4.0/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nbtools-23.4.0/.npmignore
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 nbtools-23.4.0/.prettierignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbtools-23.4.0/.prettierrc
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 nbtools-23.4.0/DEPLOY.md
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 nbtools-23.4.0/Dockerfile
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 nbtools-23.4.0/appveyor.yml
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 nbtools-23.4.0/codecov.yml
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbtools-23.4.0/dev.Dockerfile
--rwxr-xr-x   0        0        0      827 2020-02-02 00:00:00.000000 nbtools-23.4.0/docker_build.sh
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 nbtools-23.4.0/install.json
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 nbtools-23.4.0/package.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nbtools-23.4.0/postBuild
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbtools-23.4.0/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nbtools-23.4.0/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 nbtools-23.4.0/setup.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nbtools-23.4.0/tsconfig.json
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 nbtools-23.4.0/webpack.config.js
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/.gitignore
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/compiler.xml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/modules.xml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/nbtools.iml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/rSettings.xml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/vcs.xml
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 nbtools-23.4.0/.idea/workspace.xml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nbtools-23.4.0/config/overrides.json
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 nbtools-23.4.0/docs/toolmanager.md
--rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 nbtools-23.4.0/docs/uibuilder.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nbtools-23.4.0/docs/uioutput.md
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 nbtools-23.4.0/docs/wysiwyg.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nbtools-23.4.0/jupyter-config/nbtools.json
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/__init__.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/_frontend.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/_version.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/basewidget.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/event_manager.py
--rw-r--r--   0        0        0    19059 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/form.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/nbtools.json
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/parsing_manager.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/settings.py
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/tool_manager.py
--rw-r--r--   0        0        0    11827 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/uibuilder.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/uioutput.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/utils.py
--rw-r--r--   0        0        0    20298 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/build_log.json
--rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/package.json
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/schemas/@g2nb/nbtools/package.json.orig
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/schemas/@g2nb/nbtools/plugin.json
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js.map
--rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js
--rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js.map
--rw-r--r--   0        0        0   141481 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js
--rw-r--r--   0        0        0   139488 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js.map
--rw-r--r--   0        0        0    33507 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js
--rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js.map
--rw-r--r--   0        0        0    29361 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js
--rw-r--r--   0        0        0    28197 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js.map
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/style.js
--rw-r--r--   0        0        0    16904 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js
--rw-r--r--   0        0        0    14914 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js.map
--rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js
--rw-r--r--   0        0        0    13868 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js.map
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/nbextension/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/nbextension/static/extension.js
--rw-r--r--   0        0        0    21002 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/nbextension/static/notebook.css
--rw-r--r--   0        0        0    10342 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/nbextension/static/toolbox.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/tests/__init__.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/tests/conftest.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/tests/test_example.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 nbtools-23.4.0/nbtools/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nbtools-23.4.0/schema/plugin.json
--rw-r--r--   0        0        0    15823 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/basewidget.ts
--rw-r--r--   0        0        0    17444 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/context.ts
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/dataregistry.ts
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/extension.ts
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/index.ts
--rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/plugin.ts
--rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/registry.ts
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/toolbox.ts
--rw-r--r--   0        0        0    31309 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/uibuilder.ts
--rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/uioutput.ts
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/utils.ts
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nbtools-23.4.0/src/version.ts
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/basewidget.css
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/g2nb_logo.png
--rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/icon.svg
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/index.css
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/index.js
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/toolbox.css
--rw-r--r--   0        0        0     5302 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/uibuilder.css
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 nbtools-23.4.0/style/uioutput.css
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 nbtools-23.4.0/tests/karma.conf.js
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nbtools-23.4.0/tests/tsconfig.json
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nbtools-23.4.0/tests/src/index.spec.ts
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 nbtools-23.4.0/tests/src/utils.spec.ts
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 nbtools-23.4.0/.gitignore
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 nbtools-23.4.0/LICENSE.txt
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 nbtools-23.4.0/README.md
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 nbtools-23.4.0/pyproject.toml
--rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 nbtools-23.4.0/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbtools-23.5.0/.coveragerc
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nbtools-23.5.0/.eslintignore
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 nbtools-23.5.0/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nbtools-23.5.0/.npmignore
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 nbtools-23.5.0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbtools-23.5.0/.prettierrc
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 nbtools-23.5.0/DEPLOY.md
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 nbtools-23.5.0/Dockerfile
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 nbtools-23.5.0/appveyor.yml
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 nbtools-23.5.0/codecov.yml
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbtools-23.5.0/dev.Dockerfile
+-rwxr-xr-x   0        0        0      827 2020-02-02 00:00:00.000000 nbtools-23.5.0/docker_build.sh
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 nbtools-23.5.0/install.json
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 nbtools-23.5.0/package.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nbtools-23.5.0/postBuild
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbtools-23.5.0/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nbtools-23.5.0/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 nbtools-23.5.0/setup.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nbtools-23.5.0/tsconfig.json
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 nbtools-23.5.0/webpack.config.js
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/.gitignore
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/compiler.xml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/modules.xml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/nbtools.iml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/rSettings.xml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 nbtools-23.5.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nbtools-23.5.0/config/overrides.json
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 nbtools-23.5.0/docs/toolmanager.md
+-rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 nbtools-23.5.0/docs/uibuilder.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nbtools-23.5.0/docs/uioutput.md
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 nbtools-23.5.0/docs/wysiwyg.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nbtools-23.5.0/jupyter-config/nbtools.json
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/_frontend.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/_version.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/basewidget.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/event_manager.py
+-rw-r--r--   0        0        0    19059 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/form.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/nbtools.json
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/parsing_manager.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/settings.py
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/tool_manager.py
+-rw-r--r--   0        0        0    12833 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/uibuilder.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/uioutput.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/utils.py
+-rw-r--r--   0        0        0    20298 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/build_log.json
+-rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/package.json
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/schemas/@g2nb/nbtools/package.json.orig
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/schemas/@g2nb/nbtools/plugin.json
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js.map
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js
+-rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js.map
+-rw-r--r--   0        0        0   141481 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js
+-rw-r--r--   0        0        0   139488 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js.map
+-rw-r--r--   0        0        0    33507 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js
+-rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js.map
+-rw-r--r--   0        0        0    29361 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js
+-rw-r--r--   0        0        0    28197 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js.map
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/style.js
+-rw-r--r--   0        0        0    16904 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js
+-rw-r--r--   0        0        0    14914 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js.map
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js
+-rw-r--r--   0        0        0    13868 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js.map
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/nbextension/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/nbextension/static/extension.js
+-rw-r--r--   0        0        0    21002 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/nbextension/static/notebook.css
+-rw-r--r--   0        0        0    10342 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/nbextension/static/toolbox.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/tests/__init__.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/tests/conftest.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/tests/test_example.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 nbtools-23.5.0/nbtools/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nbtools-23.5.0/schema/plugin.json
+-rw-r--r--   0        0        0    15823 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/basewidget.ts
+-rw-r--r--   0        0        0    17444 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/context.ts
+-rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/dataregistry.ts
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/extension.ts
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/index.ts
+-rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/plugin.ts
+-rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/registry.ts
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/toolbox.ts
+-rw-r--r--   0        0        0    31309 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/uibuilder.ts
+-rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/uioutput.ts
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/utils.ts
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nbtools-23.5.0/src/version.ts
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/basewidget.css
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/g2nb_logo.png
+-rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/icon.svg
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/index.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/index.js
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/toolbox.css
+-rw-r--r--   0        0        0     5302 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/uibuilder.css
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 nbtools-23.5.0/style/uioutput.css
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 nbtools-23.5.0/tests/karma.conf.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nbtools-23.5.0/tests/tsconfig.json
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nbtools-23.5.0/tests/src/index.spec.ts
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 nbtools-23.5.0/tests/src/utils.spec.ts
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 nbtools-23.5.0/.gitignore
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 nbtools-23.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 nbtools-23.5.0/README.md
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 nbtools-23.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 nbtools-23.5.0/PKG-INFO
```

### Comparing `nbtools-23.4.0/.eslintrc.js` & `nbtools-23.5.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/DEPLOY.md` & `nbtools-23.5.0/DEPLOY.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/Dockerfile` & `nbtools-23.5.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/appveyor.yml` & `nbtools-23.5.0/appveyor.yml`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/dev.Dockerfile` & `nbtools-23.5.0/dev.Dockerfile`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/docker_build.sh` & `nbtools-23.5.0/docker_build.sh`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/package.json` & `nbtools-23.5.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'version'": "'23.5.0'"}*

```diff
@@ -120,9 +120,9 @@
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch",
         "watch:src": "tsc -w"
     },
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "./lib/index.d.ts",
-    "version": "23.4.0"
+    "version": "23.5.0"
 }
```

### Comparing `nbtools-23.4.0/tsconfig.json` & `nbtools-23.5.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/webpack.config.js` & `nbtools-23.5.0/webpack.config.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/.idea/nbtools.iml` & `nbtools-23.5.0/.idea/nbtools.iml`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/docs/toolmanager.md` & `nbtools-23.5.0/docs/toolmanager.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/docs/uibuilder.md` & `nbtools-23.5.0/docs/uibuilder.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/docs/uioutput.md` & `nbtools-23.5.0/docs/uioutput.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/docs/wysiwyg.md` & `nbtools-23.5.0/docs/wysiwyg.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/__init__.py` & `nbtools-23.5.0/nbtools/__init__.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/_version.py` & `nbtools-23.5.0/nbtools/_version.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/basewidget.py` & `nbtools-23.5.0/nbtools/basewidget.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/event_manager.py` & `nbtools-23.5.0/nbtools/event_manager.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/form.py` & `nbtools-23.5.0/nbtools/form.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/parsing_manager.py` & `nbtools-23.5.0/nbtools/parsing_manager.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/settings.py` & `nbtools-23.5.0/nbtools/settings.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/tool_manager.py` & `nbtools-23.5.0/nbtools/tool_manager.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/uibuilder.py` & `nbtools-23.5.0/nbtools/uibuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,18 @@
 
         # Call the super constructor
         VBox.__init__(self, [self.form, self.output])
 
         # Insert a copy of this UI Builder when added as a tool
         self.load = lambda **override_kwargs: UIBuilder(self.function_or_method, **{**kwargs, **override_kwargs})
 
+        # Create properties to pass through to UIBuilderBase
+        exclude = ['keys', 'form', 'layout', 'tabbable', 'tooltip', 'comm']
+        self.create_properties([x for x in self.form.__dict__['_trait_values'].keys() if not x.startswith('_') and x not in exclude])
+
     def _apply_defaults(self, function_or_method):
         # Set the name based on the function name
         self.name = function_or_method.__qualname__
         self.id = function_or_method.__qualname__
 
         # Set the description based on the docstring
         self.description = inspect.getdoc(function_or_method) or ''
@@ -118,14 +122,32 @@
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     def id(self):
         """Return the function name regardless of custom display name"""
         return self.function_or_method.__qualname__
 
+    def _get_property(self, name):
+        prop = getattr(self, f"_{name}", None)
+        if prop is not None: return prop
+        else:
+            if hasattr(self, 'form'): return getattr(self.form, name, None)
+            else: return None
+
+    def _set_property(self, name, value):
+        setattr(self, f"_{name}", value)
+        if hasattr(self, 'form'): setattr(self.form, name, value)
+
+    def _create_property(self, name):
+        setattr(self.__class__, name, property(lambda self: self._get_property(name),
+                                               lambda self, value: self._set_property(name, value)))
+
+    def create_properties(self, property_names):
+        for name in property_names: self._create_property(name)
+
 
 class UIBuilderBase(BaseWidget):
     """Widget that renders a function as a UI form"""
 
     _model_name = Unicode('UIBuilderModel').tag(sync=True)
     _model_module = Unicode(module_name).tag(sync=True)
     _model_module_version = Unicode(module_version).tag(sync=True)
```

### Comparing `nbtools-23.4.0/nbtools/uioutput.py` & `nbtools-23.5.0/nbtools/uioutput.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/utils.py` & `nbtools-23.5.0/nbtools/utils.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/build_log.json` & `nbtools-23.5.0/nbtools/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/package.json` & `nbtools-23.5.0/nbtools/labextension/package.json`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/schemas/@g2nb/nbtools/package.json.orig` & `nbtools-23.5.0/nbtools/labextension/schemas/@g2nb/nbtools/package.json.orig`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png` & `nbtools-23.5.0/nbtools/labextension/static/6b8c90c7eb68fb0a698ade6fa7df2e33.png`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js` & `nbtools-23.5.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js.map` & `nbtools-23.5.0/nbtools/labextension/static/lib_index_js.7be7e51ff21fbbccb028.js.map`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js` & `nbtools-23.5.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js.map` & `nbtools-23.5.0/nbtools/labextension/static/lib_plugin_js.9ee79910806137e493ce.js.map`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js` & `nbtools-23.5.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js.map` & `nbtools-23.5.0/nbtools/labextension/static/lib_registry_js-lib_uibuilder_js-lib_uioutput_js.62f16408cce9e2f6ea27.js.map`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js` & `nbtools-23.5.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js.map` & `nbtools-23.5.0/nbtools/labextension/static/node_modules_css-loader_dist_cjs_js_style_basewidget_css-node_modules_css-loader_dist_cjs_js_-444759.0a0e1ed7766bfba46905.js.map`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js` & `nbtools-23.5.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js.map` & `nbtools-23.5.0/nbtools/labextension/static/remoteEntry.ed7f531dbfb094c43618.js.map`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js` & `nbtools-23.5.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js.map` & `nbtools-23.5.0/nbtools/labextension/static/style_index_js.1f214e1107ae935d92bb.js.map`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js` & `nbtools-23.5.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js.map` & `nbtools-23.5.0/nbtools/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-926fd9.05e08e7398a87350659a.js.map`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/nbextension/static/extension.js` & `nbtools-23.5.0/nbtools/nbextension/static/extension.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/nbextension/static/notebook.css` & `nbtools-23.5.0/nbtools/nbextension/static/notebook.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/nbextension/static/toolbox.js` & `nbtools-23.5.0/nbtools/nbextension/static/toolbox.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/nbtools/tests/conftest.py` & `nbtools-23.5.0/nbtools/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/src/basewidget.ts` & `nbtools-23.5.0/src/basewidget.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/src/context.ts` & `nbtools-23.5.0/src/context.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/src/dataregistry.ts` & `nbtools-23.5.0/src/dataregistry.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/src/extension.ts` & `nbtools-23.5.0/src/extension.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/src/plugin.ts` & `nbtools-23.5.0/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/src/registry.ts` & `nbtools-23.5.0/src/registry.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/src/toolbox.ts` & `nbtools-23.5.0/src/toolbox.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/src/uibuilder.ts` & `nbtools-23.5.0/src/uibuilder.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/src/uioutput.ts` & `nbtools-23.5.0/src/uioutput.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/src/utils.ts` & `nbtools-23.5.0/src/utils.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/style/basewidget.css` & `nbtools-23.5.0/style/basewidget.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/style/g2nb_logo.png` & `nbtools-23.5.0/style/g2nb_logo.png`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/style/icon.svg` & `nbtools-23.5.0/style/icon.svg`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/style/toolbox.css` & `nbtools-23.5.0/style/toolbox.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/style/uibuilder.css` & `nbtools-23.5.0/style/uibuilder.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/style/uioutput.css` & `nbtools-23.5.0/style/uioutput.css`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/tests/karma.conf.js` & `nbtools-23.5.0/tests/karma.conf.js`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/tests/src/index.spec.ts` & `nbtools-23.5.0/tests/src/index.spec.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/tests/src/utils.spec.ts` & `nbtools-23.5.0/tests/src/utils.spec.ts`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/.gitignore` & `nbtools-23.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/LICENSE.txt` & `nbtools-23.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/README.md` & `nbtools-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nbtools-23.4.0/pyproject.toml` & `nbtools-23.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
     "ipyuploads",
     "ipywidgets>7,<9",
     "jupyterlab>=3.4",
 ]
-version = "23.4.0"
+version = "23.5.0"
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.urls]
 Homepage = "https://github.com/g2nb/nbtools"
 
@@ -91,15 +91,15 @@
     "jlpm",
 ]
 
 [tool.tbump]
 github_url = "https://github.com/g2nb/nbtools"
 
 [tool.tbump.version]
-current = "23.4.0"
+current = "23.5.0"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?P<pre>((a|b|rc)\d+))?
```

### Comparing `nbtools-23.4.0/PKG-INFO` & `nbtools-23.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbtools
-Version: 23.4.0
+Version: 23.5.0
 Summary: Framework for creating user-friendly Jupyter notebooks, accessible to both programming and non-programming users alike.
 Project-URL: Homepage, https://github.com/g2nb/nbtools
 Author-email: Thorin Tabor <tmtabor@cloud.ucsd.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Regents of the University of California & Broad Institute
         All rights reserved.
```

