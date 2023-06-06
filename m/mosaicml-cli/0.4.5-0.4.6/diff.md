# Comparing `tmp/mosaicml-cli-0.4.5.tar.gz` & `tmp/mosaicml-cli-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.5.tar", last modified: Wed May 31 00:46:57 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.6.tar", last modified: Tue Jun  6 23:19:16 2023, max compression
```

## Comparing `mosaicml-cli-0.4.5.tar` & `mosaicml-cli-0.4.6.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.685102 mosaicml-cli-0.4.5/
--rw-r--r--   0 wai        (502) staff       (20)      696 2023-05-31 00:46:57.684329 mosaicml-cli-0.4.5/PKG-INFO
--rw-r--r--   0 wai        (502) staff       (20)     7187 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/README.md
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.613771 mosaicml-cli-0.4.5/mcli/
--rw-r--r--   0 wai        (502) staff       (20)     2092 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.614497 mosaicml-cli-0.4.5/mcli/api/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.615218 mosaicml-cli-0.4.5/mcli/api/cluster/
--rw-r--r--   0 wai        (502) staff       (20)      134 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/cluster/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4237 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.615758 mosaicml-cli-0.4.5/mcli/api/engine/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/engine/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    25914 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/engine/engine.py
--rw-r--r--   0 wai        (502) staff       (20)    10685 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/exceptions.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.628369 mosaicml-cli-0.4.5/mcli/api/inference_deployments/
--rw-r--r--   0 wai        (502) staff       (20)     1521 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3301 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 wai        (502) staff       (20)     5105 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 wai        (502) staff       (20)     3603 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 wai        (502) staff       (20)     8458 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 wai        (502) staff       (20)     1277 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_ping.py
--rw-r--r--   0 wai        (502) staff       (20)     1603 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_predict_inference_deployment.py
--rw-r--r--   0 wai        (502) staff       (20)     6483 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_update_inference_deployments.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.628958 mosaicml-cli-0.4.5/mcli/api/mint/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-27 22:51:58.000000 mosaicml-cli-0.4.5/mcli/api/mint/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     7759 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/mint/shell.py
--rw-r--r--   0 wai        (502) staff       (20)     2676 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/mint/tty.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.629932 mosaicml-cli-0.4.5/mcli/api/model/
--rw-r--r--   0 wai        (502) staff       (20)     1114 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/model/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     6322 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/model/cluster_details.py
--rw-r--r--   0 wai        (502) staff       (20)     4611 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/model/inference_deployment.py
--rw-r--r--   0 wai        (502) staff       (20)    10439 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/model/run.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.632579 mosaicml-cli-0.4.5/mcli/api/runs/
--rw-r--r--   0 wai        (502) staff       (20)     1199 2023-05-30 21:28:48.000000 mosaicml-cli-0.4.5/mcli/api/runs/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2804 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_create_run.py
--rw-r--r--   0 wai        (502) staff       (20)     4211 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     8906 2023-05-30 23:51:22.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 wai        (502) staff       (20)    10933 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     5213 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_start_run.py
--rw-r--r--   0 wai        (502) staff       (20)     5405 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     3937 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 wai        (502) staff       (20)    10619 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.633205 mosaicml-cli-0.4.5/mcli/api/schema/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/schema/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      636 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.634190 mosaicml-cli-0.4.5/mcli/api/secrets/
--rw-r--r--   0 wai        (502) staff       (20)      309 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/secrets/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2386 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 wai        (502) staff       (20)     3019 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 wai        (502) staff       (20)     3718 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 wai        (502) staff       (20)     2354 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/typing_future.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.634785 mosaicml-cli-0.4.5/mcli/api/users/
--rw-r--r--   0 wai        (502) staff       (20)      139 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/api/users/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2715 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.635385 mosaicml-cli-0.4.5/mcli/cli/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/__init__.py
--rwxr-xr-x   0 wai        (502) staff       (20)     6387 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/cli.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.636113 mosaicml-cli-0.4.5/mcli/cli/common/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/common/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2461 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 wai        (502) staff       (20)     6874 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.636471 mosaicml-cli-0.4.5/mcli/cli/m_connect/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-27 22:51:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     1694 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.637186 mosaicml-cli-0.4.5/mcli/cli/m_create/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_create/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2385 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_create/m_create.py
--rw-r--r--   0 wai        (502) staff       (20)    16874 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.637827 mosaicml-cli-0.4.5/mcli/cli/m_delete/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     6184 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_delete/delete.py
--rw-r--r--   0 wai        (502) staff       (20)     5805 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.638107 mosaicml-cli-0.4.5/mcli/cli/m_deploy/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3896 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.639247 mosaicml-cli-0.4.5/mcli/cli/m_describe/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     3902 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 wai        (502) staff       (20)     9988 2023-05-30 23:51:22.000000 mosaicml-cli-0.4.5/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 wai        (502) staff       (20)     2002 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.640715 mosaicml-cli-0.4.5/mcli/cli/m_get/
--rw-r--r--   0 wai        (502) staff       (20)      467 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     6226 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/clusters.py
--rw-r--r--   0 wai        (502) staff       (20)     6447 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/display.py
--rw-r--r--   0 wai        (502) staff       (20)     5642 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 wai        (502) staff       (20)     4803 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/m_get.py
--rw-r--r--   0 wai        (502) staff       (20)     9790 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/runs.py
--rw-r--r--   0 wai        (502) staff       (20)     2189 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/secrets.py
--rw-r--r--   0 wai        (502) staff       (20)     1580 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_get/users.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.641076 mosaicml-cli-0.4.5/mcli/cli/m_init/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_init/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4115 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_init/m_init.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.641709 mosaicml-cli-0.4.5/mcli/cli/m_interactive/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     9325 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 wai        (502) staff       (20)    44284 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 wai        (502) staff       (20)     9321 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.642367 mosaicml-cli-0.4.5/mcli/cli/m_kube/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_kube/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     5523 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_kube/m_get_config.py
--rw-r--r--   0 wai        (502) staff       (20)     1398 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_kube/m_kube.py
--rw-r--r--   0 wai        (502) staff       (20)     2050 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_kube/m_merge_config.py
--rw-r--r--   0 wai        (502) staff       (20)     6946 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_kube/utils.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.642623 mosaicml-cli-0.4.5/mcli/cli/m_log/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_log/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)    10845 2023-05-30 23:51:22.000000 mosaicml-cli-0.4.5/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.643023 mosaicml-cli-0.4.5/mcli/cli/m_ping/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2091 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.643379 mosaicml-cli-0.4.5/mcli/cli/m_predict/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-04 20:22:39.000000 mosaicml-cli-0.4.5/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2610 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.643628 mosaicml-cli-0.4.5/mcli/cli/m_root/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_root/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      536 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.643904 mosaicml-cli-0.4.5/mcli/cli/m_run/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_run/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     8099 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.644938 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2973 2023-04-04 20:22:39.000000 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 wai        (502) staff       (20)     1802 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 wai        (502) staff       (20)     1940 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 wai        (502) staff       (20)     1421 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 wai        (502) staff       (20)      881 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.645305 mosaicml-cli-0.4.5/mcli/cli/m_stop/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     4047 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.645694 mosaicml-cli-0.4.5/mcli/cli/m_util/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/cli/m_util/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)      797 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_util/m_util.py
--rw-r--r--   0 wai        (502) staff       (20)     6837 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/cli/m_util/util.py
--rw-r--r--   0 wai        (502) staff       (20)    12590 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/config.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.646826 mosaicml-cli-0.4.5/mcli/models/
--rw-r--r--   0 wai        (502) staff       (20)     1047 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     2103 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/gpu_type.py
--rw-r--r--   0 wai        (502) staff       (20)    10321 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/inference_deployment_config.py
--rw-r--r--   0 wai        (502) staff       (20)      427 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/mcli_cluster.py
--rw-r--r--   0 wai        (502) staff       (20)      456 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/mcli_envvar.py
--rw-r--r--   0 wai        (502) staff       (20)     6724 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/mcli_secret.py
--rw-r--r--   0 wai        (502) staff       (20)    19547 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/models/run_config.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.646994 mosaicml-cli-0.4.5/mcli/objects/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/objects/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.648710 mosaicml-cli-0.4.5/mcli/objects/secrets/
--rw-r--r--   0 wai        (502) staff       (20)     1090 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.653650 mosaicml-cli-0.4.5/mcli/objects/secrets/create/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     1646 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/base.py
--rw-r--r--   0 wai        (502) staff       (20)     2244 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 wai        (502) staff       (20)     2408 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 wai        (502) staff       (20)     6377 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 wai        (502) staff       (20)     3858 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 wai        (502) staff       (20)     3001 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 wai        (502) staff       (20)     5342 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 wai        (502) staff       (20)      783 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 wai        (502) staff       (20)     1017 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/env_var.py
--rw-r--r--   0 wai        (502) staff       (20)      556 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/gcp.py
--rw-r--r--   0 wai        (502) staff       (20)     1267 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/mounted.py
--rw-r--r--   0 wai        (502) staff       (20)      967 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/oci.py
--rw-r--r--   0 wai        (502) staff       (20)      961 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/s3.py
--rw-r--r--   0 wai        (502) staff       (20)     1718 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.656141 mosaicml-cli-0.4.5/mcli/proto/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-04-18 23:46:04.000000 mosaicml-cli-0.4.5/mcli/proto/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     1477 2023-04-18 23:46:04.000000 mosaicml-cli-0.4.5/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.657277 mosaicml-cli-0.4.5/mcli/sdk/
--rw-r--r--   0 wai        (502) staff       (20)     1918 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/sdk/__init__.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.674046 mosaicml-cli-0.4.5/mcli/utils/
--rw-r--r--   0 wai        (502) staff       (20)        0 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/utils/__init__.py
--rw-r--r--   0 wai        (502) staff       (20)     5306 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/utils/utils_cli.py
--rw-r--r--   0 wai        (502) staff       (20)     6073 2023-04-18 16:53:02.000000 mosaicml-cli-0.4.5/mcli/utils/utils_config.py
--rw-r--r--   0 wai        (502) staff       (20)      740 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/utils/utils_date.py
--rw-r--r--   0 wai        (502) staff       (20)    10749 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_docker.py
--rw-r--r--   0 wai        (502) staff       (20)     2225 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_epilog.py
--rw-r--r--   0 wai        (502) staff       (20)    10774 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_interactive.py
--rw-r--r--   0 wai        (502) staff       (20)     4527 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_logging.py
--rw-r--r--   0 wai        (502) staff       (20)     2160 2023-04-20 18:58:30.000000 mosaicml-cli-0.4.5/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 wai        (502) staff       (20)     6614 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/utils/utils_pypi.py
--rw-r--r--   0 wai        (502) staff       (20)     3115 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/utils/utils_rich.py
--rw-r--r--   0 wai        (502) staff       (20)     5035 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_run_status.py
--rw-r--r--   0 wai        (502) staff       (20)     4350 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 wai        (502) staff       (20)     1103 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/mcli/utils/utils_spinner.py
--rw-r--r--   0 wai        (502) staff       (20)    10751 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_string_functions.py
--rw-r--r--   0 wai        (502) staff       (20)     1677 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/mcli/utils/utils_types.py
--rw-r--r--   0 wai        (502) staff       (20)     1001 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/mcli/utils/utils_yaml.py
--rw-r--r--   0 wai        (502) staff       (20)     3885 2023-05-30 23:51:33.000000 mosaicml-cli-0.4.5/mcli/version.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.680384 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/
--rw-r--r--   0 wai        (502) staff       (20)      696 2023-05-31 00:46:57.000000 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 wai        (502) staff       (20)     4868 2023-05-31 00:46:57.000000 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 wai        (502) staff       (20)        1 2023-05-31 00:46:57.000000 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 wai        (502) staff       (20)       75 2023-05-31 00:46:57.000000 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 wai        (502) staff       (20)     1655 2023-05-31 00:46:57.000000 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 wai        (502) staff       (20)        5 2023-05-31 00:46:57.000000 mosaicml-cli-0.4.5/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 wai        (502) staff       (20)    31087 2023-05-30 21:24:59.000000 mosaicml-cli-0.4.5/pyproject.toml
--rw-r--r--   0 wai        (502) staff       (20)       38 2023-05-31 00:46:57.685437 mosaicml-cli-0.4.5/setup.cfg
--rw-r--r--   0 wai        (502) staff       (20)     3057 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/setup.py
-drwxr-xr-x   0 wai        (502) staff       (20)        0 2023-05-31 00:46:57.682855 mosaicml-cli-0.4.5/tests/
--rw-r--r--   0 wai        (502) staff       (20)     5991 2023-05-30 21:28:58.000000 mosaicml-cli-0.4.5/tests/test_config.py
--rw-r--r--   0 wai        (502) staff       (20)       62 2023-02-02 22:40:35.000000 mosaicml-cli-0.4.5/tests/test_simple.py
--rw-r--r--   0 wai        (502) staff       (20)     6116 2023-03-21 22:39:53.000000 mosaicml-cli-0.4.5/tests/test_upgrade.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.337015 mosaicml-cli-0.4.6/
+-rw-r--r--   0 margaretqian   (501) staff       (20)      696 2023-06-06 23:19:16.336822 mosaicml-cli-0.4.6/PKG-INFO
+-rw-r--r--   0 margaretqian   (501) staff       (20)     7193 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/README.md
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.302299 mosaicml-cli-0.4.6/mcli/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2092 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/__init__.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.303186 mosaicml-cli-0.4.6/mcli/api/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/api/__init__.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.303864 mosaicml-cli-0.4.6/mcli/api/cluster/
+-rw-r--r--   0 margaretqian   (501) staff       (20)      134 2022-10-27 18:49:21.000000 mosaicml-cli-0.4.6/mcli/api/cluster/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4237 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.304325 mosaicml-cli-0.4.6/mcli/api/engine/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/api/engine/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    25914 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/engine/engine.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10685 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/exceptions.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.306545 mosaicml-cli-0.4.6/mcli/api/inference_deployments/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1521 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3297 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5105 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3603 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     8450 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2053 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_ping.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2356 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_predict_inference_deployment.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6483 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_update_inference_deployments.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.307054 mosaicml-cli-0.4.6/mcli/api/mint/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-03-06 23:35:18.000000 mosaicml-cli-0.4.6/mcli/api/mint/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     7759 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/mint/shell.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2676 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/mint/tty.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.307802 mosaicml-cli-0.4.6/mcli/api/model/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1114 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/model/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6322 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/model/cluster_details.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4583 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10439 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/model/run.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.310526 mosaicml-cli-0.4.6/mcli/api/runs/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1199 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.6/mcli/api/runs/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2804 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4211 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     8906 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10933 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5213 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5405 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3937 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10619 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.311020 mosaicml-cli-0.4.6/mcli/api/schema/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/api/schema/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      636 2022-08-23 17:34:43.000000 mosaicml-cli-0.4.6/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.312652 mosaicml-cli-0.4.6/mcli/api/secrets/
+-rw-r--r--   0 margaretqian   (501) staff       (20)      309 2022-09-22 23:36:49.000000 mosaicml-cli-0.4.6/mcli/api/secrets/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2386 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3019 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3718 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2354 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/api/typing_future.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.313308 mosaicml-cli-0.4.6/mcli/api/users/
+-rw-r--r--   0 margaretqian   (501) staff       (20)      139 2023-02-02 20:09:34.000000 mosaicml-cli-0.4.6/mcli/api/users/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2715 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/users/api_get_users.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.313599 mosaicml-cli-0.4.6/mcli/cli/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/__init__.py
+-rwxr-xr-x   0 margaretqian   (501) staff       (20)     6387 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/cli.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.314079 mosaicml-cli-0.4.6/mcli/cli/common/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-02-02 19:35:37.000000 mosaicml-cli-0.4.6/mcli/cli/common/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2560 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6922 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.314411 mosaicml-cli-0.4.6/mcli/cli/m_connect/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-03-06 23:35:18.000000 mosaicml-cli-0.4.6/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1935 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.6/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.315221 mosaicml-cli-0.4.6/mcli/cli/m_create/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2385 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    16900 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.315914 mosaicml-cli-0.4.6/mcli/cli/m_delete/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6448 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5805 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.316349 mosaicml-cli-0.4.6/mcli/cli/m_deploy/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4001 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.317349 mosaicml-cli-0.4.6/mcli/cli/m_describe/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-02-02 19:35:37.000000 mosaicml-cli-0.4.6/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3929 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     9988 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2002 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.319114 mosaicml-cli-0.4.6/mcli/cli/m_get/
+-rw-r--r--   0 margaretqian   (501) staff       (20)      467 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6226 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6447 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/display.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5669 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4803 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     9800 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/runs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2189 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1580 2023-02-02 20:09:34.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/users.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.319515 mosaicml-cli-0.4.6/mcli/cli/m_init/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4115 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.6/mcli/cli/m_init/m_init.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.320525 mosaicml-cli-0.4.6/mcli/cli/m_interactive/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10916 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.6/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    44284 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     9493 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.321369 mosaicml-cli-0.4.6/mcli/cli/m_kube/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_kube/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5523 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_kube/m_get_config.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1398 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_kube/m_kube.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2050 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_kube/m_merge_config.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6946 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_kube/utils.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.321685 mosaicml-cli-0.4.6/mcli/cli/m_log/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    11398 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.6/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.322103 mosaicml-cli-0.4.6/mcli/cli/m_ping/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1103 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.322409 mosaicml-cli-0.4.6/mcli/cli/m_predict/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1661 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.322714 mosaicml-cli-0.4.6/mcli/cli/m_root/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      536 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.323012 mosaicml-cli-0.4.6/mcli/cli/m_run/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     8267 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.324228 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-10-11 22:54:49.000000 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2973 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1802 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1940 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1421 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      881 2023-02-02 20:09:34.000000 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.324640 mosaicml-cli-0.4.6/mcli/cli/m_stop/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-09-27 16:43:54.000000 mosaicml-cli-0.4.6/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4066 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.325118 mosaicml-cli-0.4.6/mcli/cli/m_util/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-07-14 21:04:39.000000 mosaicml-cli-0.4.6/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      797 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6837 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_util/util.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    12876 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.6/mcli/config.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.326295 mosaicml-cli-0.4.6/mcli/models/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1047 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2103 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/gpu_type.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10317 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      427 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/mcli_cluster.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      456 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/mcli_envvar.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6724 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/mcli_secret.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    19547 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/run_config.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.326534 mosaicml-cli-0.4.6/mcli/objects/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/objects/__init__.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.328307 mosaicml-cli-0.4.6/mcli/objects/secrets/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1090 2022-12-07 22:00:09.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.330107 mosaicml-cli-0.4.6/mcli/objects/secrets/create/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1646 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2244 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2408 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6377 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3858 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3001 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5342 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      783 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1017 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      556 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1267 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      967 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/oci.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      961 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/s3.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1718 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.330567 mosaicml-cli-0.4.6/mcli/proto/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.6/mcli/proto/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1477 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.6/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.330957 mosaicml-cli-0.4.6/mcli/sdk/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1976 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/sdk/__init__.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.334695 mosaicml-cli-0.4.6/mcli/utils/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/utils/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5306 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/utils/utils_cli.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6073 2023-04-13 22:08:13.000000 mosaicml-cli-0.4.6/mcli/utils/utils_config.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      740 2022-09-27 16:43:54.000000 mosaicml-cli-0.4.6/mcli/utils/utils_date.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10749 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/utils/utils_docker.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2225 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/utils/utils_epilog.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10774 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/utils/utils_interactive.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4527 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/utils/utils_logging.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2160 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.6/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6614 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/utils/utils_pypi.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3115 2022-08-31 05:37:31.000000 mosaicml-cli-0.4.6/mcli/utils/utils_rich.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5033 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.6/mcli/utils/utils_run_status.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4350 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1103 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/utils/utils_spinner.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10751 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1677 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/utils/utils_types.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1001 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/utils/utils_yaml.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3885 2023-06-06 23:17:23.000000 mosaicml-cli-0.4.6/mcli/version.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.335603 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/
+-rw-r--r--   0 margaretqian   (501) staff       (20)      696 2023-06-06 23:19:16.000000 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4868 2023-06-06 23:19:16.000000 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 margaretqian   (501) staff       (20)        1 2023-06-06 23:19:16.000000 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 margaretqian   (501) staff       (20)       75 2023-06-06 23:19:16.000000 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1655 2023-06-06 23:19:16.000000 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 margaretqian   (501) staff       (20)        5 2023-06-06 23:19:16.000000 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 margaretqian   (501) staff       (20)    31087 2023-05-16 20:27:59.000000 mosaicml-cli-0.4.6/pyproject.toml
+-rw-r--r--   0 margaretqian   (501) staff       (20)       38 2023-06-06 23:19:16.337077 mosaicml-cli-0.4.6/setup.cfg
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3057 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/setup.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.336390 mosaicml-cli-0.4.6/tests/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5991 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/tests/test_config.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)       62 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/tests/test_simple.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6116 2023-04-11 21:00:01.000000 mosaicml-cli-0.4.6/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.5/PKG-INFO` & `mosaicml-cli-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.5
+Version: 0.4.6
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.5/README.md` & `mosaicml-cli-0.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 A few notes for later on:
 
 - To exit the virtual environment later on: `$ deactivate`
 - To get back into your virtual environment: `$ source venv/bin/activate`
 
 ## Running against mcloud as a developer
 
