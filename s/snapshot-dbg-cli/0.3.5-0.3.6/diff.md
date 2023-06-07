# Comparing `tmp/snapshot-dbg-cli-0.3.5.tar.gz` & `tmp/snapshot-dbg-cli-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapshot-dbg-cli-0.3.5.tar", last modified: Thu May 18 18:53:36 2023, max compression
+gzip compressed data, was "snapshot-dbg-cli-0.3.6.tar", last modified: Wed Jun  7 17:55:38 2023, max compression
```

## Comparing `snapshot-dbg-cli-0.3.5.tar` & `snapshot-dbg-cli-0.3.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 jcborg   (634821) primarygroup (89939)        0 2023-05-18 18:53:36.207439 snapshot-dbg-cli-0.3.5/
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    11358 2023-05-16 20:47:12.000000 snapshot-dbg-cli-0.3.5/LICENSE
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    26475 2023-05-18 18:53:36.207439 snapshot-dbg-cli-0.3.5/PKG-INFO
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    25324 2023-05-18 18:18:38.000000 snapshot-dbg-cli-0.3.5/README.md
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1262 2023-05-18 18:53:36.207439 snapshot-dbg-cli-0.3.5/setup.cfg
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)      760 2023-05-16 20:47:12.000000 snapshot-dbg-cli-0.3.5/setup.py
-drwxr-xr-x   0 jcborg   (634821) primarygroup (89939)        0 2023-05-18 18:53:36.207439 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1105 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/__init__.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)      703 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/__main__.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     8566 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/breakpoint_utils.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)      923 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     5209 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_common_arguments.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     2862 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_run.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    10122 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_services.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3653 2023-05-18 18:48:59.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_version.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     2399 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/data_formatter.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4432 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/debuggee_utils.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3940 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_breakpoints.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     6683 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_debuggees_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3379 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_logpoints_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3336 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_snapshots_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)      982 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/exceptions.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    11830 2023-05-18 18:18:38.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/firebase_management_rest_service.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3009 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/firebase_rtdb_rest_service.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     6212 2023-05-18 18:18:38.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/firebase_types.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     7871 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/gcloud_cli_service.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3690 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/get_logpoint_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     7186 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/get_snapshot_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    12100 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/http_service.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    17906 2023-05-18 18:18:38.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/init_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3556 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/list_debuggees_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3678 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/list_logpoints_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3604 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/list_snapshots_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4436 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/permissions_rest_service.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     7346 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/set_logpoint_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4911 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/set_snapshot_command.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    12463 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/snapshot_debugger_rtdb_service.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3878 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/snapshot_debugger_schema.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     5131 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/snapshot_parser.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3977 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/status_message.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     2769 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/time_utils.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1091 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/user_input.py
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4357 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/user_output.py
-drwxr-xr-x   0 jcborg   (634821) primarygroup (89939)        0 2023-05-18 18:53:36.207439 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)    26475 2023-05-18 18:53:36.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/PKG-INFO
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1606 2023-05-18 18:53:36.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)        1 2023-05-18 18:53:36.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)       63 2023-05-18 18:53:36.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/entry_points.txt
--rw-r--r--   0 jcborg   (634821) primarygroup (89939)       17 2023-05-18 18:53:36.000000 snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/top_level.txt
+drwxr-xr-x   0 jcborg   (634821) primarygroup (89939)        0 2023-06-07 17:55:38.207085 snapshot-dbg-cli-0.3.6/
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    11358 2023-05-16 20:47:12.000000 snapshot-dbg-cli-0.3.6/LICENSE
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    26416 2023-06-07 17:55:38.207085 snapshot-dbg-cli-0.3.6/PKG-INFO
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    25265 2023-06-07 17:29:57.000000 snapshot-dbg-cli-0.3.6/README.md
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1262 2023-06-07 17:55:38.207085 snapshot-dbg-cli-0.3.6/setup.cfg
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)      760 2023-05-16 20:47:12.000000 snapshot-dbg-cli-0.3.6/setup.py
+drwxr-xr-x   0 jcborg   (634821) primarygroup (89939)        0 2023-06-07 17:55:38.203085 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1105 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/__init__.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)      703 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/__main__.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     8566 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/breakpoint_utils.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)      923 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/cli.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     5209 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/cli_common_arguments.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     2862 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/cli_run.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    10122 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/cli_services.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3653 2023-06-07 17:43:28.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/cli_version.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     2399 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/data_formatter.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4432 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/debuggee_utils.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3940 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/delete_breakpoints.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     6683 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/delete_debuggees_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3379 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/delete_logpoints_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3336 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/delete_snapshots_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)      982 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/exceptions.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    11830 2023-05-18 18:18:38.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/firebase_management_rest_service.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3009 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/firebase_rtdb_rest_service.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     6212 2023-05-18 18:18:38.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/firebase_types.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     7871 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/gcloud_cli_service.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3690 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/get_logpoint_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     7186 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/get_snapshot_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    12100 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/http_service.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    17906 2023-05-18 18:18:38.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/init_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3556 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/list_debuggees_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3678 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/list_logpoints_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3604 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/list_snapshots_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4436 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/permissions_rest_service.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     7346 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/set_logpoint_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4911 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/set_snapshot_command.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    12463 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/snapshot_debugger_rtdb_service.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3878 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/snapshot_debugger_schema.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     5131 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/snapshot_parser.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     3977 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/status_message.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     2769 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/time_utils.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1091 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/user_input.py
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     4357 2023-05-16 20:48:08.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/user_output.py
+drwxr-xr-x   0 jcborg   (634821) primarygroup (89939)        0 2023-06-07 17:55:38.207085 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli.egg-info/
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)    26416 2023-06-07 17:55:38.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)     1606 2023-06-07 17:55:38.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)        1 2023-06-07 17:55:38.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)       63 2023-06-07 17:55:38.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jcborg   (634821) primarygroup (89939)       17 2023-06-07 17:55:38.000000 snapshot-dbg-cli-0.3.6/snapshot_dbg_cli.egg-info/top_level.txt
```

### Comparing `snapshot-dbg-cli-0.3.5/LICENSE` & `snapshot-dbg-cli-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/PKG-INFO` & `snapshot-dbg-cli-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshot-dbg-cli
-Version: 0.3.5
+Version: 0.3.6
 Summary: 'Snapshot Debugger CLI tool.'
 Home-page: https://github.com/GoogleCloudPlatform/snapshot-debugger
 Author: Google Inc.
 License: Apache License, Version 2.0
 Project-URL: CLI Source, https://github.com/GoogleCloudPlatform/snapshot-debugger
 Project-URL: Java Agent Source, https://github.com/GoogleCloudPlatform/cloud-debug-java
 Project-URL: Node.js Agent Source, https://github.com/googleapis/cloud-debug-nodejs
