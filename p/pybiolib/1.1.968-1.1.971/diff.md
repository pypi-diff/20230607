# Comparing `tmp/pybiolib-1.1.968.tar.gz` & `tmp/pybiolib-1.1.971.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybiolib-1.1.968.tar", max compression
+gzip compressed data, was "pybiolib-1.1.971.tar", max compression
```

## Comparing `pybiolib-1.1.968.tar` & `pybiolib-1.1.971.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0     1067 2023-06-07 07:37:15.891199 pybiolib-1.1.968/LICENSE
--rw-r--r--   0        0        0      368 2023-06-07 07:37:15.891199 pybiolib-1.1.968/README.md
--rw-r--r--   0        0        0     3337 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/__init__.py
--rw-r--r--   0        0        0       95 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/api/__init__.py
--rw-r--r--   0        0        0     3744 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/api/client.py
--rw-r--r--   0        0        0       37 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/app/__init__.py
--rw-r--r--   0        0        0     7652 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/app/app.py
--rw-r--r--   0        0        0     1493 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/app/search_apps.py
--rw-r--r--   0        0        0     4405 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/app/utils.py
--rw-r--r--   0        0        0      182 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/__init__.py
--rw-r--r--   0        0        0     5574 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/api_client.py
--rw-r--r--   0        0        0     2397 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/app_types.py
--rw-r--r--   0        0        0     1668 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/auth.py
--rw-r--r--   0        0        0      580 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/biolib_account_api.py
--rw-r--r--   0        0        0     2859 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/biolib_app_api.py
--rw-r--r--   0        0        0    10891 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/biolib_job_api.py
--rw-r--r--   0        0        0     1777 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/biolib_large_file_system_api.py
--rw-r--r--   0        0        0      123 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/common_types.py
--rw-r--r--   0        0        0     1256 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/job_types.py
--rw-r--r--   0        0        0      227 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/lfs_types.py
--rw-r--r--   0        0        0      637 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_api_client/user_state.py
--rw-r--r--   0        0        0      303 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/__init__.py
--rw-r--r--   0        0        0      959 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/base_bbf_package.py
--rw-r--r--   0        0        0      154 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/common_types.py
--rw-r--r--   0        0        0     6450 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/encrypted_module_output.py
--rw-r--r--   0        0        0     2603 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/module_input.py
--rw-r--r--   0        0        0     2640 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/module_output.py
--rw-r--r--   0        0        0     1146 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/remote_endpoints.py
--rw-r--r--   0        0        0     2269 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/rsa_encrypted_aes_package.py
--rw-r--r--   0        0        0     1125 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/saved_job.py
--rw-r--r--   0        0        0     1023 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/stdout_and_stderr.py
--rw-r--r--   0        0        0      853 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/system_exception.py
--rw-r--r--   0        0        0     1191 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/system_status_update.py
--rw-r--r--   0        0        0     8514 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/unencrypted_module_output.py
--rw-r--r--   0        0        0     4101 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_binary_format/utils.py
--rw-r--r--   0        0        0     1481 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_docker_client/__init__.py
--rw-r--r--   0        0        0      689 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_errors.py
--rw-r--r--   0        0        0     2854 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_logging.py
--rw-r--r--   0        0        0    10225 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/biolib_push.py
--rw-r--r--   0        0        0      947 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/__init__.py
--rw-r--r--   0        0        0      820 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/init.py
--rw-r--r--   0        0        0     1966 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/lfs.py
--rw-r--r--   0        0        0      798 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/push.py
--rw-r--r--   0        0        0     1309 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/run.py
--rw-r--r--   0        0        0      361 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/runtime.py
--rw-r--r--   0        0        0     1284 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli/start.py
--rw-r--r--   0        0        0     8947 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/cli_utils.py
--rw-r--r--   0        0        0       45 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/.gitignore
--rw-r--r--   0        0        0        0 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/__init__.py
--rw-r--r--   0        0        0       67 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/cloud_utils/__init__.py
--rw-r--r--   0        0        0     6878 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/cloud_utils/cloud_utils.py
--rw-r--r--   0        0        0       71 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/__init__.py
--rw-r--r--   0        0        0     3670 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/cache_state.py
--rw-r--r--   0        0        0      891 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/cache_types.py
--rw-r--r--   0        0        0     7562 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/docker_image_cache.py
--rw-r--r--   0        0        0      221 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/__init__.py
--rw-r--r--   0        0        0      448 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/base_executor.py
--rw-r--r--   0        0        0    24367 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/docker_executor.py
--rw-r--r--   0        0        0      122 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/docker_types.py
--rw-r--r--   0        0        0       91 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/remote/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/remote/remote_executor.py
--rw-r--r--   0        0        0        0 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/tars/__init__.py
--rw-r--r--   0        0        0     1564 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/executors/types.py
--rw-r--r--   0        0        0     1198 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py
--rw-r--r--   0        0        0     1174 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py
--rw-r--r--   0        0        0     4910 2023-06-07 07:37:15.891199 pybiolib-1.1.968/biolib/compute_node/job_worker/job_storage.py
--rw-r--r--   0        0        0    30595 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/job_worker/job_worker.py
--rw-r--r--   0        0        0     9363 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/job_worker/large_file_system.py
--rw-r--r--   0        0        0     2499 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/job_worker/mappings.py
--rw-r--r--   0        0        0     1282 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/job_worker/utils.py
--rw-r--r--   0        0        0    12865 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/remote_host_proxy.py
--rw-r--r--   0        0        0     1601 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/socker_listener_thread.py
--rw-r--r--   0        0        0      971 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/socket_sender_thread.py
--rw-r--r--   0        0        0     4529 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/utils.py
--rw-r--r--   0        0        0        0 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/webserver/__init__.py
--rw-r--r--   0        0        0      914 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/webserver/gunicorn_flask_application.py
--rw-r--r--   0        0        0     7647 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/webserver/webserver.py
--rw-r--r--   0        0        0      420 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/webserver/webserver_types.py
--rw-r--r--   0        0        0     4234 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/webserver/webserver_utils.py
--rw-r--r--   0        0        0     9900 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/compute_node/webserver/worker_thread.py
--rw-r--r--   0        0        0        0 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/experiments/__init__.py
--rw-r--r--   0        0        0     5939 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/experiments/experiment.py
--rw-r--r--   0        0        0      171 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/experiments/types.py
--rw-r--r--   0        0        0       32 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/jobs/__init__.py
--rw-r--r--   0        0        0    14468 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/jobs/job.py
--rw-r--r--   0        0        0     4442 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/jobs/job_result.py
--rw-r--r--   0        0        0      905 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/jobs/types.py
--rw-r--r--   0        0        0      193 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/lfs/__init__.py
--rw-r--r--   0        0        0     2226 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/lfs/cache.py
--rw-r--r--   0        0        0     9832 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/lfs/utils.py
--rw-r--r--   0        0        0       44 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/runtime/__init__.py
--rw-r--r--   0        0        0      778 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/runtime/results.py
--rw-r--r--   0        0        0      210 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/start_cli.py
--rw-r--r--   0        0        0      872 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/tables.py
--rw-r--r--   0        0        0       36 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/templates/__init__.py
--rw-r--r--   0        0        0      715 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/templates/example_app.py
--rw-r--r--   0        0        0      263 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/typing_utils.py
--rw-r--r--   0        0        0       39 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/user/__init__.py
--rw-r--r--   0        0        0     2061 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/user/sign_in.py
--rw-r--r--   0        0        0     8190 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/utils/__init__.py
--rw-r--r--   0        0        0     2727 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/utils/cache_state.py
--rw-r--r--   0        0        0     9717 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/utils/multipart_uploader.py
--rw-r--r--   0        0        0     1757 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/utils/seq_util.py
--rw-r--r--   0        0        0    23500 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/utils/zip/remote_zip.py
--rw-r--r--   0        0        0     6916 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/validators/validate_app_version.py
--rw-r--r--   0        0        0     4300 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/validators/validate_argument.py
--rw-r--r--   0        0        0    13298 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/validators/validate_module.py
--rw-r--r--   0        0        0     1655 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/validators/validate_zip_file.py
--rw-r--r--   0        0        0     2135 2023-06-07 07:37:15.895199 pybiolib-1.1.968/biolib/validators/validator_utils.py
--rw-r--r--   0        0        0     1237 2023-06-07 07:38:06.308364 pybiolib-1.1.968/pyproject.toml
--rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 pybiolib-1.1.968/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-07 09:46:16.267807 pybiolib-1.1.971/LICENSE
+-rw-r--r--   0        0        0      368 2023-06-07 09:46:16.267807 pybiolib-1.1.971/README.md
+-rw-r--r--   0        0        0     3337 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/__init__.py
+-rw-r--r--   0        0        0       95 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/api/__init__.py
+-rw-r--r--   0        0        0     3744 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/api/client.py
+-rw-r--r--   0        0        0       37 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/app/__init__.py
+-rw-r--r--   0        0        0     7652 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/app/app.py
+-rw-r--r--   0        0        0     1493 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/app/search_apps.py
+-rw-r--r--   0        0        0     4405 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/app/utils.py
+-rw-r--r--   0        0        0      182 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_api_client/__init__.py
+-rw-r--r--   0        0        0     5574 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_api_client/api_client.py
+-rw-r--r--   0        0        0     2397 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_api_client/app_types.py
+-rw-r--r--   0        0        0     1668 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_api_client/auth.py
+-rw-r--r--   0        0        0      580 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_api_client/biolib_account_api.py
+-rw-r--r--   0        0        0     2859 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_api_client/biolib_app_api.py
+-rw-r--r--   0        0        0    10891 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_api_client/biolib_job_api.py
+-rw-r--r--   0        0        0     1777 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_api_client/biolib_large_file_system_api.py
+-rw-r--r--   0        0        0      123 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_api_client/common_types.py
+-rw-r--r--   0        0        0     1256 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_api_client/job_types.py
+-rw-r--r--   0        0        0      227 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_api_client/lfs_types.py
+-rw-r--r--   0        0        0      637 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_api_client/user_state.py
+-rw-r--r--   0        0        0      303 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/__init__.py
+-rw-r--r--   0        0        0      959 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/base_bbf_package.py
+-rw-r--r--   0        0        0      154 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/common_types.py
+-rw-r--r--   0        0        0     6450 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/encrypted_module_output.py
+-rw-r--r--   0        0        0     2603 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/module_input.py
+-rw-r--r--   0        0        0     2640 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/module_output.py
+-rw-r--r--   0        0        0     1146 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/remote_endpoints.py
+-rw-r--r--   0        0        0     2269 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/rsa_encrypted_aes_package.py
+-rw-r--r--   0        0        0     1125 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/saved_job.py
+-rw-r--r--   0        0        0     1023 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/stdout_and_stderr.py
+-rw-r--r--   0        0        0      853 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/system_exception.py
+-rw-r--r--   0        0        0     1191 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/system_status_update.py
+-rw-r--r--   0        0        0     8514 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/unencrypted_module_output.py
+-rw-r--r--   0        0        0     4101 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_binary_format/utils.py
+-rw-r--r--   0        0        0     1481 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_docker_client/__init__.py
+-rw-r--r--   0        0        0      689 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_errors.py
+-rw-r--r--   0        0        0     2854 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_logging.py
+-rw-r--r--   0        0        0    10225 2023-06-07 09:46:16.267807 pybiolib-1.1.971/biolib/biolib_push.py
+-rw-r--r--   0        0        0      947 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/cli/__init__.py
+-rw-r--r--   0        0        0      820 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/cli/init.py
+-rw-r--r--   0        0        0     1966 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/cli/lfs.py
+-rw-r--r--   0        0        0      798 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/cli/push.py
+-rw-r--r--   0        0        0     1309 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/cli/run.py
+-rw-r--r--   0        0        0      361 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/cli/runtime.py
+-rw-r--r--   0        0        0     1284 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/cli/start.py
+-rw-r--r--   0        0        0     8947 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/cli_utils.py
+-rw-r--r--   0        0        0       45 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/cloud_utils/__init__.py
+-rw-r--r--   0        0        0     6878 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/cloud_utils/cloud_utils.py
+-rw-r--r--   0        0        0       71 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/__init__.py
+-rw-r--r--   0        0        0     3670 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/cache_state.py
+-rw-r--r--   0        0        0      891 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/cache_types.py
+-rw-r--r--   0        0        0     7562 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/docker_image_cache.py
+-rw-r--r--   0        0        0      221 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/executors/__init__.py
+-rw-r--r--   0        0        0      448 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/executors/base_executor.py
+-rw-r--r--   0        0        0    24003 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/executors/docker_executor.py
+-rw-r--r--   0        0        0      122 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/executors/docker_types.py
+-rw-r--r--   0        0        0       91 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/executors/remote/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/executors/remote/remote_executor.py
+-rw-r--r--   0        0        0        0 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/executors/tars/__init__.py
+-rw-r--r--   0        0        0     1466 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/executors/types.py
+-rw-r--r--   0        0        0     1198 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py
+-rw-r--r--   0        0        0     1174 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py
+-rw-r--r--   0        0        0     4910 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/job_storage.py
+-rw-r--r--   0        0        0    27432 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/job_worker.py
+-rw-r--r--   0        0        0     9363 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/large_file_system.py
+-rw-r--r--   0        0        0     2499 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/mappings.py
+-rw-r--r--   0        0        0     1282 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/job_worker/utils.py
+-rw-r--r--   0        0        0    12865 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/remote_host_proxy.py
+-rw-r--r--   0        0        0     1601 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/socker_listener_thread.py
+-rw-r--r--   0        0        0      971 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/socket_sender_thread.py
+-rw-r--r--   0        0        0     4529 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/utils.py
+-rw-r--r--   0        0        0        0 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/webserver/__init__.py
+-rw-r--r--   0        0        0      914 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/webserver/gunicorn_flask_application.py
+-rw-r--r--   0        0        0     7647 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/webserver/webserver.py
+-rw-r--r--   0        0        0      420 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/webserver/webserver_types.py
+-rw-r--r--   0        0        0     4234 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/webserver/webserver_utils.py
+-rw-r--r--   0        0        0     9900 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/compute_node/webserver/worker_thread.py
+-rw-r--r--   0        0        0        0 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/experiments/__init__.py
+-rw-r--r--   0        0        0     5939 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/experiments/experiment.py
+-rw-r--r--   0        0        0      171 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/experiments/types.py
+-rw-r--r--   0        0        0       32 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/jobs/__init__.py
+-rw-r--r--   0        0        0    14468 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/jobs/job.py
+-rw-r--r--   0        0        0     4442 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/jobs/job_result.py
+-rw-r--r--   0        0        0      905 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/jobs/types.py
+-rw-r--r--   0        0        0      193 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/lfs/__init__.py
+-rw-r--r--   0        0        0     2226 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/lfs/cache.py
+-rw-r--r--   0        0        0     9832 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/lfs/utils.py
+-rw-r--r--   0        0        0       44 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/runtime/__init__.py
+-rw-r--r--   0        0        0      778 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/runtime/results.py
+-rw-r--r--   0        0        0      210 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/start_cli.py
+-rw-r--r--   0        0        0      872 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/tables.py
+-rw-r--r--   0        0        0       36 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/templates/__init__.py
+-rw-r--r--   0        0        0      715 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/templates/example_app.py
+-rw-r--r--   0        0        0      263 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/typing_utils.py
+-rw-r--r--   0        0        0       39 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/user/__init__.py
+-rw-r--r--   0        0        0     2061 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/user/sign_in.py
+-rw-r--r--   0        0        0     8107 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/utils/__init__.py
+-rw-r--r--   0        0        0     2727 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/utils/cache_state.py
+-rw-r--r--   0        0        0     9717 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/utils/multipart_uploader.py
+-rw-r--r--   0        0        0     1757 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/utils/seq_util.py
+-rw-r--r--   0        0        0    23500 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/utils/zip/remote_zip.py
+-rw-r--r--   0        0        0     6916 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/validators/validate_app_version.py
+-rw-r--r--   0        0        0     4300 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/validators/validate_argument.py
+-rw-r--r--   0        0        0    13298 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/validators/validate_module.py
+-rw-r--r--   0        0        0     1655 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/validators/validate_zip_file.py
+-rw-r--r--   0        0        0     2135 2023-06-07 09:46:16.271807 pybiolib-1.1.971/biolib/validators/validator_utils.py
+-rw-r--r--   0        0        0     1237 2023-06-07 09:47:05.108037 pybiolib-1.1.971/pyproject.toml
+-rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 pybiolib-1.1.971/PKG-INFO
```

### Comparing `pybiolib-1.1.968/LICENSE` & `pybiolib-1.1.971/LICENSE`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/__init__.py` & `pybiolib-1.1.971/biolib/__init__.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/api/client.py` & `pybiolib-1.1.971/biolib/api/client.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/app/app.py` & `pybiolib-1.1.971/biolib/app/app.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/app/search_apps.py` & `pybiolib-1.1.971/biolib/app/search_apps.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/app/utils.py` & `pybiolib-1.1.971/biolib/app/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_api_client/api_client.py` & `pybiolib-1.1.971/biolib/biolib_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_api_client/app_types.py` & `pybiolib-1.1.971/biolib/biolib_api_client/app_types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_api_client/auth.py` & `pybiolib-1.1.971/biolib/biolib_api_client/auth.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_api_client/biolib_account_api.py` & `pybiolib-1.1.971/biolib/biolib_api_client/biolib_account_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_api_client/biolib_app_api.py` & `pybiolib-1.1.971/biolib/biolib_api_client/biolib_app_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_api_client/biolib_job_api.py` & `pybiolib-1.1.971/biolib/biolib_api_client/biolib_job_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_api_client/biolib_large_file_system_api.py` & `pybiolib-1.1.971/biolib/biolib_api_client/biolib_large_file_system_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_api_client/job_types.py` & `pybiolib-1.1.971/biolib/biolib_api_client/job_types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_api_client/user_state.py` & `pybiolib-1.1.971/biolib/biolib_api_client/user_state.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_binary_format/base_bbf_package.py` & `pybiolib-1.1.971/biolib/biolib_binary_format/base_bbf_package.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_binary_format/encrypted_module_output.py` & `pybiolib-1.1.971/biolib/biolib_binary_format/encrypted_module_output.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_binary_format/module_input.py` & `pybiolib-1.1.971/biolib/biolib_binary_format/module_input.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_binary_format/module_output.py` & `pybiolib-1.1.971/biolib/biolib_binary_format/module_output.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_binary_format/remote_endpoints.py` & `pybiolib-1.1.971/biolib/biolib_binary_format/remote_endpoints.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_binary_format/rsa_encrypted_aes_package.py` & `pybiolib-1.1.971/biolib/biolib_binary_format/rsa_encrypted_aes_package.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_binary_format/saved_job.py` & `pybiolib-1.1.971/biolib/biolib_binary_format/saved_job.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_binary_format/stdout_and_stderr.py` & `pybiolib-1.1.971/biolib/biolib_binary_format/stdout_and_stderr.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_binary_format/system_exception.py` & `pybiolib-1.1.971/biolib/biolib_binary_format/system_exception.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_binary_format/system_status_update.py` & `pybiolib-1.1.971/biolib/biolib_binary_format/system_status_update.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_binary_format/unencrypted_module_output.py` & `pybiolib-1.1.971/biolib/biolib_binary_format/unencrypted_module_output.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_binary_format/utils.py` & `pybiolib-1.1.971/biolib/biolib_binary_format/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_docker_client/__init__.py` & `pybiolib-1.1.971/biolib/biolib_docker_client/__init__.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_errors.py` & `pybiolib-1.1.971/biolib/biolib_errors.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_logging.py` & `pybiolib-1.1.971/biolib/biolib_logging.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/biolib_push.py` & `pybiolib-1.1.971/biolib/biolib_push.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/cli/__init__.py` & `pybiolib-1.1.971/biolib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/cli/init.py` & `pybiolib-1.1.971/biolib/cli/init.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/cli/lfs.py` & `pybiolib-1.1.971/biolib/cli/lfs.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/cli/push.py` & `pybiolib-1.1.971/biolib/cli/push.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/cli/run.py` & `pybiolib-1.1.971/biolib/cli/run.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/cli/start.py` & `pybiolib-1.1.971/biolib/cli/start.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/cli_utils.py` & `pybiolib-1.1.971/biolib/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/cloud_utils/cloud_utils.py` & `pybiolib-1.1.971/biolib/compute_node/cloud_utils/cloud_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/cache_state.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/cache_state.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/cache_types.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/cache_types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/docker_image_cache.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/docker_image_cache.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/executors/docker_executor.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/executors/docker_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,15 +243,14 @@
             module = self._options['module']
             logger.debug(f"Initializing docker container with command: {module['command']}")
 
             docker_volume_mounts = [lfs.docker_mount for lfs in self._options['large_file_systems'].values()]
 
             internal_network = self._options['internal_network']
             extra_hosts: Dict[str, str] = {}
-            dns_list: List[str] = []
 
             biolib_system_secret = {
                 'version': '1.0.0',
                 'job_uuid': self._options['job']['public_id'],
                 'job_auth_token': self._options['job']['auth_token'],
             }
             secrets: Dict[str, str] = dict(
@@ -291,27 +290,21 @@
                         'BIOLIB_CLOUD_JOB_STORAGE_BASE_URL': f'http://{proxy_ip}',
                         # Inform container if we are targeting public biolib as we change the BIOLIB_BASE_URL
                         'BIOLIB_ENVIRONMENT_IS_PUBLIC_BIOLIB': bool(utils.BASE_URL_IS_PUBLIC_BIOLIB)
                     })
                 else:
                     extra_hosts[proxy.hostname] = proxy_ip
 
-            if self._options['dns_proxy']:
-                container_networks = self._options['dns_proxy'].attrs['NetworkSettings']['Networks']
-                dns_proxy_ip_address: str = container_networks[internal_network.name]['IPAddress']
-                dns_list = [dns_proxy_ip_address]
-
             create_container_args = {
                 'environment': environment_vars,
                 'extra_hosts': extra_hosts,
                 'image': self._image_uri,
                 'mounts': docker_volume_mounts,
                 'network': internal_network.name,
                 'working_dir': module['working_directory'],
-                'dns': dns_list,
             }
 
             if self._options['job'].get('arguments_override_command'):
                 # In this case, arguments contains a user specified command to run in the app
                 create_container_args.update({
                     'command': module_input['arguments'],
                     'entrypoint': ''
```

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/executors/remote/remote_executor.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/executors/remote/remote_executor.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/executors/types.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/executors/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from docker.models.containers import Container  # type: ignore
 from docker.models.networks import Network  # type: ignore
 
 from biolib.compute_node.job_worker.large_file_system import LargeFileSystem
 from biolib.compute_node.webserver.webserver_types import ComputeNodeInfo
 from biolib.typing_utils import TypedDict, Callable, Optional, List, Dict
 from biolib.compute_node.remote_host_proxy import RemoteHostProxy
 from biolib.biolib_api_client.app_types import Module
