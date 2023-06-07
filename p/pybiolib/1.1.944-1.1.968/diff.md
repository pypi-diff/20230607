# Comparing `tmp/pybiolib-1.1.944.tar.gz` & `tmp/pybiolib-1.1.968.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybiolib-1.1.944.tar", max compression
+gzip compressed data, was "pybiolib-1.1.968.tar", max compression
```

## Comparing `pybiolib-1.1.944.tar` & `pybiolib-1.1.968.tar`

### file list

```diff
@@ -1,110 +1,111 @@
--rw-r--r--   0        0        0     1067 2023-06-05 12:44:22.417800 pybiolib-1.1.944/LICENSE
--rw-r--r--   0        0        0      368 2023-06-05 12:44:22.417800 pybiolib-1.1.944/README.md
--rw-r--r--   0        0        0     3337 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/__init__.py
--rw-r--r--   0        0        0       95 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/api/__init__.py
--rw-r--r--   0        0        0     3744 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/api/client.py
--rw-r--r--   0        0        0       37 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/app/__init__.py
--rw-r--r--   0        0        0     7652 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/app/app.py
--rw-r--r--   0        0        0     1493 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/app/search_apps.py
--rw-r--r--   0        0        0     4405 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/app/utils.py
--rw-r--r--   0        0        0      182 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/__init__.py
--rw-r--r--   0        0        0     5574 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/api_client.py
--rw-r--r--   0        0        0     2397 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/app_types.py
--rw-r--r--   0        0        0     1668 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/auth.py
--rw-r--r--   0        0        0      580 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/biolib_account_api.py
--rw-r--r--   0        0        0     2859 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/biolib_app_api.py
--rw-r--r--   0        0        0     9865 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/biolib_job_api.py
--rw-r--r--   0        0        0     1777 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/biolib_large_file_system_api.py
--rw-r--r--   0        0        0      123 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/common_types.py
--rw-r--r--   0        0        0     1256 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/job_types.py
--rw-r--r--   0        0        0      227 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/lfs_types.py
--rw-r--r--   0        0        0      637 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/user_state.py
--rw-r--r--   0        0        0      303 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/__init__.py
--rw-r--r--   0        0        0      959 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/base_bbf_package.py
--rw-r--r--   0        0        0      154 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/common_types.py
--rw-r--r--   0        0        0     6450 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/encrypted_module_output.py
--rw-r--r--   0        0        0     2603 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/module_input.py
--rw-r--r--   0        0        0     2640 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/module_output.py
--rw-r--r--   0        0        0     2269 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/rsa_encrypted_aes_package.py
--rw-r--r--   0        0        0     1125 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/saved_job.py
--rw-r--r--   0        0        0     1023 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/stdout_and_stderr.py
--rw-r--r--   0        0        0      853 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/system_exception.py
--rw-r--r--   0        0        0     1191 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/system_status_update.py
--rw-r--r--   0        0        0     8514 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/unencrypted_module_output.py
--rw-r--r--   0        0        0     3938 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/utils.py
--rw-r--r--   0        0        0     1481 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_docker_client/__init__.py
--rw-r--r--   0        0        0      532 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_errors.py
--rw-r--r--   0        0        0     2854 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_logging.py
--rw-r--r--   0        0        0    10225 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_push.py
--rw-r--r--   0        0        0      947 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/__init__.py
--rw-r--r--   0        0        0      820 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/init.py
--rw-r--r--   0        0        0     1966 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/lfs.py
--rw-r--r--   0        0        0      798 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/push.py
--rw-r--r--   0        0        0     1309 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/run.py
--rw-r--r--   0        0        0      361 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/runtime.py
--rw-r--r--   0        0        0     1284 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/start.py
--rw-r--r--   0        0        0     8947 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli_utils.py
--rw-r--r--   0        0        0       45 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/.gitignore
--rw-r--r--   0        0        0        0 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/__init__.py
--rw-r--r--   0        0        0       67 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/cloud_utils/__init__.py
--rw-r--r--   0        0        0     6878 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/cloud_utils/cloud_utils.py
--rw-r--r--   0        0        0       71 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/__init__.py
--rw-r--r--   0        0        0     3670 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/cache_state.py
--rw-r--r--   0        0        0      891 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/cache_types.py
--rw-r--r--   0        0        0     7562 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/docker_image_cache.py
--rw-r--r--   0        0        0      221 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/__init__.py
--rw-r--r--   0        0        0      448 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/base_executor.py
--rw-r--r--   0        0        0    24367 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/docker_executor.py
--rw-r--r--   0        0        0      122 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/docker_types.py
--rw-r--r--   0        0        0       91 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/remote/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/remote/remote_executor.py
--rw-r--r--   0        0        0        0 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/tars/__init__.py
--rw-r--r--   0        0        0     1564 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/types.py
--rw-r--r--   0        0        0     1198 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py
--rw-r--r--   0        0        0     1174 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py
--rw-r--r--   0        0        0     4858 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/job_storage.py
--rw-r--r--   0        0        0    30595 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/job_worker.py
--rw-r--r--   0        0        0     9363 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/large_file_system.py
--rw-r--r--   0        0        0     2499 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/mappings.py
--rw-r--r--   0        0        0     1282 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/utils.py
--rw-r--r--   0        0        0    12865 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/remote_host_proxy.py
--rw-r--r--   0        0        0     1601 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/socker_listener_thread.py
--rw-r--r--   0        0        0      971 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/socket_sender_thread.py
--rw-r--r--   0        0        0     4529 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/utils.py
--rw-r--r--   0        0        0        0 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/webserver/__init__.py
--rw-r--r--   0        0        0      914 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/compute_node/webserver/gunicorn_flask_application.py
--rw-r--r--   0        0        0     7647 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/compute_node/webserver/webserver.py
--rw-r--r--   0        0        0      420 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/compute_node/webserver/webserver_types.py
--rw-r--r--   0        0        0     4234 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/compute_node/webserver/webserver_utils.py
--rw-r--r--   0        0        0     9900 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/compute_node/webserver/worker_thread.py
--rw-r--r--   0        0        0        0 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/experiments/__init__.py
--rw-r--r--   0        0        0     5939 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/experiments/experiment.py
--rw-r--r--   0        0        0      171 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/experiments/types.py
--rw-r--r--   0        0        0       32 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/jobs/__init__.py
--rw-r--r--   0        0        0    14468 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/jobs/job.py
--rw-r--r--   0        0        0     5937 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/jobs/job_result.py
--rw-r--r--   0        0        0      905 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/jobs/types.py
--rw-r--r--   0        0        0      193 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/lfs/__init__.py
--rw-r--r--   0        0        0     2226 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/lfs/cache.py
--rw-r--r--   0        0        0     9832 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/lfs/utils.py
--rw-r--r--   0        0        0       44 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/runtime/__init__.py
--rw-r--r--   0        0        0      778 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/runtime/results.py
--rw-r--r--   0        0        0      210 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/start_cli.py
--rw-r--r--   0        0        0      872 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/tables.py
--rw-r--r--   0        0        0       36 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/templates/__init__.py
--rw-r--r--   0        0        0      715 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/templates/example_app.py
--rw-r--r--   0        0        0      263 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/typing_utils.py
--rw-r--r--   0        0        0       39 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/user/__init__.py
--rw-r--r--   0        0        0     2061 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/user/sign_in.py
--rw-r--r--   0        0        0     8190 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/utils/__init__.py
--rw-r--r--   0        0        0     2727 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/utils/cache_state.py
--rw-r--r--   0        0        0     9717 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/utils/multipart_uploader.py
--rw-r--r--   0        0        0     1757 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/utils/seq_util.py
--rw-r--r--   0        0        0    23500 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/utils/zip/remote_zip.py
--rw-r--r--   0        0        0     6916 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/validators/validate_app_version.py
--rw-r--r--   0        0        0     4300 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/validators/validate_argument.py
--rw-r--r--   0        0        0    13298 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/validators/validate_module.py
--rw-r--r--   0        0        0     1655 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/validators/validate_zip_file.py
--rw-r--r--   0        0        0     2135 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/validators/validator_utils.py
--rw-r--r--   0        0        0     1237 2023-06-05 12:45:11.918897 pybiolib-1.1.944/pyproject.toml
--rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 pybiolib-1.1.944/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-07 07:37:15.891199 pybiolib-1.1.968/LICENSE
+-rw-r--r--   0        0        0      368 2023-06-07 07:37:15.891199 pybiolib-1.1.968/README.md
+-rw-r--r--   0        0        0     3337 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/__init__.py
+-rw-r--r--   0        0        0       95 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/api/__init__.py
+-rw-r--r--   0        0        0     3744 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/api/client.py
+-rw-r--r--   0        0        0       37 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/app/__init__.py
+-rw-r--r--   0        0        0     7652 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/app/app.py
+-rw-r--r--   0        0        0     1493 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/app/search_apps.py
+-rw-r--r--   0        0        0     4405 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/app/utils.py
+-rw-r--r--   0        0        0      182 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/__init__.py
+-rw-r--r--   0        0        0     5574 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/api_client.py
+-rw-r--r--   0        0        0     2397 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/app_types.py
+-rw-r--r--   0        0        0     1668 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/auth.py
+-rw-r--r--   0        0        0      580 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/biolib_account_api.py
+-rw-r--r--   0        0        0     2859 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/biolib_app_api.py
+-rw-r--r--   0        0        0    10891 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/biolib_job_api.py
+-rw-r--r--   0        0        0     1777 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/biolib_large_file_system_api.py
+-rw-r--r--   0        0        0      123 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/common_types.py
+-rw-r--r--   0        0        0     1256 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/job_types.py
+-rw-r--r--   0        0        0      227 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/lfs_types.py
+-rw-r--r--   0        0        0      637 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/user_state.py
+-rw-r--r--   0        0        0      303 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/__init__.py
+-rw-r--r--   0        0        0      959 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/base_bbf_package.py
+-rw-r--r--   0        0        0      154 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/common_types.py
+-rw-r--r--   0        0        0     6450 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/encrypted_module_output.py
+-rw-r--r--   0        0        0     2603 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/module_input.py
+-rw-r--r--   0        0        0     2640 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/module_output.py
+-rw-r--r--   0        0        0     1146 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/remote_endpoints.py
+-rw-r--r--   0        0        0     2269 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/rsa_encrypted_aes_package.py
+-rw-r--r--   0        0        0     1125 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/saved_job.py
+-rw-r--r--   0        0        0     1023 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/stdout_and_stderr.py
+-rw-r--r--   0        0        0      853 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/system_exception.py
+-rw-r--r--   0        0        0     1191 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/system_status_update.py
+-rw-r--r--   0        0        0     8514 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/unencrypted_module_output.py
+-rw-r--r--   0        0        0     4101 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/utils.py
+-rw-r--r--   0        0        0     1481 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_docker_client/__init__.py
+-rw-r--r--   0        0        0      689 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_errors.py
+-rw-r--r--   0        0        0     2854 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_logging.py
+-rw-r--r--   0        0        0    10225 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_push.py
+-rw-r--r--   0        0        0      947 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/__init__.py
+-rw-r--r--   0        0        0      820 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/init.py
+-rw-r--r--   0        0        0     1966 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/lfs.py
+-rw-r--r--   0        0        0      798 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/push.py
+-rw-r--r--   0        0        0     1309 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/run.py
+-rw-r--r--   0        0        0      361 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/runtime.py
+-rw-r--r--   0        0        0     1284 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/start.py
+-rw-r--r--   0        0        0     8947 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli_utils.py
+-rw-r--r--   0        0        0       45 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/cloud_utils/__init__.py
+-rw-r--r--   0        0        0     6878 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/cloud_utils/cloud_utils.py
+-rw-r--r--   0        0        0       71 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/__init__.py
+-rw-r--r--   0        0        0     3670 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/cache_state.py
+-rw-r--r--   0        0        0      891 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/cache_types.py
+-rw-r--r--   0        0        0     7562 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/docker_image_cache.py
+-rw-r--r--   0        0        0      221 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/__init__.py
+-rw-r--r--   0        0        0      448 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/base_executor.py
+-rw-r--r--   0        0        0    24367 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/docker_executor.py
+-rw-r--r--   0        0        0      122 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/docker_types.py
+-rw-r--r--   0        0        0       91 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/remote/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/remote/remote_executor.py
+-rw-r--r--   0        0        0        0 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/tars/__init__.py
+-rw-r--r--   0        0        0     1564 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/types.py
+-rw-r--r--   0        0        0     1198 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py
+-rw-r--r--   0        0        0     1174 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py
+-rw-r--r--   0        0        0     4910 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/job_storage.py
+-rw-r--r--   0        0        0    30595 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/job_worker/job_worker.py
+-rw-r--r--   0        0        0     9363 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/job_worker/large_file_system.py
+-rw-r--r--   0        0        0     2499 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/job_worker/mappings.py
+-rw-r--r--   0        0        0     1282 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/job_worker/utils.py
+-rw-r--r--   0        0        0    12865 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/remote_host_proxy.py
+-rw-r--r--   0        0        0     1601 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/socker_listener_thread.py
+-rw-r--r--   0        0        0      971 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/socket_sender_thread.py
+-rw-r--r--   0        0        0     4529 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/utils.py
+-rw-r--r--   0        0        0        0 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/webserver/__init__.py
+-rw-r--r--   0        0        0      914 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/webserver/gunicorn_flask_application.py
+-rw-r--r--   0        0        0     7647 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/webserver/webserver.py
+-rw-r--r--   0        0        0      420 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/webserver/webserver_types.py
+-rw-r--r--   0        0        0     4234 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/webserver/webserver_utils.py
+-rw-r--r--   0        0        0     9900 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/webserver/worker_thread.py
+-rw-r--r--   0        0        0        0 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/experiments/__init__.py
+-rw-r--r--   0        0        0     5939 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/experiments/experiment.py
+-rw-r--r--   0        0        0      171 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/experiments/types.py
+-rw-r--r--   0        0        0       32 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/jobs/__init__.py
+-rw-r--r--   0        0        0    14468 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/jobs/job.py
+-rw-r--r--   0        0        0     4442 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/jobs/job_result.py
+-rw-r--r--   0        0        0      905 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/jobs/types.py
+-rw-r--r--   0        0        0      193 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/lfs/__init__.py
+-rw-r--r--   0        0        0     2226 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/lfs/cache.py
+-rw-r--r--   0        0        0     9832 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/lfs/utils.py
+-rw-r--r--   0        0        0       44 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/runtime/__init__.py
+-rw-r--r--   0        0        0      778 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/runtime/results.py
+-rw-r--r--   0        0        0      210 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/start_cli.py
+-rw-r--r--   0        0        0      872 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/tables.py
+-rw-r--r--   0        0        0       36 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/templates/__init__.py
+-rw-r--r--   0        0        0      715 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/templates/example_app.py
+-rw-r--r--   0        0        0      263 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/typing_utils.py
+-rw-r--r--   0        0        0       39 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/user/__init__.py
+-rw-r--r--   0        0        0     2061 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/user/sign_in.py
+-rw-r--r--   0        0        0     8190 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/utils/__init__.py
+-rw-r--r--   0        0        0     2727 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/utils/cache_state.py
+-rw-r--r--   0        0        0     9717 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/utils/multipart_uploader.py
+-rw-r--r--   0        0        0     1757 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/utils/seq_util.py
+-rw-r--r--   0        0        0    23500 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/utils/zip/remote_zip.py
+-rw-r--r--   0        0        0     6916 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/validators/validate_app_version.py
+-rw-r--r--   0        0        0     4300 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/validators/validate_argument.py
+-rw-r--r--   0        0        0    13298 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/validators/validate_module.py
+-rw-r--r--   0        0        0     1655 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/validators/validate_zip_file.py
+-rw-r--r--   0        0        0     2135 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/validators/validator_utils.py
+-rw-r--r--   0        0        0     1237 2023-06-07 07:38:06.308364 pybiolib-1.1.968/pyproject.toml
+-rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 pybiolib-1.1.968/PKG-INFO
```

### Comparing `pybiolib-1.1.944/LICENSE` & `pybiolib-1.1.968/LICENSE`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/__init__.py` & `pybiolib-1.1.968/biolib/__init__.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/api/client.py` & `pybiolib-1.1.968/biolib/api/client.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/app/app.py` & `pybiolib-1.1.968/biolib/app/app.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/app/search_apps.py` & `pybiolib-1.1.968/biolib/app/search_apps.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/app/utils.py` & `pybiolib-1.1.968/biolib/app/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_api_client/api_client.py` & `pybiolib-1.1.968/biolib/biolib_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_api_client/app_types.py` & `pybiolib-1.1.968/biolib/biolib_api_client/app_types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_api_client/auth.py` & `pybiolib-1.1.968/biolib/biolib_api_client/auth.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_api_client/biolib_account_api.py` & `pybiolib-1.1.968/biolib/biolib_api_client/biolib_account_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_api_client/biolib_app_api.py` & `pybiolib-1.1.968/biolib/biolib_api_client/biolib_app_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_api_client/biolib_job_api.py` & `pybiolib-1.1.968/biolib/biolib_api_client/biolib_job_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 import biolib.api
 
 from biolib import utils
 from biolib.biolib_api_client.auth import BearerAuth
 from biolib.biolib_api_client import BiolibApiClient, CreatedJobDict, CloudJob
 from biolib.biolib_binary_format.stdout_and_stderr import StdoutAndStderr
-from biolib.biolib_errors import BioLibError, RetryLimitException, StorageDownloadFailed
+from biolib.biolib_errors import BioLibError, RetryLimitException, StorageDownloadFailed, JobResultPermissionError,\
+     JobResultError, JobResultNotFound
 from biolib.compute_node.utils import SystemExceptionCodeMap
 from biolib.biolib_logging import logger
 from biolib.utils import BIOLIB_PACKAGE_VERSION, IS_RUNNING_IN_NOTEBOOK
 from biolib.typing_utils import List, TypedDict, Optional, Literal
 
 
 class PresignedS3UploadLinkResponse(TypedDict):
@@ -241,31 +242,45 @@
 
     @staticmethod
     def get_job_storage_download_url(
             job_uuid: str,
             job_auth_token: str,
             storage_type: Literal['input', 'results'],
     ) -> str:
-        response = requests.get(
-            f'{BiolibApiClient.get().base_url}/api/jobs/{job_uuid}/storage/{storage_type}/download/',
-            auth=BearerAuth(BiolibApiClient.get().access_token),
-            headers={
-                'Job-Auth-Token': job_auth_token
-            }
-        )
-
-        if not response.ok:
-            if response.status_code == 404:
-                raise StorageDownloadFailed(response.content)
+        try:
+            response = biolib.api.client.get(
+                url=f'{BiolibApiClient.get().base_url}/api/jobs/{job_uuid}/storage/{storage_type}/download/',
+                authenticate=True,
+                headers={'Job-Auth-Token': job_auth_token}
+            )
+            presigned_s3_download_link_response: PresignedS3DownloadLinkResponse = response.json()
+            presigned_download_url = presigned_s3_download_link_response['presigned_download_url']
+
+            app_caller_proxy_job_storage_base_url = os.getenv('BIOLIB_CLOUD_JOB_STORAGE_BASE_URL', '')
+            if app_caller_proxy_job_storage_base_url:
+                # Done to hit App Caller Proxy when downloading result from inside an app
+                parsed_url = urlparse(presigned_download_url)
+                presigned_download_url = f'{app_caller_proxy_job_storage_base_url}{parsed_url.path}?{parsed_url.query}'
+
+            return presigned_download_url
+
+        except requests.exceptions.HTTPError as error:
+            status_code = error.response.status_code
+            if storage_type == 'results':
+                if status_code == 401:
+                    raise JobResultPermissionError('You must be signed in to get result of the job') from None
+                elif status_code == 403:
+                    raise JobResultPermissionError(
+                        'Cannot get result of job. Maybe the job was created without being signed in?'
+                    ) from None
+                elif status_code == 404:
+                    raise JobResultNotFound('Job result not found') from None
+                else:
+                    raise JobResultError('Failed to get result of job') from error
             else:
-                raise BioLibError(response.content)
-
-        presigned_s3_download_link_response: PresignedS3DownloadLinkResponse = response.json()
-        presigned_download_url = presigned_s3_download_link_response['presigned_download_url']
+                raise StorageDownloadFailed(error.response.content) from error
 
-        app_caller_proxy_job_storage_base_url = os.getenv('BIOLIB_CLOUD_JOB_STORAGE_BASE_URL', '')
-        if app_caller_proxy_job_storage_base_url:
-            # Done to hit App Caller Proxy when downloading result from inside an app
-            parsed_url = urlparse(presigned_download_url)
-            presigned_download_url = f'{app_caller_proxy_job_storage_base_url}{parsed_url.path}?{parsed_url.query}'
-
-        return presigned_download_url
+        except Exception as error:  # pylint: disable=broad-except
+            if storage_type == 'results':
+                raise JobResultError('Failed to get result of job') from error
+            else:
+                raise StorageDownloadFailed('Failed to download from Job Storage') from error
```