@@ -300,17 +300,17 @@
 For example, you may want to set up your database in Belgium, and so would run
 ```snapshot-dbg-cli init --location=europe-west1```
 
 Make note of the database URL provided in the command output; you will need to
 provide this to your debug agent(s) and the vsCode plugin.
 
 [rtdb_locations]: https://firebase.google.com/docs/projects/locations#rtdb-locations
-[java_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-java#snapshot-debugger---firebase-realtime-database-backend
-[python_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-python/blob/main/README.md#snapshot-debugger---firebase-realtime-database-backend
-[nodejs_agent_config]: https://github.com/googleapis/cloud-debug-nodejs/blob/main/README.md#snapshot-debugger---firebase-realtime-database-backend
+[java_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-java/blob/main/README.md#configuring-the-firebase-realtime-database-url
+[python_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-python/blob/main/README.md#flag-reference
+[nodejs_agent_config]: https://github.com/googleapis/cloud-debug-nodejs/blob/main/README.md#debugger-agent-settings
 [extension_config]: https://github.com/GoogleCloudPlatform/snapshot-debugger/blob/main/snapshot_dbg_extension/README.md#configuration
 
 
 ## Set up Snapshot Debugger in your Google Cloud project
 
 ### Working Samples
```

### Comparing `snapshot-dbg-cli-0.3.5/README.md` & `snapshot-dbg-cli-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -275,17 +275,17 @@
 For example, you may want to set up your database in Belgium, and so would run
 ```snapshot-dbg-cli init --location=europe-west1```
 
 Make note of the database URL provided in the command output; you will need to
 provide this to your debug agent(s) and the vsCode plugin.
 
 [rtdb_locations]: https://firebase.google.com/docs/projects/locations#rtdb-locations
-[java_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-java#snapshot-debugger---firebase-realtime-database-backend
-[python_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-python/blob/main/README.md#snapshot-debugger---firebase-realtime-database-backend
-[nodejs_agent_config]: https://github.com/googleapis/cloud-debug-nodejs/blob/main/README.md#snapshot-debugger---firebase-realtime-database-backend
+[java_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-java/blob/main/README.md#configuring-the-firebase-realtime-database-url
+[python_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-python/blob/main/README.md#flag-reference
+[nodejs_agent_config]: https://github.com/googleapis/cloud-debug-nodejs/blob/main/README.md#debugger-agent-settings
 [extension_config]: https://github.com/GoogleCloudPlatform/snapshot-debugger/blob/main/snapshot_dbg_extension/README.md#configuration
 
 
 ## Set up Snapshot Debugger in your Google Cloud project
 
 ### Working Samples
```

### Comparing `snapshot-dbg-cli-0.3.5/setup.cfg` & `snapshot-dbg-cli-0.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/setup.py` & `snapshot-dbg-cli-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/__init__.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/__main__.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/breakpoint_utils.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/breakpoint_utils.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/cli.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_common_arguments.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/cli_common_arguments.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_run.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/cli_run.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_services.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/cli_services.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/cli_version.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/cli_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import sys
 
 from snapshot_dbg_cli.data_formatter import DataFormatter
 from snapshot_dbg_cli.exceptions import SilentlyExitError
 from snapshot_dbg_cli.http_service import HttpService
 from snapshot_dbg_cli.user_output import UserOutput
 
-VERSION = 'SNAPSHOT_DEBUGGER_CLI_VERSION_0_3_5'
+VERSION = 'SNAPSHOT_DEBUGGER_CLI_VERSION_0_3_6'
 
 VERSION_PATTERN = 'SNAPSHOT_DEBUGGER_CLI_VERSION_[0-9]+_[0-9]+_[0-9]+'
 
 VERSION_URL = ('https://raw.githubusercontent.com/GoogleCloudPlatform'
                '/snapshot-debugger/main/snapshot_dbg_cli/cli_version.py')
 
 NEWER_VERSION_MESSAGE = """
```

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/data_formatter.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/data_formatter.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/debuggee_utils.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/debuggee_utils.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_breakpoints.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/delete_breakpoints.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_debuggees_command.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/delete_debuggees_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_logpoints_command.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/delete_logpoints_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/delete_snapshots_command.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/delete_snapshots_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/exceptions.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/firebase_management_rest_service.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/firebase_management_rest_service.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/firebase_rtdb_rest_service.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/firebase_rtdb_rest_service.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/firebase_types.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/firebase_types.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/gcloud_cli_service.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/gcloud_cli_service.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/get_logpoint_command.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/get_logpoint_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/get_snapshot_command.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/get_snapshot_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/http_service.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/http_service.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/init_command.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/init_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/list_debuggees_command.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/list_debuggees_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/list_logpoints_command.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/list_logpoints_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/list_snapshots_command.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/list_snapshots_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/permissions_rest_service.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/permissions_rest_service.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/set_logpoint_command.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/set_logpoint_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/set_snapshot_command.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/set_snapshot_command.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/snapshot_debugger_rtdb_service.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/snapshot_debugger_rtdb_service.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/snapshot_debugger_schema.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/snapshot_debugger_schema.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/snapshot_parser.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/snapshot_parser.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/status_message.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/status_message.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/time_utils.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/time_utils.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/user_input.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/user_input.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli/user_output.py` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli/user_output.py`

 * *Files identical despite different names*

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/PKG-INFO` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshot-dbg-cli
-Version: 0.3.5
+Version: 0.3.6
 Summary: 'Snapshot Debugger CLI tool.'
 Home-page: https://github.com/GoogleCloudPlatform/snapshot-debugger
 Author: Google Inc.
 License: Apache License, Version 2.0
 Project-URL: CLI Source, https://github.com/GoogleCloudPlatform/snapshot-debugger
 Project-URL: Java Agent Source, https://github.com/GoogleCloudPlatform/cloud-debug-java
 Project-URL: Node.js Agent Source, https://github.com/googleapis/cloud-debug-nodejs
@@ -300,17 +300,17 @@
 For example, you may want to set up your database in Belgium, and so would run
 ```snapshot-dbg-cli init --location=europe-west1```
 
 Make note of the database URL provided in the command output; you will need to
 provide this to your debug agent(s) and the vsCode plugin.
 
 [rtdb_locations]: https://firebase.google.com/docs/projects/locations#rtdb-locations
-[java_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-java#snapshot-debugger---firebase-realtime-database-backend
-[python_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-python/blob/main/README.md#snapshot-debugger---firebase-realtime-database-backend
-[nodejs_agent_config]: https://github.com/googleapis/cloud-debug-nodejs/blob/main/README.md#snapshot-debugger---firebase-realtime-database-backend
+[java_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-java/blob/main/README.md#configuring-the-firebase-realtime-database-url
+[python_agent_config]: https://github.com/GoogleCloudPlatform/cloud-debug-python/blob/main/README.md#flag-reference
+[nodejs_agent_config]: https://github.com/googleapis/cloud-debug-nodejs/blob/main/README.md#debugger-agent-settings
 [extension_config]: https://github.com/GoogleCloudPlatform/snapshot-debugger/blob/main/snapshot_dbg_extension/README.md#configuration
 
 
 ## Set up Snapshot Debugger in your Google Cloud project
 
 ### Working Samples
```

### Comparing `snapshot-dbg-cli-0.3.5/snapshot_dbg_cli.egg-info/SOURCES.txt` & `snapshot-dbg-cli-0.3.6/snapshot_dbg_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