@@ -31,14 +30,13 @@
     biolib_base_url: str
     compute_node_info: Optional[ComputeNodeInfo]
     internal_network: Optional[Network]
     job: CreatedJobDict
     cloud_job: Optional[CloudJob]
     large_file_systems: Dict[str, LargeFileSystem]
     module: Module
-    dns_proxy: Optional[Container]
     remote_host_proxies: List[RemoteHostProxy]
     root_job_id: str
     runtime_zip_bytes: Optional[bytes]  # TODO: replace this with a module_source_serialized
     send_status_update: SendStatusUpdateType
     send_system_exception: SendSystemExceptionType
     send_stdout_and_stderr: SendStdoutAndStderrType
```

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/job_storage.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/job_storage.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/job_worker.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/job_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import io
 import json
 import socket
 import shlex
-import tarfile
 import zipfile
-from time import time, sleep
+from time import time
 from queue import Queue
 import multiprocessing
 import os
 import signal
 from types import FrameType
 
 import requests
-from docker.errors import ImageNotFound  # type: ignore
 from docker.models.networks import Network  # type: ignore
-from docker.models.containers import Container  # type: ignore
 
 from biolib.biolib_binary_format.stdout_and_stderr import StdoutAndStderr
 from biolib.compute_node.job_worker.job_legacy_input_wait_timeout_thread import JobLegacyInputWaitTimeout
 from biolib.compute_node.job_worker.job_storage import JobStorage
 from biolib.compute_node.job_worker.large_file_system import LargeFileSystem
 from biolib.biolib_errors import DockerContainerNotFoundDuringExecutionException, BioLibError, \
     StorageDownloadFailed
@@ -38,16 +35,14 @@
 from biolib.compute_node.socket_sender_thread import SocketSenderThread
 from biolib.compute_node.job_worker.mappings import Mappings, path_without_first_folder
 from biolib.compute_node.job_worker.utils import ComputeProcessException, log_disk_and_memory_usage_info
 from biolib.compute_node.utils import get_package_type, SystemExceptionCodes, SystemExceptionCodeMap
 from biolib.biolib_binary_format import SavedJob, SystemStatusUpdate, ModuleInput, SystemException, \
     UnencryptedModuleOutput
 
-_DNS_PROXY_IMAGE_URI = 'spx01/blocky@sha256:485ef739233341d3e14a64db646754aba7322c34645f804c3c0c00556d9a2cd1'
-DEFAULT_BUFFER_SIZE = 1024
 SOCKET_HOST = '127.0.0.1'
 
 
 class JobWorkerProcess(multiprocessing.Process):
 
     # note: this method is run in the parent process
     def __init__(self, socket_port: int, log_level: int):
@@ -77,16 +72,14 @@
             self._messages_to_send_queue: Queue = Queue()
             self._legacy_input_wait_timeout_thread: Optional[JobLegacyInputWaitTimeout] = None
 
             self._app_version_id_to_runtime_zip: Dict[str, bytes] = {}
             self._jobs: Dict[str, CreatedJobDict] = {}
             self._root_job_wrapper: Optional[JobWrapper] = None
 
-            self._dns_proxy: Optional[Container] = None
-
             self._remote_host_proxies: List[RemoteHostProxy] = []
             self._internal_network: Optional[Network] = None
             self._public_network: Optional[Network] = None
             self._executors: List[BaseExecutor] = []
             self.is_cleaning_up: bool = False
 
             self.job_temporary_dir: Optional[str] = None
@@ -205,22 +198,14 @@
                 except Exception as exception:  # pylint: disable=broad-except
                     logger_no_user_data.error('Failed to clean up remote host proxy')
                     logger.error(exception)
 
             self._remote_host_proxies = []
             logger_no_user_data.debug(f'Cleaned up {proxy_count} proxies in {time() - proxy_cleanup_start_time}')
 
-        if self._dns_proxy:
-            try:
-                self._dns_proxy.remove(force=True)
-                logger_no_user_data.debug('Cleaned up DNS Proxy')
-            except Exception as exception:  # pylint: disable=broad-except
-                logger_no_user_data.error('Failed to clean up DNS Proxy')
-                logger.error(exception)
-
         self._cleanup_network(self._internal_network)
         self._internal_network = None
         self._cleanup_network(self._public_network)
         self._public_network = None
 
     @staticmethod
     def _cleanup_network(network: Optional[Network]) -> None:
@@ -320,98 +305,29 @@
                         self._internal_network,
                         job_id,
                         ports
                     )
                     remote_host_proxy.start()
                     self._remote_host_proxies.append(remote_host_proxy)
 
-                if utils.BIOLIB_ENABLE_DNS_PROXY:
-                    domains_to_whitelist = list(hostname_to_ports.keys())
-                    logger_no_user_data.debug(f'Job "{job_id}" starting DNS Proxy for domains: {domains_to_whitelist}')
-                    self._start_dns_proxy(domains_to_whitelist=domains_to_whitelist)
-
             except Exception as exception:
                 raise ComputeProcessException(
                     exception,
                     SystemExceptionCodes.FAILED_TO_START_REMOTE_HOST_PROXIES.value,
                     self.send_system_exception,
                     may_contain_user_data=False
                 ) from exception
 
             logger_no_user_data.debug(f'Job "{job_id}" startup of remote host proxies completed')
 
-    def _get_dns_proxy_image(self):
-        docker = BiolibDockerClient.get_docker_client()
-        try:
-            return docker.images.get(_DNS_PROXY_IMAGE_URI)
-        except ImageNotFound:
-            logger_no_user_data.debug('Pulling DNS proxy Docker image...')
-            return docker.images.pull(_DNS_PROXY_IMAGE_URI)
-
-    def _start_dns_proxy(self, domains_to_whitelist):
-        docker = BiolibDockerClient.get_docker_client()
-        self._dns_proxy = docker.containers.create(
-            detach=True,
-            image=self._get_dns_proxy_image(),
-            name=f'biolib-dns-proxy-{self._root_job_wrapper["job"]["public_id"]}',
-            network=self._public_network.name,
-        )
-
-        blocky_config = '''
-upstream:
-    default:
-        - 127.0.0.11
-blocking:
-    whiteLists:
-        remoteHosts:
-            - |'''
-        for domain in domains_to_whitelist:
-            blocky_config += f'''
-              {domain}'''
-        blocky_config += '''
-    clientGroupsBlock:
-        default:
-            - remoteHosts
-port: 53
-'''
-
-        blocky_config_bytes = blocky_config.encode()
-        tarfile_in_memory = io.BytesIO()
-        with tarfile.open(fileobj=tarfile_in_memory, mode='w:gz') as tar:
-            info = tarfile.TarInfo('/config.yml')
-            info.size = len(blocky_config_bytes)
-            tar.addfile(info, io.BytesIO(blocky_config_bytes))
-
-        tarfile_bytes = tarfile_in_memory.getvalue()
-        tarfile_in_memory.close()
-        docker.api.put_archive(self._dns_proxy.id, '/app', tarfile_bytes)
-
-        self._internal_network.connect(self._dns_proxy.id)
-
-        self._dns_proxy.start()
-
-        proxy_is_ready = False
-        for retry_count in range(1, 5):
-            sleep(0.5 * retry_count)
-            # Use the container logs as a health check.
-            if b'TCP server is up and running' in self._dns_proxy.logs():
-                proxy_is_ready = True
-                break
-
-        if not proxy_is_ready:
-            self._dns_proxy.remove(force=True)
-            raise Exception('DNS Proxy did not start properly')
-
-        self._dns_proxy.reload()
-
     def _run_app_version(
-        self,
-        app_version_id: str,
-        module_input_serialized: bytes,
-        caller_job: CreatedJobDict
+            self,
+            app_version_id: str,
+            module_input_serialized: bytes,
+            caller_job: CreatedJobDict
     ) -> bytes:
         job: CreatedJobDict = BiolibJobApi.create(app_version_id, caller_job=caller_job['public_id'])
         self._jobs[job['public_id']] = job
         return self._run_job(job, module_input_serialized)
 
     def _run_job(self, job: CreatedJobDict, module_input_serialized: bytes) -> bytes:
         job_uuid = job['public_id']
@@ -471,15 +387,14 @@
                 internal_network=self._internal_network,
                 job=job,
                 cloud_job=self._root_job_wrapper['cloud_job'],
                 large_file_systems=lfs_dict,
                 module=main_module,
                 remote_host_proxies=self._remote_host_proxies,
                 root_job_id=root_job_id,
-                dns_proxy=self._dns_proxy,
                 runtime_zip_bytes=runtime_zip_bytes,
                 send_status_update=self._send_status_update,
                 send_system_exception=self.send_system_exception,
                 send_stdout_and_stderr=self.send_stdout_and_stderr,
             ),
             module_input_serialized,
         )
@@ -678,14 +593,13 @@
         legacy_module_output_file_path = os.path.join(self.job_temporary_dir, JobStorage.legacy_module_output_file_name)
         with open(legacy_module_output_file_path, mode='wb') as file:
             file.write(module_output_serialized)
 
         module_output_file_path = os.path.join(self.job_temporary_dir, JobStorage.module_output_file_name)
         with open(legacy_module_output_file_path, 'rb') as legacy_module_output, \
                 open(module_output_file_path, 'wb') as module_output:
-
             UnencryptedModuleOutput.write_to_file_from_legacy_module_output_file(
                 input_file=legacy_module_output,
                 output_file=module_output,
             )
 
         self._send_status_update(StatusUpdate(progress=94, log_message='Computation finished'))
```

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/large_file_system.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/large_file_system.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/mappings.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/mappings.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/job_worker/utils.py` & `pybiolib-1.1.971/biolib/compute_node/job_worker/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/remote_host_proxy.py` & `pybiolib-1.1.971/biolib/compute_node/remote_host_proxy.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/socker_listener_thread.py` & `pybiolib-1.1.971/biolib/compute_node/socker_listener_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/socket_sender_thread.py` & `pybiolib-1.1.971/biolib/compute_node/socket_sender_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/utils.py` & `pybiolib-1.1.971/biolib/compute_node/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/webserver/gunicorn_flask_application.py` & `pybiolib-1.1.971/biolib/compute_node/webserver/gunicorn_flask_application.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/webserver/webserver.py` & `pybiolib-1.1.971/biolib/compute_node/webserver/webserver.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/webserver/webserver_utils.py` & `pybiolib-1.1.971/biolib/compute_node/webserver/webserver_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/compute_node/webserver/worker_thread.py` & `pybiolib-1.1.971/biolib/compute_node/webserver/worker_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/experiments/experiment.py` & `pybiolib-1.1.971/biolib/experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/jobs/job.py` & `pybiolib-1.1.971/biolib/jobs/job.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/jobs/job_result.py` & `pybiolib-1.1.971/biolib/jobs/job_result.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/jobs/types.py` & `pybiolib-1.1.971/biolib/jobs/types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/lfs/cache.py` & `pybiolib-1.1.971/biolib/lfs/cache.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/lfs/utils.py` & `pybiolib-1.1.971/biolib/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/runtime/results.py` & `pybiolib-1.1.971/biolib/runtime/results.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/tables.py` & `pybiolib-1.1.971/biolib/tables.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/templates/example_app.py` & `pybiolib-1.1.971/biolib/templates/example_app.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/user/sign_in.py` & `pybiolib-1.1.971/biolib/user/sign_in.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/utils/__init__.py` & `pybiolib-1.1.971/biolib/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 try:
     BIOLIB_PACKAGE_VERSION = version('pybiolib')
 except PackageNotFoundError:
     BIOLIB_PACKAGE_VERSION = '0.0.0'
 
 IS_DEV = os.getenv('BIOLIB_DEV', '').upper() == 'TRUE'
 
