# Comparing `tmp/prodvana-0.1.7.tar.gz` & `tmp/prodvana-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodvana-0.1.7.tar", max compression
+gzip compressed data, was "prodvana-0.1.8.tar", max compression
```

## Comparing `prodvana-0.1.7.tar` & `prodvana-0.1.8.tar`

### file list

```diff
@@ -1,332 +1,332 @@
--rw-r--r--   0        0        0       81 2023-05-31 21:06:51.269689 prodvana-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-05-31 21:06:51.269689 prodvana-0.1.7/prodvana/__init__.py
--rw-r--r--   0        0        0     3529 2023-05-31 21:06:51.269689 prodvana-0.1.7/prodvana/client.py
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.787926 prodvana-0.1.7/prodvana/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.787926 prodvana-0.1.7/prodvana/proto/prodvana/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.799926 prodvana-0.1.7/prodvana/proto/prodvana/agent/__init__.py
--rw-r--r--   0        0        0    19183 2023-06-06 19:13:21.419926 prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
--rw-r--r--   0        0        0    18983 2023-06-06 19:13:21.631926 prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
--rw-r--r--   0        0        0    22573 2023-06-06 19:13:21.415926 prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
--rw-r--r--   0        0        0     6760 2023-06-06 19:13:21.631926 prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.807926 prodvana-0.1.7/prodvana/proto/prodvana/application/__init__.py
--rw-r--r--   0        0        0     4200 2023-06-06 19:13:21.503926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_config_pb2.py
--rw-r--r--   0        0        0     4693 2023-06-06 19:13:21.711926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.499926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.711926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    24873 2023-06-06 19:13:21.499926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2.py
--rw-r--r--   0        0        0    16394 2023-06-06 19:13:21.715926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2.pyi
--rw-r--r--   0        0        0    22241 2023-06-06 19:13:21.499926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6755 2023-06-06 19:13:21.707926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2801 2023-06-06 19:13:21.495926 prodvana-0.1.7/prodvana/proto/prodvana/application/object_pb2.py
--rw-r--r--   0        0        0     2184 2023-06-06 19:13:21.715926 prodvana-0.1.7/prodvana/proto/prodvana/application/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.503926 prodvana-0.1.7/prodvana/proto/prodvana/application/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.719926 prodvana-0.1.7/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2294 2023-06-06 19:13:21.495926 prodvana-0.1.7/prodvana/proto/prodvana/application/user_metadata_pb2.py
--rw-r--r--   0        0        0     1670 2023-06-06 19:13:21.715926 prodvana-0.1.7/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.491926 prodvana-0.1.7/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.711926 prodvana-0.1.7/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.799926 prodvana-0.1.7/prodvana/proto/prodvana/auth/__init__.py
--rw-r--r--   0        0        0    13908 2023-06-06 19:13:21.423926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2.py
--rw-r--r--   0        0        0    10206 2023-06-06 19:13:21.635926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
--rw-r--r--   0        0        0    18631 2023-06-06 19:13:21.423926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6767 2023-06-06 19:13:21.635926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     5071 2023-06-06 19:13:21.419926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_pb2.py
--rw-r--r--   0        0        0     5515 2023-06-06 19:13:21.635926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.419926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.639926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.803926 prodvana-0.1.7/prodvana/proto/prodvana/blobs/__init__.py
--rw-r--r--   0        0        0     2876 2023-06-06 19:13:21.427926 prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
--rw-r--r--   0        0        0     1129 2023-06-06 19:13:21.643926 prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
--rw-r--r--   0        0        0     2704 2023-06-06 19:13:21.431926 prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
--rw-r--r--   0        0        0      895 2023-06-06 19:13:21.643926 prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.819926 prodvana-0.1.7/prodvana/proto/prodvana/capability/__init__.py
--rw-r--r--   0        0        0     6823 2023-06-06 19:13:21.547926 prodvana-0.1.7/prodvana/proto/prodvana/capability/capability_pb2.py
--rw-r--r--   0        0        0     5455 2023-06-06 19:13:21.759926 prodvana-0.1.7/prodvana/proto/prodvana/capability/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.551926 prodvana-0.1.7/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.763926 prodvana-0.1.7/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.803926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-06 19:13:21.443926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
--rw-r--r--   0        0        0      869 2023-06-06 19:13:21.667926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.467926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.647926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
--rw-r--r--   0        0        0     2659 2023-06-06 19:13:21.451926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/env_pb2.py
--rw-r--r--   0        0        0     2017 2023-06-06 19:13:21.683926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/env_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.459926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.663926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
--rw-r--r--   0        0        0     5636 2023-06-06 19:13:21.455926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/helm_pb2.py
--rw-r--r--   0        0        0     5454 2023-06-06 19:13:21.659926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/helm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.455926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.663926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
--rw-r--r--   0        0        0     3658 2023-06-06 19:13:21.439926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
--rw-r--r--   0        0        0     4110 2023-06-06 19:13:21.671926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.467926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.651926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     1890 2023-06-06 19:13:21.463926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/links_pb2.py
--rw-r--r--   0        0        0      846 2023-06-06 19:13:21.679926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/links_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.447926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.663926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
--rw-r--r--   0        0        0     1384 2023-06-06 19:13:21.439926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/maturity_pb2.py
--rw-r--r--   0        0        0     1103 2023-06-06 19:13:21.679926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.435926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.667926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
--rw-r--r--   0        0        0     2541 2023-06-06 19:13:21.431926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/meta_pb2.py
--rw-r--r--   0        0        0     2531 2023-06-06 19:13:21.671926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.431926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.647926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0     2516 2023-06-06 19:13:21.443926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/notification_pb2.py
--rw-r--r--   0        0        0     1337 2023-06-06 19:13:21.651926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.451926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.655926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
--rw-r--r--   0        0        0    12624 2023-06-06 19:13:21.463926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/parameters_pb2.py
--rw-r--r--   0        0        0    10735 2023-06-06 19:13:21.651926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.455926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.683926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    13928 2023-06-06 19:13:21.447926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/program_pb2.py
--rw-r--r--   0        0        0    15915 2023-06-06 19:13:21.659926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/program_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.439926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.667926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
--rw-r--r--   0        0        0     1837 2023-06-06 19:13:21.459926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/ref_pb2.py
--rw-r--r--   0        0        0      743 2023-06-06 19:13:21.655926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/ref_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.447926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.675926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
--rw-r--r--   0        0        0     3229 2023-06-06 19:13:21.451926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/retry_pb2.py
--rw-r--r--   0        0        0     2757 2023-06-06 19:13:21.675926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/retry_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.435926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.647926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
--rw-r--r--   0        0        0     2867 2023-06-06 19:24:01.799926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/task_pb2.py
--rw-r--r--   0        0        0     3495 2023-06-06 19:24:01.799926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.459926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.675926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.823926 prodvana-0.1.7/prodvana/proto/prodvana/config_file/__init__.py
--rw-r--r--   0        0        0     3597 2023-06-06 19:13:21.563926 prodvana-0.1.7/prodvana/proto/prodvana/config_file/config_pb2.py
--rw-r--r--   0        0        0     4171 2023-06-06 19:13:21.775926 prodvana-0.1.7/prodvana/proto/prodvana/config_file/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.563926 prodvana-0.1.7/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.775926 prodvana-0.1.7/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.823926 prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/__init__.py
--rw-r--r--   0        0        0     1648 2023-06-06 19:13:21.567926 prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
--rw-r--r--   0        0        0     1131 2023-06-06 19:13:21.779926 prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.567926 prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.779926 prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.799926 prodvana-0.1.7/prodvana/proto/prodvana/delivery/__init__.py
--rw-r--r--   0        0        0     2652 2023-06-06 19:13:21.427926 prodvana-0.1.7/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
--rw-r--r--   0        0        0     2294 2023-06-06 19:13:21.639926 prodvana-0.1.7/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.423926 prodvana-0.1.7/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.639926 prodvana-0.1.7/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.791926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/__init__.py
--rw-r--r--   0        0        0     7432 2023-06-06 19:13:21.367926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/config_pb2.py
--rw-r--r--   0        0        0     6911 2023-06-06 19:13:21.583926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.363926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.579926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11893 2023-06-06 19:13:21.367926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
--rw-r--r--   0        0        0     7309 2023-06-06 19:13:21.583926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
--rw-r--r--   0        0        0    11002 2023-06-06 19:13:21.363926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3288 2023-06-06 19:13:21.575926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2686 2023-06-06 19:13:21.359926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/object_pb2.py
--rw-r--r--   0        0        0     1862 2023-06-06 19:13:21.579926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.367926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.583926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.791926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/__init__.py
--rw-r--r--   0        0        0    35437 2023-06-06 19:13:21.383926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2.py
--rw-r--r--   0        0        0    28895 2023-06-06 19:13:21.599926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
--rw-r--r--   0        0        0    20037 2023-06-06 19:13:21.383926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
--rw-r--r--   0        0        0     5752 2023-06-06 19:13:21.599926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.791926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/__init__.py
--rw-r--r--   0        0        0    42401 2023-06-06 19:24:01.799926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
--rw-r--r--   0        0        0    70107 2023-06-06 19:24:01.799926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.379926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.591926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
--rw-r--r--   0        0        0     4037 2023-06-06 19:24:01.803926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
--rw-r--r--   0        0        0     7935 2023-06-06 19:24:01.803926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.379926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.595926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.803926 prodvana-0.1.7/prodvana/proto/prodvana/environment/__init__.py
--rw-r--r--   0        0        0    20651 2023-06-06 19:13:21.471926 prodvana-0.1.7/prodvana/proto/prodvana/environment/clusters_pb2.py
--rw-r--r--   0        0        0    27158 2023-06-06 19:13:21.687926 prodvana-0.1.7/prodvana/proto/prodvana/environment/clusters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.471926 prodvana-0.1.7/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.687926 prodvana-0.1.7/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
--rw-r--r--   0        0        0    18211 2023-06-06 19:13:21.471926 prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2.py
--rw-r--r--   0        0        0    14932 2023-06-06 19:13:21.683926 prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
--rw-r--r--   0        0        0    17792 2023-06-06 19:13:21.467926 prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
--rw-r--r--   0        0        0     5195 2023-06-06 19:13:21.687926 prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.795926 prodvana-0.1.7/prodvana/proto/prodvana/events/__init__.py
--rw-r--r--   0        0        0     6416 2023-06-06 19:13:21.387926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2.py
--rw-r--r--   0        0        0     5547 2023-06-06 19:13:21.607926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2.pyi
--rw-r--r--   0        0        0     2714 2023-06-06 19:13:21.391926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
--rw-r--r--   0        0        0      853 2023-06-06 19:13:21.603926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3627 2023-06-06 19:13:21.391926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_pb2.py
--rw-r--r--   0        0        0     4131 2023-06-06 19:13:21.607926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.387926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.599926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
--rw-r--r--   0        0        0    15940 2023-06-06 19:13:21.387926 prodvana-0.1.7/prodvana/proto/prodvana/events/types_pb2.py
--rw-r--r--   0        0        0    30800 2023-06-06 19:13:21.603926 prodvana-0.1.7/prodvana/proto/prodvana/events/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.395926 prodvana-0.1.7/prodvana/proto/prodvana/events/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.607926 prodvana-0.1.7/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.807926 prodvana-0.1.7/prodvana/proto/prodvana/insights/__init__.py
--rw-r--r--   0        0        0     3041 2023-06-06 19:13:21.491926 prodvana-0.1.7/prodvana/proto/prodvana/insights/insights_pb2.py
--rw-r--r--   0        0        0     3508 2023-06-06 19:13:21.707926 prodvana-0.1.7/prodvana/proto/prodvana/insights/insights_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.491926 prodvana-0.1.7/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.707926 prodvana-0.1.7/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.811926 prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/__init__.py
--rw-r--r--   0        0        0    14774 2023-06-06 19:13:21.531926 prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2.py
--rw-r--r--   0        0        0    13338 2023-06-06 19:13:21.743926 prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
--rw-r--r--   0        0        0    12065 2023-06-06 19:13:21.527926 prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3657 2023-06-06 19:13:21.739926 prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.815926 prodvana-0.1.7/prodvana/proto/prodvana/metrics/__init__.py
--rw-r--r--   0        0        0     5507 2023-06-06 19:13:21.531926 prodvana-0.1.7/prodvana/proto/prodvana/metrics/metrics_pb2.py
--rw-r--r--   0        0        0     8746 2023-06-06 19:13:21.743926 prodvana-0.1.7/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.531926 prodvana-0.1.7/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.743926 prodvana-0.1.7/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.795926 prodvana-0.1.7/prodvana/proto/prodvana/object/__init__.py
--rw-r--r--   0        0        0     1844 2023-06-06 19:13:21.415926 prodvana-0.1.7/prodvana/proto/prodvana/object/meta_pb2.py
--rw-r--r--   0        0        0     1957 2023-06-06 19:13:21.627926 prodvana-0.1.7/prodvana/proto/prodvana/object/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.415926 prodvana-0.1.7/prodvana/proto/prodvana/object/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.627926 prodvana-0.1.7/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.811926 prodvana-0.1.7/prodvana/proto/prodvana/organization/__init__.py
--rw-r--r--   0        0        0    16162 2023-06-06 19:13:21.519926 prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2.py
--rw-r--r--   0        0        0     9762 2023-06-06 19:13:21.731926 prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
--rw-r--r--   0        0        0    14668 2023-06-06 19:13:21.523926 prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4779 2023-06-06 19:13:21.735926 prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2859 2023-06-06 19:13:21.519926 prodvana-0.1.7/prodvana/proto/prodvana/organization/user_metadata_pb2.py
--rw-r--r--   0        0        0     1972 2023-06-06 19:13:21.735926 prodvana-0.1.7/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.515926 prodvana-0.1.7/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.731926 prodvana-0.1.7/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.791926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/__init__.py
--rw-r--r--   0        0        0     2598 2023-06-06 19:13:21.371926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/object_pb2.py
--rw-r--r--   0        0        0     2595 2023-06-06 19:13:21.587926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.375926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.591926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    10003 2023-06-06 19:13:21.371926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
--rw-r--r--   0        0        0    11698 2023-06-06 19:13:21.587926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.371926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.587926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.795926 prodvana-0.1.7/prodvana/proto/prodvana/protection/__init__.py
--rw-r--r--   0        0        0     3412 2023-06-06 19:13:21.395926 prodvana-0.1.7/prodvana/proto/prodvana/protection/attachments_pb2.py
--rw-r--r--   0        0        0     2828 2023-06-06 19:13:21.615926 prodvana-0.1.7/prodvana/proto/prodvana/protection/attachments_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.399926 prodvana-0.1.7/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.619926 prodvana-0.1.7/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
--rw-r--r--   0        0        0     1907 2023-06-06 19:13:21.399926 prodvana-0.1.7/prodvana/proto/prodvana/protection/object_pb2.py
--rw-r--r--   0        0        0     1545 2023-06-06 19:13:21.615926 prodvana-0.1.7/prodvana/proto/prodvana/protection/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.407926 prodvana-0.1.7/prodvana/proto/prodvana/protection/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.623926 prodvana-0.1.7/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     8407 2023-06-06 19:13:21.403926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_config_pb2.py
--rw-r--r--   0        0        0     8891 2023-06-06 19:13:21.611926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.407926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.611926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    10471 2023-06-06 19:13:21.403926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2.py
--rw-r--r--   0        0        0     6767 2023-06-06 19:13:21.619926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
--rw-r--r--   0        0        0    10450 2023-06-06 19:13:21.395926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
--rw-r--r--   0        0        0     3113 2023-06-06 19:13:21.623926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     6409 2023-06-06 19:13:21.407926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_reference_pb2.py
--rw-r--r--   0        0        0     4997 2023-06-06 19:13:21.611926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.403926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.619926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.819926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/__init__.py
--rw-r--r--   0        0        0     3574 2023-06-06 19:13:21.559926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/object_pb2.py
--rw-r--r--   0        0        0     3325 2023-06-06 19:13:21.771926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.563926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.775926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    12100 2023-06-06 19:13:21.559926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
--rw-r--r--   0        0        0    12611 2023-06-06 19:13:21.771926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.555926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.767926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11989 2023-06-06 19:13:21.559926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
--rw-r--r--   0        0        0     7509 2023-06-06 19:13:21.771926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
--rw-r--r--   0        0        0    13099 2023-06-06 19:13:21.555926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4150 2023-06-06 19:13:21.767926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.811926 prodvana-0.1.7/prodvana/proto/prodvana/repo/__init__.py
--rw-r--r--   0        0        0     2441 2023-06-06 19:13:21.515926 prodvana-0.1.7/prodvana/proto/prodvana/repo/repo_pb2.py
--rw-r--r--   0        0        0     2315 2023-06-06 19:13:21.727926 prodvana-0.1.7/prodvana/proto/prodvana/repo/repo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.515926 prodvana-0.1.7/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.731926 prodvana-0.1.7/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.807926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/__init__.py
--rw-r--r--   0        0        0     1551 2023-06-06 19:13:21.507926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/features_pb2.py
--rw-r--r--   0        0        0     1320 2023-06-06 19:13:21.727926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/features_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.511926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.727926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
--rw-r--r--   0        0        0     7542 2023-06-06 19:13:21.511926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
--rw-r--r--   0        0        0     6671 2023-06-06 19:13:21.723926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.511926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.723926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.815926 prodvana-0.1.7/prodvana/proto/prodvana/scm/__init__.py
--rw-r--r--   0        0        0     1265 2023-06-06 19:13:21.535926 prodvana-0.1.7/prodvana/proto/prodvana/scm/types_pb2.py
--rw-r--r--   0        0        0      914 2023-06-06 19:13:21.747926 prodvana-0.1.7/prodvana/proto/prodvana/scm/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.539926 prodvana-0.1.7/prodvana/proto/prodvana/scm/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.751926 prodvana-0.1.7/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.811926 prodvana-0.1.7/prodvana/proto/prodvana/secrets/__init__.py
--rw-r--r--   0        0        0    10074 2023-06-06 19:13:21.523926 prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
--rw-r--r--   0        0        0     4586 2023-06-06 19:13:21.739926 prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
--rw-r--r--   0        0        0     9936 2023-06-06 19:13:21.527926 prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
--rw-r--r--   0        0        0     2847 2023-06-06 19:13:21.735926 prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.803926 prodvana-0.1.7/prodvana/proto/prodvana/service/__init__.py
--rw-r--r--   0        0        0     5498 2023-06-06 19:13:21.475926 prodvana-0.1.7/prodvana/proto/prodvana/service/object_pb2.py
--rw-r--r--   0        0        0     5760 2023-06-06 19:13:21.695926 prodvana-0.1.7/prodvana/proto/prodvana/service/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.487926 prodvana-0.1.7/prodvana/proto/prodvana/service/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.703926 prodvana-0.1.7/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2655 2023-06-06 19:13:21.487926 prodvana-0.1.7/prodvana/proto/prodvana/service/parameters_pb2.py
--rw-r--r--   0        0        0     2424 2023-06-06 19:13:21.695926 prodvana-0.1.7/prodvana/proto/prodvana/service/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.483926 prodvana-0.1.7/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.703926 prodvana-0.1.7/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    34047 2023-06-06 19:24:01.803926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_config_pb2.py
--rw-r--r--   0        0        0    47738 2023-06-06 19:24:01.803926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.479926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.699926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    47994 2023-06-06 19:13:21.483926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2.py
--rw-r--r--   0        0        0    38013 2023-06-06 19:13:21.695926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2.pyi
--rw-r--r--   0        0        0    33828 2023-06-06 19:13:21.479926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
--rw-r--r--   0        0        0     9674 2023-06-06 19:13:21.691926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2934 2023-06-06 19:13:21.479926 prodvana-0.1.7/prodvana/proto/prodvana/service/user_metadata_pb2.py
--rw-r--r--   0        0        0     2106 2023-06-06 19:13:21.703926 prodvana-0.1.7/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.475926 prodvana-0.1.7/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.691926 prodvana-0.1.7/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.815926 prodvana-0.1.7/prodvana/proto/prodvana/settings/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.819926 prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/__init__.py
--rw-r--r--   0        0        0     8509 2023-06-06 19:13:21.547926 prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2.py
--rw-r--r--   0        0        0     5677 2023-06-06 19:13:21.759926 prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
--rw-r--r--   0        0        0     8214 2023-06-06 19:13:21.547926 prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
--rw-r--r--   0        0        0     2318 2023-06-06 19:13:21.759926 prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.787926 prodvana-0.1.7/prodvana/proto/prodvana/stat/__init__.py
--rw-r--r--   0        0        0     1530 2023-06-06 19:13:21.359926 prodvana-0.1.7/prodvana/proto/prodvana/stat/efficiency_pb2.py
--rw-r--r--   0        0        0     1156 2023-06-06 19:13:21.575926 prodvana-0.1.7/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.359926 prodvana-0.1.7/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.575926 prodvana-0.1.7/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.795926 prodvana-0.1.7/prodvana/proto/prodvana/template/__init__.py
--rw-r--r--   0        0        0     2429 2023-06-06 19:13:21.411926 prodvana-0.1.7/prodvana/proto/prodvana/template/service_pb2.py
--rw-r--r--   0        0        0     1768 2023-06-06 19:13:21.623926 prodvana-0.1.7/prodvana/proto/prodvana/template/service_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.411926 prodvana-0.1.7/prodvana/proto/prodvana/template/service_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.627926 prodvana-0.1.7/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.807926 prodvana-0.1.7/prodvana/proto/prodvana/users/__init__.py
--rw-r--r--   0        0        0     1505 2023-06-06 19:13:21.507926 prodvana-0.1.7/prodvana/proto/prodvana/users/users_pb2.py
--rw-r--r--   0        0        0     1451 2023-06-06 19:13:21.723926 prodvana-0.1.7/prodvana/proto/prodvana/users/users_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.503926 prodvana-0.1.7/prodvana/proto/prodvana/users/users_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.719926 prodvana-0.1.7/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.815926 prodvana-0.1.7/prodvana/proto/prodvana/version/__init__.py
--rw-r--r--   0        0        0     2142 2023-06-06 19:13:21.535926 prodvana-0.1.7/prodvana/proto/prodvana/version/source_metadata_pb2.py
--rw-r--r--   0        0        0     2646 2023-06-06 19:13:21.747926 prodvana-0.1.7/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.535926 prodvana-0.1.7/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.747926 prodvana-0.1.7/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.819926 prodvana-0.1.7/prodvana/proto/prodvana/volumes/__init__.py
--rw-r--r--   0        0        0     4805 2023-06-06 19:13:21.555926 prodvana-0.1.7/prodvana/proto/prodvana/volumes/volumes_pb2.py
--rw-r--r--   0        0        0     4793 2023-06-06 19:13:21.763926 prodvana-0.1.7/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.551926 prodvana-0.1.7/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.763926 prodvana-0.1.7/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.815926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/__init__.py
--rw-r--r--   0        0        0     5412 2023-06-06 19:13:21.543926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/integration_config_pb2.py
--rw-r--r--   0        0        0     4328 2023-06-06 19:13:21.755926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.539926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.755926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    69010 2023-06-06 19:13:21.539926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
--rw-r--r--   0        0        0    50096 2023-06-06 19:13:21.751926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
--rw-r--r--   0        0        0    55859 2023-06-06 19:13:21.543926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
--rw-r--r--   0        0        0    16155 2023-06-06 19:13:21.755926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-06 19:13:21.823926 prodvana-0.1.7/prodvana/proto/validate/__init__.py
--rw-r--r--   0        0        0    21204 2023-06-06 19:13:21.571926 prodvana-0.1.7/prodvana/proto/validate/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-06-06 19:13:21.783926 prodvana-0.1.7/prodvana/proto/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-06 19:13:21.571926 prodvana-0.1.7/prodvana/proto/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-06 19:13:21.779926 prodvana-0.1.7/prodvana/proto/validate/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-31 21:06:51.289690 prodvana-0.1.7/prodvana/py.typed
--rw-r--r--   0        0        0        0 2023-05-31 21:06:51.289690 prodvana-0.1.7/prodvana/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-05-31 21:06:51.289690 prodvana-0.1.7/prodvana/utils/desired_states.py
--rw-r--r--   0        0        0     4079 2023-05-31 21:06:51.289690 prodvana-0.1.7/prodvana/utils/service_config.py
--rw-r--r--   0        0        0     7140 2023-05-31 21:06:51.289690 prodvana-0.1.7/prodvana/utils/tests/test_service_config.py
--rw-r--r--   0        0        0      746 2023-06-06 20:21:45.831926 prodvana-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       81 2023-05-30 13:39:12.483857 prodvana-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 13:39:12.483857 prodvana-0.1.8/prodvana/__init__.py
+-rw-r--r--   0        0        0     3529 2023-05-30 13:39:12.483857 prodvana-0.1.8/prodvana/client.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:26.990113 prodvana-0.1.8/prodvana/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:26.990113 prodvana-0.1.8/prodvana/proto/prodvana/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.018113 prodvana-0.1.8/prodvana/proto/prodvana/agent/__init__.py
+-rw-r--r--   0        0        0    19183 2023-06-06 23:34:26.678113 prodvana-0.1.8/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
+-rw-r--r--   0        0        0    18983 2023-06-06 23:34:26.926113 prodvana-0.1.8/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
+-rw-r--r--   0        0        0    22573 2023-06-06 23:34:26.678113 prodvana-0.1.8/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
+-rw-r--r--   0        0        0     6760 2023-06-06 23:34:26.926113 prodvana-0.1.8/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:26.994113 prodvana-0.1.8/prodvana/proto/prodvana/application/__init__.py
+-rw-r--r--   0        0        0     4200 2023-06-06 23:34:26.522113 prodvana-0.1.8/prodvana/proto/prodvana/application/application_config_pb2.py
+-rw-r--r--   0        0        0     4693 2023-06-06 23:34:26.794113 prodvana-0.1.8/prodvana/proto/prodvana/application/application_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.522113 prodvana-0.1.8/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.794113 prodvana-0.1.8/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    24873 2023-06-06 23:34:26.526113 prodvana-0.1.8/prodvana/proto/prodvana/application/application_manager_pb2.py
+-rw-r--r--   0        0        0    16394 2023-06-06 23:34:26.798113 prodvana-0.1.8/prodvana/proto/prodvana/application/application_manager_pb2.pyi
+-rw-r--r--   0        0        0    22241 2023-06-06 23:34:26.518113 prodvana-0.1.8/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6755 2023-06-06 23:34:26.806113 prodvana-0.1.8/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2801 2023-06-06 23:34:26.514113 prodvana-0.1.8/prodvana/proto/prodvana/application/object_pb2.py
+-rw-r--r--   0        0        0     2184 2023-06-06 23:34:26.802113 prodvana-0.1.8/prodvana/proto/prodvana/application/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.518113 prodvana-0.1.8/prodvana/proto/prodvana/application/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.798113 prodvana-0.1.8/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2294 2023-06-06 23:34:26.526113 prodvana-0.1.8/prodvana/proto/prodvana/application/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1670 2023-06-06 23:34:26.798113 prodvana-0.1.8/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.518113 prodvana-0.1.8/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.802113 prodvana-0.1.8/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.026113 prodvana-0.1.8/prodvana/proto/prodvana/auth/__init__.py
+-rw-r--r--   0        0        0    13908 2023-06-06 23:34:26.710113 prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_manager_pb2.py
+-rw-r--r--   0        0        0    10206 2023-06-06 23:34:26.958113 prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
+-rw-r--r--   0        0        0    18631 2023-06-06 23:34:26.718113 prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6767 2023-06-06 23:34:26.962113 prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5071 2023-06-06 23:34:26.714113 prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_pb2.py
+-rw-r--r--   0        0        0     5515 2023-06-06 23:34:26.962113 prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.714113 prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.958113 prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.018113 prodvana-0.1.8/prodvana/proto/prodvana/blobs/__init__.py
+-rw-r--r--   0        0        0     2876 2023-06-06 23:34:26.666113 prodvana-0.1.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
+-rw-r--r--   0        0        0     1129 2023-06-06 23:34:26.914113 prodvana-0.1.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
+-rw-r--r--   0        0        0     2704 2023-06-06 23:34:26.662113 prodvana-0.1.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      895 2023-06-06 23:34:26.914113 prodvana-0.1.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.006113 prodvana-0.1.8/prodvana/proto/prodvana/capability/__init__.py
+-rw-r--r--   0        0        0     6823 2023-06-06 23:34:26.578113 prodvana-0.1.8/prodvana/proto/prodvana/capability/capability_pb2.py
+-rw-r--r--   0        0        0     5455 2023-06-06 23:34:26.858113 prodvana-0.1.8/prodvana/proto/prodvana/capability/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.578113 prodvana-0.1.8/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.858113 prodvana-0.1.8/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:26.994113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-06 23:34:26.482113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
+-rw-r--r--   0        0        0      869 2023-06-06 23:34:26.754113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.506113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.770113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2659 2023-06-06 23:34:26.494113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/env_pb2.py
+-rw-r--r--   0        0        0     2017 2023-06-06 23:34:26.778113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/env_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.478113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.758113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5636 2023-06-06 23:34:26.506113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/helm_pb2.py
+-rw-r--r--   0        0        0     5454 2023-06-06 23:34:26.750113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/helm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.498113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.778113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3849 2023-06-07 20:08:35.728048 prodvana-0.1.8/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
+-rw-r--r--   0        0        0     4110 2023-06-06 23:34:26.786113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.510113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.766113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1890 2023-06-06 23:34:26.490113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/links_pb2.py
+-rw-r--r--   0        0        0      846 2023-06-06 23:34:26.762113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/links_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.514113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.762113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1384 2023-06-06 23:34:26.486113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/maturity_pb2.py
+-rw-r--r--   0        0        0     1103 2023-06-06 23:34:26.758113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.482113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.782113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2541 2023-06-06 23:34:26.474113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/meta_pb2.py
+-rw-r--r--   0        0        0     2531 2023-06-06 23:34:26.774113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.502113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.774113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2516 2023-06-06 23:34:26.478113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/notification_pb2.py
+-rw-r--r--   0        0        0     1337 2023-06-06 23:34:26.786113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.510113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.766113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12624 2023-06-06 23:34:26.474113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/parameters_pb2.py
+-rw-r--r--   0        0        0    10735 2023-06-06 23:34:26.786113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.502113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.778113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13928 2023-06-06 23:34:26.486113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/program_pb2.py
+-rw-r--r--   0        0        0    15915 2023-06-06 23:34:26.754113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/program_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.474113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.790113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1837 2023-06-06 23:34:26.510113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/ref_pb2.py
+-rw-r--r--   0        0        0      743 2023-06-06 23:34:26.770113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/ref_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.494113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.762113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3229 2023-06-06 23:34:26.494113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/retry_pb2.py
+-rw-r--r--   0        0        0     2757 2023-06-06 23:34:26.770113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/retry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.502113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.790113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2867 2023-06-06 23:34:26.490113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/task_pb2.py
+-rw-r--r--   0        0        0     3495 2023-06-06 23:34:26.782113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.482113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.754113 prodvana-0.1.8/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.002113 prodvana-0.1.8/prodvana/proto/prodvana/config_file/__init__.py
+-rw-r--r--   0        0        0     3597 2023-06-06 23:34:26.566113 prodvana-0.1.8/prodvana/proto/prodvana/config_file/config_pb2.py
+-rw-r--r--   0        0        0     4171 2023-06-06 23:34:26.846113 prodvana-0.1.8/prodvana/proto/prodvana/config_file/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.566113 prodvana-0.1.8/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.846113 prodvana-0.1.8/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.014113 prodvana-0.1.8/prodvana/proto/prodvana/config_writeback/__init__.py
+-rw-r--r--   0        0        0     1648 2023-06-06 23:34:26.654113 prodvana-0.1.8/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
+-rw-r--r--   0        0        0     1131 2023-06-06 23:34:26.902113 prodvana-0.1.8/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.654113 prodvana-0.1.8/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.902113 prodvana-0.1.8/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.018113 prodvana-0.1.8/prodvana/proto/prodvana/delivery/__init__.py
+-rw-r--r--   0        0        0     2652 2023-06-06 23:34:26.662113 prodvana-0.1.8/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
+-rw-r--r--   0        0        0     2294 2023-06-06 23:34:26.910113 prodvana-0.1.8/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.662113 prodvana-0.1.8/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.910113 prodvana-0.1.8/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.018113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/__init__.py
+-rw-r--r--   0        0        0     7432 2023-06-06 23:34:26.670113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/config_pb2.py
+-rw-r--r--   0        0        0     6911 2023-06-06 23:34:26.918113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.674113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.914113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11893 2023-06-06 23:34:26.678113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
+-rw-r--r--   0        0        0     7309 2023-06-06 23:34:26.922113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
+-rw-r--r--   0        0        0    11002 2023-06-06 23:34:26.674113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3288 2023-06-06 23:34:26.922113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2686 2023-06-06 23:34:26.666113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/object_pb2.py
+-rw-r--r--   0        0        0     1862 2023-06-06 23:34:26.922113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.670113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.918113 prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.006113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/__init__.py
+-rw-r--r--   0        0        0    35437 2023-06-06 23:34:26.582113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/manager_pb2.py
+-rw-r--r--   0        0        0    28895 2023-06-06 23:34:26.862113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
+-rw-r--r--   0        0        0    20037 2023-06-06 23:34:26.582113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5752 2023-06-06 23:34:26.862113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.010113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/__init__.py
+-rw-r--r--   0        0        0    42401 2023-06-06 23:34:26.590113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
+-rw-r--r--   0        0        0    70107 2023-06-06 23:34:26.866113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.586113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.870113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4037 2023-06-06 23:34:26.586113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
+-rw-r--r--   0        0        0     7935 2023-06-06 23:34:26.870113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.590113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.866113 prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.014113 prodvana-0.1.8/prodvana/proto/prodvana/environment/__init__.py
+-rw-r--r--   0        0        0    20651 2023-06-06 23:34:26.654113 prodvana-0.1.8/prodvana/proto/prodvana/environment/clusters_pb2.py
+-rw-r--r--   0        0        0    27158 2023-06-06 23:34:26.894113 prodvana-0.1.8/prodvana/proto/prodvana/environment/clusters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.646113 prodvana-0.1.8/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.894113 prodvana-0.1.8/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18211 2023-06-06 23:34:26.650113 prodvana-0.1.8/prodvana/proto/prodvana/environment/environment_manager_pb2.py
+-rw-r--r--   0        0        0    14932 2023-06-06 23:34:26.898113 prodvana-0.1.8/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
+-rw-r--r--   0        0        0    17792 2023-06-06 23:34:26.650113 prodvana-0.1.8/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5195 2023-06-06 23:34:26.894113 prodvana-0.1.8/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.026113 prodvana-0.1.8/prodvana/proto/prodvana/events/__init__.py
+-rw-r--r--   0        0        0     6416 2023-06-06 23:34:26.734113 prodvana-0.1.8/prodvana/proto/prodvana/events/events_manager_pb2.py
+-rw-r--r--   0        0        0     5547 2023-06-06 23:34:26.974113 prodvana-0.1.8/prodvana/proto/prodvana/events/events_manager_pb2.pyi
+-rw-r--r--   0        0        0     2714 2023-06-06 23:34:26.726113 prodvana-0.1.8/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      853 2023-06-06 23:34:26.982113 prodvana-0.1.8/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3627 2023-06-06 23:34:26.734113 prodvana-0.1.8/prodvana/proto/prodvana/events/events_pb2.py
+-rw-r--r--   0        0        0     4131 2023-06-06 23:34:26.982113 prodvana-0.1.8/prodvana/proto/prodvana/events/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.734113 prodvana-0.1.8/prodvana/proto/prodvana/events/events_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.974113 prodvana-0.1.8/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15940 2023-06-06 23:34:26.730113 prodvana-0.1.8/prodvana/proto/prodvana/events/types_pb2.py
+-rw-r--r--   0        0        0    30800 2023-06-06 23:34:26.978113 prodvana-0.1.8/prodvana/proto/prodvana/events/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.730113 prodvana-0.1.8/prodvana/proto/prodvana/events/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.978113 prodvana-0.1.8/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.014113 prodvana-0.1.8/prodvana/proto/prodvana/insights/__init__.py
+-rw-r--r--   0        0        0     3041 2023-06-06 23:34:26.658113 prodvana-0.1.8/prodvana/proto/prodvana/insights/insights_pb2.py
+-rw-r--r--   0        0        0     3508 2023-06-06 23:34:26.902113 prodvana-0.1.8/prodvana/proto/prodvana/insights/insights_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.658113 prodvana-0.1.8/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.906113 prodvana-0.1.8/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.002113 prodvana-0.1.8/prodvana/proto/prodvana/managed_resource/__init__.py
+-rw-r--r--   0        0        0    14774 2023-06-06 23:34:26.570113 prodvana-0.1.8/prodvana/proto/prodvana/managed_resource/manager_pb2.py
+-rw-r--r--   0        0        0    13338 2023-06-06 23:34:26.850113 prodvana-0.1.8/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
+-rw-r--r--   0        0        0    12065 2023-06-06 23:34:26.570113 prodvana-0.1.8/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3657 2023-06-06 23:34:26.850113 prodvana-0.1.8/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.026113 prodvana-0.1.8/prodvana/proto/prodvana/metrics/__init__.py
+-rw-r--r--   0        0        0     5507 2023-06-06 23:34:26.726113 prodvana-0.1.8/prodvana/proto/prodvana/metrics/metrics_pb2.py
+-rw-r--r--   0        0        0     8746 2023-06-06 23:34:26.974113 prodvana-0.1.8/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.726113 prodvana-0.1.8/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.970113 prodvana-0.1.8/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.022113 prodvana-0.1.8/prodvana/proto/prodvana/object/__init__.py
+-rw-r--r--   0        0        0     1844 2023-06-06 23:34:26.686113 prodvana-0.1.8/prodvana/proto/prodvana/object/meta_pb2.py
+-rw-r--r--   0        0        0     1957 2023-06-06 23:34:26.934113 prodvana-0.1.8/prodvana/proto/prodvana/object/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.690113 prodvana-0.1.8/prodvana/proto/prodvana/object/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.930113 prodvana-0.1.8/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.010113 prodvana-0.1.8/prodvana/proto/prodvana/organization/__init__.py
+-rw-r--r--   0        0        0    16162 2023-06-06 23:34:26.626113 prodvana-0.1.8/prodvana/proto/prodvana/organization/organization_manager_pb2.py
+-rw-r--r--   0        0        0     9762 2023-06-06 23:34:26.874113 prodvana-0.1.8/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
+-rw-r--r--   0        0        0    14668 2023-06-06 23:34:26.590113 prodvana-0.1.8/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4779 2023-06-06 23:34:26.878113 prodvana-0.1.8/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2859 2023-06-06 23:34:26.630113 prodvana-0.1.8/prodvana/proto/prodvana/organization/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1972 2023-06-06 23:34:26.874113 prodvana-0.1.8/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.594113 prodvana-0.1.8/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.874113 prodvana-0.1.8/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:26.998113 prodvana-0.1.8/prodvana/proto/prodvana/pipelines/__init__.py
+-rw-r--r--   0        0        0     2598 2023-06-06 23:34:26.554113 prodvana-0.1.8/prodvana/proto/prodvana/pipelines/object_pb2.py
+-rw-r--r--   0        0        0     2595 2023-06-06 23:34:26.842113 prodvana-0.1.8/prodvana/proto/prodvana/pipelines/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.558113 prodvana-0.1.8/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.838113 prodvana-0.1.8/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10003 2023-06-06 23:34:26.562113 prodvana-0.1.8/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
+-rw-r--r--   0        0        0    11698 2023-06-06 23:34:26.834113 prodvana-0.1.8/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.558113 prodvana-0.1.8/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.838113 prodvana-0.1.8/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:26.998113 prodvana-0.1.8/prodvana/proto/prodvana/protection/__init__.py
+-rw-r--r--   0        0        0     3412 2023-06-06 23:34:26.538113 prodvana-0.1.8/prodvana/proto/prodvana/protection/attachments_pb2.py
+-rw-r--r--   0        0        0     2828 2023-06-06 23:34:26.806113 prodvana-0.1.8/prodvana/proto/prodvana/protection/attachments_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.542113 prodvana-0.1.8/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.818113 prodvana-0.1.8/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1907 2023-06-06 23:34:26.526113 prodvana-0.1.8/prodvana/proto/prodvana/protection/object_pb2.py
+-rw-r--r--   0        0        0     1545 2023-06-06 23:34:26.822113 prodvana-0.1.8/prodvana/proto/prodvana/protection/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.530113 prodvana-0.1.8/prodvana/proto/prodvana/protection/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.814113 prodvana-0.1.8/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8407 2023-06-06 23:34:26.534113 prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_config_pb2.py
+-rw-r--r--   0        0        0     8891 2023-06-06 23:34:26.810113 prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.538113 prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.810113 prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10471 2023-06-06 23:34:26.542113 prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_manager_pb2.py
+-rw-r--r--   0        0        0     6767 2023-06-06 23:34:26.814113 prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
+-rw-r--r--   0        0        0    10450 2023-06-06 23:34:26.530113 prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3113 2023-06-06 23:34:26.810113 prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6409 2023-06-06 23:34:26.538113 prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_reference_pb2.py
+-rw-r--r--   0        0        0     4997 2023-06-06 23:34:26.818113 prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.534113 prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.822113 prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:26.998113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/__init__.py
+-rw-r--r--   0        0        0     3574 2023-06-06 23:34:26.546113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/object_pb2.py
+-rw-r--r--   0        0        0     3325 2023-06-06 23:34:26.834113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.546113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.826113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12100 2023-06-06 23:34:26.554113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
+-rw-r--r--   0        0        0    12611 2023-06-06 23:34:26.830113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.550113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.830113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11989 2023-06-06 23:34:26.550113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
+-rw-r--r--   0        0        0     7509 2023-06-06 23:34:26.826113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
+-rw-r--r--   0        0        0    13099 2023-06-06 23:34:26.550113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4150 2023-06-06 23:34:26.826113 prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.006113 prodvana-0.1.8/prodvana/proto/prodvana/repo/__init__.py
+-rw-r--r--   0        0        0     2441 2023-06-06 23:34:26.574113 prodvana-0.1.8/prodvana/proto/prodvana/repo/repo_pb2.py
+-rw-r--r--   0        0        0     2315 2023-06-06 23:34:26.854113 prodvana-0.1.8/prodvana/proto/prodvana/repo/repo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.570113 prodvana-0.1.8/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.854113 prodvana-0.1.8/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.026113 prodvana-0.1.8/prodvana/proto/prodvana/runtimes/__init__.py
+-rw-r--r--   0        0        0     1551 2023-06-06 23:34:26.718113 prodvana-0.1.8/prodvana/proto/prodvana/runtimes/features_pb2.py
+-rw-r--r--   0        0        0     1320 2023-06-06 23:34:26.966113 prodvana-0.1.8/prodvana/proto/prodvana/runtimes/features_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.722113 prodvana-0.1.8/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.962113 prodvana-0.1.8/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7542 2023-06-06 23:34:26.718113 prodvana-0.1.8/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
+-rw-r--r--   0        0        0     6671 2023-06-06 23:34:26.970113 prodvana-0.1.8/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.722113 prodvana-0.1.8/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.966113 prodvana-0.1.8/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.006113 prodvana-0.1.8/prodvana/proto/prodvana/scm/__init__.py
+-rw-r--r--   0        0        0     1265 2023-06-06 23:34:26.578113 prodvana-0.1.8/prodvana/proto/prodvana/scm/types_pb2.py
+-rw-r--r--   0        0        0      914 2023-06-06 23:34:26.854113 prodvana-0.1.8/prodvana/proto/prodvana/scm/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.574113 prodvana-0.1.8/prodvana/proto/prodvana/scm/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.858113 prodvana-0.1.8/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.022113 prodvana-0.1.8/prodvana/proto/prodvana/secrets/__init__.py
+-rw-r--r--   0        0        0    10074 2023-06-06 23:34:26.694113 prodvana-0.1.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
+-rw-r--r--   0        0        0     4586 2023-06-06 23:34:26.934113 prodvana-0.1.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
+-rw-r--r--   0        0        0     9936 2023-06-06 23:34:26.690113 prodvana-0.1.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     2847 2023-06-06 23:34:26.938113 prodvana-0.1.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.022113 prodvana-0.1.8/prodvana/proto/prodvana/service/__init__.py
+-rw-r--r--   0        0        0     5498 2023-06-06 23:34:26.698113 prodvana-0.1.8/prodvana/proto/prodvana/service/object_pb2.py
+-rw-r--r--   0        0        0     5760 2023-06-06 23:34:26.954113 prodvana-0.1.8/prodvana/proto/prodvana/service/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.702113 prodvana-0.1.8/prodvana/proto/prodvana/service/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.946113 prodvana-0.1.8/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2655 2023-06-06 23:34:26.694113 prodvana-0.1.8/prodvana/proto/prodvana/service/parameters_pb2.py
+-rw-r--r--   0        0        0     2424 2023-06-06 23:34:26.954113 prodvana-0.1.8/prodvana/proto/prodvana/service/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.710113 prodvana-0.1.8/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.950113 prodvana-0.1.8/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    34055 2023-06-07 20:08:35.728048 prodvana-0.1.8/prodvana/proto/prodvana/service/service_config_pb2.py
+-rw-r--r--   0        0        0    47738 2023-06-06 23:34:26.938113 prodvana-0.1.8/prodvana/proto/prodvana/service/service_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.706113 prodvana-0.1.8/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.942113 prodvana-0.1.8/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    47994 2023-06-06 23:34:26.698113 prodvana-0.1.8/prodvana/proto/prodvana/service/service_manager_pb2.py
+-rw-r--r--   0        0        0    38013 2023-06-06 23:34:26.950113 prodvana-0.1.8/prodvana/proto/prodvana/service/service_manager_pb2.pyi
+-rw-r--r--   0        0        0    33828 2023-06-06 23:34:26.706113 prodvana-0.1.8/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     9674 2023-06-06 23:34:26.942113 prodvana-0.1.8/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2934 2023-06-06 23:34:26.710113 prodvana-0.1.8/prodvana/proto/prodvana/service/user_metadata_pb2.py
+-rw-r--r--   0        0        0     2106 2023-06-06 23:34:26.942113 prodvana-0.1.8/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.702113 prodvana-0.1.8/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.954113 prodvana-0.1.8/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:26.998113 prodvana-0.1.8/prodvana/proto/prodvana/settings/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.002113 prodvana-0.1.8/prodvana/proto/prodvana/settings/organization/__init__.py
+-rw-r--r--   0        0        0     8509 2023-06-06 23:34:26.562113 prodvana-0.1.8/prodvana/proto/prodvana/settings/organization/users_pb2.py
+-rw-r--r--   0        0        0     5677 2023-06-06 23:34:26.842113 prodvana-0.1.8/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
+-rw-r--r--   0        0        0     8214 2023-06-06 23:34:26.562113 prodvana-0.1.8/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
+-rw-r--r--   0        0        0     2318 2023-06-06 23:34:26.842113 prodvana-0.1.8/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:26.994113 prodvana-0.1.8/prodvana/proto/prodvana/stat/__init__.py
+-rw-r--r--   0        0        0     1530 2023-06-06 23:34:26.470113 prodvana-0.1.8/prodvana/proto/prodvana/stat/efficiency_pb2.py
+-rw-r--r--   0        0        0     1156 2023-06-06 23:34:26.746113 prodvana-0.1.8/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.470113 prodvana-0.1.8/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.750113 prodvana-0.1.8/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.014113 prodvana-0.1.8/prodvana/proto/prodvana/template/__init__.py
+-rw-r--r--   0        0        0     2429 2023-06-06 23:34:26.646113 prodvana-0.1.8/prodvana/proto/prodvana/template/service_pb2.py
+-rw-r--r--   0        0        0     1768 2023-06-06 23:34:26.890113 prodvana-0.1.8/prodvana/proto/prodvana/template/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.642113 prodvana-0.1.8/prodvana/proto/prodvana/template/service_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.890113 prodvana-0.1.8/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.022113 prodvana-0.1.8/prodvana/proto/prodvana/users/__init__.py
+-rw-r--r--   0        0        0     1505 2023-06-06 23:34:26.686113 prodvana-0.1.8/prodvana/proto/prodvana/users/users_pb2.py
+-rw-r--r--   0        0        0     1451 2023-06-06 23:34:26.930113 prodvana-0.1.8/prodvana/proto/prodvana/users/users_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.682113 prodvana-0.1.8/prodvana/proto/prodvana/users/users_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.930113 prodvana-0.1.8/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:26.994113 prodvana-0.1.8/prodvana/proto/prodvana/version/__init__.py
+-rw-r--r--   0        0        0     2142 2023-06-06 23:34:26.466113 prodvana-0.1.8/prodvana/proto/prodvana/version/source_metadata_pb2.py
+-rw-r--r--   0        0        0     2646 2023-06-06 23:34:26.746113 prodvana-0.1.8/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.466113 prodvana-0.1.8/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.746113 prodvana-0.1.8/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.010113 prodvana-0.1.8/prodvana/proto/prodvana/volumes/__init__.py
+-rw-r--r--   0        0        0     4805 2023-06-06 23:34:26.642113 prodvana-0.1.8/prodvana/proto/prodvana/volumes/volumes_pb2.py
+-rw-r--r--   0        0        0     4793 2023-06-06 23:34:26.886113 prodvana-0.1.8/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.638113 prodvana-0.1.8/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.886113 prodvana-0.1.8/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.010113 prodvana-0.1.8/prodvana/proto/prodvana/workflow/__init__.py
+-rw-r--r--   0        0        0     5412 2023-06-06 23:34:26.634113 prodvana-0.1.8/prodvana/proto/prodvana/workflow/integration_config_pb2.py
+-rw-r--r--   0        0        0     4328 2023-06-06 23:34:26.882113 prodvana-0.1.8/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.630113 prodvana-0.1.8/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.886113 prodvana-0.1.8/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    69010 2023-06-06 23:34:26.634113 prodvana-0.1.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
+-rw-r--r--   0        0        0    50096 2023-06-06 23:34:26.882113 prodvana-0.1.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
+-rw-r--r--   0        0        0    55859 2023-06-06 23:34:26.638113 prodvana-0.1.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
+-rw-r--r--   0        0        0    16155 2023-06-06 23:34:26.878113 prodvana-0.1.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 23:34:27.030113 prodvana-0.1.8/prodvana/proto/validate/__init__.py
+-rw-r--r--   0        0        0    21204 2023-06-06 23:34:26.742113 prodvana-0.1.8/prodvana/proto/validate/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-06-06 23:34:26.986113 prodvana-0.1.8/prodvana/proto/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 23:34:26.738113 prodvana-0.1.8/prodvana/proto/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 23:34:26.982113 prodvana-0.1.8/prodvana/proto/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-30 13:39:12.503857 prodvana-0.1.8/prodvana/py.typed
+-rw-r--r--   0        0        0        0 2023-05-30 13:39:12.503857 prodvana-0.1.8/prodvana/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-05-30 13:39:12.503857 prodvana-0.1.8/prodvana/utils/desired_states.py
+-rw-r--r--   0        0        0     4079 2023-05-30 13:39:12.503857 prodvana-0.1.8/prodvana/utils/service_config.py
+-rw-r--r--   0        0        0     7140 2023-05-30 13:39:12.503857 prodvana-0.1.8/prodvana/utils/tests/test_service_config.py
+-rw-r--r--   0        0        0      746 2023-06-07 20:52:09.016021 prodvana-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.1.8/PKG-INFO
```

### Comparing `prodvana-0.1.7/prodvana/client.py` & `prodvana-0.1.8/prodvana/client.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/agent/agent_interaction_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/application/application_config_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/application/application_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/application/application_config_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/application/application_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/application/application_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/application/application_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/application/object_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/application/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/application/object_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/application/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/application/user_metadata_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/application/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/application/user_metadata_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/application/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/auth/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/capability/capability_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/capability/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/capability/capability_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/capability/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/env_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/env_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/env_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/env_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/helm_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/helm_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/helm_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/helm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.prodvana/common_config/kubernetes_config.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\"$\n\x0bLocalConfig\x12\x15\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\xa5\x03\n\x10KubernetesConfig\x12;\n\x04type\x18\x01 \x01(\x0e\x32-.prodvana.common_config.KubernetesConfig.Type\x12\x1a\n\x07inlined\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12\x34\n\x05local\x18\x03 \x01(\x0b\x32#.prodvana.common_config.LocalConfigH\x00\x12U\n\x12\x65nv_injection_mode\x18\x04 \x01(\x0e\x32\x39.prodvana.common_config.KubernetesConfig.EnvInjectionMode\"2\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nKUBERNETES\x10\x01\x12\r\n\tKUSTOMIZE\x10\x02\"b\n\x10\x45nvInjectionMode\x12\x16\n\x12\x45NV_INJECT_UNKNOWN\x10\x00\x12\x17\n\x13\x45NV_INJECT_DISABLED\x10\x01\x12\x1d\n\x19\x45NV_INJECT_NON_SECRET_ENV\x10\x02\x42\x13\n\x0csource_oneof\x12\x03\xf8\x42\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.prodvana/common_config/kubernetes_config.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\"$\n\x0bLocalConfig\x12\x15\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\xaf\x03\n\x10KubernetesConfig\x12\x45\n\x04type\x18\x01 \x01(\x0e\x32-.prodvana.common_config.KubernetesConfig.TypeB\x08\xfa\x42\x05\x82\x01\x02 \x00\x12\x1a\n\x07inlined\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12\x34\n\x05local\x18\x03 \x01(\x0b\x32#.prodvana.common_config.LocalConfigH\x00\x12U\n\x12\x65nv_injection_mode\x18\x04 \x01(\x0e\x32\x39.prodvana.common_config.KubernetesConfig.EnvInjectionMode\"2\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nKUBERNETES\x10\x01\x12\r\n\tKUSTOMIZE\x10\x02\"b\n\x10\x45nvInjectionMode\x12\x16\n\x12\x45NV_INJECT_UNKNOWN\x10\x00\x12\x17\n\x13\x45NV_INJECT_DISABLED\x10\x01\x12\x1d\n\x19\x45NV_INJECT_NON_SECRET_ENV\x10\x02\x42\x13\n\x0csource_oneof\x12\x03\xf8\x42\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
 
 
 _LOCALCONFIG = DESCRIPTOR.message_types_by_name['LocalConfig']
 _KUBERNETESCONFIG = DESCRIPTOR.message_types_by_name['KubernetesConfig']
 _KUBERNETESCONFIG_TYPE = _KUBERNETESCONFIG.enum_types_by_name['Type']
 _KUBERNETESCONFIG_ENVINJECTIONMODE = _KUBERNETESCONFIG.enum_types_by_name['EnvInjectionMode']
