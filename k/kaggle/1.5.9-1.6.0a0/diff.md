# Comparing `tmp/kaggle-1.5.9.tar.gz` & `tmp/kaggle-1.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kaggle-1.5.9.tar", last modified: Wed Oct 21 18:13:20 2020, max compression
+gzip compressed data, was "kaggle-1.6.0a0.tar", last modified: Wed Jun  7 17:10:58 2023, max compression
```

## Comparing `kaggle-1.5.9.tar` & `kaggle-1.6.0a0.tar`

### file list

```diff
@@ -1,39 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-21 18:13:20.000000 kaggle-1.5.9/
--rw-r-----   0 root         (0) root         (0)       19 2020-10-21 18:12:49.000000 kaggle-1.5.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      431 2020-10-21 18:13:20.000000 kaggle-1.5.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24776 2020-10-21 18:12:49.000000 kaggle-1.5.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-21 18:13:20.000000 kaggle-1.5.9/kaggle/
--rw-r--r--   0 root         (0) root         (0)      799 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-21 18:13:20.000000 kaggle-1.5.9/kaggle/api/
--rw-r--r--   0 root         (0) root         (0)      742 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   125827 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/api/kaggle_api.py
--rw-r-----   0 root         (0) root         (0)   110604 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/api/kaggle_api_extended.py
--rw-r--r--   0 root         (0) root         (0)    25458 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/api_client.py
--rw-r-----   0 root         (0) root         (0)    53449 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/cli.py
--rw-r--r--   0 root         (0) root         (0)     8858 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-21 18:13:20.000000 kaggle-1.5.9/kaggle/models/
--rw-r--r--   0 root         (0) root         (0)     1481 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4851 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/models/collaborator.py
--rw-r--r--   0 root         (0) root         (0)     7424 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/models/dataset_column.py
--rw-r--r--   0 root         (0) root         (0)    12317 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/models/dataset_new_request.py
--rw-r--r--   0 root         (0) root         (0)    10027 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/models/dataset_new_version_request.py
--rw-r--r--   0 root         (0) root         (0)    10114 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/models/dataset_update_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     5544 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/models/dataset_upload_file.py
--rw-r--r--   0 root         (0) root         (0)     4342 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/models/error.py
--rw-r-----   0 root         (0) root         (0)     6180 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/models/kaggle_models_extended.py
--rw-r--r--   0 root         (0) root         (0)    18059 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/models/kernel_push_request.py
--rw-r--r--   0 root         (0) root         (0)     4077 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/models/license.py
--rw-r--r--   0 root         (0) root         (0)     2895 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/models/result.py
--rw-r--r--   0 root         (0) root         (0)    13927 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-21 18:13:20.000000 kaggle-1.5.9/kaggle/tests/
--rw-r-----   0 root         (0) root         (0)      596 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/tests/__init__.py
--rw-r-----   0 root         (0) root         (0)     1780 2020-10-21 18:12:50.000000 kaggle-1.5.9/kaggle/tests/test_authenticate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-21 18:13:20.000000 kaggle-1.5.9/kaggle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      431 2020-10-21 18:13:20.000000 kaggle-1.5.9/kaggle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      861 2020-10-21 18:13:20.000000 kaggle-1.5.9/kaggle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-21 18:13:20.000000 kaggle-1.5.9/kaggle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2020-10-21 18:13:20.000000 kaggle-1.5.9/kaggle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2020-10-21 18:13:20.000000 kaggle-1.5.9/kaggle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2020-10-21 18:13:20.000000 kaggle-1.5.9/kaggle.egg-info/top_level.txt
--rw-r-----   0 root         (0) root         (0)       79 2020-10-21 18:13:20.000000 kaggle-1.5.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1464 2020-10-21 18:12:50.000000 kaggle-1.5.9/setup.py
+drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-07 17:10:57.997743 kaggle-1.6.0a0/
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    11541 2023-06-07 17:10:55.000000 kaggle-1.6.0a0/LICENSE
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)       19 2023-06-07 17:10:55.000000 kaggle-1.6.0a0/MANIFEST.in
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)      609 2023-06-07 17:10:57.997743 kaggle-1.6.0a0/PKG-INFO
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    34704 2023-06-07 17:10:55.000000 kaggle-1.6.0a0/README.md
+drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-07 17:10:57.985743 kaggle-1.6.0a0/kaggle/
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)      799 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/__init__.py
+drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-07 17:10:57.989743 kaggle-1.6.0a0/kaggle/api/
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)      742 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/api/__init__.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)   191004 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/api/kaggle_api.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)   152973 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/api/kaggle_api_extended.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    25458 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/api_client.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    73219 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/cli.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     8858 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/configuration.py
+drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-07 17:10:57.997743 kaggle-1.6.0a0/kaggle/models/
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     1849 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/__init__.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     4851 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/models/collaborator.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     7424 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/dataset_column.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    12281 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/dataset_new_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     9991 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/dataset_new_version_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    10114 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/models/dataset_update_settings_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     4342 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/error.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     6915 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/kaggle_models_extended.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    19316 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/models/kernel_push_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     4077 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/license.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     5051 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/models/model_instance_new_version_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     9699 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/model_instance_update_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    12103 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/model_new_instance_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    10055 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/models/model_new_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     9096 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/model_update_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     2895 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/models/result.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     5439 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/upload_file.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    13927 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/rest.py
+drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-07 17:10:57.997743 kaggle-1.6.0a0/kaggle/tests/
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)      596 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/tests/__init__.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     1782 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/tests/test_authenticate.py
+drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-07 17:10:57.989743 kaggle-1.6.0a0/kaggle.egg-info/
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)      609 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle.egg-info/PKG-INFO
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     1077 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle.egg-info/SOURCES.txt
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)        1 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle.egg-info/dependency_links.txt
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)       43 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle.egg-info/entry_points.txt
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)       78 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle.egg-info/requires.txt
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)        7 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle.egg-info/top_level.txt
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)       79 2023-06-07 17:10:57.997743 kaggle-1.6.0a0/setup.cfg
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     1680 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kaggle-1.5.9/README.md` & `kaggle-1.6.0a0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 
 The command line tool supports the following commands:
 
 ``` 
 kaggle competitions {list, files, download, submit, submissions, leaderboard}
 kaggle datasets {list, files, download, create, version, init}
 kaggle kernels {list, init, push, pull, output, status}
+kaggle models {get, list, init, create, delete, update}
+kaggle models instances {init, create, delete, update}
+kaggle models instances versions {init, create, download, delete}
 kaggle config {view, set, unset}
 ```
 
 See more details below for using each of these commands.
 
 ### Competitions
 
@@ -530,14 +533,304 @@
   kernel      Kernel URL suffix in format <owner>/<kernel-name> (use "kaggle kernels list" to show options)
 ```
 
 Example:
 
 `kaggle kernels status mrisdal/exploring-survival-on-the-titanic`
 
+### Models
+
+The API supports the following commands for Kaggle Models.
+
+```
+usage: kaggle models [-h]
+                     {get, list, init, create} ...
+
+optional arguments:
+  -h, --help            show this help message and exit
+
+commands:
+  {get, list, init, create}
+    get                 Get the model
+    list                List models
+    init                Initialize metadata file for model creation
+    create              Create a new model
+```
+
+##### Get model
+
+```
+usage: kaggle models get [-h] [-p FOLDER] [model]
+
+required arguments:
+  model                 Model URL suffix in format <owner>/<model-name>
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p PATH, --path PATH  Folder where the special model-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata) will be downloaded (if specified).
+```
+
+Example:
+
+`kaggle models get tensorflow/toxicity`
+
+##### List models
+
+```
+usage: kaggle models list [--sort-by SORT_BY] [-s SEARCH] [--owner OWNER] [--page-token PAGE_TOKEN] [--page-size PAGE_SIZE] [--csv]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --sort-by SORT_BY     Sort list results. Default is 'hotness'. Valid options are 'hotness', 'downloadCount', 'voteCount', 'notebookCount' and 'createTime'
+  -s SEARCH, --search SEARCH
+                        Term(s) to search for
+  --owner OWNER         Find models owned by a specific user or organization
+  --page-token PAGE_TOKEN  
+                        Page token for pagination
+  --page-size PAGE_SIZE Number of items to show on a page. Default size is 20, max is 50
+  -v, --csv             Print results in CSV format (if not set print in table format)
+```
+
+Example:
+
+`kaggle models list -s llm`
+
+`kaggle models list --sort-by downloadCount`
+
+##### Initialize metadata file for a model
+
+```
+usage: kaggle models init [-h] [-p FOLDER]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p FOLDER, --path FOLDER
+                        Folder to create the model-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata). Defaults to current working directory
+```
+
+Example:
+
+`kaggle models init -p /path/to/model`
+
+##### Create a new model
+
+If you want to create a new model, you need to initiate metadata file at first. You could fulfill this by running `kaggle models init` as describe above.
+
+```
+usage: kaggle models create [-h] [-p FOLDER]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p FOLDER, --path FOLDER
+                        Folder containing the special model-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata). Defaults to current working directory
+```
+
+Example:
+
+`kaggle models create -p /path/to/model`
+
+##### Delete model
+
+```
+usage: kaggle models delete [-h] [model]
+
+optional arguments:
+  -h, --help  show this help message and exit
+  model       Model URL suffix in format <owner>/<model-name>
+```
+
+Example:
+
+`kaggle models delete tensorflow/toxicity`
+
+##### Update a model
+
+If you want to update a new model, you need a metadata file at first. You can fetch the data by running `kaggle models get owner/slug -p folder`.
+
+```
+usage: kaggle models update [-h] [-p FOLDER]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p FOLDER, --path FOLDER
+                        Folder containing the special model-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata). Defaults to current working directory
+```
+
+Example:
+
+`kaggle models update -p /path/to/model`
+
+#### Model Instances
+
+The API supports the following commands for Kaggle Model Instances.
+
+```
+usage: kaggle models instances [-h]
+                             {init, create, delete, update} ...
+
+optional arguments:
+  -h, --help            show this help message and exit
+
+commands:
+  {init, create}
+    init                Initialize metadata file for model instance creation
+    create              Create a new model instance
+    delete              Delete a model instance
+```
+
+##### Initialize metadata file for a model instance
+
+```
+usage: kaggle models instances init [-h] [-p FOLDER]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p FOLDER, --path FOLDER
+                        Folder to create the model-instance-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata). Defaults to current working directory
+```
+
+Example:
+
+`kaggle models instances init -p /path/to/modelinstance`
+
+##### Create a new model instance
+
+If you want to create a new model instance, you need to initiate metadata file at first. You could fulfill this by running `kaggle models instances init` as describe above.
+
+```
+usage: kaggle models instances create [-h] [-p FOLDER]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p FOLDER, --path FOLDER
+                        Folder containing the special model-instance-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata). Defaults to current working directory
+  -q, --quiet           Suppress printing information about the upload progress
+  -r {skip,zip,tar}, --dir-mode {skip,zip,tar}
+                        What to do with directories: "skip" - ignore; "zip" - compressed upload; "tar" - uncompressed upload
+```
+
+Example:
+
+`kaggle models instances create -p /path/to/modelinstance`
+
+##### Delete model instance
+
+```
+usage: kaggle models instances delete [-h] [modelInstance]
+
+optional arguments:
+  -h, --help     show this help message and exit
+  modelInstance  Model Instance URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>
+```
+
+Example:
+
+`kaggle models instances delete tensorflow/toxicity/tfjs/default`
+
+##### Update a model instance
+
+```
+usage: kaggle models instances update [-h] [-p FOLDER]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p FOLDER, --path FOLDER
+                        Folder containing the special model-instance-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata). Defaults to current working directory
+```
+
+Example:
+
+`kaggle models instances update -p /path/to/model`
+
+#### Model Instance Versions
+
+The API supports the following commands for Kaggle Model Instance Versions.
+
+```
+usage: kaggle models instances versions [-h]
+                             {init, create, download, delete} ...
+
+optional arguments:
+  -h, --help            show this help message and exit
+
+commands:
+  {init, create}
+    init                Initialize metadata file for model instance version creation
+    create              Create a new model instance version
+    delete              Delete a model instance version
+```
+
+##### Initialize metadata file for a model instance version
+
+```
+usage: kaggle models instances versions init [-h] [-p FOLDER]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p FOLDER, --path FOLDER
+                        Folder to create the model-instance-version-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata). Defaults to current working directory
+```
+
+Example:
+
+`kaggle models instances versions init -p /path/to/modelinstanceversion`
+
+##### Create a new model instance version
+
+If you want to create a new model instance version, you need to initiate metadata file at first. You could fulfill this by running `kaggle models instances versions init` as describe above.
+
+```
+usage: kaggle models instances versions create [-h] [-p FOLDER]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p FOLDER, --path FOLDER
+                        Folder containing the special model-instance-version-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata). Defaults to current working directory
+  -q, --quiet           Suppress printing information about the upload progress
+  -r {skip,zip,tar}, --dir-mode {skip,zip,tar}
+                        What to do with directories: "skip" - ignore; "zip" - compressed upload; "tar" - uncompressed upload
+```
+
+Example:
+
+`kaggle models instances versions create -p /path/to/modelinstanceversion`
+
+##### Download a model instance version
+
+```
+usage: kaggle models instances versions download [-h] [-p PATH] [--untar] [-f] [-q] [modelInstanceVersion]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  modelInstanceVersion  Model Instance version URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>/<version_number>
+  -p PATH, --path PATH  Folder where file(s) will be downloaded, defaults to current working directory
+  --untar               Untar the downloaded file. Will delete the tar file when completed.
+  -f, --force           Skip check whether local version of file is up to date, force file download
+  -q, --quiet           Suppress printing information about the download progress
+```
+
+
+Examples:
+
+`kaggle models instances versions download tensorflow/toxicity/tfjs/default/1`
+
+##### Delete model instance
+
+```
+usage: kaggle models instances versions delete [-h] [modelInstanceVersion]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  modelInstanceVersion  Model Instance version URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>/<version_number>
+```
+
+Example:
+
+`kaggle models instances versions delete tensorflow/toxicity/tfjs/default/1`
+
 ### Config
 
 The API supports the following commands for configuration.
 
 ```
 usage: kaggle config [-h] {view,set,unset} ...
