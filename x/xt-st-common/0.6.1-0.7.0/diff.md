# Comparing `tmp/xt_st_common-0.6.1.tar.gz` & `tmp/xt_st_common-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.6.1.tar", max compression
+gzip compressed data, was "xt_st_common-0.7.0.tar", max compression
```

## Comparing `xt_st_common-0.6.1.tar` & `xt_st_common-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      720 2023-06-07 01:57:03.161414 xt_st_common-0.6.1/README.md
--rw-r--r--   0        0        0     2603 2023-06-07 01:57:03.161414 xt_st_common-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     6128 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/__init__.py
--rw-r--r--   0        0        0      180 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/.env
--rw-r--r--   0        0        0       67 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/.prettierrc
--rw-r--r--   0        0        0      859 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2052 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/index.html
--rw-r--r--   0        0        0      564 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
--rw-r--r--   0        0        0     1183 2023-06-07 01:56:21.500751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/service-worker.js
--rw-r--r--   0        0        0  4138182 2023-06-07 01:56:21.524751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
--rw-r--r--   0        0        0     3326 2023-06-07 01:56:21.524751 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 16152785 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
--rw-r--r--   0        0        0     1442 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
--rw-r--r--   0        0        0     3848 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
--rw-r--r--   0        0        0     1598 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0        0        0     8317 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
--rw-r--r--   0        0        0     1141 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/package.json
--rw-r--r--   0        0        0      839 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/public/index.html
--rw-r--r--   0        0        0     1922 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
--rw-r--r--   0        0        0      274 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/tsconfig.json
--rw-r--r--   0        0        0       22 2023-06-07 01:57:03.161414 xt_st_common-0.6.1/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5010 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/components.py
--rw-r--r--   0        0        0     2371 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/config.py
--rw-r--r--   0        0        0     3177 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/database.py
--rw-r--r--   0        0        0     6303 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0    25276 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/project_components.py
--rw-r--r--   0        0        0     6518 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/project_models.py
--rw-r--r--   0        0        0     5976 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/session.py
--rw-r--r--   0        0        0     6380 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1957 2023-06-07 01:56:21.600753 xt_st_common-0.6.1/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-06-07 09:30:36.324167 xt_st_common-0.7.0/README.md
+-rw-r--r--   0        0        0     2603 2023-06-07 09:30:36.324167 xt_st_common-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6128 2023-06-07 09:30:03.195672 xt_st_common-0.7.0/src/streamlit_plotly_events/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-07 09:30:03.195672 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/.env
+-rw-r--r--   0        0        0       67 2023-06-07 09:30:03.195672 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/.prettierrc
+-rw-r--r--   0        0        0      859 2023-06-07 09:30:03.195672 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2052 2023-06-07 09:30:03.195672 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/index.html
+-rw-r--r--   0        0        0      564 2023-06-07 09:30:03.195672 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
+-rw-r--r--   0        0        0     1183 2023-06-07 09:30:03.195672 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/service-worker.js
+-rw-r--r--   0        0        0  4138182 2023-06-07 09:30:03.215672 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
+-rw-r--r--   0        0        0     3326 2023-06-07 09:30:03.215672 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 16152785 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
+-rw-r--r--   0        0        0     1442 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
+-rw-r--r--   0        0        0     3848 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
+-rw-r--r--   0        0        0     1598 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0        0        0     8317 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0        0        0     1141 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/package.json
+-rw-r--r--   0        0        0      839 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/public/index.html
+-rw-r--r--   0        0        0     1922 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
+-rw-r--r--   0        0        0      274 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/tsconfig.json
+-rw-r--r--   0        0        0       22 2023-06-07 09:30:36.324167 xt_st_common-0.7.0/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5010 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     2371 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     3177 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/xt_st_common/database.py
+-rw-r--r--   0        0        0     6303 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0    35057 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/xt_st_common/project_components.py
+-rw-r--r--   0        0        0     6518 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/xt_st_common/project_models.py
+-rw-r--r--   0        0        0     5976 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     6450 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1957 2023-06-07 09:30:03.295673 xt_st_common-0.7.0/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.7.0/PKG-INFO
```

### Comparing `xt_st_common-0.6.1/README.md` & `xt_st_common-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.6.1
+# XT-STREAMLIT - 0.7.0
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

### Comparing `xt_st_common-0.6.1/pyproject.toml` & `xt_st_common-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.6.1"
+version = "0.7.0"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}, {include = "streamlit_plotly_events", from= "src"}]
 
 [tool.poe.tasks]
 test = { cmd="pytest --cov=src/xt_st_common", help="Run unit tests"}
