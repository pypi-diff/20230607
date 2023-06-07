# Comparing `tmp/rising_plugin-0.222.100.tar.gz` & `tmp/rising_plugin-0.333.1.tar.gz`

## Comparing `rising_plugin-0.222.100.tar` & `rising_plugin-0.333.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.github/workflows/lint.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/.gitignore
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/Rising_Plugin.iml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/vcs.xml
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/workspace.xml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/inspectionProfiles/profiles_settings.xml
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/__init__.py
--rwxr-xr-x   0        0        0      796 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/csv_embed.py
--rwxr-xr-x   0        0        0     1756 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/image_embedding.py
--rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/pinecone_engine.py
--rwxr-xr-x   0        0        0     3604 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/risingplugin.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/common/__init__.py
--rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/common/utils.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/__init__.py
--rwxr-xr-x   0        0        0      881 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/config.yml
--rwxr-xr-x   0        0        0      552 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/general.co
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/off-security.co
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/__init__.py
--rwxr-xr-x   0        0        0     3030 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/actions.py
--rwxr-xr-x   0        0        0     2415 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/phone.csv
--rwxr-xr-x   0        0        0   486145 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/phone.json
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/tests/__init__.py
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/LICENSE
--rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/README.md
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/pyproject.toml
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/PKG-INFO
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/.idea/.gitignore
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/.idea/Rising_Plugin.iml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/.idea/watcherTasks.xml
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/.idea/inspectionProfiles/profiles_settings.xml
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/__init__.py
+-rwxr-xr-x   0        0        0      796 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/csv_embed.py
+-rwxr-xr-x   0        0        0     1756 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/image_embedding.py
+-rwxr-xr-x   0        0        0     1916 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/pinecone_engine.py
+-rwxr-xr-x   0        0        0     3664 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/risingplugin.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/common/__init__.py
+-rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/common/utils.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/guardrails-config/__init__.py
+-rwxr-xr-x   0        0        0      881 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/guardrails-config/config.yml
+-rwxr-xr-x   0        0        0      552 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/guardrails-config/general.co
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/guardrails-config/off-security.co
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/guardrails-config/actions/__init__.py
+-rwxr-xr-x   0        0        0     3056 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/guardrails-config/actions/actions.py
+-rwxr-xr-x   0        0        0     2415 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/guardrails-config/actions/phone.csv
+-rwxr-xr-x   0        0        0   486145 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/src/rising_plugin/guardrails-config/actions/phone.json
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/tests/__init__.py
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/LICENSE
+-rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/README.md
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/pyproject.toml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 rising_plugin-0.333.1/PKG-INFO
```

### Comparing `rising_plugin-0.222.100/.idea/workspace.xml` & `rising_plugin-0.333.1/.idea/workspace.xml`

 * *Files 19% similar despite different names*

#### Comparing `rising_plugin-0.222.100/.idea/workspace.xml` & `rising_plugin-0.333.1/.idea/workspace.xml`

```diff
@@ -1,29 +1,25 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="ed398cd8-e9f5-42d3-bcf0-bd7cc45baf32" name="Changes" comment="Updated with stable version: 0.1.2">
+    <list default="true" id="ed398cd8-e9f5-42d3-bcf0-bd7cc45baf32" name="Changes" comment="feature: fixed image relatedness issue">
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/rising_plugin/common/utils.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/rising_plugin/common/utils.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/rising_plugin/guardrails-config/actions/actions.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/rising_plugin/guardrails-config/actions/actions.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/rising_plugin/guardrails-config/actions/phone.csv" beforeDir="false" afterPath="$PROJECT_DIR$/src/rising_plugin/guardrails-config/actions/phone.csv" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/rising_plugin/guardrails-config/actions/phone.json" beforeDir="false" afterPath="$PROJECT_DIR$/src/rising_plugin/guardrails-config/actions/phone.json" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_BRANCH_BY_REPOSITORY">
       <map>
-        <entry key="$PROJECT_DIR$" value="main"/>
+        <entry key="$PROJECT_DIR$" value="feature/delete_all_namespace_pinecone"/>
       </map>
     </option>
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
@@ -32,21 +28,21 @@
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "WebServerToolWindowFactoryState": "false",
-    "git-widget-placeholder": "bugfix/open__browser__21",
+    "git-widget-placeholder": "bugfix/image__relatedness",
     "last_opened_file_path": "/home/luck/work/projects/risingland/public_release/Rising_Plugin/src/rising_plugin/risingplugin.py",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
-    "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable",
+    "settings.editor.selected.configurable": "watcher.settings",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="RunManager">
     <configuration name="Plugin" type="PythonConfigurationType" factoryName="Python">
       <module name="Rising_Plugin"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
