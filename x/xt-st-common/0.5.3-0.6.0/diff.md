# Comparing `tmp/xt_st_common-0.5.3.tar.gz` & `tmp/xt_st_common-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.5.3.tar", max compression
+gzip compressed data, was "xt_st_common-0.6.0.tar", max compression
```

## Comparing `xt_st_common-0.5.3.tar` & `xt_st_common-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      720 2023-06-01 11:30:34.282081 xt_st_common-0.5.3/README.md
--rw-r--r--   0        0        0     2603 2023-06-01 11:30:34.282081 xt_st_common-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     6128 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/__init__.py
--rw-r--r--   0        0        0      180 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/.env
--rw-r--r--   0        0        0       67 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/.prettierrc
--rw-r--r--   0        0        0      859 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2052 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/index.html
--rw-r--r--   0        0        0      564 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
--rw-r--r--   0        0        0     1183 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/service-worker.js
--rw-r--r--   0        0        0  4138182 2023-06-01 11:29:58.926504 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
--rw-r--r--   0        0        0     3326 2023-06-01 11:29:58.926504 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 16152785 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
--rw-r--r--   0        0        0     1442 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
--rw-r--r--   0        0        0     3848 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
--rw-r--r--   0        0        0     1598 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0        0        0     8317 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
--rw-r--r--   0        0        0     1141 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/package.json
--rw-r--r--   0        0        0      839 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/public/index.html
--rw-r--r--   0        0        0     1922 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
--rw-r--r--   0        0        0      274 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/tsconfig.json
--rw-r--r--   0        0        0       22 2023-06-01 11:30:34.282081 xt_st_common-0.5.3/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5010 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/components.py
--rw-r--r--   0        0        0     2371 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/config.py
--rw-r--r--   0        0        0     3177 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/database.py
--rw-r--r--   0        0        0     6303 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0    21814 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/project_components.py
--rw-r--r--   0        0        0     6518 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/project_models.py
--rw-r--r--   0        0        0     5976 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/session.py
--rw-r--r--   0        0        0     6251 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1957 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-06-07 01:40:04.921259 xt_st_common-0.6.0/README.md
+-rw-r--r--   0        0        0     2603 2023-06-07 01:40:04.921259 xt_st_common-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6128 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/.env
+-rw-r--r--   0        0        0       67 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/.prettierrc
+-rw-r--r--   0        0        0      859 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2052 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/index.html
+-rw-r--r--   0        0        0      564 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
+-rw-r--r--   0        0        0     1183 2023-06-07 01:39:18.341642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/service-worker.js
+-rw-r--r--   0        0        0  4138182 2023-06-07 01:39:18.369642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
+-rw-r--r--   0        0        0     3326 2023-06-07 01:39:18.369642 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 16152785 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
+-rw-r--r--   0        0        0     1442 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
+-rw-r--r--   0        0        0     3848 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
+-rw-r--r--   0        0        0     1598 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0        0        0     8317 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0        0        0     1141 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/package.json
+-rw-r--r--   0        0        0      839 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/public/index.html
+-rw-r--r--   0        0        0     1922 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
+-rw-r--r--   0        0        0      274 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/tsconfig.json
+-rw-r--r--   0        0        0       22 2023-06-07 01:40:04.921259 xt_st_common-0.6.0/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5010 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     2371 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     3177 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/database.py
+-rw-r--r--   0        0        0     6303 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0    25276 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/project_components.py
+-rw-r--r--   0        0        0     6518 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/project_models.py
+-rw-r--r--   0        0        0     5976 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     6251 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1957 2023-06-07 01:39:18.461641 xt_st_common-0.6.0/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.6.0/PKG-INFO
```

### Comparing `xt_st_common-0.5.3/README.md` & `xt_st_common-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.5.3
+# XT-STREAMLIT - 0.6.0
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

### Comparing `xt_st_common-0.5.3/pyproject.toml` & `xt_st_common-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.5.3"
+version = "0.6.0"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}, {include = "streamlit_plotly_events", from= "src"}]
 
 [tool.poe.tasks]
 test = { cmd="pytest --cov=src/xt_st_common", help="Run unit tests"}