@@ -13,15 +13,15 @@
 install = {cmd = "poetry install --all-extras", help="Install all dependecnies"}
 format-black = { cmd = "black .", help="Run Black formater"}
 format-ruff = { cmd = "ruff src/xt_st_common --fix", help="Run Ruff linter and apply fixes"}
 format = { sequence=["format-black", "format-ruff"], help="Run all formatters" }
 
 [tool.poetry.dependencies]
 python = ">3.9.7, <4.0"
-streamlit = ">=1.22.0"
+streamlit = ">=1.23.1"
 pydantic = ">=1.10.7"
 pyjwt = {extras = ["crypto"], version = "^2.6.0"}
 streamlit-js-eval = "^0.1.5"
 chardet = ">=4.0.0, <6.0"
 streamlit-tree-select = "^0.0.5"
 minio = {version="^7.1.14", optional = true}
 plotly = ">= 4.14.3"
```

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/__init__.py` & `xt_st_common-0.7.0/src/streamlit_plotly_events/__init__.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/asset-manifest.json` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/index.html` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/service-worker.js` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/package.json` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/package.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/public/index.html` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx` & `xt_st_common-0.7.0/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/xt_st_common/components.py` & `xt_st_common-0.7.0/src/xt_st_common/components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/xt_st_common/config.py` & `xt_st_common-0.7.0/src/xt_st_common/config.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/xt_st_common/database.py` & `xt_st_common-0.7.0/src/xt_st_common/database.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/xt_st_common/fs_upload_page.py` & `xt_st_common-0.7.0/src/xt_st_common/fs_upload_page.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/xt_st_common/project_components.py` & `xt_st_common-0.7.0/src/xt_st_common/project_components.py`

 * *Files 20% similar despite different names*

```diff
@@ -328,22 +328,23 @@
     selected_project = None
 
     if header_text is not None:
         st_context.subheader(header_text)
     include_public = st_context.checkbox("Include Public", value=False, key="include_public_projects")
     options, projects, sel_idx = get_proj_options(include_public, get_project_cache())
     proj_options = {-1: null_option} if null_option is not None else {}
+    sel_idx = 0 if len(proj_options) < 2 else sel_idx  # ensure sel_idx is never greater than proj_options
     if options is not None:
         proj_options = {**proj_options, **options}
 
     if len(proj_options) > 0:
         proj_idx = st_context.selectbox(
             select_box_label,
             key="project_select",
-            # index=sel_idx,
+            index=sel_idx,
             # on_change=on_project_select,
             options=proj_options.keys(),
             format_func=lambda x: proj_options[x],
         )
 
         selected_project = None
         if proj_idx is not None and proj_idx > -1:
@@ -433,24 +434,25 @@
     key = get_state(f"{prefix}file_manager_key{'_replace' if replace else ''}", None)
     return _update_key(prefix, replace) if key is None else key
 
 
 def file_manager(
     project: Project,
     types: List[str],
-    label: str,
     st_context=st.sidebar,
+    upload_label: str = "Upload file(s) to selected folder",
     help_text: Optional[str] = None,
     allow_upload=True,
     allow_multiple_uploads=False,
     allow_delete=True,
     allow_replace=True,
     allow_folder_add=False,
     key_prefix: str = "",
     expand_file_actions=False,
+    expand_folder_actions=True,
     folder_select_text="Select Borehole/Run",
     auto_parse_csv=True,
     render_layout: Literal["vertical", "horizontal", "compact"] = "vertical",
 ):
     file_delete_confirm = get_state(ProjectState.FILE_DELETE_CONFIRM)
     file_to_delete = get_state(ProjectState.FILE_TO_DELETE)
     file_success_message = get_state(ProjectState.FILE_SUCCESS_MESSAGE)
@@ -490,38 +492,16 @@
     folder = container1.selectbox(
         folder_select_text,
         options=folders_dict.keys(),
         format_func=lambda x: folders_dict[x],
     )
     path = project.get_folder_path(folder) if folder else None
     if path is not None and folder is not None:
-        row = container1.expander("Folder Actions", expanded=expand_file_actions)
+        row = container1.expander("Folder Actions", expanded=expand_folder_actions)
 