+
 def _get_base_url() -> str:
     base_url = os.getenv('BIOLIB_BASE_URL')
     if base_url:
         return base_url.lower().rstrip('/')
 
     try:
         search_list = []
@@ -40,19 +41,20 @@
                     logger.debug(f'Found search list: {search_list} when resolving base url.')
                     break
 
         for search_host in search_list:
             host_to_try = f'biolib.{search_host}'
             if len(socket.getaddrinfo(host_to_try, 443)) > 0:
                 return f'https://{host_to_try}'.lower()
-    except BaseException: # pylint: disable=broad-except
+    except BaseException:  # pylint: disable=broad-except
         pass
 
     return 'https://biolib.com'
 
+
 BIOLIB_BASE_URL = _get_base_url()
 
 BIOLIB_CLOUD_BASE_URL = os.getenv('BIOLIB_CLOUD_BASE_URL', '').lower()
 
 BIOLIB_PACKAGE_ROOT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 BIOLIB_CLOUD_ENVIRONMENT = os.getenv('BIOLIB_CLOUD_ENVIRONMENT', '').lower()
@@ -74,16 +76,14 @@
 
 if BIOLIB_CLOUD_ENVIRONMENT and not IS_RUNNING_IN_CLOUD:
     logger_no_user_data.warning((
         'BIOLIB_CLOUD_ENVIRONMENT defined but does not specify the cloud environment correctly. ',
         'The compute node will not act as a cloud compute node'
     ))
 