@@ -85,15 +81,16 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="ed398cd8-e9f5-42d3-bcf0-bd7cc45baf32" name="Changes" comment=""/>
       <created>1685979036747</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1685979036747</updated>
-      <workItem from="1685979037968" duration="7567000"/>
+      <workItem from="1685979037968" duration="11832000"/>
+      <workItem from="1686068572794" duration="16557000"/>
     </task>
     <task id="LOCAL-00001" summary="Initial Commit">
       <created>1685979134698</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1685979134698</updated>
@@ -101,19 +98,51 @@
     <task id="LOCAL-00002" summary="Updated with stable version: 0.1.2">
       <created>1685979287411</created>
       <option name="number" value="00002"/>
       <option name="presentableId" value="LOCAL-00002"/>
       <option name="project" value="LOCAL"/>
       <updated>1685979287411</updated>
     </task>
-    <option name="localTasksCounter" value="3"/>
+    <task id="LOCAL-00003" summary="feature(#21) Updated with stable version: 0.1.3 with fixing to launch a browser in its prompt.">
+      <created>1686066822051</created>
+      <option name="number" value="00003"/>
+      <option name="presentableId" value="LOCAL-00003"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1686066822051</updated>
+    </task>
+    <task id="LOCAL-00004" summary="feature(#21) black lint issue fixed.">
+      <created>1686069587066</created>
+      <option name="number" value="00004"/>
+      <option name="presentableId" value="LOCAL-00004"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1686069587066</updated>
+    </task>
+    <task id="LOCAL-00005" summary="feature(#31) implemented to delete all items in pinecone namespace.">
+      <created>1686091888487</created>
+      <option name="number" value="00005"/>
+      <option name="presentableId" value="LOCAL-00005"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1686091888487</updated>
+    </task>
+    <task id="LOCAL-00006" summary="feature: fixed image relatedness issue">
+      <created>1686167046207</created>
+      <option name="number" value="00006"/>
+      <option name="presentableId" value="LOCAL-00006"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1686167046207</updated>
+    </task>
+    <option name="localTasksCounter" value="7"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="Initial Commit"/>
     <MESSAGE value="Updated with stable version: 0.1.2"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Updated with stable version: 0.1.2"/>
+    <MESSAGE value="feature(#21) Updated with stable version: 0.1.3 with fixing to launch a browser in its prompt."/>
+    <MESSAGE value="feature(#21) black lint issue fixed."/>
+    <MESSAGE value="feature(#31) implemented to delete all items in pinecone namespace."/>
+    <MESSAGE value="feature: fixed image relatedness issue"/>
+    <option name="LAST_COMMIT_MESSAGE" value="feature: fixed image relatedness issue"/>
   </component>
 </project>
```

### Comparing `rising_plugin-0.222.100/.idea/inspectionProfiles/Project_Default.xml` & `rising_plugin-0.333.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.222.100/src/rising_plugin/csv_embed.py` & `rising_plugin-0.333.1/src/rising_plugin/csv_embed.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.222.100/src/rising_plugin/image_embedding.py` & `rising_plugin-0.333.1/src/rising_plugin/image_embedding.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.222.100/src/rising_plugin/pinecone_engine.py` & `rising_plugin-0.333.1/src/rising_plugin/pinecone_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,14 +57,23 @@
 
 def delete_pinecone(namespace: str, key: str) -> Any:
     index = init_pinecone(PINECONE_INDEX_NAME)
     delete_response = index.delete(ids=[key], namespace=namespace)
     return delete_response
 
 
+"""delete all item in the namespace"""
+
+
+def delete_all_pinecone(namespace: str) -> Any:
+    index = init_pinecone(PINECONE_INDEX_NAME)
+    delete_response = index.delete(delete_all=True, namespace=namespace)
+    return delete_response
+
+
 """generate index name of pinecone"""
 
 
 def get_pinecone_index_name(uuid):
     return PINECONE_INDEX_NAME + "-" + uuid
```

### Comparing `rising_plugin-0.222.100/src/rising_plugin/risingplugin.py` & `rising_plugin-0.333.1/src/rising_plugin/risingplugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,17 @@
 
     message = app.generate(messages=[{"role": "user", "content": query}])
     return message["content"]
 
 
 def query_image_ask(image_content, message, uuid):
     prompt_template = get_prompt_image_with_message(image_content, message)
-    data = getCompletion(prompt_template, uuid, False)
-    chain_data = json.loads(data.replace("'", '"'))
+    data = getCompletion(query=prompt_template, uuid=uuid, image_search=False)
+    # chain_data = json.loads(data.replace("'", '"'))
+    chain_data = json.loads(data)
     if chain_data["program"] == "image":
         return True
     return False
 
 
 def getTextFromImage(filename):
     # Create a reference to the image file you want to download