-        if allow_delete and folder != "/":
-            row.button(
-                "Delete Selected",
-                key=f"{key_prefix}folder_delete_btn",
-                on_click=submit_delete_folder,
-                args=(folder,),
-            )
-        if allow_folder_add:
-            row.caption("Add Sub Folders")
-            row.text_input(
-                "New Folders (use ',' to separate multiple folders and '/' to separate levels) ",
-                key="add_project_folder_name",
-                help="All folders are created relative to the project root. "
-                + "Create multiple folders at once by using ',' as a separator, folders can be "
-                + "multiple levels deep using '/' e.g. folder1/subfolder1, folder1/subfolder22",
-                placeholder="folder1/subfolder1, folder1/subfolder2",
-            )
-            row.button(
-                label="Add",
-                help="Create new folder(s)",
-                on_click=add_folders,
-            )
         state = _state_name(str(project.id), folder)
         if state not in st.session_state:
             st.session_state[state] = 0
 
         if allow_upload:
             if auto_parse_csv:
                 try_parse_csv = st.checkbox(
@@ -530,16 +510,16 @@
                     help=(
                         "If a CSV or TXT file is uploaded you will be given options to help "
                         + "calibrate it for use as a dataset."
                     ),
                 )
             else:
                 try_parse_csv = False
-            uploaded_files = container1.file_uploader(
-                label,
+            uploaded_files = row.file_uploader(
+                upload_label,
                 key=_get_key(key_prefix),
                 type=types,
                 help=help_text,
                 accept_multiple_files=allow_multiple_uploads,
             )
 
             # handle cases where allow_multiple_uploads is false
@@ -596,27 +576,60 @@
                         filename=uploaded_file.name,
                     )
 
                 if uploaded_file and file_ref:
                     uploaded_file.close()
                     upload_messages.append(
                         f"File: **'{file_ref.name}'** {' and ' + file_ref_units.name if file_ref_units else ''} "
-                        + " uploaded successfully",
+                        + f" uploaded successfully to folder **'{file_ref.get_folder()}'**",
                     )
 
             if len(upload_messages) > 0:
                 save_project(project)
                 _update_key(key_prefix)
                 set_state(
                     ProjectState.FILE_SUCCESS_MESSAGE,
                     "".join([f"> 1. {msg} \n" for msg in upload_messages]),
                 )
                 st.experimental_rerun()
 
-        files = project.get_files_in_folder(folder)
+        if render_layout == "compact":
+            folder_container1 = row.container()
+            folder_container2 = row.container()
+            folder_container3 = row.container()
+
+        else:
+            folder_container1, folder_container2, folder_container3 = row.columns([4, 1, 1])
+            folder_container2.markdown("#")
+            folder_container3.markdown("#")
+
+        if allow_folder_add:
+            folder_container1.text_input(
+                "Add sub folders (use ',' to separate multiple folders and '/' to separate levels) ",
+                key="add_project_folder_name",
+                help="All folders are created relative to the project root. "
+                + "Create multiple folders at once by using ',' as a separator, folders can be "
+                + "multiple levels deep using '/' e.g. folder1/subfolder1, folder1/subfolder22",
+                placeholder="folder1/subfolder1, folder1/subfolder2",
+            )
+            folder_container2.button(
+                label="Add Folders",
+                help="Create new folder(s)",
+                on_click=add_folders,
+            )
+
+        if allow_delete and folder != "/":
+            folder_container3.button(
+                "Delete Selected",
+                key=f"{key_prefix}folder_delete_btn",
+                on_click=submit_delete_folder,
+                args=(folder,),
+            )
+
+        files = project.get_files_in_folder(folder, include_subfolders=False)
         if files is not None and len(files) > 0:
             selected_key = container2.selectbox(
                 "Select File",
                 options=files.keys(),
                 key=f"{key_prefix}file_manager_file_select",
             )
             selected_file = files[selected_key] if selected_key in files else None
@@ -683,7 +696,248 @@
                     st.experimental_rerun()
         else:
             container2.markdown("##")
             container2.info("No files in selected folder")
 
         state_reset()
     return path, folder