```

### Comparing `kaggle-1.5.9/kaggle/__init__.py` & `kaggle-1.6.0a0/kaggle/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kaggle-1.5.9/kaggle/api/__init__.py` & `kaggle-1.6.0a0/kaggle/api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kaggle-1.5.9/kaggle/api/kaggle_api_extended.py` & `kaggle-1.6.0a0/kaggle/api/kaggle_api_extended.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -37,68 +37,81 @@
 import io
 import json
 import os
 from os.path import expanduser
 from os.path import isfile
 import sys
 import shutil
+import tarfile
 import zipfile
 import tempfile
 from ..api_client import ApiClient
 from kaggle.configuration import Configuration
 from .kaggle_api import KaggleApi
 from ..models.collaborator import Collaborator
 from ..models.dataset_column import DatasetColumn
 from ..models.dataset_new_request import DatasetNewRequest
 from ..models.dataset_new_version_request import DatasetNewVersionRequest
 from ..models.dataset_update_settings_request import DatasetUpdateSettingsRequest
-from ..models.dataset_upload_file import DatasetUploadFile
 from ..models.kaggle_models_extended import Competition
 from ..models.kaggle_models_extended import Dataset
 from ..models.kaggle_models_extended import DatasetNewResponse
 from ..models.kaggle_models_extended import DatasetNewVersionResponse
 from ..models.kaggle_models_extended import File
 from ..models.kaggle_models_extended import FileUploadInfo
 from ..models.kaggle_models_extended import Kernel
 from ..models.kaggle_models_extended import KernelPushResponse
 from ..models.kaggle_models_extended import LeaderboardEntry
 from ..models.kaggle_models_extended import ListFilesResult
 from ..models.kaggle_models_extended import Metadata
+from ..models.kaggle_models_extended import Model
+from ..models.kaggle_models_extended import ModelNewResponse
+from ..models.kaggle_models_extended import ModelDeleteResponse
 from ..models.kaggle_models_extended import Submission
 from ..models.kaggle_models_extended import SubmitResult
 from ..models.kernel_push_request import KernelPushRequest
 from ..models.license import License
+from ..models.model_new_request import ModelNewRequest
+from ..models.model_new_instance_request import ModelNewInstanceRequest
+from ..models.model_instance_new_version_request import ModelInstanceNewVersionRequest
+from ..models.model_update_request import ModelUpdateRequest
+from ..models.model_instance_update_request import ModelInstanceUpdateRequest
+from ..models.upload_file import UploadFile
 import requests
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from ..rest import ApiException
 import six
 from slugify import slugify
 from tqdm import tqdm
+import bleach
 
 try:
     unicode  # Python 2
 except NameError:
     unicode = str  # Python 3
 
 
 class KaggleApi(KaggleApi):
-    __version__ = '1.5.9'
+    __version__ = '1.6.0a0'
 
     CONFIG_NAME_PROXY = 'proxy'
     CONFIG_NAME_COMPETITION = 'competition'
     CONFIG_NAME_PATH = 'path'
     CONFIG_NAME_USER = 'username'
     CONFIG_NAME_KEY = 'key'
     CONFIG_NAME_SSL_CA_CERT = 'ssl_ca_cert'
 
     HEADER_API_VERSION = 'X-Kaggle-ApiVersion'
     DATASET_METADATA_FILE = 'dataset-metadata.json'
     OLD_DATASET_METADATA_FILE = 'datapackage.json'
     KERNEL_METADATA_FILE = 'kernel-metadata.json'
+    MODEL_METADATA_FILE = 'model-metadata.json'
+    MODEL_INSTANCE_METADATA_FILE = 'model-instance-metadata.json'
+    MODEL_INSTANCE_VERSION_METADATA_FILE = 'model-instance-version-metadata.json'
 
     config_dir = os.environ.get('KAGGLE_CONFIG_DIR') or os.path.join(
         expanduser('~'), '.kaggle')
     if not os.path.exists(config_dir):
         os.makedirs(config_dir)
 
     config_file = 'kaggle.json'
@@ -114,15 +127,15 @@
     valid_list_kernel_types = ['all', 'script', 'notebook']
     valid_list_output_types = ['all', 'visualization', 'data']
     valid_list_sort_by = [
         'hotness', 'commentCount', 'dateCreated', 'dateRun', 'relevance',
         'scoreAscending', 'scoreDescending', 'viewCount', 'voteCount'
     ]
 
-    # Competitoins valid types
+    # Competitions valid types
     valid_competition_groups = ['general', 'entered', 'inClass']
     valid_competition_categories = [
         'all', 'featured', 'research', 'recruitment', 'gettingStarted',
         'masters', 'playground'
     ]
     valid_competition_sort_by = [
         'grouped', 'prize', 'earliestDeadline', 'latestDeadline',
@@ -132,14 +145,19 @@
     # Datasets valid types
     valid_dataset_file_types = ['all', 'csv', 'sqlite', 'json', 'bigQuery']
     valid_dataset_license_names = ['all', 'cc', 'gpl', 'odb', 'other']
     valid_dataset_sort_bys = [
         'hottest', 'votes', 'updated', 'active', 'published'
     ]
 
+    # Models valid types
+    valid_model_sort_bys = [
+        'hotness', 'downloadCount', 'voteCount', 'notebookCount', 'createTime'
+    ]
+
     # Hack for https://github.com/Kaggle/kaggle-api/issues/22 / b/78194015
     if six.PY2:
         reload(sys)
         sys.setdefaultencoding('latin1')
 
     ## Authentication
 
@@ -930,15 +948,15 @@
                          search=None,
                          user=None,
                          mine=False,
                          page=1,
                          csv_display=False,
                          max_size=None,
                          min_size=None):
-        """ a wrapper to datasets_list for the client. Additional parameters
+        """ a wrapper to dataset_list for the client. Additional parameters
             are described here, see dataset_list for others.
 
             Parameters
             ==========
             sort_by: how to sort the result, see valid_dataset_sort_bys for options
             size: DEPRECATED
             file_type: the format, see valid_dataset_file_types for string options
@@ -1272,15 +1290,14 @@
                      should be in format [owner]/[dataset-name]
             dataset_opt: an alternative option to providing a dataset
             file_name: the dataset configuration file
             path: the path to download the dataset to
             force: force the download if the file already exists (default False)
             quiet: suppress verbose output (default is False)
             unzip: if True, unzip files upon download (default is False)
-            path: the path to download the dataset to
         """
         dataset = dataset or dataset_opt
         if file_name is None:
             self.dataset_download_files(dataset,
                                         path=path,
                                         unzip=unzip,
                                         force=force,
@@ -1288,29 +1305,41 @@
         else:
             self.dataset_download_file(dataset,
                                        file_name,
                                        path=path,
                                        force=force,
                                        quiet=quiet)
 
-    def dataset_upload_file(self, path, quiet):
-        """ upload a dataset file
+    def upload_file(self, path, quiet, entity='dataset'):
+        """ upload a file
 
             Parameters
             ==========
             path: the complete path to upload
             quiet: suppress verbose output (default is False)
+            dataset: whether is a dataset file, otherwise it's a model file
+            entity: dataset or model
         """
         file_name = os.path.basename(path)
         content_length = os.path.getsize(path)
         last_modified_date_utc = int(os.path.getmtime(path))
-        result = FileUploadInfo(
-            self.process_response(
-                self.datasets_upload_file_with_http_info(
-                    file_name, content_length, last_modified_date_utc)))
+        result = None
+
+        if entity == 'dataset':
+            result = FileUploadInfo(
+                self.process_response(
+                    self.datasets_upload_file_with_http_info(
+                        file_name, content_length, last_modified_date_utc)))
+        elif entity == 'model':
+            result = FileUploadInfo(
+                self.process_response(
+                    self.models_upload_file_with_http_info(
+                        file_name, content_length, last_modified_date_utc)))
+        else:
+            raise ValueError('Invalid entity to upload: ' + entity)
 
         success = self.upload_complete(path, result.createUrl, quiet)
 
         if success:
             return result.token
         return None
 