-There are currently 6 MCLI Modes. To use a mode other than the default `PROD`, set your local environment variable `MCLI_MODE` or specify the mode when you run MCLI commands (e.g. `MCLI_MODE=DEV mcli get runs`)
+There are currently several MCLI Modes. To use a mode other than the default `PROD`, set your local environment variable `MCLI_MODE` or specify the mode when you run MCLI commands (e.g. `MCLI_MODE=DEV mcli get runs`)
 
 | Mode       | Used By         | MAPI Endpoint                            | Use cases                                              | API Key                                                      |
 | ---------- | --------------- | ---------------------------------------- | ------------------------------------------------------ | ------------------------------------------------------------ |
 | `PROD`     | Default         | https://api.mosaicml.com/graphql         | Demos, simulating customer behavior, integration tests | Create one [here](https://console.mosaicml.com/account#)     |
 | `INTERNAL` | Internal users  | https://api.mosaicml.com/graphql         | Internal/alpha features in a prod environment          | Create one [here](https://console.mosaicml.com/account#)     |
 | `STAGING`  | Developers only | https://staging.api.mosaicml.com/graphql | Test changes queued for prod release                   | Testing api key                                              |
 | `DEV`      | Developers only | https://dev.api.mosaicml.com/graphql     | Test against dev branch of mcloud                      | Create one [here](https://dev.console.mosaicml.com/account#) |