### Comparing `pybiolib-1.1.944/biolib/biolib_api_client/biolib_large_file_system_api.py` & `pybiolib-1.1.968/biolib/biolib_api_client/biolib_large_file_system_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_api_client/job_types.py` & `pybiolib-1.1.968/biolib/biolib_api_client/job_types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_api_client/user_state.py` & `pybiolib-1.1.968/biolib/biolib_api_client/user_state.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_binary_format/base_bbf_package.py` & `pybiolib-1.1.968/biolib/biolib_binary_format/base_bbf_package.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_binary_format/encrypted_module_output.py` & `pybiolib-1.1.968/biolib/biolib_binary_format/encrypted_module_output.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_binary_format/module_input.py` & `pybiolib-1.1.968/biolib/biolib_binary_format/module_input.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_binary_format/module_output.py` & `pybiolib-1.1.968/biolib/biolib_binary_format/module_output.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_binary_format/rsa_encrypted_aes_package.py` & `pybiolib-1.1.968/biolib/biolib_binary_format/rsa_encrypted_aes_package.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_binary_format/saved_job.py` & `pybiolib-1.1.968/biolib/biolib_binary_format/saved_job.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_binary_format/stdout_and_stderr.py` & `pybiolib-1.1.968/biolib/biolib_binary_format/stdout_and_stderr.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_binary_format/system_exception.py` & `pybiolib-1.1.968/biolib/biolib_binary_format/system_exception.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_binary_format/system_status_update.py` & `pybiolib-1.1.968/biolib/biolib_binary_format/system_status_update.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_binary_format/unencrypted_module_output.py` & `pybiolib-1.1.968/biolib/biolib_binary_format/unencrypted_module_output.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_binary_format/utils.py` & `pybiolib-1.1.968/biolib/biolib_binary_format/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 from abc import ABC, abstractmethod
 
 import io