-BIOLIB_ENABLE_DNS_PROXY = os.getenv('BIOLIB_ENABLE_DNS_PROXY', '').upper() == 'TRUE'
-
 RUN_DEV_JOB_ID = 'run-dev-mocked-job-id'
 
 
 def get_absolute_container_image_uri(base_url: str, relative_image_uri: str, job_is_federated: bool = False):
     if base_url == 'https://biolib.com' or job_is_federated:
         container_registry_hostname = 'containers.biolib.com'
     elif base_url in ('https://staging-elb.biolib.com', 'https://staging.biolib.com'):
```

### Comparing `pybiolib-1.1.968/biolib/utils/cache_state.py` & `pybiolib-1.1.971/biolib/utils/cache_state.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/utils/multipart_uploader.py` & `pybiolib-1.1.971/biolib/utils/multipart_uploader.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/utils/seq_util.py` & `pybiolib-1.1.971/biolib/utils/seq_util.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/utils/zip/remote_zip.py` & `pybiolib-1.1.971/biolib/utils/zip/remote_zip.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/validators/validate_app_version.py` & `pybiolib-1.1.971/biolib/validators/validate_app_version.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/validators/validate_argument.py` & `pybiolib-1.1.971/biolib/validators/validate_argument.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/validators/validate_module.py` & `pybiolib-1.1.971/biolib/validators/validate_module.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/validators/validate_zip_file.py` & `pybiolib-1.1.971/biolib/validators/validate_zip_file.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/biolib/validators/validator_utils.py` & `pybiolib-1.1.971/biolib/validators/validator_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.968/pyproject.toml` & `pybiolib-1.1.971/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybiolib"
-version = "1.1.968"
+version = "1.1.971"
 description = "BioLib Python Client"
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/biolib"
 keywords = ["biolib"]
 authors = [
     "biolib <hello@biolib.com>",
```

### Comparing `pybiolib-1.1.968/PKG-INFO` & `pybiolib-1.1.971/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybiolib
-Version: 1.1.968
+Version: 1.1.971
 Summary: BioLib Python Client
 Home-page: https://github.com/biolib
 License: MIT
 Keywords: biolib
 Author: biolib
 Author-email: hello@biolib.com
 Requires-Python: >=3.6.3,<4.0.0
```