@@ -1360,15 +1389,16 @@
             version_notes=version_notes,
             subtitle=subtitle,
             description=description,
             files=[],
             convert_to_csv=convert_to_csv,
             category_ids=keywords,
             delete_old_versions=delete_old_versions)
-        self.upload_files(request, resources, folder, quiet, dir_mode)
+        self.upload_files(request, resources, folder, 'dataset', quiet,
+                          dir_mode)
 
         if id_no:
             result = DatasetNewVersionResponse(
                 self.process_response(
                     self.datasets_create_version_by_id_with_http_info(
                         id_no, request)))
         else:
@@ -1463,15 +1493,15 @@
                            quiet=False,
                            convert_to_csv=True,
                            dir_mode='skip'):
         """ create a new dataset, meaning the same as creating a version but
             with extra metadata like license and user/owner.
              Parameters
             ==========
-            folder: the folder to initialize the metadata file in
+            folder: the folder to get the metadata file from
             public: should the dataset be public?
             quiet: suppress verbose output (default is False)
             convert_to_csv: if True, convert data to comma separated value
             dir_mode: What to do with directories: "skip" - ignore; "zip" - compress and upload
         """
         if not os.path.isdir(folder):
             raise ValueError('Invalid folder: ' + folder)
@@ -1524,16 +1554,16 @@
                                     license_name=license_name,
                                     subtitle=subtitle,
                                     description=description,
                                     files=[],
                                     is_private=not public,
                                     convert_to_csv=convert_to_csv,
                                     category_ids=keywords)
-        resources = meta_data.get('resources')
-        self.upload_files(request, resources, folder, quiet, dir_mode)
+        self.upload_files(request, resources, folder, 'dataset', quiet,
+                          dir_mode)
         result = DatasetNewResponse(
             self.process_response(
                 self.datasets_create_new_with_http_info(request)))
 
         return result
 
     def dataset_create_new_cli(self,
@@ -1541,15 +1571,15 @@
                                public=False,
                                quiet=False,
                                convert_to_csv=True,
                                dir_mode='skip'):
         """ client wrapper for creating a new dataset
              Parameters
             ==========
-            folder: the folder to initialize the metadata file in
+            folder: the folder to get the metadata file from
             public: should the dataset be public?
             quiet: suppress verbose output (default is False)
             convert_to_csv: if True, convert data to comma separated value
             dir_mode: What to do with directories: "skip" - ignore; "zip" - compress and upload
         """
         folder = folder or os.getcwd()
         result = self.dataset_create_new(folder, public, quiet, convert_to_csv,
@@ -1759,14 +1789,15 @@
             'enable_gpu':
             'false',
             'enable_internet':
             'true',
             'dataset_sources': [],
             'competition_sources': [],
             'kernel_sources': [],
+            'model_sources': [],
         }
         meta_file = os.path.join(folder, self.KERNEL_METADATA_FILE)
         with open(meta_file, 'w') as f:
             json.dump(meta_data, f, indent=2)
 
         return meta_file
 
@@ -1852,14 +1883,18 @@
         for source in dataset_sources:
             self.validate_dataset_string(source)
 
         kernel_sources = self.get_or_default(meta_data, 'kernel_sources', [])
         for source in kernel_sources:
             self.validate_kernel_string(source)
 
+        model_sources = self.get_or_default(meta_data, 'model_sources', [])
+        for source in model_sources:
+            self.validate_model_string(source)
+
         docker_pinning_type = self.get_or_default(meta_data,
                                                   'docker_image_pinning_type',
                                                   None)
         if (docker_pinning_type is not None
                 and docker_pinning_type not in self.valid_push_pinning_types):
             raise ValueError(
                 'If specified, the docker_image_pinning_type must be '
@@ -1887,14 +1922,15 @@
             enable_gpu=self.get_or_default(meta_data, 'enable_gpu', None),
             enable_internet=self.get_or_default(meta_data, 'enable_internet',
                                                 None),
             dataset_data_sources=dataset_sources,
             competition_data_sources=self.get_or_default(
                 meta_data, 'competition_sources', []),
             kernel_data_sources=kernel_sources,
+            model_data_sources=model_sources,
             category_ids=self.get_or_default(meta_data, 'keywords', []),
             docker_image_pinning_type=docker_pinning_type)
 
         result = KernelPushResponse(
             self.process_response(
                 self.kernel_push_with_http_info(
                     kernel_push_request=kernel_push_request)))
@@ -2037,15 +2073,15 @@
                     'correct language')
                 file_name = 'script.py'
             script_path = os.path.join(effective_path, file_name)
         else:
             script_path = effective_path
             file_name = os.path.basename(effective_path)
 
-        with open(script_path, 'w') as f:
+        with open(script_path, 'w', encoding="utf-8") as f:
             f.write(blob['source'])
 
         if metadata:
             data = {}
 
             server_metadata = response['metadata']
             data['id'] = server_metadata['ref']
@@ -2064,14 +2100,16 @@
                                 'keywords')
             self.set_if_present(server_metadata, 'datasetDataSources', data,
                                 'dataset_sources')
             self.set_if_present(server_metadata, 'kernelDataSources', data,
                                 'kernel_sources')
             self.set_if_present(server_metadata, 'competitionDataSources',
                                 data, 'competition_sources')
+            self.set_if_present(server_metadata, 'modelDataSources', data,
+                                'model_sources')
             with open(metadata_path, 'w') as f:
                 json.dump(data, f, indent=2)
 
             return effective_dir
         else:
             return script_path
 
@@ -2197,14 +2235,858 @@
         message = response['failureMessage']
         if message:
             print('%s has status "%s"' % (kernel, status))
             print('Failure message: "%s"' % message)
         else:
             print('%s has status "%s"' % (kernel, status))
 