+
 import requests
 
 from biolib.typing_utils import Iterable
 from biolib.utils.multipart_uploader import get_chunk_iterator_from_bytes
 
 
+class RemoteEndpoint(ABC):
+    @abstractmethod
+    def get_remote_url(self):
+        pass
+
+
 class IndexableBuffer(ABC):
 
     def __init__(self):
         self.pointer = 0
 
     @abstractmethod
     def get_data(self, start: int, length: int) -> bytes:
@@ -40,27 +47,27 @@
         data = self.get_data_as_string(start=self.pointer, length=length)
         self.pointer += length
         return data
 
 
 class RemoteIndexableBuffer(IndexableBuffer):
 
-    def __init__(self, url: str):
+    def __init__(self, endpoint: RemoteEndpoint):
         super().__init__()
-        self._url = url
+        self._endpoint = endpoint
 
     def get_data(self, start: int, length: int) -> bytes:
         if length < 0:
             raise Exception('get_data length must be positive')
 
         if length == 0:
             return bytes(0)
 
         end = start + length - 1
-        response = requests.get(url=self._url, headers={'range': f'bytes={start}-{end}'})
+        response = requests.get(url=self._endpoint.get_remote_url(), headers={'range': f'bytes={start}-{end}'})
         if not response.ok:
             raise Exception(f'get_data got not ok response status {response.status_code}')
 
         data: bytes = response.content
         if len(data) != length:
             raise Exception(f'get_data got response of unexpected length. Got {len(data)} expected {length}.')
 