```

### Comparing `mosaicml-cli-0.4.5/mcli/__init__.py` & `mosaicml-cli-0.4.6/mcli/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.6/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.6/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/exceptions.py` & `mosaicml-cli-0.4.6/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.6/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     timeout: Optional[float] = 10,
     future: bool = False,
 ) -> Union[InferenceDeployment, Future[InferenceDeployment]]:
     """Launch a inference deployment in the MosaicML platform
 
     The provided :class:`deploy <mcli.models.inference_deployment_config.InferenceDeploymentConfig>` must contain
     enough information to fully detail the inference deployment
-    
+
     Args:
         deployment: A fully-configured inference deployment to launch. The deployment will be queued and persisted
             in the deployment database.
         timeout: Time, in seconds, in which the call should complete. If the deployment creation
             takes too long, a TimeoutError will be raised. If ``future`` is ``True``, this
             value will be ignored.
         future: Return the output as a :type concurrent.futures.Future:. If True, the
```

### Comparing `mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     *,
     timeout: Optional[float] = 10,
     future: bool = False,
 ):
     """Gets a single inference deployment that has been launched in the MosaicML platform
 
     The returned object will contain all of the details stored about the requested deployment.
-    
+
     Arguments:
         deployment: Inference deployment object or name string
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised. If ``future`` is ``True``, this
             value will be ignored.
         future: Return the output as a :type concurrent.futures.Future:. If True, the
             call to `get_inference_deployment` will return immediately and the request will be