+    def model_get(self, model):
+        """ call to get a model from the API
+             Parameters
+            ==========
+            model: the string identified of the model
+                     should be in format [owner]/[model-name]
+        """
+        if model is None:
+            raise ValueError('A model must be specified')
+        if '/' in model:
+            self.validate_model_string(model)
+            model_urls = model.split('/')
+            owner_slug = model_urls[0]
+            model_slug = model_urls[1]
+        else:
+            owner_slug = self.get_config_value(self.CONFIG_NAME_USER)
+            model_slug = model
+
+        model_get_result = self.process_response(
+            self.get_model_with_http_info(owner_slug, model_slug))
+        return model_get_result
+
+    def model_get_cli(self, model, folder=None, model_opt=None):
+        """ wrapper for client for model_get, with additional
+            model_opt to get a model from the API
+             Parameters
+            ==========
+            folder: the folder to download the model metadata file
+            model_opt: an alternative to model
+        """
+        m = model or model_opt
+        model = self.model_get(m)
+        if folder is None:
+            self.print_obj(model)
+        else:
+            meta_file = os.path.join(folder, self.MODEL_METADATA_FILE)
+
+            data = {}
+            data['id'] = model['id']
+            model_ref_split = model['ref'].split('/')
+            data['ownerSlug'] = model_ref_split[0]
+            data['slug'] = model_ref_split[1]
+            data['title'] = model['title']
+            data['subtitle'] = model['subtitle']
+            data['isPrivate'] = model['isPrivate']
+            data['description'] = model['description']
+            data['publishTime'] = model['publishTime']
+
+            with open(meta_file, 'w') as f:
+                json.dump(data, f, indent=2)
+            print('Metadata file written to {}'.format(meta_file))
+
+    def model_list(self,
+                   sort_by=None,
+                   search=None,
+                   owner=None,
+                   page_size=20,
+                   page_token=None):
+        """ return a list of models!
+
+            Parameters
+            ==========
+            sort_by: how to sort the result, see valid_model_sort_bys for options
+            search: a search term to use (default is empty string)
+            owner: username or organization slug to filter the search to
+            page_size: the page size to return (default is 20)
+            page_token: the page token for pagination
+        """
+        if sort_by and sort_by not in self.valid_model_sort_bys:
+            raise ValueError('Invalid sort by specified. Valid options are ' +
+                             str(self.valid_model_sort_bys))
+
+        if int(page_size) <= 0:
+            raise ValueError('Page size must be >= 1')
+
+        models_list_result = self.process_response(
+            self.models_list_with_http_info(sort_by=sort_by or 'hotness',
+                                            search=search or '',
+                                            owner=owner or '',
+                                            page_size=page_size,
+                                            page_token=page_token))
+
+        next_page_token = models_list_result['nextPageToken']
+        if next_page_token != '':
+            print('Next Page Token = {}'.format(next_page_token))
+
+        return [Model(m) for m in models_list_result['models']]
+
+    def model_list_cli(self,
+                       sort_by=None,
+                       search=None,
+                       owner=None,
+                       page_size=20,
+                       page_token=None,
+                       csv_display=False):
+        """ a wrapper to model_list for the client. Additional parameters
+            are described here, see model_list for others.
+
+            Parameters
+            ==========
+            sort_by: how to sort the result, see valid_model_sort_bys for options
+            search: a search term to use (default is empty string)
+            owner: username or organization slug to filter the search to
+            page_size: the page size to return (default is 20)
+            page_token: the page token for pagination
+            csv_display: if True, print comma separated values instead of table
+        """
+        models = self.model_list(sort_by, search, owner, page_size, page_token)
+        fields = ['id', 'ref', 'title', 'subtitle', 'author']
+        if models:
+            if csv_display:
+                self.print_csv(models, fields)
+            else:
+                self.print_table(models, fields)
+        else:
+            print('No models found')
+
+    def model_initialize(self, folder):
+        """ initialize a folder with a model configuration (metadata) file
+            Parameters
+            ==========
+            folder: the folder to initialize the metadata file in
+        """
+        if not os.path.isdir(folder):
+            raise ValueError('Invalid folder: ' + folder)
+
+        meta_data = {
+            'ownerSlug': 'INSERT_OWNER_SLUG_HERE',
+            'title': 'INSERT_TITLE_HERE',
+            'slug': 'INSERT_SLUG_HERE',
+            'subtitle': '',
+            'isPrivate': True,
+            'description': '''# Model Summary
+
+# Model Characteristics
+
+# Data Overview
+
+# Evaluation Results
+''',
+            'publishTime': '',
+            'provenanceSources': ''
+        }
+        meta_file = os.path.join(folder, self.MODEL_METADATA_FILE)
+        with open(meta_file, 'w') as f:
+            json.dump(meta_data, f, indent=2)
+
+        print('Model template written to: ' + meta_file)
+        return meta_file
+
+    def model_initialize_cli(self, folder=None):
+        folder = folder or os.getcwd()
+        self.model_initialize(folder)
+
+    def model_create_new(self, folder):
+        """ create a new model.
+             Parameters
+            ==========
+            folder: the folder to get the metadata file from
+        """
+        if not os.path.isdir(folder):
+            raise ValueError('Invalid folder: ' + folder)
+
+        meta_file = self.get_model_metadata_file(folder)
+
+        # read json
+        with open(meta_file) as f:
+            meta_data = json.load(f)
+        owner_slug = self.get_or_fail(meta_data, 'ownerSlug')
+        slug = self.get_or_fail(meta_data, 'slug')
+        title = self.get_or_fail(meta_data, 'title')
+        subtitle = meta_data.get('subtitle')
+        is_private = self.get_or_fail(meta_data, 'isPrivate')
+        description = self.sanitize_markdown(
+            self.get_or_fail(meta_data, 'description'))
+        publish_time = meta_data.get('publishTime')
+        provenance_sources = meta_data.get('provenanceSources')
+
+        # validations
+        if owner_slug == 'INSERT_OWNER_SLUG_HERE':
+            raise ValueError(
+                'Default ownerSlug detected, please change values before uploading'
+            )
+        if title == 'INSERT_TITLE_HERE':
+            raise ValueError(
+                'Default title detected, please change values before uploading'
+            )
+        if slug == 'INSERT_SLUG_HERE':
+            raise ValueError(
+                'Default slug detected, please change values before uploading')
+        if not isinstance(is_private, bool):
+            raise ValueError('model.isPrivate must be a boolean')
+
+        request = ModelNewRequest(owner_slug=owner_slug,
+                                  slug=slug,
+                                  title=title,
+                                  subtitle=subtitle,
+                                  is_private=is_private,
+                                  description=description,
+                                  publish_time=publish_time,
+                                  provenance_sources=provenance_sources)
+        result = ModelNewResponse(
+            self.process_response(
+                self.models_create_new_with_http_info(request)))
+
+        return result
+
+    def model_create_new_cli(self, folder=None):
+        """ client wrapper for creating a new model
+             Parameters
+            ==========
+            folder: the folder to get the metadata file from
+        """
+        folder = folder or os.getcwd()
+        result = self.model_create_new(folder)
+
+        if result.hasId:
+            print('Your model was created. Id={}. Url={}'.format(
+                result.id, result.url))
+        else:
+            print('Model creation error: ' + result.error)
+
+    def model_delete(self, model):
+        """ call to delete a model from the API
+             Parameters
+            ==========
+            model: the string identified of the model
+                     should be in format [owner]/[model-name]
+        """
+        if model is None:
+            raise ValueError('A model must be specified')
+        if '/' in model:
+            self.validate_model_string(model)
+            model_urls = model.split('/')
+            owner_slug = model_urls[0]
+            model_slug = model_urls[1]
+        else:
+            owner_slug = self.get_config_value(self.CONFIG_NAME_USER)
+            model_slug = model
+
+        res = ModelDeleteResponse(
+            self.process_response(
+                self.delete_model_with_http_info(owner_slug, model_slug)))
+        return res
+
+    def model_delete_cli(self, model, model_opt=None):
+        """ wrapper for client for model_delete, with additional
+            model_opt to get a model from the API
+             Parameters
+            ==========
+            model_opt: an alternative to model
+        """
+        m = model or model_opt
+        result = self.model_delete(m)
+
+        if result.hasError:
+            print('Model deletion error: ' + result.error)
+        else:
+            print('The model was deleted.')
+
+    def model_update(self, folder):
+        """ update a model.
+             Parameters
+            ==========
+            folder: the folder to get the metadata file from
+        """
+        if not os.path.isdir(folder):
+            raise ValueError('Invalid folder: ' + folder)
+
+        meta_file = self.get_model_metadata_file(folder)
+
+        # read json
+        with open(meta_file) as f:
+            meta_data = json.load(f)
+        owner_slug = self.get_or_fail(meta_data, 'ownerSlug')
+        slug = self.get_or_fail(meta_data, 'slug')
+        title = self.get_or_default(meta_data, 'title', None)
+        subtitle = self.get_or_default(meta_data, 'subtitle', None)
+        is_private = self.get_or_default(meta_data, 'isPrivate', None)
+        description = self.get_or_default(meta_data, 'description', None)
+        publish_time = self.get_or_default(meta_data, 'publishTime', None)
+        provenance_sources = self.get_or_default(meta_data,
+                                                 'provenanceSources', None)
+
+        # validations
+        if owner_slug == 'INSERT_OWNER_SLUG_HERE':
+            raise ValueError(
+                'Default ownerSlug detected, please change values before uploading'
+            )
+        if slug == 'INSERT_SLUG_HERE':
+            raise ValueError(
+                'Default slug detected, please change values before uploading')
+        if is_private != None and not isinstance(is_private, bool):
+            raise ValueError('model.isPrivate must be a boolean')
+
+        # mask
+        update_mask = {'paths': []}
+        if title != None:
+            update_mask['paths'].append('title')
+        if subtitle != None:
+            update_mask['paths'].append('subtitle')
+        if is_private != None:
+            update_mask['paths'].append('is_private')
+        else:
+            is_private = True  # default value, not updated
+        if description != None:
+            description = self.sanitize_markdown(description)
+            update_mask['paths'].append('description')
+        if publish_time != None:
+            update_mask['paths'].append('publish_time')
+        if provenance_sources != None:
+            update_mask['paths'].append('provenance_sources')
+
+        request = ModelUpdateRequest(title=title,
+                                     subtitle=subtitle,
+                                     is_private=is_private,
+                                     description=description,
+                                     publish_time=publish_time,
+                                     provenance_sources=provenance_sources,
+                                     update_mask=update_mask)
+        result = ModelNewResponse(
+            self.process_response(
+                self.update_model_with_http_info(owner_slug, slug, request)))
+
+        return result
+
+    def model_update_cli(self, folder=None):
+        """ client wrapper for updating a model
+             Parameters
+            ==========
+            folder: the folder to get the metadata file from
+        """
+        folder = folder or os.getcwd()
+        result = self.model_update(folder)
+
+        if result.hasId:
+            print('Your model was updated. Id={}. Url={}'.format(
+                result.id, result.url))
+        else:
+            print('Model update error: ' + result.error)
+
+    def model_instance_initialize(self, folder):
+        """ initialize a folder with a model instance configuration (metadata) file
+             Parameters
+            ==========
+            folder: the folder to initialize the metadata file in
+        """
+        if not os.path.isdir(folder):
+            raise ValueError('Invalid folder: ' + folder)
+
+        meta_data = {
+            'ownerSlug': 'INSERT_OWNER_SLUG_HERE',
+            'modelSlug': 'INSERT_EXISTING_MODEL_SLUG_HERE',
+            'instanceSlug': 'INSERT_INSTANCE_SLUG_HERE',
+            'framework': 'INSERT_FRAMEWORK_HERE',
+            'overview': '',
+            'usage': '''# Model Format
+
+# Training Data
+
+# Model Inputs
+
+# Model Outputs
+
+# Model Usage
+
+# Fine-tuning
+
+# Changelog
+''',
+            'licenseName': 'Apache 2.0',
+            'fineTunable': False,
+            'trainingData': []
+        }
+        meta_file = os.path.join(folder, self.MODEL_INSTANCE_METADATA_FILE)
+        with open(meta_file, 'w') as f:
+            json.dump(meta_data, f, indent=2)
+
+        print('Model Instance template written to: ' + meta_file)
+        return meta_file
+
+    def model_instance_initialize_cli(self, folder):
+        folder = folder or os.getcwd()
+        self.model_instance_initialize(folder)
+
+    def model_instance_create(self, folder, quiet=False, dir_mode='skip'):
+        """ create a new model instance.
+             Parameters
+            ==========
+            folder: the folder to get the metadata file from
+            quiet: suppress verbose output (default is False)
+            dir_mode: what to do with directories: "skip" - ignore; "zip" - compress and upload
+        """
+        if not os.path.isdir(folder):
+            raise ValueError('Invalid folder: ' + folder)
+
+        meta_file = self.get_model_instance_metadata_file(folder)
+
+        # read json
+        with open(meta_file) as f:
+            meta_data = json.load(f)
+        owner_slug = self.get_or_fail(meta_data, 'ownerSlug')
+        model_slug = self.get_or_fail(meta_data, 'modelSlug')
+        instance_slug = self.get_or_fail(meta_data, 'instanceSlug')
+        framework = self.get_or_fail(meta_data, 'framework')
+        overview = self.sanitize_markdown(
+            self.get_or_default(meta_data, 'overview', ''))
+        usage = self.sanitize_markdown(
+            self.get_or_default(meta_data, 'usage', ''))
+        license_name = self.get_or_fail(meta_data, 'licenseName')
+        fine_tunable = self.get_or_default(meta_data, 'fineTunable', False)
+        training_data = self.get_or_default(meta_data, 'trainingData', [])
+
+        # validations
+        if owner_slug == 'INSERT_OWNER_SLUG_HERE':
+            raise ValueError(
+                'Default ownerSlug detected, please change values before uploading'
+            )
+        if model_slug == 'INSERT_EXISTING_MODEL_SLUG_HERE':
+            raise ValueError(
+                'Default modelSlug detected, please change values before uploading'
+            )
+        if instance_slug == 'INSERT_INSTANCE_SLUG_HERE':
+            raise ValueError(
+                'Default instanceSlug detected, please change values before uploading'
+            )
+        if framework == 'INSERT_FRAMEWORK_HERE':
+            raise ValueError(
+                'Default framework detected, please change values before uploading'
+            )
+        if license_name == '':
+            raise ValueError('Please specify a license')
+        if not isinstance(fine_tunable, bool):
+            raise ValueError('modelInstance.fineTunable must be a boolean')
+        if not isinstance(training_data, list):
+            raise ValueError('modelInstance.trainingData must be a list')
+
+        request = ModelNewInstanceRequest(instance_slug=instance_slug,
+                                          framework=framework,
+                                          overview=overview,
+                                          usage=usage,
+                                          license_name=license_name,
+                                          fine_tunable=fine_tunable,
+                                          training_data=training_data,
+                                          files=[])
+        resources = meta_data.get('resources')
+        self.upload_files(request, resources, folder, 'model', quiet, dir_mode)
+        result = ModelNewResponse(
+            self.process_response(
+                self.models_create_instance_with_http_info(
+                    owner_slug, model_slug, request)))
+
+        return result
+
+    def model_instance_create_cli(self, folder, quiet=False, dir_mode='skip'):
+        """ client wrapper for creating a new model instance
+             Parameters
+            ==========
+            folder: the folder to get the metadata file from
+            quiet: suppress verbose output (default is False)
+            dir_mode: what to do with directories: "skip" - ignore; "zip" - compress and upload
+        """
+        folder = folder or os.getcwd()
+        result = self.model_instance_create(folder, quiet, dir_mode)
+
+        if result.hasId:
+            print('Your model instance was created. Id={}. Url={}'.format(
+                result.id, result.url))
+        else:
+            print('Model instance creation error: ' + result.error)
+
+    def model_instance_delete(self, model_instance):
+        """ call to delete a model instance from the API
+             Parameters
+            ==========
+            model_instance: the string identified of the model instance
+                     should be in format [owner]/[model-name]/[framework]/[instance-slug]
+        """
+        if model_instance is None:
+            raise ValueError('A model instance must be specified')
+
+        self.validate_model_instance_string(model_instance)
+        urls = model_instance.split('/')
+        owner_slug = urls[0]
+        model_slug = urls[1]
+        framework = urls[2]
+        instance_slug = urls[3]
+
+        res = ModelDeleteResponse(
+            self.process_response(
+                self.delete_model_instance_with_http_info(
+                    owner_slug, model_slug, framework, instance_slug)))
+        return res
+
+    def model_instance_delete_cli(self,
+                                  model_instance,
+                                  model_instance_opt=None):
+        """ wrapper for client for model_instance_delete, with additional
+            model_instance_opt to get a model instance from the API
+             Parameters
+            ==========
+            model_instance_opt: an alternative to model instance
+        """
+        mi = model_instance or model_instance_opt
+        result = self.model_instance_delete(mi)
+
+        if result.hasError:
+            print('Model instance deletion error: ' + result.error)
+        else:
+            print('The model instance was deleted.')
+
+    def model_instance_update(self, folder):
+        """ update a model instance.
+             Parameters
+            ==========
+            folder: the folder to get the metadata file from
+        """
+        if not os.path.isdir(folder):
+            raise ValueError('Invalid folder: ' + folder)
+
+        meta_file = self.get_model_instance_metadata_file(folder)
+
+        # read json
+        with open(meta_file) as f:
+            meta_data = json.load(f)
+        owner_slug = self.get_or_fail(meta_data, 'ownerSlug')
+        model_slug = self.get_or_fail(meta_data, 'modelSlug')
+        framework = self.get_or_fail(meta_data, 'framework')
+        instance_slug = self.get_or_fail(meta_data, 'instanceSlug')
+        overview = self.get_or_default(meta_data, 'overview', None)
+        usage = self.get_or_default(meta_data, 'usage', None)
+        license_name = self.get_or_default(meta_data, 'licenseName', None)
+        fine_tunable = self.get_or_default(meta_data, 'fineTunable', None)
+        training_data = self.get_or_default(meta_data, 'trainingData', None)
+
+        # validations
+        if owner_slug == 'INSERT_OWNER_SLUG_HERE':
+            raise ValueError(
+                'Default ownerSlug detected, please change values before uploading'
+            )
+        if model_slug == 'INSERT_SLUG_HERE':
+            raise ValueError(
+                'Default model slug detected, please change values before uploading'
+            )
+        if instance_slug == 'INSERT_INSTANCE_SLUG_HERE':
+            raise ValueError(
+                'Default instance slug detected, please change values before uploading'
+            )
+        if framework == 'INSERT_FRAMEWORK_HERE':
+            raise ValueError(
+                'Default framework detected, please change values before uploading'
+            )
+        if fine_tunable != None and not isinstance(fine_tunable, bool):
+            raise ValueError('modelInstance.fineTunable must be a boolean')
+        if training_data != None and not isinstance(training_data, list):
+            raise ValueError('modelInstance.trainingData must be a list')
+
+        # mask
+        update_mask = {'paths': []}
+        if overview != None:
+            overview = self.sanitize_markdown(overview)
+            update_mask['paths'].append('overview')
+        if usage != None:
+            usage = self.sanitize_markdown(usage)
+            update_mask['paths'].append('usage')
+        if license_name != None:
+            update_mask['paths'].append('license_name')
+        else:
+            license_name = "Apache 2.0"  # default value even if not updated
+        if fine_tunable != None:
+            update_mask['paths'].append('fine_tunable')
+        if training_data != None:
+            update_mask['paths'].append('training_data')
+
+        request = ModelInstanceUpdateRequest(overview=overview,
+                                             usage=usage,
+                                             license_name=license_name,
+                                             fine_tunable=fine_tunable,
+                                             training_data=training_data,
+                                             update_mask=update_mask)
+        result = ModelNewResponse(
+            self.process_response(
+                self.update_model_instance_with_http_info(
+                    owner_slug, model_slug, framework, instance_slug,
+                    request)))
+
+        return result
+
+    def model_instance_update_cli(self, folder=None):
+        """ client wrapper for updating a model instance
+             Parameters
+            ==========
+            folder: the folder to get the metadata file from
+        """
+        folder = folder or os.getcwd()
+        result = self.model_instance_update(folder)
+
+        if result.hasId:
+            print('Your model instance was updated. Id={}. Url={}'.format(
+                result.id, result.url))
+        else:
+            print('Model update error: ' + result.error)
+
+    def model_instance_version_initialize(self, folder):
+        """ initialize a folder with a a model instance version configuration (metadata) file
+            Parameters
+            ==========
+            folder: the folder to initialize the metadata file in
+        """
+        if not os.path.isdir(folder):
+            raise ValueError('Invalid folder: ' + folder)
+
+        meta_data = {
+            'ownerSlug': 'INSERT_OWNER_SLUG_HERE',
+            'modelSlug': 'INSERT_EXISTING_MODEL_SLUG_HERE',
+            'instanceSlug': 'INSERT_EXISTING_INSTANCE_SLUG_HERE',
+            'framework': 'INSERT_EXISTING_FRAMEWORK_SLUG_HERE',
+            'versionNotes': '',
+        }
+        meta_file = os.path.join(folder,
+                                 self.MODEL_INSTANCE_VERSION_METADATA_FILE)
+        with open(meta_file, 'w') as f:
+            json.dump(meta_data, f, indent=2)
+
+        print('Model Instance Version template written to: ' + meta_file)
+        return meta_file
+
+    def model_instance_version_initialize_cli(self, folder):
+        folder = folder or os.getcwd()
+        self.model_instance_version_initialize(folder)
+
+    def model_instance_version_create(self,
+                                      folder,
+                                      quiet=False,
+                                      dir_mode='skip'):
+        """ create a new model instance version.
+             Parameters
+            ==========
+            folder: the folder to get the metadata file from
+            quiet: suppress verbose output (default is False)
+            dir_mode: what to do with directories: "skip" - ignore; "zip" - compress and upload
+        """
+        if not os.path.isdir(folder):
+            raise ValueError('Invalid folder: ' + folder)
+
+        meta_file = self.get_model_instance_version_metadata_file(folder)
+
+        # read json
+        with open(meta_file) as f:
+            meta_data = json.load(f)
+        owner_slug = self.get_or_fail(meta_data, 'ownerSlug')
+        model_slug = self.get_or_fail(meta_data, 'modelSlug')
+        instance_slug = self.get_or_fail(meta_data, 'instanceSlug')
+        framework = self.get_or_fail(meta_data, 'framework')
+        version_notes = self.get_or_fail(meta_data, 'versionNotes')
+
+        # validations
+        if owner_slug == 'INSERT_OWNER_SLUG_HERE':
+            raise ValueError(
+                'Default ownerSlug detected, please change values before uploading'
+            )
+        if model_slug == 'INSERT_EXISTING_MODEL_SLUG_HERE':
+            raise ValueError(
+                'Default modelSlug detected, please change values before uploading'
+            )
+        if instance_slug == 'INSERT_EXISTING_INSTANCE_SLUG_HERE':
+            raise ValueError(
+                'Default instanceSlug detected, please change values before uploading'
+            )
+        if framework == 'INSERT_EXISTING_FRAMEWORK_SLUG_HERE':
+            raise ValueError(
+                'Default framework detected, please change values before uploading'
+            )
+
+        request = ModelInstanceNewVersionRequest(version_notes=version_notes,
+                                                 files=[])
+        resources = meta_data.get('resources')
+        self.upload_files(request, resources, folder, 'model', quiet, dir_mode)
+        result = ModelNewResponse(
+            self.process_response(
+                self.models_create_instance_version_with_http_info(
+                    owner_slug, model_slug, framework, instance_slug,
+                    request)))
+
+        return result
+
+    def model_instance_version_create_cli(self,
+                                          folder,
+                                          quiet=False,
+                                          dir_mode='skip'):
+        """ client wrapper for creating a new model instance version
+             Parameters
+            ==========
+            folder: the folder to get the metadata file from
+            quiet: suppress verbose output (default is False)
+            dir_mode: what to do with directories: "skip" - ignore; "zip" - compress and upload
+        """
+        folder = folder or os.getcwd()
+        result = self.model_instance_version_create(folder, quiet, dir_mode)
+
+        if result.hasId:
+            print('Your model instance version was created. Url={}'.format(
+                result.url))
+        else:
+            print('Model instance version creation error: ' + result.error)
+
+    def model_instance_version_download(self,
+                                        model_instance_version,
+                                        path=None,
+                                        force=False,
+                                        quiet=True,
+                                        untar=False):
+        """ download all files for a model instance version
+
+            Parameters
+            ==========
+            model_instance_version: the string identified of the model instance version
+                    should be in format [owner]/[model-name]/[framework]/[instance-slug]/[version-number]
+            path: the path to download the model instance version to
+            force: force the download if the file already exists (default False)
+            quiet: suppress verbose output (default is True)
+            untar: if True, untar files upon download (default is False)
+        """
+        if model_instance_version is None:
+            raise ValueError('A model_instance_version must be specified')
+
+        self.validate_model_instance_version_string(model_instance_version)
+        urls = model_instance_version.split('/')
+        owner_slug = urls[0]
+        model_slug = urls[1]
+        framework = urls[2]
+        instance_slug = urls[3]
+        version_number = urls[4]
+
+        if path is None:
+            effective_path = self.get_default_download_dir(
+                'models', owner_slug, model_slug, framework, instance_slug,
+                version_number)
+        else:
+            effective_path = path
+
+        response = self.process_response(
+            self.model_instance_versions_download_with_http_info(
+                owner_slug=owner_slug,
+                model_slug=model_slug,
+                framework=framework,
+                instance_slug=instance_slug,
+                version_number=version_number,
+                _preload_content=False))
+
+        outfile = os.path.join(effective_path, model_slug + '.tar.gz')
+        if force or self.download_needed(response, outfile, quiet):
+            self.download_file(response, outfile, quiet)
+            downloaded = True
+        else:
+            downloaded = False
+
+        if downloaded:
+            if untar:
+                try:
+                    with tarfile.open(outfile, mode='r:gz') as t:
+                        t.extractall(effective_path)
+                except Exception as e:
+                    raise ValueError(
+                        'Error extracting the tar.gz file, please report on '
+                        'www.github.com/kaggle/kaggle-api', e)
+
+                try:
+                    os.remove(outfile)
+                except OSError as e:
+                    print('Could not delete tar file, got %s' % e)
+
+    def model_instance_version_download_cli(self,
+                                            model_instance_version,
+                                            model_instance_version_opt=None,
+                                            path=None,
+                                            untar=False,
+                                            force=False,
+                                            quiet=False):
+        """ client wrapper for model_instance_version_download.
+
+            Parameters
+            ==========
+            model_instance_version: the string identified of the model instance version
+                    should be in format [owner]/[model-name]/[framework]/[instance-slug]/[version-number]
+            model_instance_version_opt: an alternative option to providing a model instance version
+            path: the path to download the model instance version to
+            force: force the download if the file already exists (default False)
+            quiet: suppress verbose output (default is False)
+            untar: if True, untar files upon download (default is False)
+        """
+        miv = model_instance_version or model_instance_version_opt
+        self.model_instance_version_download(model_instance_version,
+                                             path=path,
+                                             untar=untar,
+                                             force=force,
+                                             quiet=quiet)
+
+    def model_instance_version_delete(self, model_instance_version):
+        """ call to delete a model instance version from the API
+             Parameters
+            ==========
+            model_instance_version: the string identified of the model instance version
+                     should be in format [owner]/[model-name]/[framework]/[instance-slug]/[version-number]
+        """
+        if model_instance_version is None:
+            raise ValueError('A model instance version must be specified')
+
+        self.validate_model_instance_version_string(model_instance_version)
+        urls = model_instance_version.split('/')
+        owner_slug = urls[0]
+        model_slug = urls[1]
+        framework = urls[2]
+        instance_slug = urls[3]
+        version_number = urls[4]
+
+        res = ModelDeleteResponse(
+            self.process_response(
+                self.delete_model_instance_version_with_http_info(
+                    owner_slug, model_slug, framework, instance_slug,
+                    version_number)))
+        return res
+
+    def model_instance_version_delete_cli(self,
+                                          model_instance_version,
+                                          model_instance_version_opt=None):
+        """ wrapper for client for model_instance_version_delete, with additional
+            model_instance_version_opt to get a model instance version from the API
+             Parameters
+            ==========
+            model_instance_version_opt: an alternative to model instance version
+        """
+        miv = model_instance_version or model_instance_version_opt
+        result = self.model_instance_version_delete(miv)
+
+        if result.hasError:
+            print('Model instance version deletion error: ' + result.error)
+        else:
+            print('The model instance version was deleted.')
+
+    def print_obj(self, obj, indent=2):
+        pretty = json.dumps(obj, indent=indent)
+        print(pretty)
+
     def download_needed(self, response, outfile, quiet=True):
         """ determine if a download is needed based on timestamp. Return True
             if needed (remote is newer) or False if local is newest.
              Parameters
             ==========
             response: the response from the API
             outfile: the output file to write to
@@ -2290,14 +3172,36 @@
         if not os.path.isfile(meta_file):
             meta_file = os.path.join(folder, self.OLD_DATASET_METADATA_FILE)
             if not os.path.isfile(meta_file):
                 raise ValueError('Metadata file not found: ' +
                                  self.DATASET_METADATA_FILE)
         return meta_file
 
+    def get_model_metadata_file(self, folder):
+        meta_file = os.path.join(folder, self.MODEL_METADATA_FILE)
+        if not os.path.isfile(meta_file):
+            raise ValueError('Metadata file not found: ' +
+                             self.MODEL_METADATA_FILE)
+        return meta_file
+
+    def get_model_instance_metadata_file(self, folder):
+        meta_file = os.path.join(folder, self.MODEL_INSTANCE_METADATA_FILE)
+        if not os.path.isfile(meta_file):
+            raise ValueError('Metadata file not found: ' +
+                             self.MODEL_INSTANCE_METADATA_FILE)
+        return meta_file
+
+    def get_model_instance_version_metadata_file(self, folder):
+        meta_file = os.path.join(folder,
+                                 self.MODEL_INSTANCE_VERSION_METADATA_FILE)
+        if not os.path.isfile(meta_file):
+            raise ValueError('Metadata file not found: ' +
+                             self.MODEL_INSTANCE_VERSION_METADATA_FILE)
+        return meta_file
+
     def process_response(self, result):
         """ process a response from the API. We check the API version against
             the client's to see if it's old, and give them a warning (once)
 
             Parameters
             ==========
             result: the result from the API
