# Comparing `tmp/bodosdk-1.3.3.tar.gz` & `tmp/bodosdk-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodosdk-1.3.3.tar", last modified: Tue May 30 20:55:17 2023, max compression
+gzip compressed data, was "bodosdk-1.3.4.tar", last modified: Wed Jun  7 19:58:29 2023, max compression
```

## Comparing `bodosdk-1.3.3.tar` & `bodosdk-1.3.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:17.471089 bodosdk-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-05-30 20:55:09.000000 bodosdk-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-30 20:55:09.000000 bodosdk-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    50452 2023-05-30 20:55:17.471089 bodosdk-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    49757 2023-05-30 20:55:09.000000 bodosdk-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:17.471089 bodosdk-1.3.3/bodosdk/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-30 20:55:17.471089 bodosdk-1.3.3/bodosdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:17.467089 bodosdk-1.3.3/bodosdk/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     8160 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    14676 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/request_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:17.467089 bodosdk-1.3.3/bodosdk/client/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6724 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    13203 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/workspace.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:17.471089 bodosdk-1.3.3/bodosdk/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1411 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3729 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    14785 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/job.py
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:17.463089 bodosdk-1.3.3/bodosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    50452 2023-05-30 20:55:17.000000 bodosdk-1.3.3/bodosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-05-30 20:55:17.000000 bodosdk-1.3.3/bodosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 20:55:17.000000 bodosdk-1.3.3/bodosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-30 20:55:17.000000 bodosdk-1.3.3/bodosdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-30 20:55:17.000000 bodosdk-1.3.3/bodosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-30 20:55:17.471089 bodosdk-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-05-30 20:55:09.000000 bodosdk-1.3.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    80044 2023-05-30 20:55:09.000000 bodosdk-1.3.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:58:29.482819 bodosdk-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-06-07 19:58:20.000000 bodosdk-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-07 19:58:20.000000 bodosdk-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    50506 2023-06-07 19:58:29.482819 bodosdk-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    49811 2023-06-07 19:58:20.000000 bodosdk-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:58:29.482819 bodosdk-1.3.4/bodosdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-07 19:58:29.482819 bodosdk-1.3.4/bodosdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:58:29.478819 bodosdk-1.3.4/bodosdk/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/api/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8160 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/api/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/api/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15138 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/api/request_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/api/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/api/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:58:29.478819 bodosdk-1.3.4/bodosdk/client/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/client/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/client/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6724 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/client/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/client/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13222 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/client/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/client/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/client/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/client/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:58:29.482819 bodosdk-1.3.4/bodosdk/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1411 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/models/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/models/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/models/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14785 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/models/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-06-07 19:58:20.000000 bodosdk-1.3.4/bodosdk/models/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 19:58:29.478819 bodosdk-1.3.4/bodosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    50506 2023-06-07 19:58:29.000000 bodosdk-1.3.4/bodosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-07 19:58:29.000000 bodosdk-1.3.4/bodosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 19:58:29.000000 bodosdk-1.3.4/bodosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-07 19:58:29.000000 bodosdk-1.3.4/bodosdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-07 19:58:29.000000 bodosdk-1.3.4/bodosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-07 19:58:29.482819 bodosdk-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-06-07 19:58:20.000000 bodosdk-1.3.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    80044 2023-06-07 19:58:20.000000 bodosdk-1.3.4/versioneer.py
```

### Comparing `bodosdk-1.3.3/LICENSE` & `bodosdk-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/PKG-INFO` & `bodosdk-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 1.3.3
+Version: 1.3.4
 Summary: Bodo Platform SDK
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -676,34 +676,36 @@
 | `batch_job_id`    | `List[str]`         | List of Ids of the batch job definitions | No                |
 | `status`          | `List[JobRunStatus]`| List of Job Run Statuses                 | No                |
 | `cluster_id`      | `List[str]`         | List of Ids of the clusters              | No                |
 
 Lists all batch job runs in the given workspace filtered by given parameters.
 
 **Example:**