```

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/__init__.py` & `xt_st_common-0.6.0/src/streamlit_plotly_events/__init__.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/asset-manifest.json` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/index.html` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/service-worker.js` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/package.json` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/package.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/public/index.html` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx` & `xt_st_common-0.6.0/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/xt_st_common/components.py` & `xt_st_common-0.6.0/src/xt_st_common/components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/xt_st_common/config.py` & `xt_st_common-0.6.0/src/xt_st_common/config.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/xt_st_common/database.py` & `xt_st_common-0.6.0/src/xt_st_common/database.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/xt_st_common/fs_upload_page.py` & `xt_st_common-0.6.0/src/xt_st_common/fs_upload_page.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/xt_st_common/project_components.py` & `xt_st_common-0.6.0/src/xt_st_common/project_components.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from io import BytesIO
 from pathlib import Path
 from random import randint
-from typing import List, Optional, Tuple, Union  # , Optional
+from typing import List, Literal, Optional, Tuple, Union  # , Optional
 
 import pandas as pd
 import streamlit as st
 
 # from mpl_toolbox_ui.common.config import Settings
 from xt_st_common.database import (
     Project,
@@ -16,21 +16,32 @@
     get_projects,
     project_duplicate_exists,
     save_project,
 )
 from xt_st_common.project_models import ProjectState
 from xt_st_common.session import get_user_email
 from xt_st_common.storage import FileRef, storage_client
-from xt_st_common.utils import get_encoding_and_dialect, get_state, seperate_users, set_state
+from xt_st_common.utils import (
+    get_encoding_and_dialect,
+    get_state,
+    seperate_users,
+    set_state,
+)
 
 # from bson.objectid import ObjectId
 
 # mapping for language options for streamlit code formatter. For other available options
 # see: https://github.com/react-syntax-highlighter/react-syntax-highlighter/blob/master/AVAILABLE_LANGUAGES_PRISM.MD
-CODE_FORMAT_MAPPING = {"json": "json", "yaml": "yaml", "yml": "yaml", "toml": "toml", "md": "markfown"}
+CODE_FORMAT_MAPPING = {
+    "json": "json",
+    "yaml": "yaml",
+    "yml": "yaml",
+    "toml": "toml",
+    "md": "markfown",
+}
 
 REPLACE_FILE_HELP_TXT = (
     "The new file can have a different name but must have the same extension."
     "Warning: Uploading a new file that is significantly different to the original "
     "can have catastrophic results."
 )
 
@@ -70,24 +81,27 @@
     if project is None:
         set_state(ProjectState.PROJECT_WARNING_MESSAGE, "No project is selected")
     else:
         set_state(
             ProjectState.PROJECT_DELETE_CONFIRM,
             (
                 "Deleting will remove all files that are part of project: "
-                + f"**{project.name}**. Are you sure you want to continue?"
+                + f"**'{project.name}'**. Are you sure you want to continue?"
             ),
         )
         set_state(ProjectState.PROJECT_TO_DELETE, project)
 
 
 def action_delete(project: Project):
     if project.id is not None:
         delete_project(project.id)
-    set_state(ProjectState.PROJECT_SUCCESS_MESSAGE, f"Project {project.name} deleted successfully")
+    set_state(
+        ProjectState.PROJECT_SUCCESS_MESSAGE,
+        f"Project **'{project.name}'** deleted successfully",
+    )
 
 
 def submit_delete_folder(folder: str):
     """Callback function to set state in order to enable a delete on the next run."""
     # display a warning if the user entered an existing name
     project = st.session_state.selected_project
     if project is None:
@@ -95,39 +109,45 @@
     if folder is None:
         set_state(ProjectState.UPLOAD_WARNING_MESSAGE, "No folder is selected")
     else:
         set_state(
             ProjectState.UPLOAD_DELETE_CONFIRM,
             (
                 "Deleting will remove all files that are part of this folder: "
-                + f"**{folder}**. Are you sure you want to continue?"
+                + f"**'{folder}'**. Are you sure you want to continue?"
             ),
         )
         set_state(ProjectState.FOLDER_TO_DELETE, folder)
 
 
 def action_delete_folder(folder):
     project = get_selected_project_or_error()
     project.delete_folder(folder)
     save_project(project)
 
     set_state(ProjectState.FOLDER_ADDED, None)