@@ -41,18 +41,20 @@
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
   _LOCALCONFIG.fields_by_name['path']._options = None
   _LOCALCONFIG.fields_by_name['path']._serialized_options = b'\372B\004r\002\020\001'
   _KUBERNETESCONFIG.oneofs_by_name['source_oneof']._options = None
   _KUBERNETESCONFIG.oneofs_by_name['source_oneof']._serialized_options = b'\370B\001'
+  _KUBERNETESCONFIG.fields_by_name['type']._options = None
+  _KUBERNETESCONFIG.fields_by_name['type']._serialized_options = b'\372B\005\202\001\002 \000'
   _KUBERNETESCONFIG.fields_by_name['inlined']._options = None
   _KUBERNETESCONFIG.fields_by_name['inlined']._serialized_options = b'\372B\004r\002\020\001'
   _LOCALCONFIG._serialized_start=99
   _LOCALCONFIG._serialized_end=135
   _KUBERNETESCONFIG._serialized_start=138
-  _KUBERNETESCONFIG._serialized_end=559
-  _KUBERNETESCONFIG_TYPE._serialized_start=388
-  _KUBERNETESCONFIG_TYPE._serialized_end=438
-  _KUBERNETESCONFIG_ENVINJECTIONMODE._serialized_start=440
-  _KUBERNETESCONFIG_ENVINJECTIONMODE._serialized_end=538
+  _KUBERNETESCONFIG._serialized_end=569
+  _KUBERNETESCONFIG_TYPE._serialized_start=398
+  _KUBERNETESCONFIG_TYPE._serialized_end=448
+  _KUBERNETESCONFIG_ENVINJECTIONMODE._serialized_start=450
+  _KUBERNETESCONFIG_ENVINJECTIONMODE._serialized_end=548
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/links_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/links_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/links_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/maturity_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/maturity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/maturity_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/maturity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/meta_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/meta_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/notification_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/notification_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/parameters_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/parameters_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/program_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/program_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/program_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/program_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/ref_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/ref_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/ref_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/ref_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/retry_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/retry_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/retry_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/retry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/task_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/task_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/common_config/task_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/common_config/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/config_file/config_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/config_file/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/config_file/config_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/config_file/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/writeback_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/config_writeback/writeback_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/delivery/delivery_config_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/delivery/delivery_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/config_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/object_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/desired_state/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/desired_state/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/entity_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/environment/clusters_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/environment/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/environment/clusters_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/environment/clusters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/environment/environment_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/events/events_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/events/events_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/events/events_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/events/events_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/events/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/events/types_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/events/types_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/events/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/insights/insights_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/insights/insights_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/insights/insights_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/insights/insights_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/managed_resource/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/metrics/metrics_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/metrics/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/metrics/metrics_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/metrics/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/object/meta_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/object/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/object/meta_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/object/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/organization/organization_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/organization/user_metadata_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/organization/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/pipelines/object_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/pipelines/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/pipelines/object_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/pipelines/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/pipelines/pipelines_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/pipelines/pipelines_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/protection/attachments_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/protection/attachments_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/protection/attachments_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/protection/attachments_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/protection/object_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/protection/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/protection/object_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/protection/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_config_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_config_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_reference_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_reference_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/object_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/release_channel/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/object_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/release_channel/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/repo/repo_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/repo/repo_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/repo/repo_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/repo/repo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/runtimes/features_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/runtimes/features_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/runtimes/features_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/runtimes/features_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/scm/types_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/scm/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/scm/types_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/scm/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/service/object_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/service/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/service/object_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/service/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/service/parameters_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/service/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/service/parameters_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/service/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/service/service_config_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/service/service_config_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 from prodvana.proto.prodvana.workflow import integration_config_pb2 as prodvana_dot_workflow_dot_integration__config__pb2
 from prodvana.proto.prodvana.service import parameters_pb2 as prodvana_dot_service_dot_parameters__pb2
 from prodvana.proto.prodvana.volumes import volumes_pb2 as prodvana_dot_volumes_dot_volumes__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/service/service_config.proto\x12\x10prodvana.service\x1a\x1egoogle/protobuf/duration.proto\x1a$prodvana/capability/capability.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a!prodvana/common_config/helm.proto\x1a%prodvana/common_config/maturity.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a prodvana/common_config/ref.proto\x1a\"prodvana/common_config/retry.proto\x1a!prodvana/common_config/task.proto\x1a\'prodvana/delivery/delivery_config.proto\x1a(prodvana/delivery_extension/config.proto\x1a.prodvana/protection/protection_reference.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a!prodvana/service/parameters.proto\x1a\x1eprodvana/volumes/volumes.proto\x1a\x17validate/validate.proto\"1\n\x0eReplicasConfig\x12\x0f\n\x05\x66ixed\x18\x01 \x01(\x05H\x00\x42\x0e\n\x0c\x63onfig_oneof\"\xaa\x02\n\x0eMetricAnalysis\x12J\n\x0csuccess_rate\x18\x02 \x01(\x0b\x32\x32.prodvana.service.MetricAnalysis.SuccessRateConfigH\x00\x12\x45\n\x0blatency_p95\x18\x03 \x01(\x0b\x32..prodvana.service.MetricAnalysis.LatencyConfigH\x00\x1a\x32\n\x11SuccessRateConfig\x12\x1d\n\x15min_threshold_percent\x18\x01 \x01(\x01\x1a?\n\rLatencyConfig\x12.\n\x0bmax_latency\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x10\n\x0e\x61nalysis_oneof\"\xb7\x02\n\x15ReleaseStrategyConfig\x12<\n\x19individual_stage_deadline\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1a\x61utomated_testing_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12:\n\x10metrics_analysis\x18\x03 \x03(\x0b\x32 .prodvana.service.MetricAnalysis\x12\x17\n\x0fmanual_approval\x18\x04 \x01(\x08\x12\x31\n\x0e\x63heck_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x66\x61ilure_threshold\x18\x06 \x01(\x05\"f\n\tTLSSecret\x12\x14\n\nraw_secret\x18\x03 \x01(\tH\x00\x12\x30\n\x06secret\x18\x04 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x11\n\ntls_secret\x12\x03\xf8\x42\x01\"\x81\x01\n\x0eTLSCertificate\x12\x37\n\x08tls_cert\x18\x01 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x36\n\x07tls_key\x18\x02 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"j\n\x0b\x43\x65rtificate\x12/\n\x03tls\x18\x01 \x01(\x0b\x32 .prodvana.service.TLSCertificateH\x00\x12\x16\n\x0c\x61ws_acm_cert\x18\x02 \x01(\tH\x00\x42\x12\n\x0b\x63\x65rtificate\x12\x03\xf8\x42\x01\"\xc4\x07\n\x17PerReleaseChannelConfig\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12&\n\x10\x63ustom_hostnames\x18\x02 \x03(\tB\x0c\xfa\x42\t\x92\x01\x06\"\x04r\x02h\x01\x12W\n\x08programs\x18\x05 \x03(\x0b\x32\x36.prodvana.common_config.PerReleaseChannelProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12+\n\x04\x63\x65rt\x18\x06 \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12:\n\x0f\x64\x65livery_config\x18\x07 \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x08 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\t \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x43\n\x0epre_push_tasks\x18\n \x03(\x0b\x32\x1c.prodvana.service.TaskConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12U\n\x13\x64\x65livery_extensions\x18\x12 \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x41\n\x10runtime_specific\x18\x0b \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x11 \x01(\t\x12\x45\n\x11runtime_extension\x18\r \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x0e \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x10 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x0f \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x0c\x10\rR\x0bprotections\",\n\x13\x43\x61pabilityReference\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x18\x43ompiledCapabilityConfig\x12\x39\n\ncapability\x18\x01 \x01(\x0b\x32%.prodvana.capability.CapabilityConfig\".\n\x10ProgramReference\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"6\n\rTaskReference\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"\xf1\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x0c\x62\x61se_program\x18\x02 \x01(\x0b\x32\".prodvana.service.ProgramReference\x12\x39\n\x0cretry_config\x18\x03 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12,\n\x03ref\x18\x04 \x01(\x0b\x32\x1f.prodvana.service.TaskReference\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xb9\x01\n\x17\x44\x65liveryExtensionConfig\x12G\n\x07inlined\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12\x42\n\tlifecycle\x18\x02 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycleB\x08\xfa\x42\x05\x82\x01\x02 \x00\x42\x11\n\ndefinition\x12\x03\xf8\x42\x01\"\x9c\x02\n\x15RuntimeSpecificConfig\x12@\n\x03k8s\x18\x01 \x01(\x0b\x32\x31.prodvana.service.RuntimeSpecificConfig.K8SConfigH\x00\x1a\xae\x01\n\tK8SConfig\x12\x66\n\x13service_annotations\x18\x01 \x03(\x0b\x32I.prodvana.service.RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry\x1a\x39\n\x17ServiceAnnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0eruntime_config\"Z\n\x16RuntimeExtensionConfig\x12@\n\x10parameter_values\x18\x01 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"&\n\x12\x41utoRollbackConfig\x12\x10\n\x08\x64isabled\x18\x01 \x01(\x08\"\xec\x01\n\x1fProtectionConvergenceAttachment\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12?\n\x03ref\x18\x02 \x01(\x0b\x32(.prodvana.protection.ProtectionReferenceB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12L\n\tlifecycle\x18\x03 \x03(\x0b\x32(.prodvana.protection.ProtectionLifecycleB\x0f\xfa\x42\x0c\x92\x01\t\x08\x01\"\x05\x8a\x01\x02\x10\x01\"\xad\r\n\rServiceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x13\n\x0b\x61pplication\x18\x14 \x01(\t\x12\x46\n\x08programs\x18\x02 \x03(\x0b\x32%.prodvana.common_config.ProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x41\n\x10release_strategy\x18\x05 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12U\n\x13per_release_channel\x18\t \x03(\x0b\x32).prodvana.service.PerReleaseChannelConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\x0c\x63\x61pabilities\x18\n \x03(\x0b\x32%.prodvana.service.CapabilityReferenceB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12:\n\x0f\x64\x65livery_config\x18\x0b \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0c \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\r \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x0e \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x0f \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1d \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12\x41\n\x10runtime_specific\x18\x10 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x1c \x01(\t\x12N\n\nparameters\x18\x15 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x42\n\x10parameter_values\x18\x16 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12\x34\n\x11progress_deadline\x18\x18 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x12 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x13 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x1b \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1a \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12M\n\x12parameters_autogen\x18\x17 \x01(\x0e\x32\x31.prodvana.service.ServiceConfig.ParametersAutogen\x12;\n\rauto_rollback\x18\x19 \x01(\x0b\x32$.prodvana.service.AutoRollbackConfig\"M\n\x11ParametersAutogen\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05IMAGE\x10\x02\x12\x16\n\x12IMAGE_AND_REPLICAS\x10\x03\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\x11\x10\x12R\x08\x65xternalR\x10image_repositoryR\x15\x63ontainer_registry_idR\x0bprotections\"\x91\r\n\x1d\x43ompiledServiceInstanceConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x12 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x32\n\x08maturity\x18\x05 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x41\n\x10release_strategy\x18\x06 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12\x18\n\x10\x63ustom_hostnames\x18\x07 \x03(\t\x12+\n\x04\x63\x65rt\x18\n \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12\x46\n\x07runtime\x18\x0b \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x1b \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12@\n\x0c\x63\x61pabilities\x18\x0c \x03(\x0b\x32*.prodvana.service.CompiledCapabilityConfig\x12:\n\x0f\x64\x65livery_config\x18\r \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0e \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\x0f \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x10 \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x11 \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1e \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12\x41\n\x10runtime_specific\x18\x13 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12?\n\nparameters\x18\x18 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x19 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x34\n\x11progress_deadline\x18\x1a \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x16 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x17 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1d \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12n\n\x03\x65nv\x18\x1c \x03(\x0b\x32\x38.prodvana.service.CompiledServiceInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16R\x0bprotectionsR\x0cruntime_type\"\x88\x02\n\x11\x43ompiledJobConfig\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x46\n\x07runtime\x18\x04 \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x05 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/service/service_config.proto\x12\x10prodvana.service\x1a\x1egoogle/protobuf/duration.proto\x1a$prodvana/capability/capability.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a!prodvana/common_config/helm.proto\x1a%prodvana/common_config/maturity.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a prodvana/common_config/ref.proto\x1a\"prodvana/common_config/retry.proto\x1a!prodvana/common_config/task.proto\x1a\'prodvana/delivery/delivery_config.proto\x1a(prodvana/delivery_extension/config.proto\x1a.prodvana/protection/protection_reference.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a!prodvana/service/parameters.proto\x1a\x1eprodvana/volumes/volumes.proto\x1a\x17validate/validate.proto\"1\n\x0eReplicasConfig\x12\x0f\n\x05\x66ixed\x18\x01 \x01(\x05H\x00\x42\x0e\n\x0c\x63onfig_oneof\"\xaa\x02\n\x0eMetricAnalysis\x12J\n\x0csuccess_rate\x18\x02 \x01(\x0b\x32\x32.prodvana.service.MetricAnalysis.SuccessRateConfigH\x00\x12\x45\n\x0blatency_p95\x18\x03 \x01(\x0b\x32..prodvana.service.MetricAnalysis.LatencyConfigH\x00\x1a\x32\n\x11SuccessRateConfig\x12\x1d\n\x15min_threshold_percent\x18\x01 \x01(\x01\x1a?\n\rLatencyConfig\x12.\n\x0bmax_latency\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x10\n\x0e\x61nalysis_oneof\"\xb7\x02\n\x15ReleaseStrategyConfig\x12<\n\x19individual_stage_deadline\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1a\x61utomated_testing_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12:\n\x10metrics_analysis\x18\x03 \x03(\x0b\x32 .prodvana.service.MetricAnalysis\x12\x17\n\x0fmanual_approval\x18\x04 \x01(\x08\x12\x31\n\x0e\x63heck_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x66\x61ilure_threshold\x18\x06 \x01(\x05\"f\n\tTLSSecret\x12\x14\n\nraw_secret\x18\x03 \x01(\tH\x00\x12\x30\n\x06secret\x18\x04 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x11\n\ntls_secret\x12\x03\xf8\x42\x01\"\x81\x01\n\x0eTLSCertificate\x12\x37\n\x08tls_cert\x18\x01 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x36\n\x07tls_key\x18\x02 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"j\n\x0b\x43\x65rtificate\x12/\n\x03tls\x18\x01 \x01(\x0b\x32 .prodvana.service.TLSCertificateH\x00\x12\x16\n\x0c\x61ws_acm_cert\x18\x02 \x01(\tH\x00\x42\x12\n\x0b\x63\x65rtificate\x12\x03\xf8\x42\x01\"\xc4\x07\n\x17PerReleaseChannelConfig\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12&\n\x10\x63ustom_hostnames\x18\x02 \x03(\tB\x0c\xfa\x42\t\x92\x01\x06\"\x04r\x02h\x01\x12W\n\x08programs\x18\x05 \x03(\x0b\x32\x36.prodvana.common_config.PerReleaseChannelProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12+\n\x04\x63\x65rt\x18\x06 \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12:\n\x0f\x64\x65livery_config\x18\x07 \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x08 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\t \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x43\n\x0epre_push_tasks\x18\n \x03(\x0b\x32\x1c.prodvana.service.TaskConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12U\n\x13\x64\x65livery_extensions\x18\x12 \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x41\n\x10runtime_specific\x18\x0b \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x11 \x01(\t\x12\x45\n\x11runtime_extension\x18\r \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x0e \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x10 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x0f \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x0c\x10\rR\x0bprotections\",\n\x13\x43\x61pabilityReference\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x18\x43ompiledCapabilityConfig\x12\x39\n\ncapability\x18\x01 \x01(\x0b\x32%.prodvana.capability.CapabilityConfig\".\n\x10ProgramReference\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"6\n\rTaskReference\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"\xf1\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x0c\x62\x61se_program\x18\x02 \x01(\x0b\x32\".prodvana.service.ProgramReference\x12\x39\n\x0cretry_config\x18\x03 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12,\n\x03ref\x18\x04 \x01(\x0b\x32\x1f.prodvana.service.TaskReference\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xbb\x01\n\x17\x44\x65liveryExtensionConfig\x12G\n\x07inlined\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12\x44\n\tlifecycle\x18\x02 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycleB\n\xfa\x42\x07\x82\x01\x04 \x00 \x01\x42\x11\n\ndefinition\x12\x03\xf8\x42\x01\"\x9c\x02\n\x15RuntimeSpecificConfig\x12@\n\x03k8s\x18\x01 \x01(\x0b\x32\x31.prodvana.service.RuntimeSpecificConfig.K8SConfigH\x00\x1a\xae\x01\n\tK8SConfig\x12\x66\n\x13service_annotations\x18\x01 \x03(\x0b\x32I.prodvana.service.RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry\x1a\x39\n\x17ServiceAnnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0eruntime_config\"Z\n\x16RuntimeExtensionConfig\x12@\n\x10parameter_values\x18\x01 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"&\n\x12\x41utoRollbackConfig\x12\x10\n\x08\x64isabled\x18\x01 \x01(\x08\"\xec\x01\n\x1fProtectionConvergenceAttachment\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12?\n\x03ref\x18\x02 \x01(\x0b\x32(.prodvana.protection.ProtectionReferenceB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12L\n\tlifecycle\x18\x03 \x03(\x0b\x32(.prodvana.protection.ProtectionLifecycleB\x0f\xfa\x42\x0c\x92\x01\t\x08\x01\"\x05\x8a\x01\x02\x10\x01\"\xad\r\n\rServiceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x13\n\x0b\x61pplication\x18\x14 \x01(\t\x12\x46\n\x08programs\x18\x02 \x03(\x0b\x32%.prodvana.common_config.ProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x41\n\x10release_strategy\x18\x05 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12U\n\x13per_release_channel\x18\t \x03(\x0b\x32).prodvana.service.PerReleaseChannelConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\x0c\x63\x61pabilities\x18\n \x03(\x0b\x32%.prodvana.service.CapabilityReferenceB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12:\n\x0f\x64\x65livery_config\x18\x0b \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0c \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\r \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x0e \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x0f \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1d \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12\x41\n\x10runtime_specific\x18\x10 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x1c \x01(\t\x12N\n\nparameters\x18\x15 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x42\n\x10parameter_values\x18\x16 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12\x34\n\x11progress_deadline\x18\x18 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x12 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x13 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x1b \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1a \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12M\n\x12parameters_autogen\x18\x17 \x01(\x0e\x32\x31.prodvana.service.ServiceConfig.ParametersAutogen\x12;\n\rauto_rollback\x18\x19 \x01(\x0b\x32$.prodvana.service.AutoRollbackConfig\"M\n\x11ParametersAutogen\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05IMAGE\x10\x02\x12\x16\n\x12IMAGE_AND_REPLICAS\x10\x03\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\x11\x10\x12R\x08\x65xternalR\x10image_repositoryR\x15\x63ontainer_registry_idR\x0bprotections\"\x91\r\n\x1d\x43ompiledServiceInstanceConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x12 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x32\n\x08maturity\x18\x05 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x41\n\x10release_strategy\x18\x06 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12\x18\n\x10\x63ustom_hostnames\x18\x07 \x03(\t\x12+\n\x04\x63\x65rt\x18\n \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12\x46\n\x07runtime\x18\x0b \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x1b \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12@\n\x0c\x63\x61pabilities\x18\x0c \x03(\x0b\x32*.prodvana.service.CompiledCapabilityConfig\x12:\n\x0f\x64\x65livery_config\x18\r \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0e \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\x0f \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x10 \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x11 \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1e \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12\x41\n\x10runtime_specific\x18\x13 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12?\n\nparameters\x18\x18 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x19 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x34\n\x11progress_deadline\x18\x1a \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x16 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x17 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1d \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12n\n\x03\x65nv\x18\x1c \x03(\x0b\x32\x38.prodvana.service.CompiledServiceInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16R\x0bprotectionsR\x0cruntime_type\"\x88\x02\n\x11\x43ompiledJobConfig\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x46\n\x07runtime\x18\x04 \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x05 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
 
 
 
 _REPLICASCONFIG = DESCRIPTOR.message_types_by_name['ReplicasConfig']
 _METRICANALYSIS = DESCRIPTOR.message_types_by_name['MetricAnalysis']
 _METRICANALYSIS_SUCCESSRATECONFIG = _METRICANALYSIS.nested_types_by_name['SuccessRateConfig']
 _METRICANALYSIS_LATENCYCONFIG = _METRICANALYSIS.nested_types_by_name['LatencyConfig']
@@ -283,15 +283,15 @@
   _TASKREFERENCE.oneofs_by_name['ref']._options = None
   _TASKREFERENCE.oneofs_by_name['ref']._serialized_options = b'\370B\001'
   _TASKCONFIG.fields_by_name['program']._options = None
   _TASKCONFIG.fields_by_name['program']._serialized_options = b'\372B\005\212\001\002\020\001'
   _DELIVERYEXTENSIONCONFIG.oneofs_by_name['definition']._options = None
   _DELIVERYEXTENSIONCONFIG.oneofs_by_name['definition']._serialized_options = b'\370B\001'
   _DELIVERYEXTENSIONCONFIG.fields_by_name['lifecycle']._options = None
-  _DELIVERYEXTENSIONCONFIG.fields_by_name['lifecycle']._serialized_options = b'\372B\005\202\001\002 \000'
+  _DELIVERYEXTENSIONCONFIG.fields_by_name['lifecycle']._serialized_options = b'\372B\007\202\001\004 \000 \001'
   _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._options = None
   _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_options = b'8\001'
   _PROTECTIONCONVERGENCEATTACHMENT.fields_by_name['name']._options = None
   _PROTECTIONCONVERGENCEATTACHMENT.fields_by_name['name']._serialized_options = b'\372B)r\'\020\000\030?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$'
   _PROTECTIONCONVERGENCEATTACHMENT.fields_by_name['ref']._options = None
   _PROTECTIONCONVERGENCEATTACHMENT.fields_by_name['ref']._serialized_options = b'\372B\005\212\001\002\020\001'
   _PROTECTIONCONVERGENCEATTACHMENT.fields_by_name['lifecycle']._options = None
@@ -341,31 +341,31 @@
   _TASKREFERENCE._serialized_start=2990
   _TASKREFERENCE._serialized_end=3044
   _TASKCONFIG._serialized_start=3047
   _TASKCONFIG._serialized_end=3288
   _PROTECTIONLINK._serialized_start=3290
   _PROTECTIONLINK._serialized_end=3402
   _DELIVERYEXTENSIONCONFIG._serialized_start=3405
-  _DELIVERYEXTENSIONCONFIG._serialized_end=3590
-  _RUNTIMESPECIFICCONFIG._serialized_start=3593
-  _RUNTIMESPECIFICCONFIG._serialized_end=3877
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_start=3685
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_end=3859
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_start=3802
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_end=3859
-  _RUNTIMEEXTENSIONCONFIG._serialized_start=3879
-  _RUNTIMEEXTENSIONCONFIG._serialized_end=3969
-  _AUTOROLLBACKCONFIG._serialized_start=3971
-  _AUTOROLLBACKCONFIG._serialized_end=4009
-  _PROTECTIONCONVERGENCEATTACHMENT._serialized_start=4012
-  _PROTECTIONCONVERGENCEATTACHMENT._serialized_end=4248
-  _SERVICECONFIG._serialized_start=4251
-  _SERVICECONFIG._serialized_end=5960
-  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_start=5779
-  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_end=5856
-  _COMPILEDSERVICEINSTANCECONFIG._serialized_start=5963
-  _COMPILEDSERVICEINSTANCECONFIG._serialized_end=7644
-  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_start=7501
-  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_end=7577
-  _COMPILEDJOBCONFIG._serialized_start=7647
-  _COMPILEDJOBCONFIG._serialized_end=7911
+  _DELIVERYEXTENSIONCONFIG._serialized_end=3592
+  _RUNTIMESPECIFICCONFIG._serialized_start=3595
+  _RUNTIMESPECIFICCONFIG._serialized_end=3879
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_start=3687
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_end=3861
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_start=3804
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_end=3861
+  _RUNTIMEEXTENSIONCONFIG._serialized_start=3881
+  _RUNTIMEEXTENSIONCONFIG._serialized_end=3971
+  _AUTOROLLBACKCONFIG._serialized_start=3973
+  _AUTOROLLBACKCONFIG._serialized_end=4011
+  _PROTECTIONCONVERGENCEATTACHMENT._serialized_start=4014
+  _PROTECTIONCONVERGENCEATTACHMENT._serialized_end=4250
+  _SERVICECONFIG._serialized_start=4253
+  _SERVICECONFIG._serialized_end=5962
+  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_start=5781
+  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_end=5858
+  _COMPILEDSERVICEINSTANCECONFIG._serialized_start=5965
+  _COMPILEDSERVICEINSTANCECONFIG._serialized_end=7646
+  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_start=7503
+  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_end=7579
+  _COMPILEDJOBCONFIG._serialized_start=7649
+  _COMPILEDJOBCONFIG._serialized_end=7913
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/service/service_config_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/service/service_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/service/service_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/service/service_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/service/user_metadata_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/service/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/service/user_metadata_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/service/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/settings/organization/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/settings/organization/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/stat/efficiency_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/stat/efficiency_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/stat/efficiency_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/stat/efficiency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/template/service_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/template/service_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/template/service_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/template/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/users/users_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/users/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/users/users_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/users/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/version/source_metadata_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/version/source_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/version/source_metadata_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/version/source_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/volumes/volumes_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/volumes/volumes_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/volumes/volumes_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/volumes/volumes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/workflow/integration_config_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/workflow/integration_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py` & `prodvana-0.1.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py` & `prodvana-0.1.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi` & `prodvana-0.1.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/validate/validate_pb2.py` & `prodvana-0.1.8/prodvana/proto/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/proto/validate/validate_pb2.pyi` & `prodvana-0.1.8/prodvana/proto/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/utils/desired_states.py` & `prodvana-0.1.8/prodvana/utils/desired_states.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/utils/service_config.py` & `prodvana-0.1.8/prodvana/utils/service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/prodvana/utils/tests/test_service_config.py` & `prodvana-0.1.8/prodvana/utils/tests/test_service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.7/pyproject.toml` & `prodvana-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodvana"
-version = "0.1.7"
+version = "0.1.8"
 description = "Prodvana's client libraries"
 readme = "README.md"
 authors = []
 homepage = "https://prodvana.io"
 documentation = "https://docs.prodvana.io"
 repository = "https://github.com/prodvana/prodvana-public"
 exclude = ["examples"]
```

### Comparing `prodvana-0.1.7/PKG-INFO` & `prodvana-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodvana
-Version: 0.1.7
+Version: 0.1.8
 Summary: Prodvana's client libraries
 Home-page: https://prodvana.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-api-python-client (>=2.58.0,<3.0)
```