@@ -71,15 +78,15 @@
             raise Exception('get_data length must be positive')
 
         if length == 0:
             return []
 
         end = start + length - 1
         response = requests.get(
-            url=self._url,
+            url=self._endpoint.get_remote_url(),
             headers={'range': f'bytes={start}-{end}'},
             stream=True,
             timeout=60,
         )
         return response.iter_content(chunk_size=chunk_size)
```

### Comparing `pybiolib-1.1.944/biolib/biolib_docker_client/__init__.py` & `pybiolib-1.1.968/biolib/biolib_docker_client/__init__.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_logging.py` & `pybiolib-1.1.968/biolib/biolib_logging.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/biolib_push.py` & `pybiolib-1.1.968/biolib/biolib_push.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/cli/__init__.py` & `pybiolib-1.1.968/biolib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/cli/init.py` & `pybiolib-1.1.968/biolib/cli/init.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/cli/lfs.py` & `pybiolib-1.1.968/biolib/cli/lfs.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/cli/push.py` & `pybiolib-1.1.968/biolib/cli/push.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/cli/run.py` & `pybiolib-1.1.968/biolib/cli/run.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/cli/start.py` & `pybiolib-1.1.968/biolib/cli/start.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/cli_utils.py` & `pybiolib-1.1.968/biolib/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/cloud_utils/cloud_utils.py` & `pybiolib-1.1.968/biolib/compute_node/cloud_utils/cloud_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/cache_state.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/cache_state.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/cache_types.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/cache_types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/docker_image_cache.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/docker_image_cache.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/executors/docker_executor.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/executors/docker_executor.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/executors/remote/remote_executor.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/executors/remote/remote_executor.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/executors/types.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/executors/types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/job_storage.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/job_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import requests
 
 from biolib import utils
 from biolib.biolib_api_client import BiolibApiClient, CreatedJobDict
 from biolib.biolib_api_client.biolib_job_api import BiolibJobApi
 from biolib.biolib_binary_format.utils import RemoteIndexableBuffer