-    set_state(ProjectState.UPLOAD_SUCCESS_MESSAGE, f"Folders {project.name} was deleted successfully")
+    set_state(
+        ProjectState.UPLOAD_SUCCESS_MESSAGE,
+        f"Folders **'{folder}'** was deleted successfully",
+    )
 
 
 def submit_delete_file(file: FileRef):
     """Callback function to set state in order to enable a delete on the next run."""
     # display a warning if the user entered an existing name
     project = st.session_state.selected_project
     if project is None:
         set_state(ProjectState.FILE_WARNING_MESSAGE, "No project is selected")
     if file is None:
         set_state(ProjectState.FILE_WARNING_MESSAGE, "No file is selected")
     else:
-        set_state(ProjectState.FILE_DELETE_CONFIRM, f"Are you sure you want to delete file **{file.name}**?")
+        set_state(
+            ProjectState.FILE_DELETE_CONFIRM,
+            f"Are you sure you want to delete file **'{file.name}'**?",
+        )
         set_state(ProjectState.FILE_TO_DELETE, file)
 
 
 def action_delete_file(_file: FileRef):
     project = get_selected_project_or_error()
     project.delete_file(_file)
     save_project(project)
@@ -149,31 +169,45 @@
         container.warning("No project name was provided")
         return
 
     users_list = seperate_users(users)
     if project is None:
         message_verb = "created"
         project = Project(
-            name=name, owner=get_user_email(), description=description, users=users_list, public=is_public
+            name=name,
+            owner=get_user_email(),
+            description=description,
+            users=users_list,
+            public=is_public,
         )
         if project_duplicate_exists(project.name, project.owner, str(project.id)):
-            st.session_state.proj_warning_message = f"A Project with the name: **{name}** already exists"
+            st.session_state.proj_warning_message = f"A Project with the name: **'{name}'** already exists"
             return
     else:
         # Get latest DB copy of the project
         project = get_project(str(project.id), st.session_state.project_cache)
         if project is None:
-            st.session_state.proj_warning_message = f"Cannot update project: **{name}** not found in database"
+            st.session_state.proj_warning_message = f"Cannot update project: **'{name}'** not found in database"
             return
-        project.__dict__.update({"name": name, "description": description, "users": users_list, "public": is_public})
+        project.__dict__.update(
+            {
+                "name": name,
+                "description": description,
+                "users": users_list,
+                "public": is_public,
+            }
+        )
 
     project = save_project(project)
     set_selected_project(project)
 