@@ -2332,50 +3236,55 @@
         # Make both lists the same length
         for i in range(client_len, server_len):
             client_split.append('0')
         for i in range(server_len, client_len):
             server_split.append('0')
 
         for i in range(0, client_len):
-            if 'b' in client_split[i]:
-                # Using a beta version, don't check
+            if 'a' in client_split[i] or 'b' in client_split[i]:
+                # Using a alpha/beta version, don't check
                 return True
             client = int(client_split[i])
             server = int(server_split[i])
             if client < server:
                 return False
             elif server < client:
                 return True
 
         return True
 
     def upload_files(self,
                      request,
                      resources,
                      folder,
+                     entity='dataset',
                      quiet=False,
                      dir_mode='skip'):
         """ upload files in a folder
              Parameters
             ==========
             request: the prepared request
             resources: the files to upload
             folder: the folder to upload from
+            entity: dataset or model
             quiet: suppress verbose output (default is False)
         """
         for file_name in os.listdir(folder):
-            if (file_name == self.DATASET_METADATA_FILE
-                    or file_name == self.OLD_DATASET_METADATA_FILE
-                    or file_name == self.KERNEL_METADATA_FILE):
+            if (file_name in [
+                    self.DATASET_METADATA_FILE, self.OLD_DATASET_METADATA_FILE,
+                    self.KERNEL_METADATA_FILE, self.MODEL_METADATA_FILE,
+                    self.MODEL_INSTANCE_METADATA_FILE,
+                    self.MODEL_INSTANCE_VERSION_METADATA_FILE
+            ]):
                 continue
             full_path = os.path.join(folder, file_name)
 
             if os.path.isfile(full_path):
                 exitcode = self._upload_file(file_name, full_path, quiet,
-                                             request, resources)
+                                             request, resources, entity)
                 if exitcode:
                     return
             elif os.path.isdir(full_path):
                 if dir_mode in ['zip', 'tar']:
                     temp_dir = tempfile.mkdtemp()
                     try:
                         _, dir_name = os.path.split(full_path)
