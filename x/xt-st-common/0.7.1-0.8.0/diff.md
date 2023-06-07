# Comparing `tmp/xt_st_common-0.7.1.tar.gz` & `tmp/xt_st_common-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.7.1.tar", max compression
+gzip compressed data, was "xt_st_common-0.8.0.tar", max compression
```

## Comparing `xt_st_common-0.7.1.tar` & `xt_st_common-0.8.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      720 2023-06-07 13:41:54.002649 xt_st_common-0.7.1/README.md
--rw-r--r--   0        0        0     2603 2023-06-07 13:41:54.002649 xt_st_common-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6128 2023-06-07 13:41:22.998116 xt_st_common-0.7.1/src/streamlit_plotly_events/__init__.py
--rw-r--r--   0        0        0      180 2023-06-07 13:41:22.998116 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/.env
--rw-r--r--   0        0        0       67 2023-06-07 13:41:22.998116 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/.prettierrc
--rw-r--r--   0        0        0      859 2023-06-07 13:41:22.998116 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2052 2023-06-07 13:41:22.998116 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/index.html
--rw-r--r--   0        0        0      564 2023-06-07 13:41:22.998116 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
--rw-r--r--   0        0        0     1183 2023-06-07 13:41:22.998116 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/service-worker.js
--rw-r--r--   0        0        0  4138182 2023-06-07 13:41:23.018116 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
--rw-r--r--   0        0        0     3326 2023-06-07 13:41:23.018116 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 16152785 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
--rw-r--r--   0        0        0     1442 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
--rw-r--r--   0        0        0     3848 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
--rw-r--r--   0        0        0     1598 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0        0        0     8317 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
--rw-r--r--   0        0        0     1141 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/package.json
--rw-r--r--   0        0        0      839 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/public/index.html
--rw-r--r--   0        0        0     1922 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
--rw-r--r--   0        0        0      274 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/tsconfig.json
--rw-r--r--   0        0        0       22 2023-06-07 13:41:54.002649 xt_st_common-0.7.1/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5010 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/xt_st_common/components.py
--rw-r--r--   0        0        0     2371 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/xt_st_common/config.py
--rw-r--r--   0        0        0     3177 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/xt_st_common/database.py
--rw-r--r--   0        0        0     6303 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0    35075 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/xt_st_common/project_components.py
--rw-r--r--   0        0        0     6518 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/xt_st_common/project_models.py
--rw-r--r--   0        0        0     5976 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/xt_st_common/session.py
--rw-r--r--   0        0        0     6450 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1957 2023-06-07 13:41:23.098118 xt_st_common-0.7.1/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-06-07 15:01:42.693166 xt_st_common-0.8.0/README.md
+-rw-r--r--   0        0        0     2603 2023-06-07 15:01:42.689166 xt_st_common-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6128 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/.env
+-rw-r--r--   0        0        0       67 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/.prettierrc
+-rw-r--r--   0        0        0      859 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2052 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/index.html
+-rw-r--r--   0        0        0      564 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
+-rw-r--r--   0        0        0     1183 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/service-worker.js
+-rw-r--r--   0        0        0  4138182 2023-06-07 15:01:03.696755 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
+-rw-r--r--   0        0        0     3326 2023-06-07 15:01:03.696755 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 16152785 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
+-rw-r--r--   0        0        0     1442 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
+-rw-r--r--   0        0        0     3848 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
+-rw-r--r--   0        0        0     1598 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0        0        0     8317 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0        0        0     1141 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/package.json
+-rw-r--r--   0        0        0      839 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/public/index.html
+-rw-r--r--   0        0        0     1922 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
+-rw-r--r--   0        0        0      274 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/tsconfig.json
+-rw-r--r--   0        0        0       22 2023-06-07 15:01:42.689166 xt_st_common-0.8.0/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5010 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     2371 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     3177 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/database.py
+-rw-r--r--   0        0        0     6303 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0    35117 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/project_components.py
+-rw-r--r--   0        0        0     6518 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/project_models.py
+-rw-r--r--   0        0        0     5976 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     6450 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1957 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.8.0/PKG-INFO
```

### Comparing `xt_st_common-0.7.1/README.md` & `xt_st_common-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.7.1
+# XT-STREAMLIT - 0.8.0
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

### Comparing `xt_st_common-0.7.1/pyproject.toml` & `xt_st_common-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.7.1"
+version = "0.8.0"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}, {include = "streamlit_plotly_events", from= "src"}]
 
 [tool.poe.tasks]
 test = { cmd="pytest --cov=src/xt_st_common", help="Run unit tests"}