@@ -136,15 +136,15 @@
     statuses: Optional[List[str]] = None,
     timeout: Optional[float] = 10,
     future: bool = False,
 ):
     """List inference deployments that have been launched in the MosaicML platform
 
     The returned list will contain all of the details stored about the requested deployments.
-    
+
     Arguments:
         deployments: List of inference deployments on which to get information
         clusters: List of clusters to filter inference deployments. This can be a list of str or
             :type Cluster: objects. Only deployments submitted to these clusters will be
             returned.
         before: Only inference deployments created strictly before this time will be returned. This
             can be a str in ISO 8601 format(e.g 2023-03-31T12:23:04.34+05:30)
```

### Comparing `mosaicml-cli-0.4.5/mcli/api/inference_deployments/api_update_inference_deployments.py` & `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_update_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.6/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.6/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/model/__init__.py` & `mosaicml-cli-0.4.6/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.6/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.6/mcli/api/model/inference_deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from mcli.api.schema.generic_model import DeserializableModel, convert_datetime
 from mcli.models.inference_deployment_config import FinalInferenceDeploymentConfig, InferenceDeploymentConfig
 
 
 @dataclass
 class InferenceDeployment(DeserializableModel):
     """A deployment that has been launched on the MosaicML Cloud
-    
+
     Args:
         deployment_uid (`str`): Unique identifier for the deployment
         name (`str`): User-defined name of the deployment
         status (:class:`~mcli.utils.utils_deployment_status.DeploymentStatus`): Status of the deployment
         at a moment in time
         created_at (`datetime`): Date and time when the deployment was created
         updated_at (`datetime`): Date and time when the deployment was last updated
@@ -67,42 +67,42 @@
                    created_by=response['createdByEmail'],
                    config=FinalInferenceDeploymentConfig.from_mapi_response(response['inferenceDeploymentInput']),
                    submitted_config=submit_config)
 
     def refresh(self) -> "InferenceDeployment":
         """
         Refreshed the data on the deployment object
-        
+
         Returns:
             Refreshed :class:`~mcli.api.model.inference_deployment.InferenceDeployment` object
         """
         # pylint: disable-next=import-outside-toplevel
         from mcli.api.inference_deployments import get_inference_deployment
 
         return get_inference_deployment(self)
 
     def ping(self) -> dict:
         """
         Pings the deployment
-        
+
         Returns:
             Dictionary containing the status of the deployment
         """
         # pylint: disable-next=import-outside-toplevel
         from mcli.api.inference_deployments import ping
 
         return ping(self)
 
     def predict(self, inputs: Dict[str, Any]) -> dict:
         """
         Sends input to the deployment and runs prediction on the input
 
         Args:
             inputs: Input data to run prediction on in the form of dictionary
-        
+
         Returns:
             Dictionary containing the output produced by the model
         """
         # pylint: disable-next=import-outside-toplevel
         from mcli.api.inference_deployments import predict
 
         return predict(self, inputs)