+from biolib.biolib_binary_format.remote_endpoints import RemoteJobStorageResultEndpoint
 from biolib.biolib_binary_format.unencrypted_module_output import UnencryptedModuleOutput
 from biolib.compute_node.cloud_utils import CloudUtils
 from biolib.biolib_logging import logger_no_user_data
 from biolib.utils.multipart_uploader import get_chunk_iterator_from_file_object
 
 
 class JobStorage:
@@ -99,15 +100,13 @@
         response.raise_for_status()
         data: bytes = response.content
         logger_no_user_data.debug(f'Job "{job_uuid}" module input downloaded')
         return data
 
     @staticmethod
     def get_module_output(job: CreatedJobDict) -> UnencryptedModuleOutput:
-        presigned_download_url = BiolibJobApi.get_job_storage_download_url(
-            job_uuid=job['public_id'],
-            job_auth_token=job['auth_token'],
-            storage_type='results',
+        remote_job_storage_endpoint = RemoteJobStorageResultEndpoint(
+            job_id=job['public_id'],
+            job_auth_token=job['auth_token']
         )
-
-        buffer = RemoteIndexableBuffer(url=presigned_download_url)
+        buffer = RemoteIndexableBuffer(endpoint=remote_job_storage_endpoint)
         return UnencryptedModuleOutput(buffer)
```

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/job_worker.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/job_worker.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/large_file_system.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/large_file_system.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/mappings.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/mappings.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/job_worker/utils.py` & `pybiolib-1.1.968/biolib/compute_node/job_worker/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/remote_host_proxy.py` & `pybiolib-1.1.968/biolib/compute_node/remote_host_proxy.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/socker_listener_thread.py` & `pybiolib-1.1.968/biolib/compute_node/socker_listener_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/socket_sender_thread.py` & `pybiolib-1.1.968/biolib/compute_node/socket_sender_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/utils.py` & `pybiolib-1.1.968/biolib/compute_node/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/webserver/gunicorn_flask_application.py` & `pybiolib-1.1.968/biolib/compute_node/webserver/gunicorn_flask_application.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/webserver/webserver.py` & `pybiolib-1.1.968/biolib/compute_node/webserver/webserver.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/webserver/webserver_utils.py` & `pybiolib-1.1.968/biolib/compute_node/webserver/webserver_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/compute_node/webserver/worker_thread.py` & `pybiolib-1.1.968/biolib/compute_node/webserver/worker_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/experiments/experiment.py` & `pybiolib-1.1.968/biolib/experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/jobs/job.py` & `pybiolib-1.1.968/biolib/jobs/job.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/jobs/types.py` & `pybiolib-1.1.968/biolib/jobs/types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/lfs/cache.py` & `pybiolib-1.1.968/biolib/lfs/cache.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/lfs/utils.py` & `pybiolib-1.1.968/biolib/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/runtime/results.py` & `pybiolib-1.1.968/biolib/runtime/results.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/tables.py` & `pybiolib-1.1.968/biolib/tables.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/templates/example_app.py` & `pybiolib-1.1.968/biolib/templates/example_app.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/user/sign_in.py` & `pybiolib-1.1.968/biolib/user/sign_in.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/utils/__init__.py` & `pybiolib-1.1.968/biolib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/utils/cache_state.py` & `pybiolib-1.1.968/biolib/utils/cache_state.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/utils/multipart_uploader.py` & `pybiolib-1.1.968/biolib/utils/multipart_uploader.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/utils/seq_util.py` & `pybiolib-1.1.968/biolib/utils/seq_util.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/utils/zip/remote_zip.py` & `pybiolib-1.1.968/biolib/utils/zip/remote_zip.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/validators/validate_app_version.py` & `pybiolib-1.1.968/biolib/validators/validate_app_version.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/validators/validate_argument.py` & `pybiolib-1.1.968/biolib/validators/validate_argument.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/validators/validate_module.py` & `pybiolib-1.1.968/biolib/validators/validate_module.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/validators/validate_zip_file.py` & `pybiolib-1.1.968/biolib/validators/validate_zip_file.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/biolib/validators/validator_utils.py` & `pybiolib-1.1.968/biolib/validators/validator_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.944/pyproject.toml` & `pybiolib-1.1.968/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybiolib"
-version = "1.1.944"
+version = "1.1.968"
 description = "BioLib Python Client"
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/biolib"
 keywords = ["biolib"]
 authors = [
     "biolib <hello@biolib.com>",
```

### Comparing `pybiolib-1.1.944/PKG-INFO` & `pybiolib-1.1.968/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybiolib
-Version: 1.1.944
+Version: 1.1.968
 Summary: BioLib Python Client
 Home-page: https://github.com/biolib
 License: MIT
 Keywords: biolib
 Author: biolib
 Author-email: hello@biolib.com
 Requires-Python: >=3.6.3,<4.0.0
```