+
 ```python
-from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
-    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType,
+  WorkspaceDef, CreateBatchJobDefinition
 from bodosdk.client import get_bodo_client
 from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
 
 keys = WorkspaceKeys(
-    client_id="XYZ",
-    secret_key="XYZ"
+  client_id="XYZ",
+  secret_key="XYZ"
 )
 
 client = get_bodo_client(keys)
-jobruns = client.job.list_batch_job_runs(status=[JobRunStatus.FAILED], cluster_id=['ba62e653-312a-490e-9457-71d7bc096959'])
+jobruns = client.job.list_batch_job_runs(statuses=[JobRunStatus.FAILED],
+                                         cluster_ids=['ba62e653-312a-490e-9457-71d7bc096959'])
 ```
 
 <br/>
 
 ##### List batch job runs by batch job name
 
-`BodoClient.job.list_batch_job_runs_by_names()`
+`BodoClient.job.list_job_runs_by_batch_job_name()`
 
 | Parameter            | Type                | Description                              | Required          |
 |----------------------|---------------------|------------------------------------------|-------------------|
 | `batch_job_names`    | `List[str]`         | List of Ids of the batch job definitions | No                |
 | `status`             | `List[JobRunStatus]`| List of Job Run Statuses                 | No                |
 | `cluster_id`         | `List[str]`         | List of Ids of the clusters              | No                |
 
@@ -719,15 +721,15 @@
 
 keys = WorkspaceKeys(
     client_id="XYZ",
     secret_key="XYZ"
 )
 
 client = get_bodo_client(keys)
-jobruns = client.job.list_batch_job_runs_by_names(batch_job_names=['production-job-1'], status=[JobRunStatus.FAILED], cluster_id=['ba62e653-312a-490e-9457-71d7bc096959'])
+jobruns = client.job.list_job_runs_by_batch_job_name(batch_job_names=['production-job-1'], statuses=[JobRunStatus.FAILED], cluster_ids=['ba62e653-312a-490e-9457-71d7bc096959'])
 ```
 
 <br/>
 
 #####  Get batch job run 
 
 
@@ -834,15 +836,15 @@
             sqlQueryText="SELECT * FROM PUBLIC.TABLE LIMIT 10"))
 ```
 
 <br/>
 
 ##### Job Run waiter<a id="job-waiter"></a>
 
-`BodoClient.job.get_waiter()`
+`BodoClient.job.get_job_run_waiter()`
 
 Returns a waiter object that waits until the job run uuid specified finishes.
 To wait for job run to be finished, invoke the waiter.wait() function,
 which can take the following parameters.
 
 ```python3
 from typing import Callable
```

### Comparing `bodosdk-1.3.3/README.md` & `bodosdk-1.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -655,34 +655,36 @@
 | `batch_job_id`    | `List[str]`         | List of Ids of the batch job definitions | No                |
 | `status`          | `List[JobRunStatus]`| List of Job Run Statuses                 | No                |
 | `cluster_id`      | `List[str]`         | List of Ids of the clusters              | No                |
 
 Lists all batch job runs in the given workspace filtered by given parameters.
 
 **Example:**
+
 ```python
-from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
-    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType,
+  WorkspaceDef, CreateBatchJobDefinition
 from bodosdk.client import get_bodo_client
 from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
 
 keys = WorkspaceKeys(
-    client_id="XYZ",
-    secret_key="XYZ"
+  client_id="XYZ",
+  secret_key="XYZ"
 )
 
 client = get_bodo_client(keys)
-jobruns = client.job.list_batch_job_runs(status=[JobRunStatus.FAILED], cluster_id=['ba62e653-312a-490e-9457-71d7bc096959'])
+jobruns = client.job.list_batch_job_runs(statuses=[JobRunStatus.FAILED],
+                                         cluster_ids=['ba62e653-312a-490e-9457-71d7bc096959'])
 ```
 
 <br/>
 
 ##### List batch job runs by batch job name
 
-`BodoClient.job.list_batch_job_runs_by_names()`
+`BodoClient.job.list_job_runs_by_batch_job_name()`
 
 | Parameter            | Type                | Description                              | Required          |
 |----------------------|---------------------|------------------------------------------|-------------------|
 | `batch_job_names`    | `List[str]`         | List of Ids of the batch job definitions | No                |
 | `status`             | `List[JobRunStatus]`| List of Job Run Statuses                 | No                |
 | `cluster_id`         | `List[str]`         | List of Ids of the clusters              | No                |
 