```

### Comparing `mosaicml-cli-0.4.5/mcli/api/model/run.py` & `mosaicml-cli-0.4.6/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.6/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.6/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.6/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.6/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.6/mcli/api/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.4.6/mcli/api/runs/api_start_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.4.6/mcli/api/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.6/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.6/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.6/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.6/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.6/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.6/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/typing_future.py` & `mosaicml-cli-0.4.6/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.6/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/cli.py` & `mosaicml-cli-0.4.6/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.6/mcli/cli/common/deployment_filters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ MCLI Deployment Filters """
 import fnmatch
 import logging
 from typing import Dict, List, Optional
 
 from mcli.api.exceptions import MCLIException
+from mcli.api.inference_deployments.api_get_inference_deployments import get_inference_deployments
+from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.cli.common.run_filters import _split_glob_filters
-from mcli.sdk import InferenceDeployment, get_inference_deployments
 from mcli.utils.utils_spinner import console_status
 
 logger = logging.getLogger(__name__)
 
 
 def get_deployments_with_filters(
     name_filter: Optional[List[str]] = None,
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.6/mcli/cli/common/run_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import argparse
 import fnmatch
 import functools
 import logging
 from typing import Dict, List, Optional, Tuple
 
 from mcli.api.exceptions import MCLIException
-from mcli.sdk import Run, get_runs
+from mcli.api.model.run import Run
+from mcli.api.runs.api_get_runs import get_runs
 from mcli.utils.utils_cli import SubmissionType, comma_separated, date_time_parse
 from mcli.utils.utils_run_status import RunStatus
 from mcli.utils.utils_spinner import console_status
 from mcli.utils.utils_string_functions import is_glob
 
 logger = logging.getLogger(__name__)
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.6/mcli/cli/m_connect/m_connect.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,24 @@
         '-l',
         '--latest',
         action='store_true',
         dest='latest',
         default=False,
         help='Connect to the latest run',
     )
-    parser.add_argument(
+    command_grp = parser.add_mutually_exclusive_group()
+    command_grp.add_argument(
         '--command',
         help='The command to execute in the run. By default you will be dropped into a bash shell',
     )
+    command_grp.add_argument(
+        '--tmux',
+        action='store_true',
+        help='Use tmux as the entrypoint for your run so your session is robust to disconnects',
+    )
 
     parser.set_defaults(func=connect_entrypoint)
     return parser
 
 
 def add_connect_argparser(subparser: argparse._SubParsersAction,) -> argparse.ArgumentParser:
     """Adds the get parser to a subparser
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.6/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.4.6/mcli/cli/m_create/secret.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """ mcli create secret Entrypoint """
 import argparse
 import logging
 import textwrap
 from typing import Callable, Optional
 
 from mcli.api.exceptions import cli_error_handler
+from mcli.api.secrets.api_create_secret import create_secret
 from mcli.models import SecretType
 from mcli.objects.secrets.create.docker_registry import DockerSecretCreator
 from mcli.objects.secrets.create.gcp import GCPSecretCreator
 from mcli.objects.secrets.create.generic import EnvVarSecretCreator, FileSecretCreator
 from mcli.objects.secrets.create.oci import OCISecretCreator
 from mcli.objects.secrets.create.s3 import S3SecretCreator
 from mcli.objects.secrets.create.ssh import SSHSecretCreator
-from mcli.sdk import create_secret
 from mcli.utils.utils_interactive import input_disabled
 from mcli.utils.utils_logging import OK
 from mcli.utils.utils_spinner import console_status
 
 logger = logging.getLogger(__name__)
 
 CREATORS = {
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.4.6/mcli/cli/m_delete/delete.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """ Functions for deleting MCLI objects """
 import logging
 from typing import List, Optional
 
 from mcli.api.exceptions import cli_error_handler
+from mcli.api.inference_deployments.api_delete_inference_deployments import delete_inference_deployments
+from mcli.api.model.inference_deployment import InferenceDeployment
+from mcli.api.model.run import Run
+from mcli.api.runs.api_delete_runs import delete_runs
+from mcli.api.secrets.api_delete_secrets import delete_secrets
+from mcli.api.secrets.api_get_secrets import get_secrets
 from mcli.cli.common.deployment_filters import get_deployments_with_filters
 from mcli.cli.common.run_filters import get_runs_with_filters
-from mcli.sdk import InferenceDeployment, Run, delete_inference_deployments, delete_runs, delete_secrets, get_secrets
 from mcli.utils.utils_interactive import query_yes_no
 from mcli.utils.utils_logging import FAIL, INFO, OK, WARN, get_indented_list
 from mcli.utils.utils_run_status import RunStatus
 from mcli.utils.utils_spinner import console_status
 
 logger = logging.getLogger(__name__)
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.6/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.6/mcli/cli/m_deploy/m_deploy.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import argparse
 import logging
 import textwrap
 from http import HTTPStatus
 from typing import Optional
 
 from mcli.api.exceptions import MAPIException, MCLIDeploymentConfigValidationError
-from mcli.sdk import InferenceDeploymentConfig, create_inference_deployment
+from mcli.api.inference_deployments.api_create_inference_deployment import create_inference_deployment
+from mcli.models.inference_deployment_config import InferenceDeploymentConfig
 from mcli.utils.utils_logging import FAIL, OK
 
 logger = logging.getLogger(__name__)
 
 
 def print_help(**kwargs) -> int:
     del kwargs
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.6/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from enum import Enum
 from typing import Any, Dict, Generator, List, Optional, Tuple
 
 from rich.table import Table
 
 from mcli.api.exceptions import MAPIException
 from mcli.api.inference_deployments.api_get_inference_deployments import get_inference_deployment
+from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, create_vertical_display_table
-from mcli.sdk import InferenceDeployment
 from mcli.utils.utils_logging import FAIL, FormatString, format_string
 
 logger = logging.getLogger(__name__)
 
 
 class DescribeDeployMetadataColumns(Enum):
     NAME = 'name'
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.6/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.6/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.4.6/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.6/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.6/mcli/cli/m_get/inference_deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import argparse
 from dataclasses import dataclass
 from enum import Enum
 from typing import Dict, Generator, List, Optional
 
 from mcli import config
 from mcli.api.exceptions import cli_error_handler
+from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.cli.common.deployment_filters import get_deployments_with_filters
 from mcli.cli.common.run_filters import configure_submission_filter_argparser
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, format_timestamp
-from mcli.sdk import InferenceDeployment
 from mcli.utils.utils_cli import SubmissionType
 
 
 class InferenceDeploymentColumns(Enum):
     ID = 'id'
     NAME = 'name'
     USER = 'user'
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.4.6/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.6/mcli/cli/m_get/runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import math
 from dataclasses import dataclass
 from enum import Enum
 from typing import Dict, Generator, List, Optional, Tuple
 
 from mcli import config
 from mcli.api.exceptions import cli_error_handler
+from mcli.api.model.run import Run
 from mcli.cli.common.run_filters import configure_submission_filter_argparser, get_runs_with_filters
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, format_timestamp
-from mcli.sdk import Run
 from mcli.utils.utils_cli import comma_separated
 from mcli.utils.utils_logging import WARN
 from mcli.utils.utils_run_status import RunStatus
 
 DEFAULT_DISPLAY_LIMIT = 50
 
 logger = logging.getLogger(__name__)
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.4.6/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.6/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.6/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.6/mcli/cli/m_interactive/interactive.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 import argparse
 import logging
 from typing import Optional
 
 from mcli.api.cluster import get_clusters
 from mcli.api.exceptions import MintException
 from mcli.api.mint import shell
+from mcli.api.model.run import Run, RunConfig, RunStatus
+from mcli.api.runs.api_create_run import create_run
+from mcli.api.runs.api_get_runs import get_runs
 from mcli.api.runs.api_watch_run import EpilogSpinner as CloudEpilogSpinner
 from mcli.cli.m_get.display import format_timestamp
-from mcli.sdk import Run, RunConfig, RunStatus, create_run, get_runs
 from mcli.utils.utils_epilog import CommonLog
 from mcli.utils.utils_interactive import choose_one
 from mcli.utils.utils_logging import FAIL
 from mcli.utils.utils_types import get_hours_type
 
 logger = logging.getLogger(__name__)
 
@@ -53,14 +55,15 @@
     cluster: Optional[str] = None,
     gpu_type: Optional[str] = None,
     gpus: Optional[int] = None,
     hours: Optional[float] = None,
     image: str = 'mosaicml/pytorch',
     rank: int = 0,
     connect: bool = True,
+    command: Optional[str] = None,
     **kwargs,
 ) -> int:
     del kwargs
 
     if not cluster:
         clusters = get_clusters()
         if not clusters:
@@ -88,26 +91,27 @@
         return 1
 
     if not connect:
         return 0
 
     try:
         mint_shell = shell.MintShell(run.name, rank=rank)
-        mint_shell.connect()
+        mint_shell.connect(command=command)
     except MintException as e:
         logger.error(f'{FAIL} {e}')
         return 1
     return 0
 
 
 def connect_entrypoint(
     name: Optional[str] = None,
     rank: int = 0,
     latest: bool = False,
     command: Optional[str] = None,
+    tmux: Optional[bool] = None,
     **kwargs,
 ):
     del kwargs
 
     if name:
         runs = get_runs([name])
         if not runs:
@@ -145,33 +149,53 @@
                     formatter=get_name,
                 )
 
     ready = wait_for_run(run)
     if not ready:
         return 1
 
+    if tmux:
+        command = get_tmux_command()
+
     try:
         mint_shell = shell.MintShell(run.name, rank=rank)
         mint_shell.connect(command=command)
     except MintException as e:
         logger.error(f'{FAIL} {e}')
         return 1
     return 0
 
 
+def get_tmux_command() -> str:
+    # set the command to a tmux entrypoint
+    # Check if tmux already exists
+    # command -v tmux >/dev/null 2>&1: Check if tmux already exists
+    # apt update && apt install -yq tmux: If not, quietly install. Assumes debian-based systems with apt
+    install_command = 'command -v tmux >/dev/null 2>&1 || (apt update && apt install -yq tmux)'
+
+    # new-session: Create a session
+    # -A: Attach if one exists (for auto-reconnect)
+    # -s main: Name the session ("main") for clarity
+    # -D: Disconnect other clients (from previous connections)
+    session_command = 'tmux new-session -A -s main -D'
+    return f'/bin/bash -c "({install_command}) && {session_command}"'
+
+
 def interactive_entrypoint(
     name: Optional[str] = None,
     cluster: Optional[str] = None,
     gpu_type: Optional[str] = None,
     gpus: Optional[int] = None,
     hrs: Optional[float] = None,
     hours: Optional[float] = None,
     image: str = 'mosaicml/pytorch',
     connect: bool = True,
     rank: int = 0,
+    command: Optional[str] = None,
+    tmux: Optional[bool] = None,
     **kwargs,
 ) -> int:
     del kwargs
 
     # Hours can be specified as a positional argument (hrs) or named argument (hours)
     if hours and hrs:
         logger.error(f'{FAIL} The duration of your interactive session was specified twice. '
@@ -179,15 +203,29 @@
                      'See mcli interactive --help for more details.')
 
     hours = hrs or hours
     if hours is None:
         logger.error(f'{FAIL} Please specify the duration of your interactive session. '
                      'See mcli interactive --help for details.')
         return 1