@@ -2393,39 +3302,46 @@
                 elif not quiet:
                     print("Skipping folder: " + file_name +
                           "; use '--dir-mode' to upload folders")
             else:
                 if not quiet:
                     print('Skipping: ' + file_name)
 
-    def _upload_file(self, file_name, full_path, quiet, request, resources):
+    def _upload_file(self,
+                     file_name,
+                     full_path,
+                     quiet,
+                     request,
+                     resources,
+                     entity='dataset'):
         """ Helper function to upload a single file
             Parameters
             ==========
             file_name: name of the file to upload
             full_path: path to the file to upload
+            quiet: suppress verbose output
             request: the prepared request
             resources: optional file metadata
-            quiet: suppress verbose output
+            entity: dataset or model
             :return: True - upload unsuccessful; False - upload successful
         """
 
         if not quiet:
             print('Starting upload for file ' + file_name)
 
         content_length = os.path.getsize(full_path)
-        token = self.dataset_upload_file(full_path, quiet)
+        token = self.upload_file(full_path, quiet, entity)
         if token is None:
             if not quiet:
                 print('Upload unsuccessful: ' + file_name)
             return True
         if not quiet:
             print('Upload successful: ' + file_name + ' (' +
                   File.get_size(content_length) + ')')
-        upload_file = DatasetUploadFile()
+        upload_file = UploadFile()
         upload_file.token = token
         if resources:
             for item in resources:
                 if file_name == item.get('path'):
                     upload_file.description = item.get('description')
                     if 'schema' in item:
                         fields = self.get_or_default(item['schema'], 'fields',
@@ -2512,14 +3428,76 @@
                 raise ValueError('Dataset must be specified in the form of '
                                  '\'{username}/{dataset-slug}\'')
 
             split = dataset.split('/')
             if not split[0] or not split[1]:
                 raise ValueError('Invalid dataset specification ' + dataset)
 
+    def validate_model_string(self, model):
+        """ determine if a model string is valid, meaning it is in the format
+            of {owner}/{model-slug}.
+             Parameters
+            ==========
+            model: the model name to validate
+        """
+        if model:
+            if model.count('/') != 1:
+                raise ValueError('Model must be specified in the form of '
+                                 '\'{owner}/{model-slug}\'')
+
+            split = model.split('/')
+            if not split[0] or not split[1]:
+                raise ValueError('Invalid model specification ' + model)
+
+    def validate_model_instance_string(self, model_instance):
+        """ determine if a model instance string is valid, meaning it is in the format
+            of {owner}/{model-slug}/{framework}/{instance-slug}.
+             Parameters
+            ==========
+            model_instance: the model instance name to validate
+        """
+        if model_instance:
+            if model_instance.count('/') != 3:
+                raise ValueError(
+                    'Model instance must be specified in the form of '
+                    '\'{owner}/{model-slug}/{framework}/{instance-slug}\'')
+
+            split = model_instance.split('/')
+            if not split[0] or not split[1] or not split[2] or not split[3]:
+                raise ValueError('Invalid model instance specification ' +
+                                 model_instance)
+
+    def validate_model_instance_version_string(self, model_instance_version):
+        """ determine if a model instance version string is valid, meaning it is in the format
+            of {owner}/{model-slug}/{framework}/{instance-slug}/{version-number}.
+             Parameters
+            ==========
+            model_instance_version: the model instance version name to validate
+        """
+        if model_instance_version:
+            if model_instance_version.count('/') != 4:
+                raise ValueError(
+                    'Model instance version must be specified in the form of '
+                    '\'{owner}/{model-slug}/{framework}/{instance-slug}/{version-number}\''
+                )
+
+            split = model_instance_version.split('/')
+            if not split[0] or not split[1] or not split[2] or not split[
+                    3] or not split[4]:
+                raise ValueError(
+                    'Invalid model instance version specification ' +
+                    model_instance_version)
+
+            try:
+                version_number = int(split[4])
+            except:
+                raise ValueError(
+                    'Model instance version\'s version-number must be an integer'
+                )
+
     def validate_kernel_string(self, kernel):
         """ determine if a kernel string is valid, meaning it is in the format
             of {username}/{kernel-slug}.
              Parameters
             ==========
             kernel: the kernel name to validate
         """
@@ -2533,14 +3511,32 @@
                 raise ValueError('Kernel must be specified in the form of '
                                  '\'{username}/{kernel-slug}\'')
 
             if len(split[1]) < 5:
                 raise ValueError(
                     'Kernel slug must be at least five characters')
 
+    def validate_model_string(self, model):
+        """ determine if a model string is valid, meaning it is in the format
+            of {username}/{model-slug}/{framework}/{variation-slug}/{version-number}.
+             Parameters
+            ==========
+            model: the model name to validate
+        """
+        if model:
+            if '/' not in model:
+                raise ValueError(
+                    'Model must be specified in the form of '
+                    '\'{username}/{model-slug}/{framework}/{variation-slug}/{version-number}\''
+                )
+
+            split = model.split('/')
+            if not split[0] or not split[1]:
+                raise ValueError('Invalid model specification ' + model)
+
     def validate_resources(self, folder, resources):
         """ validate resources is a wrapper to validate the existence of files
             and that there are no duplicates for a folder and set of resources.
 
             Parameters
             ==========
             folder: the folder to validate
@@ -2603,16 +3599,23 @@
             }
             fields.append(field)
         schema['fields'] = fields
         as_metadata['schema'] = schema
 
         return as_metadata
 
+    def validate_date(self, date):
+        datetime.strptime(date, "%Y-%m-%d")
+
+    def sanitize_markdown(self, markdown):
+        return bleach.clean(markdown)
+
 
 class TqdmBufferedReader(io.BufferedReader):
+
     def __init__(self, raw, progress_bar):
         """ helper class to implement an io.BufferedReader
              Parameters
             ==========
             raw: bytes data to pass to the buffered reader
             progress_bar: a progress bar to initialize the reader
         """
```

### Comparing `kaggle-1.5.9/kaggle/api_client.py` & `kaggle-1.6.0a0/kaggle/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kaggle-1.5.9/kaggle/configuration.py` & `kaggle-1.6.0a0/kaggle/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kaggle-1.5.9/kaggle/models/__init__.py` & `kaggle-1.6.0a0/kaggle/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -32,12 +32,17 @@
 
 # import models into model package
 from kaggle.models.collaborator import Collaborator
 from kaggle.models.dataset_column import DatasetColumn
 from kaggle.models.dataset_new_request import DatasetNewRequest
 from kaggle.models.dataset_new_version_request import DatasetNewVersionRequest
 from kaggle.models.dataset_update_settings_request import DatasetUpdateSettingsRequest
-from kaggle.models.dataset_upload_file import DatasetUploadFile
 from kaggle.models.error import Error
 from kaggle.models.kernel_push_request import KernelPushRequest
 from kaggle.models.license import License
+from kaggle.models.model_instance_new_version_request import ModelInstanceNewVersionRequest
+from kaggle.models.model_instance_update_request import ModelInstanceUpdateRequest
+from kaggle.models.model_new_instance_request import ModelNewInstanceRequest
+from kaggle.models.model_new_request import ModelNewRequest
+from kaggle.models.model_update_request import ModelUpdateRequest
 from kaggle.models.result import Result
+from kaggle.models.upload_file import UploadFile
```

### Comparing `kaggle-1.5.9/kaggle/models/collaborator.py` & `kaggle-1.6.0a0/kaggle/models/collaborator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kaggle-1.5.9/kaggle/models/dataset_column.py` & `kaggle-1.6.0a0/kaggle/models/dataset_column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kaggle-1.5.9/kaggle/models/dataset_new_request.py` & `kaggle-1.6.0a0/kaggle/models/dataset_new_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -28,15 +28,15 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from kaggle.models.dataset_upload_file import DatasetUploadFile  # noqa: F401,E501
+from kaggle.models.upload_file import UploadFile  # noqa: F401,E501
 
 
 class DatasetNewRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
@@ -51,15 +51,15 @@
     swagger_types = {
         'title': 'str',
         'slug': 'str',
         'owner_slug': 'str',
         'license_name': 'str',
         'subtitle': 'str',
         'description': 'str',
-        'files': 'list[DatasetUploadFile]',
+        'files': 'list[UploadFile]',
         'is_private': 'bool',
         'convert_to_csv': 'bool',
         'category_ids': 'list[str]'
     }
 
     attribute_map = {
         'title': 'title',
@@ -257,26 +257,26 @@
     @property
     def files(self):
         """Gets the files of this DatasetNewRequest.  # noqa: E501
 
         A list of files that should be associated with the dataset  # noqa: E501
 
         :return: The files of this DatasetNewRequest.  # noqa: E501
-        :rtype: list[DatasetUploadFile]
+        :rtype: list[UploadFile]
         """
         return self._files
 
     @files.setter
     def files(self, files):
         """Sets the files of this DatasetNewRequest.
 
         A list of files that should be associated with the dataset  # noqa: E501
 
         :param files: The files of this DatasetNewRequest.  # noqa: E501
-        :type: list[DatasetUploadFile]
+        :type: list[UploadFile]
         """
         if files is None:
             raise ValueError("Invalid value for `files`, must not be `None`")  # noqa: E501
 
         self._files = files
 
     @property
```

### Comparing `kaggle-1.5.9/kaggle/models/dataset_new_version_request.py` & `kaggle-1.6.0a0/kaggle/models/dataset_new_version_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -28,15 +28,15 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from kaggle.models.dataset_upload_file import DatasetUploadFile  # noqa: F401,E501
+from kaggle.models.upload_file import UploadFile  # noqa: F401,E501
 
 
 class DatasetNewVersionRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
@@ -48,15 +48,15 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'version_notes': 'str',
         'subtitle': 'str',
         'description': 'str',
-        'files': 'list[DatasetUploadFile]',
+        'files': 'list[UploadFile]',
         'convert_to_csv': 'bool',
         'category_ids': 'list[str]',
         'delete_old_versions': 'bool'
     }
 
     attribute_map = {
         'version_notes': 'versionNotes',
@@ -167,26 +167,26 @@
     @property
     def files(self):
         """Gets the files of this DatasetNewVersionRequest.  # noqa: E501
 
         A list of files that should be associated with the dataset  # noqa: E501
 
         :return: The files of this DatasetNewVersionRequest.  # noqa: E501
-        :rtype: list[DatasetUploadFile]
+        :rtype: list[UploadFile]
         """
         return self._files
 
     @files.setter
     def files(self, files):
         """Sets the files of this DatasetNewVersionRequest.
 
         A list of files that should be associated with the dataset  # noqa: E501
 
         :param files: The files of this DatasetNewVersionRequest.  # noqa: E501
-        :type: list[DatasetUploadFile]
+        :type: list[UploadFile]
         """
         if files is None:
             raise ValueError("Invalid value for `files`, must not be `None`")  # noqa: E501
 
         self._files = files
 
     @property
```

### Comparing `kaggle-1.5.9/kaggle/models/dataset_update_settings_request.py` & `kaggle-1.6.0a0/kaggle/models/dataset_update_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kaggle-1.5.9/kaggle/models/dataset_upload_file.py` & `kaggle-1.6.0a0/kaggle/models/model_instance_new_version_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -28,125 +28,98 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from kaggle.models.dataset_column import DatasetColumn  # noqa: F401,E501
+from kaggle.models.upload_file import UploadFile  # noqa: F401,E501
 
 
-class DatasetUploadFile(object):
+class ModelInstanceNewVersionRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'token': 'str',
-        'description': 'str',
-        'columns': 'list[DatasetColumn]'
+        'version_notes': 'str',
+        'files': 'list[UploadFile]'
     }
 
     attribute_map = {
-        'token': 'token',
-        'description': 'description',
-        'columns': 'columns'
+        'version_notes': 'versionNotes',
+        'files': 'files'
     }
 
-    def __init__(self, token=None, description=None, columns=None):  # noqa: E501
-        """DatasetUploadFile - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, version_notes=None, files=None):  # noqa: E501
+        """ModelInstanceNewVersionRequest - a model defined in Swagger"""  # noqa: E501
 