+
+
+def get_projects_data(projects):
+    selected_project = get_selected_project()
+    proj_data = []
+    for proj in projects:
+        proj_dict = proj.dict(exclude={"files"})
+        # proj_dict = proj.dict(exclude={"files", "folders", "id"})
+
+        # proj_dict["folders"] = "\n".join(proj.folders)
+        proj_dict["files"] = [file.name for file in proj.files]
+        proj_dict["users"] = ", ".join(proj.users)
+        proj_dict["select"] = proj.name == selected_project.name
+
+        proj_data.append(proj_dict)
+    return proj_data
+
+
+def add_new_project(number=1):
+    user_email = get_user_email()
+    default_proj_name = f"{user_email.split('@')[0]}_#{number}"
+    project = Project(name=default_proj_name, owner=get_user_email())
+
+    project = save_project(project)
+    set_selected_project(project)
+
+    set_state(
+        ProjectState.PROJECT_SUCCESS_MESSAGE,
+        f"Project **'{default_proj_name}'** has been initialised.",
+    )
+
+    st.experimental_rerun()
+
+
+def get_next_project_number(projects: list[Project]):
+    highest_number = len(projects) + 1
+    for proj in projects:
+        proj_number = proj.name.split("#")[1]
+        try:
+            proj_number = int(proj_number)
+            if proj_number >= highest_number:
+                highest_number = proj_number + 1
+        except ValueError:
+            pass
+    return highest_number
+
+
+def project_manager(
+    st_context=st.sidebar,
+    render_layout: Literal["vertical", "horizontal", "compact"] = "vertical",
+):
+    delete_confirm = get_state(ProjectState.PROJECT_DELETE_CONFIRM)
+    project_to_delete = get_state(ProjectState.PROJECT_TO_DELETE, None)
+    success_message = get_state(ProjectState.PROJECT_SUCCESS_MESSAGE)
+    warning_message = get_state(ProjectState.PROJECT_WARNING_MESSAGE)
+    get_state(ProjectState.UPLOAD_DELETE_CONFIRM)
+    get_state(ProjectState.FOLDER_TO_DELETE)
+    get_state(ProjectState.UPLOAD_SUCCESS_MESSAGE)
+    get_state(ProjectState.UPLOAD_WARNING_MESSAGE)
+
+    st_context.subheader("Manage Projects")
+
+    if success_message:
+        st.success(success_message)
+    if warning_message:
+        st.warning(warning_message)
+    if delete_confirm and project_to_delete:
+        st.warning(delete_confirm)
+        st.button("I'm Sure", on_click=action_delete, args=(project_to_delete,))
+
+    if render_layout == "vertical":
+        grid_container = st_context.container()
+
+        select_container = st_context.container()
+
+        container1, container2, container3 = st_context.columns([1, 1, 1])
+    elif render_layout == "horizontal":
+        grid_container = st_context.container()
+        select_container, container1, container2, container3, _ = st_context.columns([6, 1, 1, 1, 3])
+
+        # do some spacing that is particular to this layout
+        container1.markdown("#")
+        container1.markdown("#")
+        container2.markdown("#")
+        container2.markdown("#")
+        container3.markdown("#")
+        container3.markdown("#")
+    else:
+        grid_container = st_context.container()
+
+        select_container = st_context.container()
+
+        container1 = st_context.container()
+        container2 = st_context.container()
+        container3 = st_context.container()
+
+    with select_container:
+        project, projects = project_selector(
+            header_text=None,
+            null_option=None,
+            select_box_label="Select Project",
+            st_context=select_container,  # type: ignore
+        )
+
+        if len(projects) < 1:
+            add_new_project()
+
+    with grid_container:
+        if render_layout == "compact":
+            column_order = [
+                "name",
+                "description",
+                "public",
+                "owner",
+                "users",
+            ]
+
+            set_col_width = "small"
+        else:
+            column_order = [
+                # "select",
+                # "id",
+                "select",
+                "name",
+                "description",
+                "application",
+                "public",
+                "owner",
+                "users",
+                "folders",
+                "files",
+            ]
+            set_col_width = None  # columns will be sized to fit thier contents
+
+        edited_project_data = st.data_editor(
+            pd.DataFrame(get_projects_data(projects)),
+            key="project_editor_key",
+            use_container_width=True,
+            hide_index=True,
+            # num_rows="dynamic",
+            column_order=column_order,
+            column_config={
+                "select": st.column_config.CheckboxColumn(
+                    label="Selected",
+                    help="Currently selected project",
+                    width=None,
+                    disabled=True,
+                ),
+                "name": st.column_config.TextColumn(label="Project Name", help="The name of the project", width=None),
+                "description": st.column_config.Column(
+                    label="Description",
+                    help="General project description",
+                    width=set_col_width,
+                ),
+                "application": st.column_config.Column(
+                    label="Application",
+                    help="The application that utilises this project",
+                    disabled=True,
+                    width=None,
+                ),
+                "owner": st.column_config.Column(
+                    label="Owner",
+                    help="The owner of the project",
+                    disabled=True,
+                    width=set_col_width,
+                ),
+                "public": st.column_config.CheckboxColumn(
+                    label="Public",
+                    help="Whether the project is available to all users",
+                    width=None,
+                ),
+                "files": st.column_config.Column(
+                    help="The list of files contained with the project",
+                    disabled=True,
+                    width=None,
+                ),
+                "folders": st.column_config.Column(
+                    help="The list of folders contained with the project",
+                    disabled=True,
+                ),
+                "users": st.column_config.Column(
+                    label="Allowed Users (emails , separated)",
+                    help="The list of users with access to the project",
+                    disabled=False,
+                    width=set_col_width,
+                ),
+            },
+        )
+
+        with container1:
+            if st.button("Add New"):
+                new_proj_number = get_next_project_number(projects)
+                add_new_project(new_proj_number)
+
+        with container2:
+            if st.button("Delete Selected"):
+                submit_delete_project(project)
+                st.experimental_rerun()
+
+        with container3:
+            if st.button("Save Changes") and st.session_state.get("project_editor_key").get("edited_rows") is not None:
+                update_messages = []
+                project_table_data = st.session_state.get("project_editor_key")
+                for changed_id in project_table_data["edited_rows"]:
+                    # Get latest DB copy of the project
+                    db_project = get_project(
+                        str(edited_project_data["id"][changed_id]),
+                        st.session_state.project_cache,
+                    )
+                    if db_project is None:
+                        set_state(
+                            ProjectState.PROJECT_WARNING_MESSAGE,
+                            f"Cannot update project: **'{edited_project_data['name'][changed_id]}'** "
+                            + " not found in database",
+                        )
+                    else:
+                        db_project.__dict__.update(
+                            {
+                                "name": edited_project_data["name"][changed_id],
+                                "description": edited_project_data["description"][changed_id],
+                                "users": seperate_users(edited_project_data["users"][changed_id]),
+                                "public": bool(edited_project_data["public"][changed_id]),
+                            }
+                        )
+                        if project_duplicate_exists(db_project.name, db_project.owner, str(db_project.id)):
+                            set_state(
+                                ProjectState.PROJECT_WARNING_MESSAGE,
+                                f"Cannot update project: A Project with the name: **'{db_project.name}'** "
+                                + "already exists",
+                            )
+                        else:
+                            db_project = save_project(db_project)
+                            update_messages.append(f"Project **'{db_project.name}'** updated successfully")
+
+                set_state(
+                    ProjectState.PROJECT_SUCCESS_MESSAGE,
+                    "".join([f"> 1. {msg} \n" for msg in update_messages]),
+                )
+                st.experimental_rerun()
+
+    return project, projects
```

### Comparing `xt_st_common-0.6.1/src/xt_st_common/project_models.py` & `xt_st_common-0.7.0/src/xt_st_common/project_models.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/xt_st_common/session.py` & `xt_st_common-0.7.0/src/xt_st_common/session.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/src/xt_st_common/storage.py` & `xt_st_common-0.7.0/src/xt_st_common/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     def set_size(self, _bytes: int):
         self.size = sizeof_fmt(_bytes)
         self.size_bytes = _bytes
 
     def get_prefix(self):
         return self.path.rsplit("/", 1)[0]
 