```

### Comparing `rising_plugin-0.222.100/src/rising_plugin/common/utils.py` & `rising_plugin-0.333.1/src/rising_plugin/common/utils.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.222.100/src/rising_plugin/guardrails-config/config.yml` & `rising_plugin-0.333.1/src/rising_plugin/guardrails-config/config.yml`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.222.100/src/rising_plugin/guardrails-config/general.co` & `rising_plugin-0.333.1/src/rising_plugin/guardrails-config/general.co`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/actions.py` & `rising_plugin-0.333.1/src/rising_plugin/guardrails-config/actions/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 )
 from rising_plugin.image_embedding import (
     query_image_text,
 )
 
 from nemoguardrails.actions import action
 
-from src.rising_plugin.common.utils import COMMAND_BROWSER_OPEN
+from rising_plugin.common.utils import COMMAND_BROWSER_OPEN
 
 
 @action()
 async def general_question(query, model, uuid, image_search):
     llm = ChatOpenAI(model_name=model, temperature=0, openai_api_key=OPENAI_API_KEY)
     chain = load_qa_chain(llm, chain_type="stuff")
     file_path = os.path.dirname(os.path.abspath(__file__))
@@ -74,9 +74,11 @@
             #     return result
         return str(result)
     except ValueError as e:
         # Check sms andd browser query
         if doc_list[0] in COMMAND_SMS_INDEXS:
             return str(json.dumps({"program": "sms", "content": chain_data}))
         elif doc_list[0] in COMMAND_BROWSER_OPEN:
-            return str(json.dumps({"program": "browser", "content": "https://google.com"}))
+            return str(
+                json.dumps({"program": "browser", "content": "https://google.com"})
+            )
         return str(json.dumps({"program": "message", "content": chain_data}))
```

### Comparing `rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/phone.csv` & `rising_plugin-0.333.1/src/rising_plugin/guardrails-config/actions/phone.csv`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/phone.json` & `rising_plugin-0.333.1/src/rising_plugin/guardrails-config/actions/phone.json`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.222.100/LICENSE` & `rising_plugin-0.333.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.222.100/pyproject.toml` & `rising_plugin-0.333.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rising_plugin"
-version = "0.222.100"
+version = "0.333.1"
 authors = [
   { name="Thomas Richardson", email="thomasr37oss@gmail.com" },
 ]
 description = "It is a plugin for Rising GPT"
 readme = "README.md"
 dependencies = [
-    "langchain >= 0.0.148",
-    "pinecone-client >= 2.2.1",
-    "openai >= 0.27.4",
-    "pydantic>=1.2.4",
+    "langchain==0.0.191",
+    "pinecone-client==2.2.1",
+    "openai==0.27.4",
+    "pydantic==1.10.6",
     "aiohttp==3.8.4",
-    "langchain==0.0.167",
+    "langchain==0.0.191",
     "requests==2.28.2",
     "typer==0.7.0",
     "PyYAML~=6.0",
-    "setuptools>=50.5.1",
+    "setuptools==59.6.0",
     "annoy==1.17.1",
     "sentence-transformers==2.2.2",
     "fastapi==0.95.0",
     "starlette==0.26.1",
     "uvicorn==0.21.1",
     "httpx==0.23.3",
     "simpleeval==0.9.13",
```

### Comparing `rising_plugin-0.222.100/PKG-INFO` & `rising_plugin-0.333.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: rising_plugin
-Version: 0.222.100
+Version: 0.333.1
 Summary: It is a plugin for Rising GPT
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Thomas Richardson <thomasr37oss@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: annoy==1.17.1
 Requires-Dist: fastapi==0.95.0
 Requires-Dist: httpx==0.23.3
-Requires-Dist: langchain==0.0.167
-Requires-Dist: langchain>=0.0.148
+Requires-Dist: langchain==0.0.191
 Requires-Dist: nemoguardrails==0.2.0
-Requires-Dist: openai>=0.27.4
-Requires-Dist: pinecone-client>=2.2.1
-Requires-Dist: pydantic>=1.2.4
+Requires-Dist: openai==0.27.4
+Requires-Dist: pinecone-client==2.2.1
+Requires-Dist: pydantic==1.10.6
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: requests==2.28.2
 Requires-Dist: sentence-transformers==2.2.2
-Requires-Dist: setuptools>=50.5.1
+Requires-Dist: setuptools==59.6.0
 Requires-Dist: simpleeval==0.9.13
 Requires-Dist: starlette==0.26.1
 Requires-Dist: typer==0.7.0
 Requires-Dist: typing-extensions==4.5.0
 Requires-Dist: uvicorn==0.21.1
 Description-Content-Type: text/markdown
```