-        self._token = None
-        self._description = None
-        self._columns = None
+        self._version_notes = None
+        self._files = None
         self.discriminator = None
 
-        if token is not None:
-            self.token = token
-        if description is not None:
-            self.description = description
-        if columns is not None:
-            self.columns = columns
+        if version_notes is not None:
+            self.version_notes = version_notes
+        self.files = files
 
     @property
-    def token(self):
-        """Gets the token of this DatasetUploadFile.  # noqa: E501
+    def version_notes(self):
+        """Gets the version_notes of this ModelInstanceNewVersionRequest.  # noqa: E501
 
-        A token referencing a specific file upload that can be used across requests  # noqa: E501
+        The version notes for the model instance version  # noqa: E501
 
-        :return: The token of this DatasetUploadFile.  # noqa: E501
+        :return: The version_notes of this ModelInstanceNewVersionRequest.  # noqa: E501
         :rtype: str
         """
-        return self._token
+        return self._version_notes
 
-    @token.setter
-    def token(self, token):
-        """Sets the token of this DatasetUploadFile.
+    @version_notes.setter
+    def version_notes(self, version_notes):
+        """Sets the version_notes of this ModelInstanceNewVersionRequest.
 
-        A token referencing a specific file upload that can be used across requests  # noqa: E501
+        The version notes for the model instance version  # noqa: E501
 
-        :param token: The token of this DatasetUploadFile.  # noqa: E501
+        :param version_notes: The version_notes of this ModelInstanceNewVersionRequest.  # noqa: E501
         :type: str
         """
 
-        self._token = token
+        self._version_notes = version_notes
 
     @property
-    def description(self):
-        """Gets the description of this DatasetUploadFile.  # noqa: E501
+    def files(self):
+        """Gets the files of this ModelInstanceNewVersionRequest.  # noqa: E501
 
-        The file description  # noqa: E501
+        A list of files that should be associated with the model instance version  # noqa: E501
 
-        :return: The description of this DatasetUploadFile.  # noqa: E501
-        :rtype: str
-        """
-        return self._description
-
-    @description.setter
-    def description(self, description):
-        """Sets the description of this DatasetUploadFile.
-
-        The file description  # noqa: E501
-
-        :param description: The description of this DatasetUploadFile.  # noqa: E501
-        :type: str
-        """
-
-        self._description = description
-
-    @property
-    def columns(self):
-        """Gets the columns of this DatasetUploadFile.  # noqa: E501
-
-        A list of dataset column metadata  # noqa: E501
-
-        :return: The columns of this DatasetUploadFile.  # noqa: E501
-        :rtype: list[DatasetColumn]
+        :return: The files of this ModelInstanceNewVersionRequest.  # noqa: E501
+        :rtype: list[UploadFile]
         """
-        return self._columns
+        return self._files
 
-    @columns.setter
-    def columns(self, columns):
-        """Sets the columns of this DatasetUploadFile.
+    @files.setter
+    def files(self, files):
+        """Sets the files of this ModelInstanceNewVersionRequest.
 
-        A list of dataset column metadata  # noqa: E501
+        A list of files that should be associated with the model instance version  # noqa: E501
 
-        :param columns: The columns of this DatasetUploadFile.  # noqa: E501
-        :type: list[DatasetColumn]
+        :param files: The files of this ModelInstanceNewVersionRequest.  # noqa: E501
+        :type: list[UploadFile]
         """
+        if files is None:
+            raise ValueError("Invalid value for `files`, must not be `None`")  # noqa: E501
 