+    def get_folder(self):
+        return self.path.rsplit("/", 2)[1]
+
     def get_ext(self):
         parts = self.name.rsplit(".", 1)
         return None if len(parts) <= 1 else f".{parts[-1]}"
 
 
 class StorageClient(ABC):
     @abstractmethod
```

### Comparing `xt_st_common-0.6.1/src/xt_st_common/utils.py` & `xt_st_common-0.7.0/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.6.1/PKG-INFO` & `xt_st_common-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.6.1
+Version: 0.7.0
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
 Requires-Python: >3.9.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,20 +14,20 @@
 Requires-Dist: chardet (>=4.0.0,<6.0)
 Requires-Dist: minio (>=7.1.14,<8.0.0) ; extra == "storage"
 Requires-Dist: plotly (>=4.14.3)
 Requires-Dist: pydantic (>=1.10.7)
 Requires-Dist: pyjwt[crypto] (>=2.6.0,<3.0.0)
 Requires-Dist: pymongo (>=4.3.3) ; extra == "databases"
 Requires-Dist: pymongo-auth-aws (>=1.1.0) ; extra == "databases"
-Requires-Dist: streamlit (>=1.22.0)
+Requires-Dist: streamlit (>=1.23.1)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.6.1
+# XT-STREAMLIT - 0.7.0
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