@@ -698,15 +700,15 @@
 
 keys = WorkspaceKeys(
     client_id="XYZ",
     secret_key="XYZ"
 )
 
 client = get_bodo_client(keys)
-jobruns = client.job.list_batch_job_runs_by_names(batch_job_names=['production-job-1'], status=[JobRunStatus.FAILED], cluster_id=['ba62e653-312a-490e-9457-71d7bc096959'])
+jobruns = client.job.list_job_runs_by_batch_job_name(batch_job_names=['production-job-1'], statuses=[JobRunStatus.FAILED], cluster_ids=['ba62e653-312a-490e-9457-71d7bc096959'])
 ```
 
 <br/>
 
 #####  Get batch job run 
 
 
@@ -813,15 +815,15 @@
             sqlQueryText="SELECT * FROM PUBLIC.TABLE LIMIT 10"))
 ```
 
 <br/>
 
 ##### Job Run waiter<a id="job-waiter"></a>
 
-`BodoClient.job.get_waiter()`
+`BodoClient.job.get_job_run_waiter()`
 
 Returns a waiter object that waits until the job run uuid specified finishes.
 To wait for job run to be finished, invoke the waiter.wait() function,
 which can take the following parameters.
 
 ```python3
 from typing import Callable
```

### Comparing `bodosdk-1.3.3/bodosdk/api/auth.py` & `bodosdk-1.3.4/bodosdk/api/auth.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/api/base.py` & `bodosdk-1.3.4/bodosdk/api/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/api/catalog.py` & `bodosdk-1.3.4/bodosdk/api/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/api/cloud_config.py` & `bodosdk-1.3.4/bodosdk/api/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/api/cluster.py` & `bodosdk-1.3.4/bodosdk/api/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/api/instance_role.py` & `bodosdk-1.3.4/bodosdk/api/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/api/job.py` & `bodosdk-1.3.4/bodosdk/api/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,25 @@
                 param = f"{k}={v}"
             query_params.append(param)
     if query_params:
         return "?" + "&".join(query_params)
     return ""
 
 
+def handle_pydantic_validation_issues_for_batch_job_def_response_json(response_json):
+    try:
+        return BatchJobDefinitionResponse(**response_json)
+    except pydantic.ValidationError:
+        logging.error(
+            f"Failed to parse batch job definition for batch job id: {response_json['uuid']}"
+        )
+    except Exception as e:
+        logging.error(f"Bad Response: {e}")
+
+
 class JobApi(BackendApi):
     def __init__(self, *args, **kwargs):
         super(JobApi, self).__init__(*args, **kwargs)
         self._resource_url = "job"
 
     def create_job(self, job_definition: JobDefinition) -> JobCreateResponse:
         headers = {"Content-type": "application/json"}
@@ -182,67 +193,70 @@
         raise UnknownError(resp.content)
 
     # Todo: add query semantics for filtering
     @validate_arguments
     def list_batch_job_definitions(
         self,
         page: int = DEFAULT_PAGE,
-        page_size: int = DEFAULT_PAGE_SIZE,
-        sort_order: PaginationOrder = DEFAULT_ORDER,
+        size: int = DEFAULT_PAGE_SIZE,
+        order: PaginationOrder = DEFAULT_ORDER,
     ) -> List[BatchJobDefinitionResponse]:
         query_string_args = {
             k: v for k, v in locals().items() if v and k in LIST_QUERY_PARAMS
         }
         headers = self.get_auth_header()
         resource_url = f"{self.get_resource_url()}/batch_job_def{build_query_string(query_string_args)}"
         resp = self._requests.get(resource_url, headers=headers)
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
         if str(resp.status_code).startswith("4"):
             raise ResourceNotFound(resp.json()["message"])
 
         result = []
         for json_data in resp.json()["data"]:
-            try:
-                result.append(BatchJobDefinitionResponse(**json_data))
-            except pydantic.ValidationError:
-                logging.error(
-                    f"Failed to parse batch job definition for batch job id: {json_data['uuid']}"
+            batch_job_def = (
+                handle_pydantic_validation_issues_for_batch_job_def_response_json(
+                    json_data
                 )
-            except Exception as e:
-                logging.error(f"Bad Response: {e}")
+            )
+            if batch_job_def:
+                result.append(batch_job_def)
         return result
 
     @validate_arguments
     def get_batch_job_definition(self, uuid: UUID) -> BatchJobDefinitionResponse:
         headers = self.get_auth_header()
         resp = self._requests.get(
             f"{self.get_resource_url()}/batch_job_def/{uuid}", headers=headers
         )
         if resp.status_code == 404:
             raise ResourceNotFound
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable(resp.content)
         json_data = resp.json()
-        return BatchJobDefinitionResponse(**json_data)
+        return handle_pydantic_validation_issues_for_batch_job_def_response_json(
+            json_data
+        )
 
     @validate_arguments
     def get_batch_job_definition_by_name(self, name: str) -> BatchJobDefinitionResponse:
         headers = self.get_auth_header()
         resp = self._requests.get(
             f"{self.get_resource_url()}/batch_job_def?name={name}", headers=headers
         )
         if resp.status_code == 404:
             raise ResourceNotFound
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
 
         # Based on DB criteria there can be only one element
         for json_data in resp.json()["data"]:
-            return BatchJobDefinitionResponse(**json_data)
+            return handle_pydantic_validation_issues_for_batch_job_def_response_json(
+                json_data
+            )
 
         raise ResourceNotFound
 
     @validate_arguments
     def update_batch_job_definition(
         self, uuid: UUID, config_override: JobConfigOverride
     ) -> BatchJobDefinitionResponse:
@@ -348,22 +362,22 @@
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
         return
 
     @validate_arguments
     def list_job_runs(
         self,
-        job_type: List[JobRunType] = None,
-        batch_job_id: Union[List[UUID], None] = None,
+        type: List[JobRunType] = None,
+        batchJobDefinitionUUID: Union[List[UUID], None] = None,
         status: Union[List[JobRunStatus], None] = None,
-        cluster_id: Union[List[UUID], None] = None,
-        started_at: Union[datetime, None] = None,
-        finished_at: Union[datetime, None] = None,
+        clusterUUID: Union[List[UUID], None] = None,
+        startedAt: Union[datetime, None] = None,
+        finishedAt: Union[datetime, None] = None,
         page: int = DEFAULT_PAGE,
-        page_size: int = DEFAULT_PAGE_SIZE,
+        size: int = DEFAULT_PAGE_SIZE,
         order: PaginationOrder = DEFAULT_ORDER,
     ) -> List[JobRunResponse]:
         args = LIST_QUERY_PARAMS
         query_string_args = {
             k: v for k, v in locals().items() if k in args and v is not None
         }
         headers = self.get_auth_header()
@@ -376,11 +390,12 @@
             raise ResourceNotFound(resp.json()["message"])
         result = []
         for json_data in resp.json()["data"]:
             try:
                 result.append(JobRunResponse(**json_data))
             except pydantic.ValidationError:
                 logging.warning(
-                    f"Failed to parse job run response: {json_data['uuid']}"
+                    f"Failed to validate job run response: {json_data['uuid']}"
                 )
+                result.append(JobRunResponse.construct(**json_data))
 
         return result
```

### Comparing `bodosdk-1.3.3/bodosdk/api/request_wrapper.py` & `bodosdk-1.3.4/bodosdk/api/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/api/secret_group.py` & `bodosdk-1.3.4/bodosdk/api/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/api/secrets.py` & `bodosdk-1.3.4/bodosdk/api/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/api/workspace.py` & `bodosdk-1.3.4/bodosdk/api/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/client/base.py` & `bodosdk-1.3.4/bodosdk/client/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/client/catalog.py` & `bodosdk-1.3.4/bodosdk/client/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/client/cloud_config.py` & `bodosdk-1.3.4/bodosdk/client/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/client/cluster.py` & `bodosdk-1.3.4/bodosdk/client/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/client/instance_role.py` & `bodosdk-1.3.4/bodosdk/client/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/client/job.py` & `bodosdk-1.3.4/bodosdk/client/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,33 +254,33 @@
             self._api.delete_batch_job_definition(uuid)
         except Exception as exception:
             raise exception
 
     def list_batch_job_runs(
         self,
         batch_job_ids: List[UUID] = None,
-        status: List[JobRunStatus] = None,
-        cluster_id: List[UUID] = None,
+        statuses: List[JobRunStatus] = None,
+        cluster_ids: List[UUID] = None,
         started_at: datetime = None,
         finished_at: datetime = None,
     ) -> List[JobRunResponse]:
         batch_job_runs = self._api.list_job_runs(
-            job_type=[JobRunType.BATCH],
-            batch_job_id=batch_job_ids,
-            status=status,
-            cluster_id=cluster_id,
-            started_at=started_at,
-            finished_at=finished_at,
+            type=[JobRunType.BATCH],
+            batchJobDefinitionUUID=batch_job_ids,
+            status=statuses,
+            clusterUUID=cluster_ids,
+            startedAt=started_at,
+            finishedAt=finished_at,
         )
 
         if len(batch_job_runs) == 0:
             logging.warning("No batch job runs found.")
         return batch_job_runs
 
-    def list_batch_job_runs_by_names(
+    def list_job_runs_by_batch_job_name(
         self,
         batch_job_names: List[str] = None,
         status: List[JobRunStatus] = None,
         cluster_id: List[UUID] = None,
         started_at: datetime = None,
         finished_at: datetime = None,
     ) -> List[JobRunResponse]:
@@ -303,20 +303,20 @@
         """
         batch_job_ids = []
         for name in batch_job_names:
             batch_job_def_uuid = self.get_batch_job_definition_by_name(name).uuid
             batch_job_ids.append(batch_job_def_uuid)
 
         batch_job_runs = self._api.list_job_runs(
-            job_type=[JobRunType.BATCH],
-            batch_job_id=batch_job_ids,
+            type=[JobRunType.BATCH],
+            batchJobDefinitionUUID=batch_job_ids,
             status=status,
-            cluster_id=cluster_id,
-            started_at=started_at,
-            finished_at=finished_at,
+            clusterUUID=cluster_id,
+            startedAt=started_at,
+            finishedAt=finished_at,
         )
         return batch_job_runs
 
     def get_batch_job_run(self, uuid: Union[str, UUID]) -> JobRunResponse:
         """
         Gets specific batch job run from workspace
```

### Comparing `bodosdk-1.3.3/bodosdk/client/secret_group.py` & `bodosdk-1.3.4/bodosdk/client/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/client/secrets.py` & `bodosdk-1.3.4/bodosdk/client/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/client/workspace.py` & `bodosdk-1.3.4/bodosdk/client/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/models/__init__.py` & `bodosdk-1.3.4/bodosdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/models/base.py` & `bodosdk-1.3.4/bodosdk/models/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/models/catalog.py` & `bodosdk-1.3.4/bodosdk/models/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/models/cloud_config.py` & `bodosdk-1.3.4/bodosdk/models/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk/models/cluster.py` & `bodosdk-1.3.4/bodosdk/models/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,9 +89,9 @@
 
 
 class ModifyCluster(CamelCaseBase):
     uuid: Union[str, UUID]
     auto_shutdown: Optional[int] = Field(None, alias="autoshutdown")
     auto_pause: Optional[int] = Field(None, alias="autopause")
     description: Optional[str] = Field(None, alias="description")
-    workers_quantity: Optional[int] = Field(-1, alias="workersQuantity")
+    workers_quantity: Optional[int] = Field(None, alias="workersQuantity")
     autoresume: Optional[bool] = Field(True, alias="autoresume")
```

### Comparing `bodosdk-1.3.3/bodosdk/models/job.py` & `bodosdk-1.3.4/bodosdk/models/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -597,17 +597,17 @@
 
 
 DEFAULT_PAGE_SIZE = 5
 DEFAULT_PAGE = 1
 DEFAULT_ORDER = PaginationOrder.ASC
 
 LIST_QUERY_PARAMS = [
-    "job_type",
-    "batch_job_id",
+    "type",
+    "batchJobDefinitionUUID",
     "status",
-    "cluster_id",
-    "started_at",
-    "finished_at",
+    "clusterUUID",
+    "startedAt",
+    "finishedAt",
     "page",
-    "page_size",
+    "size",
     "order",
 ]
```

### Comparing `bodosdk-1.3.3/bodosdk/models/workspace.py` & `bodosdk-1.3.4/bodosdk/models/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/bodosdk.egg-info/PKG-INFO` & `bodosdk-1.3.4/bodosdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 1.3.3
+Version: 1.3.4
 Summary: Bodo Platform SDK
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -676,34 +676,36 @@
 | `batch_job_id`    | `List[str]`         | List of Ids of the batch job definitions | No                |
 | `status`          | `List[JobRunStatus]`| List of Job Run Statuses                 | No                |
 | `cluster_id`      | `List[str]`         | List of Ids of the clusters              | No                |
 
 Lists all batch job runs in the given workspace filtered by given parameters.
 
 **Example:**
+
 ```python
-from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
-    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType,
+  WorkspaceDef, CreateBatchJobDefinition
 from bodosdk.client import get_bodo_client
 from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
 
 keys = WorkspaceKeys(
-    client_id="XYZ",
-    secret_key="XYZ"
+  client_id="XYZ",
+  secret_key="XYZ"
 )
 
 client = get_bodo_client(keys)
-jobruns = client.job.list_batch_job_runs(status=[JobRunStatus.FAILED], cluster_id=['ba62e653-312a-490e-9457-71d7bc096959'])
+jobruns = client.job.list_batch_job_runs(statuses=[JobRunStatus.FAILED],
+                                         cluster_ids=['ba62e653-312a-490e-9457-71d7bc096959'])
 ```
 
 <br/>
 
 ##### List batch job runs by batch job name
 
-`BodoClient.job.list_batch_job_runs_by_names()`
+`BodoClient.job.list_job_runs_by_batch_job_name()`
 
 | Parameter            | Type                | Description                              | Required          |
 |----------------------|---------------------|------------------------------------------|-------------------|
 | `batch_job_names`    | `List[str]`         | List of Ids of the batch job definitions | No                |
 | `status`             | `List[JobRunStatus]`| List of Job Run Statuses                 | No                |
 | `cluster_id`         | `List[str]`         | List of Ids of the clusters              | No                |
 
@@ -719,15 +721,15 @@
 
 keys = WorkspaceKeys(
     client_id="XYZ",
     secret_key="XYZ"
 )
 
 client = get_bodo_client(keys)
-jobruns = client.job.list_batch_job_runs_by_names(batch_job_names=['production-job-1'], status=[JobRunStatus.FAILED], cluster_id=['ba62e653-312a-490e-9457-71d7bc096959'])
+jobruns = client.job.list_job_runs_by_batch_job_name(batch_job_names=['production-job-1'], statuses=[JobRunStatus.FAILED], cluster_ids=['ba62e653-312a-490e-9457-71d7bc096959'])
 ```
 
 <br/>
 
 #####  Get batch job run 
 
 
@@ -834,15 +836,15 @@
             sqlQueryText="SELECT * FROM PUBLIC.TABLE LIMIT 10"))
 ```
 
 <br/>
 
 ##### Job Run waiter<a id="job-waiter"></a>
 
-`BodoClient.job.get_waiter()`
+`BodoClient.job.get_job_run_waiter()`
 
 Returns a waiter object that waits until the job run uuid specified finishes.
 To wait for job run to be finished, invoke the waiter.wait() function,
 which can take the following parameters.
 
 ```python3
 from typing import Callable
```

### Comparing `bodosdk-1.3.3/bodosdk.egg-info/SOURCES.txt` & `bodosdk-1.3.4/bodosdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/setup.py` & `bodosdk-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.3/versioneer.py` & `bodosdk-1.3.4/versioneer.py`

 * *Files identical despite different names*