-    return interactive(name, cluster, gpu_type, gpus, hours, image, rank, connect)
+
+    if tmux:
+        command = get_tmux_command()
+
+    return interactive(
+        name=name,
+        cluster=cluster,
+        gpu_type=gpu_type,
+        gpus=gpus,
+        hours=hours,
+        image=image,
+        rank=rank,
+        connect=connect,
+        command=command,
+    )
 
 
 # TODO: Move into mcli/cli/m_interactive/m_interactive.py once kube mcli deprecated
 def configure_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
 
     hrs_grp = parser.add_mutually_exclusive_group()
     hrs_grp.add_argument(
@@ -236,14 +274,25 @@
 
     parser.add_argument(
         '--image',
         default='mosaicml/pytorch',
         help='Docker image to use',
     )
 
+    command_grp = parser.add_mutually_exclusive_group()
+    command_grp.add_argument(
+        '--command',
+        help='The command you\'d like to execute on entry into your run. Defaults to /bin/bash',
+    )
+    command_grp.add_argument(
+        '--tmux',
+        action='store_true',
+        help='Use tmux as the entrypoint for your run so your session is robust to disconnects',
+    )
+
     parser.add_argument(
         '--no-connect',
         dest='connect',
         action='store_false',
         help='Do not connect to the interactive session immediately',
     )
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_interactive/kube_config.py` & `mosaicml-cli-0.4.6/mcli/cli/m_interactive/kube_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.4.6/mcli/cli/m_interactive/m_interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """ mcli interactive Entrypoint """
 import argparse
 import logging
 import shlex
 import subprocess
 from typing import Optional
 
+from mcli.api.cluster.api_get_clusters import get_clusters
 from mcli.api.exceptions import cli_error_handler
+from mcli.api.model.run import RunConfig, RunStatus
+from mcli.api.runs.api_create_run import create_run
+from mcli.api.runs.api_get_runs import get_run
+from mcli.api.runs.api_watch_run import wait_for_run_status
 from mcli.cli.m_interactive import kube_config
 from mcli.config import MCLIConfig
-from mcli.sdk import RunConfig, RunStatus, create_run, get_clusters, get_run, wait_for_run_status
 from mcli.utils.utils_interactive import simple_prompt
 from mcli.utils.utils_logging import FAIL, INFO, OK, WARN
 from mcli.utils.utils_types import get_hours_type
 
 logger = logging.getLogger(__name__)
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_kube/m_get_config.py` & `mosaicml-cli-0.4.6/mcli/cli/m_kube/m_get_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_kube/m_kube.py` & `mosaicml-cli-0.4.6/mcli/cli/m_kube/m_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_kube/m_merge_config.py` & `mosaicml-cli-0.4.6/mcli/cli/m_kube/m_merge_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_kube/utils.py` & `mosaicml-cli-0.4.6/mcli/cli/m_kube/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.4.6/mcli/cli/m_log/m_log.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 import os
 import sys
 from functools import partial
 from http import HTTPStatus
 from typing import List, Optional, Tuple, Union
 
 from mcli.api.exceptions import MAPIException
+from mcli.api.inference_deployments.api_get_inference_deployment_logs import get_inference_deployment_logs
 from mcli.api.model.inference_deployment import InferenceDeployment
+from mcli.api.model.run import Run
+from mcli.api.runs.api_get_run_logs import follow_run_logs, get_run_logs
 from mcli.api.runs.api_watch_run import EpilogSpinner as CloudEpilogSpinner
 from mcli.cli.common.deployment_filters import get_deployments_with_filters
 from mcli.cli.common.run_filters import get_runs_with_filters
 from mcli.config import MESSAGE, MCLIConfigError
-from mcli.sdk import Run, follow_run_logs, get_inference_deployment_logs, get_run_logs
 from mcli.utils.utils_cli import SubmissionType
 from mcli.utils.utils_epilog import CommonLog
 from mcli.utils.utils_logging import FAIL, INFO, err_console
 from mcli.utils.utils_run_status import RunStatus
 
 logger = logging.getLogger(__name__)
 
@@ -63,15 +65,22 @@
 """
 
 
 def _get_run_logs(run: Run, follow: bool, rank: Optional[int], failed: bool,
                   attempt: Optional[int]) -> Tuple[Optional[str], int]:
 
     if run.status == RunStatus.FAILED and not failed and rank is None:
-        logger.info(f'{INFO} Run {run.name} has failed. Defaulting to show the first failed node rank.')
+        if run.reason and run.reason == "FailedImagePull":
+            suggestion = 'Try `mcli describe run {run.name}` and double-check that your image name is correct.'
+            logger.info(
+                f'{INFO} Run {run.name} has failed during image pull, so there are likely no logs. {suggestion}')
+        else:
+            err_message = f'({run.reason})' if run.reason else ''
+            logger.info(
+                f'{INFO} Run {run.name} has failed. {err_message} Defaulting to show the first failed node rank.')
         failed = True
 
     if follow and run.status.before(RunStatus.RUNNING):
         with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
             run = watcher.follow()
 
     if run.status == RunStatus.FAILED_PULL:
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_ping.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,51 @@
-""" mcli ping entrypoint """
-import argparse
-import logging
-from typing import Callable, Union, cast
+""" Ping a InferenceDeployment """
+from __future__ import annotations
 
+from http import HTTPStatus
+from typing import Callable, Optional, Union, cast
+
+import requests
 import validators
+from requests import Response
 
 from mcli.api.exceptions import MAPIException
-from mcli.api.inference_deployments import ping as api_ping
+from mcli.api.inference_deployments import get_inference_deployments
 from mcli.api.model.inference_deployment import InferenceDeployment
-from mcli.cli.common.deployment_filters import get_deployments_with_filters
-from mcli.utils.utils_logging import FAIL, err_console
 
-logger = logging.getLogger(__name__)
+__all__ = ['ping']
 
 
 def ping(
-    deployment: str,
-    **kwargs,
-) -> int:
-    del kwargs
-    try:
-        deployment_obj_or_url: Union[InferenceDeployment, str] = deployment
-        validate_url = cast(Callable[[str], bool], validators.url)
-        if not deployment_obj_or_url or not validate_url(deployment):
-            # if a url is not passed in then lookup the deployment and get the name
-            deployment_objs = get_deployments_with_filters(name_filter=[deployment])
-            if len(deployment_objs) == 0:
-
-                if not deployment:
-                    err_console.print("No inference deployments found.")
-                else:
-                    err_console.log(f'No inference deployment found with name {deployment}.')
-                return 1
-
-            deployment_obj_or_url = deployment_objs[0]
-
-        resp = api_ping(deployment_obj_or_url)
-        name_or_url = deployment_obj_or_url if isinstance(deployment_obj_or_url, str) else deployment_obj_or_url.name
-        print(f'{name_or_url}\'s status: {resp.get("status", resp)}')
-        return 0
-    except RuntimeError as e:
-        logger.error(f'{FAIL} {e}')
-        return 1
-    except MAPIException as e:
-        logger.error(f'{FAIL} {e}')
-        return 1
-
-
-def add_ping_parser(subparser: argparse._SubParsersAction):
-    ping_parser: argparse.ArgumentParser = subparser.add_parser(
-        'ping',
-        help='Ping a inference deployment in the MosaicML platform for health metrics',
-    )
-    ping_parser.add_argument('deployment', metavar='DEPLOYMENT', help='The name or url of the inference deployment.')
-
-    ping_parser.set_defaults(func=ping)
+    deployment: Union[InferenceDeployment, str],
+    *,
+    timeout: Optional[float] = 10,
+) -> dict:
+    """Pings an inference deployment that has been launched in the MosaicML platform
+    and returns the status of the deployment. The deployment must have a '/ping' endpoint
+    defined.
+    Arguments:
+        deployment: The deployment to check the status of. Can be a InferenceDeployment object,
+        the name of an deployment, or a string which is of the form https://<deployment dns>.
+        timeout: Time, in seconds, in which the call should complete. If the call
+            takes too long, a TimeoutError will be raised.
+    Raises:
+        HTTPError: If pinging the endpoint fails
+        MAPIException: If connecting to MAPI, raised when a MAPI communication error occurs
+    """
+    validate_url = cast(Callable[[str], bool], validators.url)
+    if isinstance(deployment, str) and not validate_url(deployment):
+        # if a string is passed in that is not a url then lookup the deployment and get the name
+        deployment_objs = get_inference_deployments(deployments=[deployment])
+        if len(deployment_objs) == 0:
+            raise MAPIException(HTTPStatus.NOT_FOUND, f'No inference deployment found with name {deployment}.')
+        deployment = deployment_objs[0]
+    base_url = deployment
+    if isinstance(deployment, InferenceDeployment):
+        base_url = f'https://{deployment.public_dns}'
+    resp: Response = requests.get(url=f'{base_url}/ping', timeout=timeout)
+
+    if resp.ok:
+        return {"status": resp.status_code}
+    else:
+        resp.raise_for_status()
+        return {}
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.4.6/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.4.6/mcli/cli/m_run/m_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 import argparse
 import logging
 import textwrap
 from http import HTTPStatus
 from typing import Optional
 
 from mcli.api.exceptions import MAPIException, cli_error_handler
+from mcli.api.model.run import Run, RunConfig
 from mcli.api.runs import create_run, delete_runs
+from mcli.api.runs.api_get_run_logs import follow_run_logs
+from mcli.api.runs.api_get_runs import get_run
+from mcli.api.runs.api_start_run import start_run
 from mcli.api.runs.api_watch_run import EpilogSpinner as CloudEpilogSpinner
+from mcli.api.runs.api_watch_run import wait_for_run_status
 from mcli.config import MCLIConfig
 from mcli.models.run_config import VALID_OPTIMIZATION_LEVELS
-from mcli.sdk import Run, RunConfig, follow_run_logs, get_run, start_run, wait_for_run_status
 from mcli.utils.utils_epilog import CommonLog
 from mcli.utils.utils_logging import INFO, OK
 from mcli.utils.utils_run_status import RunStatus
 from mcli.utils.utils_spinner import console_status
 
 logger = logging.getLogger(__name__)
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.6/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.4.6/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.4.6/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.6/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.6/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.6/mcli/cli/m_stop/m_stop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ mcli stop Entrypoint """
 import argparse
 import logging
 from typing import List, Optional
 
 from mcli.api.exceptions import cli_error_handler
+from mcli.api.runs.api_stop_runs import stop_runs
 from mcli.cli.common.run_filters import configure_submission_filter_argparser, get_runs_with_filters
 from mcli.cli.m_delete.delete import confirm_run_update
-from mcli.sdk import stop_runs
 from mcli.utils.utils_logging import FAIL, OK, WARN
 from mcli.utils.utils_run_status import RunStatus
 from mcli.utils.utils_spinner import console_status
 
 logger = logging.getLogger(__name__)
```

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.4.6/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.6/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/config.py` & `mosaicml-cli-0.4.6/mcli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,14 +363,20 @@
             feature (FeatureFlag): The feature to check
         """
 
         if not self.internal and feature not in FeatureFlag.get_external_features():
             # Only enable select features for external use
             return False
 
+        # Force internal users onto mint, but give them the option to disable it
+        if self.internal and feature == FeatureFlag.MCLOUD_INTERACTIVE:
+            if os.environ.get('MCLI_DISABLE_MINT', 'false').lower() == 'true':
+                return False
+            return True
+
         if feature.value in self.feature_flags:
             enabled = self.feature_flags.get(feature.value, False)
             return bool(enabled)
 
         return False
 
     def __str__(self) -> str:
```

### Comparing `mosaicml-cli-0.4.5/mcli/models/__init__.py` & `mosaicml-cli-0.4.6/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/models/gpu_type.py` & `mosaicml-cli-0.4.6/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.6/mcli/models/inference_deployment_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
 
 @dataclass
 class InferenceDeploymentConfig(BaseSubmissionConfig):
     """A deployment configuration for the MosaicML Cloud
 
     Values in here are not yet validated and some required values may be missing.
-    
+
     Args:
         name (`Optional[str]`): User-defined name of the deployment
         gpu_type (`Optional[str]`): GPU type (optional if only one gpu type for your cluster)
         gpu_num (`Optional[int]`): Number of GPUs
         cluster (`Optional[str]`): Cluster to use (optional if you only have one)
         image (`Optional[str]`): Docker image (e.g. `mosaicml/composer`)
         command (`str`): Command to use when a deployment starts
```

### Comparing `mosaicml-cli-0.4.5/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.6/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/models/run_config.py` & `mosaicml-cli-0.4.6/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.4.6/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.6/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/sdk/__init__.py` & `mosaicml-cli-0.4.6/mcli/sdk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Primary import target for the Python API"""
 
 from mcli.api.cluster import get_clusters
 from mcli.api.exceptions import MAPIException
 from mcli.api.inference_deployments import (InferenceDeployment, InferenceDeploymentConfig, create_inference_deployment,
-                                            delete_inference_deployments, get_inference_deployment_logs,
-                                            get_inference_deployments, ping, predict, update_inference_deployment,
-                                            update_inference_deployments)
+                                            delete_inference_deployments, get_inference_deployment,
+                                            get_inference_deployment_logs, get_inference_deployments, ping, predict,
+                                            update_inference_deployment, update_inference_deployments)
 from mcli.api.runs import (FinalRunConfig, Run, RunConfig, RunStatus, create_run, delete_run, delete_runs,
                            follow_run_logs, get_run, get_run_logs, get_runs, start_run, start_runs, stop_run, stop_runs,
                            update_run_metadata, wait_for_run_status, watch_run_status)
 from mcli.api.secrets import create_secret, delete_secrets, get_secrets
 from mcli.cli.m_init.m_init import initialize
 from mcli.cli.m_set_unset.api_key import set_api_key
 from mcli.config import FeatureFlag, MCLIConfig