-        self._columns = columns
+        self._files = files
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -174,15 +147,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DatasetUploadFile):
+        if not isinstance(other, ModelInstanceNewVersionRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `kaggle-1.5.9/kaggle/models/error.py` & `kaggle-1.6.0a0/kaggle/models/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kaggle-1.5.9/kaggle/models/kaggle_models_extended.py` & `kaggle-1.6.0a0/kaggle/models/kaggle_models_extended.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -32,89 +32,107 @@
 
 # coding=utf-8
 import os
 from datetime import datetime
 
 
 class Competition(object):
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
         self.tags = [Tag(t) for t in self.tags]
 
     def __repr__(self):
         return self.ref
 
 
 class SubmitResult(object):
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
 
     def __repr__(self):
         return self.message
 
 
 class Submission(object):
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
         if self.totalBytes is None:
             self.size = None
         else:
             self.size = File.get_size(self.totalBytes)
 
     def __repr__(self):
         return str(self.ref)
 
 
 class LeaderboardEntry(object):
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
 
     def __repr__(self):
         return self.teamId
 
 
 class Dataset(object):
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
         self.tags = [Tag(t) for t in self.tags]
         self.files = [File(f) for f in self.files]
         self.versions = [DatasetVersion(v) for v in self.versions]
         self.size = File.get_size(self.totalBytes)
 
     def __repr__(self):
         return self.ref
 
 
+class Model(object):
+
+    def __init__(self, init_dict):
+        parsed_dict = {k: parse(v) for k, v in init_dict.items()}
+        self.__dict__.update(parsed_dict)
+
+    def __repr__(self):
+        return self.ref
+
+
 class Metadata(object):
+
     def __init__(self, init_info):
         parsed_info = {k: parse(v) for k, v in init_info.items()}
         # backwards compatibility
         self.id = parsed_info["ownerUser"] + "/" + parsed_info['datasetSlug']
         self.id_no = parsed_info['datasetId']
         self.__dict__.update(parsed_info)
 
     def __repr__(self):
         return str(self.datasetId)
 
 
 class DatasetVersion(object):
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
 
     def __repr__(self):
         return str(self.versionNumber)
 
 
 class File(object):
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
         self.size = File.get_size(self.totalBytes)
 
     def __repr__(self):
         return self.ref
@@ -126,80 +144,107 @@
         while size >= 1024 and suffix_index < 4:
             suffix_index += 1
             size /= 1024.0
         return '%.*f%s' % (precision, size, suffixes[suffix_index])
 
 
 class Tag(object):
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
 
     def __repr__(self):
         return self.ref
 
 
 class FileUploadInfo(object):
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
 
     def __repr__(self):
         return self.token
 
 
 class DatasetNewVersionResponse(object):
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
 
     def __repr__(self):
         return self.url
 
 
 class DatasetNewResponse(object):
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
 
     def __repr__(self):
         return self.url
 
 
 class ListFilesResult(object):
+
     def __init__(self, init_dict):
         self.error_message = init_dict['errorMessage']
         files = init_dict['datasetFiles']
         if files:
             self.files = [File(f) for f in files]
         else:
             self.files = {}
 
     def __repr__(self):
         return self.error_message
 
 
 class Kernel:
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
 
     def __repr__(self):
         return self.title
 
 
 class KernelPushResponse(object):
+
     def __init__(self, init_dict):
         parsed_dict = {k: parse(v) for k, v in init_dict.items()}
         self.__dict__.update(parsed_dict)
 
     def __repr__(self):
         return self.newUrl
 
 
+class ModelNewResponse(object):
+
+    def __init__(self, init_dict):
+        parsed_dict = {k: parse(v) for k, v in init_dict.items()}
+        self.__dict__.update(parsed_dict)
+
+    def __repr__(self):
+        return self.url
+
+
+class ModelDeleteResponse(object):
+
+    def __init__(self, init_dict):
+        parsed_dict = {k: parse(v) for k, v in init_dict.items()}
+        self.__dict__.update(parsed_dict)
+
+    def __repr__(self):
+        return self.error
+
+
 def parse(string):
     time_formats = [
         '%Y-%m-%dT%H:%M:%S', '%Y-%m-%dT%H:%M:%SZ', '%Y-%m-%dT%H:%M:%S.%f',
         '%Y-%m-%dT%H:%M:%S.%fZ'
     ]
     for t in time_formats:
         try:
```

### Comparing `kaggle-1.5.9/kaggle/models/kernel_push_request.py` & `kaggle-1.6.0a0/kaggle/models/kernel_push_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -55,14 +55,15 @@
         'kernel_type': 'str',
         'is_private': 'bool',
         'enable_gpu': 'bool',
         'enable_internet': 'bool',
         'dataset_data_sources': 'list[str]',
         'competition_data_sources': 'list[str]',
         'kernel_data_sources': 'list[str]',
+        'model_data_sources': 'list[str]',
         'category_ids': 'list[str]',
         'docker_image_pinning_type': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'slug': 'slug',
@@ -72,33 +73,35 @@
         'kernel_type': 'kernelType',
         'is_private': 'isPrivate',
         'enable_gpu': 'enableGpu',
         'enable_internet': 'enableInternet',
         'dataset_data_sources': 'datasetDataSources',
         'competition_data_sources': 'competitionDataSources',
         'kernel_data_sources': 'kernelDataSources',
+        'model_data_sources': 'modelDataSources',
         'category_ids': 'categoryIds',
         'docker_image_pinning_type': 'dockerImagePinningType'
     }
 
-    def __init__(self, id=None, slug=None, new_title=None, text=None, language=None, kernel_type=None, is_private=None, enable_gpu=None, enable_internet=None, dataset_data_sources=None, competition_data_sources=None, kernel_data_sources=None, category_ids=None, docker_image_pinning_type=None):  # noqa: E501
+    def __init__(self, id=None, slug=None, new_title=None, text=None, language=None, kernel_type=None, is_private=None, enable_gpu=None, enable_internet=None, dataset_data_sources=None, competition_data_sources=None, kernel_data_sources=None, model_data_sources=None, category_ids=None, docker_image_pinning_type=None):  # noqa: E501
         """KernelPushRequest - a model defined in Swagger"""  # noqa: E501
 
         self._id = None
         self._slug = None
         self._new_title = None
         self._text = None
         self._language = None
         self._kernel_type = None
         self._is_private = None
         self._enable_gpu = None
         self._enable_internet = None
         self._dataset_data_sources = None
         self._competition_data_sources = None
         self._kernel_data_sources = None
+        self._model_data_sources = None
         self._category_ids = None
         self._docker_image_pinning_type = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         if slug is not None:
@@ -116,14 +119,16 @@
             self.enable_internet = enable_internet
         if dataset_data_sources is not None:
             self.dataset_data_sources = dataset_data_sources
         if competition_data_sources is not None:
             self.competition_data_sources = competition_data_sources
         if kernel_data_sources is not None:
             self.kernel_data_sources = kernel_data_sources
+        if model_data_sources is not None:
+            self.model_data_sources = model_data_sources
         if category_ids is not None:
             self.category_ids = category_ids
         if docker_image_pinning_type is not None:
             self.docker_image_pinning_type = docker_image_pinning_type
 
     @property
     def id(self):
@@ -416,14 +421,37 @@
         :param kernel_data_sources: The kernel_data_sources of this KernelPushRequest.  # noqa: E501
         :type: list[str]
         """
 
         self._kernel_data_sources = kernel_data_sources
 
     @property
+    def model_data_sources(self):
+        """Gets the model_data_sources of this KernelPushRequest.  # noqa: E501
+
+        A list of model data sources that the kernel should use. Each model is specified as `USERNAME/MODEL-SLUG/FRAMEWORK/VARIATION-SLUG/VERSION-NUMBER`  # noqa: E501
+
+        :return: The model_data_sources of this KernelPushRequest.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._model_data_sources
+
+    @model_data_sources.setter
+    def model_data_sources(self, model_data_sources):
+        """Sets the model_data_sources of this KernelPushRequest.
+
+        A list of model data sources that the kernel should use. Each model is specified as `USERNAME/MODEL-SLUG/FRAMEWORK/VARIATION-SLUG/VERSION-NUMBER`  # noqa: E501
+
+        :param model_data_sources: The model_data_sources of this KernelPushRequest.  # noqa: E501
+        :type: list[str]
+        """
+
+        self._model_data_sources = model_data_sources
+
+    @property
     def category_ids(self):
         """Gets the category_ids of this KernelPushRequest.  # noqa: E501
 
         A list of tag IDs to associated with the kernel  # noqa: E501
 
         :return: The category_ids of this KernelPushRequest.  # noqa: E501
         :rtype: list[str]
```

### Comparing `kaggle-1.5.9/kaggle/models/license.py` & `kaggle-1.6.0a0/kaggle/models/license.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kaggle-1.5.9/kaggle/models/result.py` & `kaggle-1.6.0a0/kaggle/models/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kaggle-1.5.9/kaggle/rest.py` & `kaggle-1.6.0a0/kaggle/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kaggle-1.5.9/kaggle/tests/__init__.py` & `kaggle-1.6.0a0/kaggle/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `kaggle-1.5.9/kaggle/tests/test_authenticate.py` & `kaggle-1.6.0a0/kaggle/tests/test_authenticate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,14 +19,15 @@
 # python -m unittest tests.test_authenticate
 
 import os
 import unittest
 
 
 class TestAuthenticate(unittest.TestCase):
+
     def setUp(self):
         print("setup             class:%s" % self)
 
     def tearDown(self):
         print("teardown          class:TestStuff")
 
     # Environment
```

### Comparing `kaggle-1.5.9/kaggle.egg-info/SOURCES.txt` & `kaggle-1.6.0a0/kaggle.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 kaggle/__init__.py
 kaggle/api_client.py
 kaggle/cli.py
@@ -18,15 +19,20 @@
 kaggle/api/kaggle_api_extended.py
 kaggle/models/__init__.py
 kaggle/models/collaborator.py
 kaggle/models/dataset_column.py
 kaggle/models/dataset_new_request.py
 kaggle/models/dataset_new_version_request.py
 kaggle/models/dataset_update_settings_request.py
-kaggle/models/dataset_upload_file.py
 kaggle/models/error.py
 kaggle/models/kaggle_models_extended.py
 kaggle/models/kernel_push_request.py
 kaggle/models/license.py
+kaggle/models/model_instance_new_version_request.py
+kaggle/models/model_instance_update_request.py
+kaggle/models/model_new_instance_request.py
+kaggle/models/model_new_request.py
+kaggle/models/model_update_request.py
 kaggle/models/result.py
+kaggle/models/upload_file.py
 kaggle/tests/__init__.py
 kaggle/tests/test_authenticate.py
```

### Comparing `kaggle-1.5.9/setup.py` & `kaggle-1.6.0a0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2020 Kaggle Inc
+# Copyright 2023 Kaggle Inc
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,30 +15,35 @@
 # limitations under the License.
 
 # coding=utf-8
 from setuptools import setup, find_packages
 
 setup(
     name='kaggle',
-    version='1.5.9',
+    version='1.6.0a0',
     description='Kaggle API',
     long_description=
     ('Official API for https://www.kaggle.com, accessible using a command line '
      'tool implemented in Python. Beta release - Kaggle reserves the right to '
      'modify the API functionality currently offered.'),
     author='Kaggle',
     author_email='support@kaggle.com',
     url='https://github.com/Kaggle/kaggle-api',
+    project_urls={
+        'Documentation': 'https://www.kaggle.com/docs/api',
+        'GitHub': 'https://github.com/Kaggle/kaggle-api',
+        'Tracker': 'https://github.com/Kaggle/kaggle-api/issues',
+    },
     keywords=['Kaggle', 'API'],
     entry_points={'console_scripts': ['kaggle = kaggle.cli:main']},
     install_requires=[
         'six >= 1.10',
         'certifi',
         'python-dateutil',
         'requests',
         'tqdm',
         'python-slugify',
-        'slugify',
         'urllib3',
+        'bleach',
     ],
     packages=find_packages(),
     license='Apache 2.0')
```