```

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/__init__.py` & `xt_st_common-0.8.0/src/streamlit_plotly_events/__init__.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/asset-manifest.json` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/index.html` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/service-worker.js` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/package.json` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/package.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/public/index.html` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx` & `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/xt_st_common/components.py` & `xt_st_common-0.8.0/src/xt_st_common/components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/xt_st_common/config.py` & `xt_st_common-0.8.0/src/xt_st_common/config.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/xt_st_common/database.py` & `xt_st_common-0.8.0/src/xt_st_common/database.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/xt_st_common/fs_upload_page.py` & `xt_st_common-0.8.0/src/xt_st_common/fs_upload_page.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/xt_st_common/project_components.py` & `xt_st_common-0.8.0/src/xt_st_common/project_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
 def get_proj_options(include_public: bool, cache_id=None):
     selected_project = get_selected_project()
     projects = get_projects(include_public, get_project_cache())
     sel_idx = 0
     options = {}
     for idx, proj in enumerate(projects):
         if selected_project and proj.id == selected_project.id:
-            sel_idx = idx + 1
+            sel_idx = idx
         options[idx] = proj.name
     return options, projects, sel_idx
 
 
 def on_project_select():
     proj_idx = get_state("project_select")
     include_public = bool(get_state("include_public_projects", False))
@@ -327,33 +327,39 @@
     """
     selected_project = None
 
     if header_text is not None:
         st_context.subheader(header_text)
     include_public = st_context.checkbox("Include Public", value=False, key="include_public_projects")
     options, projects, sel_idx = get_proj_options(include_public, get_project_cache())
-    proj_options = {-1: null_option} if null_option is not None else {}
-    sel_idx = 0 if len(proj_options) < 2 else sel_idx  # ensure sel_idx is never greater than proj_options
+    proj_options = {}
+
+    # accomodate the null option if one is provided
+    if null_option is not None:
+        proj_options = {-1: null_option}
+        sel_idx = sel_idx + 1
+
     if options is not None:
         proj_options = {**proj_options, **options}
 
     if len(proj_options) > 0:
         proj_idx = st_context.selectbox(
             select_box_label,
             key="project_select",
             index=sel_idx,
             # on_change=on_project_select,
             options=proj_options.keys(),
             format_func=lambda x: proj_options[x],
         )
 
         selected_project = None
-        if proj_idx is not None and proj_idx > -1:
+        if proj_idx is not None:
             selected_project = projects[proj_idx] if proj_idx != -1 else None
             set_selected_project(selected_project)
+
     else:
         st_context.warning("No projects were found")
 
     return selected_project, projects
 
 
 def load_csv(
@@ -701,22 +707,23 @@
         state_reset()
     return path, folder
 
 
 def get_projects_data(projects):
     selected_project = get_selected_project()
     proj_data = []
+
     for proj in projects:
         proj_dict = proj.dict(exclude={"files"})
         # proj_dict = proj.dict(exclude={"files", "folders", "id"})
 
         # proj_dict["folders"] = "\n".join(proj.folders)
         proj_dict["files"] = [file.name for file in proj.files]
         proj_dict["users"] = ", ".join(proj.users)
-        proj_dict["select"] = proj.name == selected_project.name
+        proj_dict["select"] = selected_project is not None and proj.name == selected_project.name
 
         proj_data.append(proj_dict)
     return proj_data
 
 
 def add_new_project(number=1):
     user_email = get_user_email()
@@ -745,14 +752,15 @@
         except (ValueError, IndexError):
             pass
     return highest_number
 
 
 def project_manager(
     st_context=st.sidebar,
+    null_option=None,
     render_layout: Literal["vertical", "horizontal", "compact"] = "vertical",
 ):
     delete_confirm = get_state(ProjectState.PROJECT_DELETE_CONFIRM)
     project_to_delete = get_state(ProjectState.PROJECT_TO_DELETE, None)
     success_message = get_state(ProjectState.PROJECT_SUCCESS_MESSAGE)
     warning_message = get_state(ProjectState.PROJECT_WARNING_MESSAGE)
     get_state(ProjectState.UPLOAD_DELETE_CONFIRM)
@@ -795,15 +803,15 @@
         container1 = st_context.container()
         container2 = st_context.container()
         container3 = st_context.container()
 
     with select_container:
         project, projects = project_selector(
             header_text=None,
-            null_option=None,
+            null_option=null_option,
             select_box_label="Select Project",
             st_context=select_container,  # type: ignore
         )
 
         if len(projects) < 1:
             add_new_project()
```

### Comparing `xt_st_common-0.7.1/src/xt_st_common/project_models.py` & `xt_st_common-0.8.0/src/xt_st_common/project_models.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/xt_st_common/session.py` & `xt_st_common-0.8.0/src/xt_st_common/session.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/xt_st_common/storage.py` & `xt_st_common-0.8.0/src/xt_st_common/storage.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/src/xt_st_common/utils.py` & `xt_st_common-0.8.0/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.7.1/PKG-INFO` & `xt_st_common-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.7.1
+Version: 0.8.0
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
 Requires-Dist: streamlit (>=1.23.1)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.7.1
+# XT-STREAMLIT - 0.8.0
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