@@ -19,14 +19,15 @@
     'MAPIException',
     'InferenceDeployment',
     'InferenceDeploymentConfig',
     'create_inference_deployment',
     'delete_inference_deployments',
     'get_inference_deployment_logs',
     'get_inference_deployments',
+    'get_inference_deployment',
     'ping',
     'predict',
     'FinalRunConfig',
     'Run',
     'RunConfig',
     'RunStatus',
     'create_run',
```

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_run_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,17 +121,17 @@
             other: Another :class:`~mcli.utils.utils_run_status.RunStatus`
             inclusive: If True, equality evaluates to True. Default False.
 
         Returns:
             If this state is "after" the other
 
         Example:
-            >>> RunStatus.RUNNING.before(RunStatus.COMPLETED)
+            >>> RunStatus.COMPLETED.after(RunStatus.RUNNING)
             True
-            >>> RunStatus.PENDING.before(RunStatus.RUNNING)
+            >>> RunStatus.RUNNING.after(RunStatus.PENDING)
             True
         """
         return (self > other) or (inclusive and self == other)
 
     @classmethod
     def from_string(cls, run_status: Union[str, RunStatus]) -> RunStatus:
         """Convert a string to a valid RunStatus Enum
```

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_types.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.6/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mcli/version.py` & `mosaicml-cli-0.4.6/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = '0.4.5'
+__version__ = '0.4.6'
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.5/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.6/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.5
+Version: 0.4.6
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.5/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.4.6/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.6/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -9,47 +9,47 @@
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 validators>=0.20.0
 
 [all]
-build>=0.10.0
+sphinxcontrib-serializinghtml==1.1.5
+myst-parser>=0.16.1
+sphinxemoji==0.2.0
+sphinx-copybutton==0.5.2
+sphinx_external_toc==0.3.0
+pytest-cov>=4.0.0
+sphinx==4.4.0
 radon>=5.1.0
 yapf>=0.33.0
-toml>=0.10.2
-sphinx-argparse==0.4.0
 sphinx-markdown-tables==0.0.17
-sphinx-design
-pre-commit>=2.17.0
-isort>=5.9.3
-pylint>=2.12.2
-sphinx==4.4.0
-pytest>=6.2.5
-sphinxcontrib-serializinghtml==1.1.5
-sphinxemoji==0.2.0
-sphinxcontrib-jsmath>=1.0.1
 twine>=4.0.2
-sphinx-panels==0.6.0
+pre-commit>=2.17.0
+sphinxcontrib-devhelp>=1.0.2
+sphinxcontrib-katex==0.9.4
+sphinxext-opengraph==0.8.2
+sphinx-argparse==0.4.0
 furo==2022.9.29
-pytest-cov>=4.0.0
+docutils>=0.17.0
+sphinx-design
 sphinxcontrib-applehelp>=1.0.2
-sphinxext-opengraph==0.8.2
-sphinxcontrib-katex==0.9.4
-sphinxcontrib-qthelp>=1.0.3
-myst-parser>=0.16.1
-sphinx-copybutton==0.5.2
-pyright>=1.1.256
 sphinxcontrib-htmlhelp>=2.0.0
-sphinxcontrib-images>=0.9.4
-sphinxcontrib-devhelp>=1.0.2
-sphinx-rtd-theme==1.0.0
-docutils>=0.17.0
-sphinx_external_toc==0.3.0
+toml>=0.10.2
+pylint>=2.12.2
 pytest-mock>=3.7.0
+pyright>=1.1.256
+sphinx-rtd-theme==1.0.0
+sphinxcontrib-images>=0.9.4
+build>=0.10.0
+pytest>=6.2.5
+isort>=5.9.3
+sphinx-panels==0.6.0
+sphinxcontrib-qthelp>=1.0.3
+sphinxcontrib-jsmath>=1.0.1
 
 [dev]
 build>=0.10.0
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright>=1.1.256
```

### Comparing `mosaicml-cli-0.4.5/pyproject.toml` & `mosaicml-cli-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/setup.py` & `mosaicml-cli-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/tests/test_config.py` & `mosaicml-cli-0.4.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.5/tests/test_upgrade.py` & `mosaicml-cli-0.4.6/tests/test_upgrade.py`

 * *Files identical despite different names*