-    set_state(ProjectState.PROJECT_SUCCESS_MESSAGE, f"Project **{name}** has been {message_verb}.")
+    set_state(
+        ProjectState.PROJECT_SUCCESS_MESSAGE,
+        f"Project **'{name}'** has been {message_verb}.",
+    )
     return
 
 
 def project_form(project: Optional[Project] = None):
     """A form that allows for creating an updating projects
 
     Parameters
@@ -213,20 +247,26 @@
 
 
 def add_folders():
     project = st.session_state.selected_project
     folders_string = st.session_state.add_project_folder_name
 
     if not folders_string:
-        set_state(ProjectState.UPLOAD_WARNING_MESSAGE, "Cannot add new folders: Folder name was empty")
+        set_state(
+            ProjectState.UPLOAD_WARNING_MESSAGE,
+            "Cannot add new folders: Folder name was empty",
+        )
         return
 
     count = project.add_folders(folders_string)
     save_project(project)
-    set_state(ProjectState.UPLOAD_SUCCESS_MESSAGE, f"{count} folders were added to {project.name}")
+    set_state(
+        ProjectState.UPLOAD_SUCCESS_MESSAGE,
+        f"{count} folders were added to **'{project.name}'**",
+    )
 
 
 @st.cache_data(ttl=300)
 def get_df_preview(path: str, ext: Optional[str], num_rows=10):
     # if filepath.suffix == ".zip":
     #     frame = get_gdf_from_file(filepath)
     #     return frame.iloc[:num_rows, :-1]
@@ -281,36 +321,40 @@
     null_option="-- Select Project --",
     st_context=st.sidebar,
 ) -> Tuple[Union["Project", None], List["Project"]]:
     """UI to select and create projects
     Args:
         root_path (Path): The root Path to where the project folders live
     """
+    selected_project = None
 
     if header_text is not None:
         st_context.subheader(header_text)
     include_public = st_context.checkbox("Include Public", value=False, key="include_public_projects")
     options, projects, sel_idx = get_proj_options(include_public, get_project_cache())
-    proj_options = {-1: null_option}
+    proj_options = {-1: null_option} if null_option is not None else {}
     if options is not None:
         proj_options = {**proj_options, **options}
 
-    proj_idx = st_context.selectbox(
-        select_box_label,
-        key="project_select",
-        index=sel_idx,
-        # on_change=on_project_select,
-        options=proj_options.keys(),
-        format_func=lambda x: proj_options[x],
-    )
+    if len(proj_options) > 0:
+        proj_idx = st_context.selectbox(
+            select_box_label,
+            key="project_select",
+            # index=sel_idx,
+            # on_change=on_project_select,
+            options=proj_options.keys(),
+            format_func=lambda x: proj_options[x],
+        )
 
-    selected_project = None
-    if proj_idx is not None and proj_idx > -1:
-        selected_project = projects[proj_idx] if proj_idx != -1 else None
-        set_selected_project(selected_project)
+        selected_project = None
+        if proj_idx is not None and proj_idx > -1:
+            selected_project = projects[proj_idx] if proj_idx != -1 else None
+            set_selected_project(selected_project)
+    else:
+        st_context.warning("No projects were found")
 
     return selected_project, projects
 
 
 def load_csv(
     data_file,
     st_context=st,
@@ -393,130 +437,195 @@
 def file_manager(
     project: Project,
     types: List[str],
     label: str,
     st_context=st.sidebar,
     help_text: Optional[str] = None,
     allow_upload=True,
+    allow_multiple_uploads=False,
     allow_delete=True,
     allow_replace=True,
+    allow_folder_add=False,
     key_prefix: str = "",
     expand_file_actions=False,
     folder_select_text="Select Borehole/Run",
     auto_parse_csv=True,
+    render_layout: Literal["vertical", "horizontal", "compact"] = "vertical",
 ):
     file_delete_confirm = get_state(ProjectState.FILE_DELETE_CONFIRM)
     file_to_delete = get_state(ProjectState.FILE_TO_DELETE)
     file_success_message = get_state(ProjectState.FILE_SUCCESS_MESSAGE)
     file_warning_message = get_state(ProjectState.FILE_WARNING_MESSAGE)
 
+    folder_to_delete = get_state(ProjectState.FOLDER_TO_DELETE)
+    folder_delete_confirm = get_state(ProjectState.UPLOAD_DELETE_CONFIRM)
+    folder_success_message = get_state(ProjectState.UPLOAD_SUCCESS_MESSAGE)
+    folder_warning_message = get_state(ProjectState.UPLOAD_WARNING_MESSAGE)
+
     st_context.subheader(f"Files: {project.name}")
     if file_delete_confirm and file_to_delete:
-        st_context.warning(file_delete_confirm)
-        st_context.button("I'm Sure", on_click=action_delete_file, args=(file_to_delete,))
+        st.warning(file_delete_confirm)
+        st.button("I'm Sure", on_click=action_delete_file, args=(file_to_delete,))
 
     if file_success_message:
-        st_context.success(file_success_message)
+        st.success(file_success_message)
     if file_warning_message:
-        st_context.warning(file_warning_message)
-    # col1, col2 = st.columns([1, 2])
+        st.warning(file_warning_message)
+
+    if folder_delete_confirm and folder_to_delete:
+        st.warning(folder_delete_confirm)
+        st.button("I'm Sure", on_click=action_delete_folder, args=(folder_to_delete,))
+
+    if folder_success_message:
+        st.success(folder_success_message)
+    if folder_warning_message:
+        st.warning(folder_warning_message)
+
+    if render_layout == "horizontal":
+        container1, container2 = st_context.columns(2)
+    else:
+        container1 = st_context.container()
+        container2 = st_context.container()
+
     folders_dict = project.get_folders_map()
-    folder = st_context.selectbox(
-        folder_select_text, options=folders_dict.keys(), format_func=lambda x: folders_dict[x]
+    folder = container1.selectbox(
+        folder_select_text,
+        options=folders_dict.keys(),
+        format_func=lambda x: folders_dict[x],
     )
     path = project.get_folder_path(folder) if folder else None
     if path is not None and folder is not None:
+        row = container1.expander("Folder Actions", expanded=expand_file_actions)
+
+        if allow_delete and folder != "/":
+            row.button(
+                "Delete Selected",
+                key=f"{key_prefix}folder_delete_btn",
+                on_click=submit_delete_folder,
+                args=(folder,),
+            )
+        if allow_folder_add:
+            row.caption("Add Sub Folders")
+            row.text_input(
+                "New Folders (use ',' to separate multiple folders and '/' to separate levels) ",
+                key="add_project_folder_name",
+                help="All folders are created relative to the project root. "
+                + "Create multiple folders at once by using ',' as a separator, folders can be "
+                + "multiple levels deep using '/' e.g. folder1/subfolder1, folder1/subfolder22",
+                placeholder="folder1/subfolder1, folder1/subfolder2",
+            )
+            row.button(
+                label="Add",
+                help="Create new folder(s)",
+                on_click=add_folders,
+            )
         state = _state_name(str(project.id), folder)
         if state not in st.session_state:
             st.session_state[state] = 0
 
         if allow_upload:
             if auto_parse_csv:
-                try_parse_csv = st_context.checkbox(
+                try_parse_csv = st.checkbox(
                     "Parse CSV/TXT as Dataset",
                     value=True,
                     help=(
                         "If a CSV or TXT file is uploaded you will be given options to help "
                         + "calibrate it for use as a dataset."
                     ),
                 )
             else:
                 try_parse_csv = False
-            uploaded_file = st_context.file_uploader(
+            uploaded_files = container1.file_uploader(
                 label,
                 key=_get_key(key_prefix),
                 type=types,
                 help=help_text,
-                # accept_multiple_files=True,
+                accept_multiple_files=allow_multiple_uploads,
             )
-            file_ref = None
-            file_ref_units = None
-            if (
-                uploaded_file
-                and try_parse_csv
-                and (uploaded_file.name.lower().endswith(".csv") or uploaded_file.name.lower().endswith(".txt"))
-            ):
-                frame = None
-                try:
-                    frame, units = load_csv(uploaded_file, st)
-                except ValueError:
-                    st_context.warning(
-                        "Could not parse CSV/TXT as a dataset. "
-                        + "This may mean the file requires special parsing (such as a PWAVE file)"
-                    )
-                    try_parse_csv = not st_context.button("Upload anyway")
-                    units = None
 
-                if frame is not None:
-                    data_name = f"{Path(uploaded_file.name).stem}.feather"
-                    with BytesIO() as buffer:
-                        frame.to_feather(buffer)
-                        buffer.seek(0)
-                        file_ref = project.add_replace_file(
-                            buffer,
-                            folder=folder,
-                            filename=data_name,
-                        )
-                    units_name = ""
-                    if units:
-                        units_name = f"{Path(uploaded_file.name).stem}_units.json"
-                        units_string = json.dumps(units)
-                        file_ref_units = project.add_replace_file(
-                            units_string,
-                            folder=folder,
-                            filename=units_name,
-                            content_type="application/json",
+            # handle cases where allow_multiple_uploads is false
+            if uploaded_files is None:
+                uploaded_files = []
+            elif not isinstance(uploaded_files, list):
+                uploaded_files = [uploaded_files]
+
+            upload_messages = []
+            for uploaded_file in uploaded_files:
+                file_ref = None
+                file_ref_units = None
+                if (
+                    uploaded_file
+                    and try_parse_csv
+                    and (uploaded_file.name.lower().endswith(".csv") or uploaded_file.name.lower().endswith(".txt"))
+                ):
+                    frame = None
+                    try:
+                        frame, units = load_csv(uploaded_file, st)
+                    except ValueError:
+                        st.warning(
+                            "Could not parse CSV/TXT as a dataset. "
+                            + "This may mean the file requires special parsing (such as a PWAVE file)"
                         )
+                        try_parse_csv = not st.button("Upload anyway")
+                        units = None
 
-            elif uploaded_file:
-                file_ref = project.add_replace_file(
-                    uploaded_file.getvalue(), folder=folder, filename=uploaded_file.name
-                )
+                    if frame is not None:
+                        data_name = f"{Path(uploaded_file.name).stem}.feather"
+                        with BytesIO() as buffer:
+                            frame.to_feather(buffer)
+                            buffer.seek(0)
+                            file_ref = project.add_replace_file(
+                                buffer,
+                                folder=folder,
+                                filename=data_name,
+                            )
+                        units_name = ""
+                        if units:
+                            units_name = f"{Path(uploaded_file.name).stem}_units.json"
+                            units_string = json.dumps(units)
+                            file_ref_units = project.add_replace_file(
+                                units_string,
+                                folder=folder,
+                                filename=units_name,
+                                content_type="application/json",
+                            )
+
+                elif uploaded_file:
+                    file_ref = project.add_replace_file(
+                        uploaded_file.getvalue(),
+                        folder=folder,
+                        filename=uploaded_file.name,
+                    )
+
+                if uploaded_file and file_ref:
+                    uploaded_file.close()
+                    upload_messages.append(
+                        f"File: **'{file_ref.name}'** {' and ' + file_ref_units.name if file_ref_units else ''} "
+                        + " uploaded successfully",
+                    )
 
-            if uploaded_file and file_ref:
-                uploaded_file.close()
+            if len(upload_messages) > 0:
                 save_project(project)
                 _update_key(key_prefix)
                 set_state(
                     ProjectState.FILE_SUCCESS_MESSAGE,
-                    f"File: {file_ref.name}{' and ' + file_ref_units.name if file_ref_units else ''} "
-                    + "Uploaded successfully",
+                    "".join([f"> 1. {msg} \n" for msg in upload_messages]),
                 )
                 st.experimental_rerun()
 
         files = project.get_files_in_folder(folder)
         if files is not None and len(files) > 0:
-            selected_key = st_context.selectbox(
+            selected_key = container2.selectbox(
                 "Select File",
                 options=files.keys(),
                 key=f"{key_prefix}file_manager_file_select",
             )
             selected_file = files[selected_key] if selected_key in files else None
             if selected_file is not None and selected_key is not None:
-                row = st_context.expander("File Actions", expanded=expand_file_actions)
+                row = container2.expander("File Actions", expanded=expand_file_actions)
                 if len(selected_key) > 30:
                     row.caption(selected_key)
                 # options = []
                 if allow_delete:
                     row.button(
                         "Delete",
                         key=f"{key_prefix}file_delete_btn",
@@ -533,20 +642,23 @@
                             st.dataframe(get_df_preview(selected_file.path, selected_file.get_ext()))
                 if selected_key.lower().endswith((".json", ".yml", ".yaml", ".toml", ".md", ".txt")) and (
                     preview_frame := row.button(
                         "Preview File",
                         key=f"{key_prefix}file_manager_preview_file",
                     )
                 ):
-                    with st.expander(f"**Frame Viewer:** {selected_file.name}", expanded=True):
+                    with st.expander(f"**File Viewer:** {selected_file.name}", expanded=True):
                         code_format = CODE_FORMAT_MAPPING.get(selected_key.lower().split(".")[-1])
                         if code_format is None:
                             st.write(get_string_preview(selected_file))
                         else:
-                            st.code(get_string_preview(selected_file), language=code_format)
+                            st.code(
+                                get_string_preview(selected_file),
+                                language=code_format,
+                            )
                 if row.checkbox(
                     "Prepare Download",
                     key=f"{key_prefix}file_manager_download_chbx",
                 ):
                     file_data = storage_client().get_file(selected_file.path)
 
                     row.download_button(
@@ -566,11 +678,12 @@
                 ):
                     project.add_replace_file_by_path(uploaded_replace_file, selected_file.path)
                     save_project(project)
                     uploaded_replace_file.close()
                     _update_key(key_prefix, True)
                     st.experimental_rerun()
         else:
-            st_context.info("No files in folder.")
+            container2.markdown("##")
+            container2.info("No files in selected folder")
 
         state_reset()
     return path, folder
```

### Comparing `xt_st_common-0.5.3/src/xt_st_common/project_models.py` & `xt_st_common-0.6.0/src/xt_st_common/project_models.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/xt_st_common/session.py` & `xt_st_common-0.6.0/src/xt_st_common/session.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/xt_st_common/storage.py` & `xt_st_common-0.6.0/src/xt_st_common/storage.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/src/xt_st_common/utils.py` & `xt_st_common-0.6.0/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.3/PKG-INFO` & `xt_st_common-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.5.3
+Version: 0.6.0
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
 Requires-Python: >3.9.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,15 +19,15 @@
 Requires-Dist: pymongo (>=4.3.3) ; extra == "databases"
 Requires-Dist: pymongo-auth-aws (>=1.1.0) ; extra == "databases"
 Requires-Dist: streamlit (>=1.22.0)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.5.3
+# XT-STREAMLIT - 0.6.0
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

