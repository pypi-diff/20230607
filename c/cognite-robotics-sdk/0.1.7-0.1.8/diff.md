# Comparing `tmp/cognite_robotics_sdk-0.1.7.tar.gz` & `tmp/cognite_robotics_sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_robotics_sdk-0.1.7.tar", max compression
+gzip compressed data, was "cognite_robotics_sdk-0.1.8.tar", max compression
```

## Comparing `cognite_robotics_sdk-0.1.7.tar` & `cognite_robotics_sdk-0.1.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1252 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/README.md
--rw-r--r--   0        0        0       74 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/__init__.py
--rw-r--r--   0        0        0     1190 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/config/config.py
--rw-r--r--   0        0        0      560 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/data_classes.py
--rw-r--r--   0        0        0       67 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/data_classes.py
--rw-r--r--   0        0        0    11878 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/data_uploader.py
--rw-r--r--   0        0        0     1662 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/data_uploader_task.py
--rw-r--r--   0        0        0    11669 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/helpers.py
--rw-r--r--   0        0        0     9034 2023-05-23 10:59:30.348037 cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/clients/robot_interface_client.py
--rw-r--r--   0        0        0     1505 2023-05-23 10:59:30.348037 cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/clients/web_interface_client.py
--rw-r--r--   0        0        0       62 2023-05-23 10:59:30.348037 cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/__init__.py
--rw-r--r--   0        0        0      821 2023-05-23 10:59:30.348037 cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/bearer_token_auth.py
--rw-r--r--   0        0        0      826 2023-05-23 10:59:30.348037 cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/channel.py
--rw-r--r--   0        0        0    10327 2023-05-23 10:59:30.348037 cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/messages.py
--rw-r--r--   0        0        0        0 2023-05-23 11:12:39.124992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/__init__.py
--rw-r--r--   0        0        0     1453 2023-05-23 11:12:39.126992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/common_pb2.py
--rw-r--r--   0        0        0     1702 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/common_pb2.pyi
--rw-r--r--   0        0        0     2519 2023-05-23 11:12:39.126992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/connectivity_pb2.py
--rw-r--r--   0        0        0     6430 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/connectivity_pb2.pyi
--rw-r--r--   0        0        0     3047 2023-05-23 11:12:39.127992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/control_authority_pb2.py
--rw-r--r--   0        0        0     7303 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/control_authority_pb2.pyi
--rw-r--r--   0        0        0     2302 2023-05-23 11:12:39.127992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/data_pb2.py
--rw-r--r--   0        0        0     4811 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/data_pb2.pyi
--rw-r--r--   0        0        0     3228 2023-05-23 11:12:39.127992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/geometry_pb2.py
--rw-r--r--   0        0        0     8503 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/geometry_pb2.pyi
--rw-r--r--   0        0        0     1444 2023-05-23 11:12:39.127992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/joint_state_pb2.py
--rw-r--r--   0        0        0     1705 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/joint_state_pb2.pyi
--rw-r--r--   0        0        0     2590 2023-05-23 11:12:39.127992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_event_pb2.py
--rw-r--r--   0        0        0     5930 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_event_pb2.pyi
--rw-r--r--   0        0        0     1842 2023-05-23 11:12:39.127992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_log_pb2.py
--rw-r--r--   0        0        0     2460 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_log_pb2.pyi
--rw-r--r--   0        0        0     2384 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_pb2.py
--rw-r--r--   0        0        0     5977 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_pb2.pyi
--rw-r--r--   0        0        0     1461 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/payloads_pb2.py
--rw-r--r--   0        0        0     1805 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/payloads_pb2.pyi
--rw-r--r--   0        0        0     8330 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_control_pb2.py
--rw-r--r--   0        0        0    23660 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_control_pb2.pyi
--rw-r--r--   0        0        0     2549 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_registration_pb2.py
--rw-r--r--   0        0        0     4966 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_registration_pb2.pyi
--rw-r--r--   0        0        0     4899 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_state_pb2.py
--rw-r--r--   0        0        0    12598 2023-05-23 11:12:39.107991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_state_pb2.pyi
--rw-r--r--   0        0        0     4507 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/video_pb2.py
--rw-r--r--   0        0        0    15277 2023-05-23 11:12:39.107991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/video_pb2.pyi
--rw-r--r--   0        0        0     1597 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/web_pb2.py
--rw-r--r--   0        0        0     2003 2023-05-23 11:12:39.107991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/web_pb2.pyi
--rw-r--r--   0        0        0     2845 2023-05-23 11:12:39.129993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/robot_interface_pb2.py
--rw-r--r--   0        0        0      165 2023-05-23 11:12:39.107991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/robot_interface_pb2.pyi
--rw-r--r--   0        0        0    15062 2023-05-23 11:12:39.129993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/robot_interface_pb2_grpc.py
--rw-r--r--   0        0        0     2853 2023-05-23 11:12:39.129993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/web_interface_pb2.py
--rw-r--r--   0        0        0      165 2023-05-23 11:12:39.107991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/web_interface_pb2.pyi
--rw-r--r--   0        0        0    14820 2023-05-23 11:12:39.129993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/web_interface_pb2_grpc.py
--rw-r--r--   0        0        0       60 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/rest/__init__.py
--rw-r--r--   0        0        0      943 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/rest/base_model.py
--rw-r--r--   0        0        0       64 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/rest/client.py
--rw-r--r--   0        0        0    50682 2023-05-23 11:12:41.111128 cognite_robotics_sdk-0.1.7/cognite_robotics/rest/models.py
--rw-r--r--   0        0        0       58 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/utils/__init__.py
--rw-r--r--   0        0        0      645 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/utils/env_utils.py
--rw-r--r--   0        0        0     3016 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/utils/token.py
--rw-r--r--   0        0        0     3865 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/utils/utils.py
--rw-r--r--   0        0        0     1462 2023-05-23 10:59:30.351037 cognite_robotics_sdk-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 cognite_robotics_sdk-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1252 2023-06-07 07:10:51.050380 cognite_robotics_sdk-0.1.8/README.md
+-rw-r--r--   0        0        0       74 2023-06-07 07:10:51.050380 cognite_robotics_sdk-0.1.8/cognite_robotics/__init__.py
+-rw-r--r--   0        0        0     1190 2023-06-07 07:10:51.050380 cognite_robotics_sdk-0.1.8/cognite_robotics/config/config.py
+-rw-r--r--   0        0        0      560 2023-06-07 07:10:51.050380 cognite_robotics_sdk-0.1.8/cognite_robotics/data_classes.py
+-rw-r--r--   0        0        0       67 2023-06-07 07:10:51.050380 cognite_robotics_sdk-0.1.8/cognite_robotics/data_uploader/__init__.py
+-rw-r--r--   0        0        0     2903 2023-06-07 07:10:51.050380 cognite_robotics_sdk-0.1.8/cognite_robotics/data_uploader/data_classes.py
+-rw-r--r--   0        0        0    11901 2023-06-07 07:10:51.050380 cognite_robotics_sdk-0.1.8/cognite_robotics/data_uploader/data_uploader.py
+-rw-r--r--   0        0        0     1662 2023-06-07 07:10:51.050380 cognite_robotics_sdk-0.1.8/cognite_robotics/data_uploader/data_uploader_task.py
+-rw-r--r--   0        0        0    16466 2023-06-07 07:10:51.050380 cognite_robotics_sdk-0.1.8/cognite_robotics/data_uploader/helpers.py
+-rw-r--r--   0        0        0     9034 2023-06-07 07:10:51.050380 cognite_robotics_sdk-0.1.8/cognite_robotics/grpc/clients/robot_interface_client.py
+-rw-r--r--   0        0        0     1505 2023-06-07 07:10:51.050380 cognite_robotics_sdk-0.1.8/cognite_robotics/grpc/clients/web_interface_client.py
+-rw-r--r--   0        0        0       62 2023-06-07 07:10:51.051380 cognite_robotics_sdk-0.1.8/cognite_robotics/grpc/helpers/__init__.py
+-rw-r--r--   0        0        0      821 2023-06-07 07:10:51.051380 cognite_robotics_sdk-0.1.8/cognite_robotics/grpc/helpers/bearer_token_auth.py
+-rw-r--r--   0        0        0      826 2023-06-07 07:10:51.051380 cognite_robotics_sdk-0.1.8/cognite_robotics/grpc/helpers/channel.py
+-rw-r--r--   0        0        0    10327 2023-06-07 07:10:51.051380 cognite_robotics_sdk-0.1.8/cognite_robotics/grpc/helpers/messages.py
+-rw-r--r--   0        0        0        0 2023-06-07 07:25:21.926252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/__init__.py
+-rw-r--r--   0        0        0     1453 2023-06-07 07:25:21.928252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/common_pb2.py
+-rw-r--r--   0        0        0     1702 2023-06-07 07:25:21.908251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/common_pb2.pyi
+-rw-r--r--   0        0        0     2519 2023-06-07 07:25:21.928252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/connectivity_pb2.py
+-rw-r--r--   0        0        0     6430 2023-06-07 07:25:21.908251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/connectivity_pb2.pyi
+-rw-r--r--   0        0        0     3047 2023-06-07 07:25:21.928252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/control_authority_pb2.py
+-rw-r--r--   0        0        0     7303 2023-06-07 07:25:21.908251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/control_authority_pb2.pyi
+-rw-r--r--   0        0        0     2302 2023-06-07 07:25:21.929252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/data_pb2.py
+-rw-r--r--   0        0        0     4811 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/data_pb2.pyi
+-rw-r--r--   0        0        0     3228 2023-06-07 07:25:21.929252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/geometry_pb2.py
+-rw-r--r--   0        0        0     8503 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/geometry_pb2.pyi
+-rw-r--r--   0        0        0     1444 2023-06-07 07:25:21.929252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/joint_state_pb2.py
+-rw-r--r--   0        0        0     1705 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/joint_state_pb2.pyi
+-rw-r--r--   0        0        0     2590 2023-06-07 07:25:21.929252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/mission_event_pb2.py
+-rw-r--r--   0        0        0     5930 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/mission_event_pb2.pyi
+-rw-r--r--   0        0        0     1842 2023-06-07 07:25:21.929252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/mission_log_pb2.py
+-rw-r--r--   0        0        0     2460 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/mission_log_pb2.pyi
+-rw-r--r--   0        0        0     2384 2023-06-07 07:25:21.929252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/mission_pb2.py
+-rw-r--r--   0        0        0     5977 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/mission_pb2.pyi
+-rw-r--r--   0        0        0     1461 2023-06-07 07:25:21.930252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/payloads_pb2.py
+-rw-r--r--   0        0        0     1805 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/payloads_pb2.pyi
+-rw-r--r--   0        0        0     8330 2023-06-07 07:25:21.930252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/robot_control_pb2.py
+-rw-r--r--   0        0        0    23660 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/robot_control_pb2.pyi
+-rw-r--r--   0        0        0     2549 2023-06-07 07:25:21.930252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/robot_registration_pb2.py
+-rw-r--r--   0        0        0     4966 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/robot_registration_pb2.pyi
+-rw-r--r--   0        0        0     4899 2023-06-07 07:25:21.930252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/robot_state_pb2.py
+-rw-r--r--   0        0        0    12598 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/robot_state_pb2.pyi
+-rw-r--r--   0        0        0     4206 2023-06-07 07:25:21.930252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/video_pb2.py
+-rw-r--r--   0        0        0    14069 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/video_pb2.pyi
+-rw-r--r--   0        0        0     1597 2023-06-07 07:25:21.930252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/web_pb2.py
+-rw-r--r--   0        0        0     2003 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/web_pb2.pyi
+-rw-r--r--   0        0        0     2845 2023-06-07 07:25:21.931252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/services/robot_interface_pb2.py
+-rw-r--r--   0        0        0      165 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/services/robot_interface_pb2.pyi
+-rw-r--r--   0        0        0    15062 2023-06-07 07:25:21.931252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/services/robot_interface_pb2_grpc.py
+-rw-r--r--   0        0        0     2853 2023-06-07 07:25:21.931252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/services/web_interface_pb2.py
+-rw-r--r--   0        0        0      165 2023-06-07 07:25:21.909251 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/services/web_interface_pb2.pyi
+-rw-r--r--   0        0        0    14820 2023-06-07 07:25:21.931252 cognite_robotics_sdk-0.1.8/cognite_robotics/protos/services/web_interface_pb2_grpc.py
+-rw-r--r--   0        0        0       60 2023-06-07 07:10:51.053380 cognite_robotics_sdk-0.1.8/cognite_robotics/rest/__init__.py
+-rw-r--r--   0        0        0      943 2023-06-07 07:10:51.053380 cognite_robotics_sdk-0.1.8/cognite_robotics/rest/base_model.py
+-rw-r--r--   0        0        0       64 2023-06-07 07:10:51.053380 cognite_robotics_sdk-0.1.8/cognite_robotics/rest/client.py
+-rw-r--r--   0        0        0    50682 2023-06-07 07:25:23.718371 cognite_robotics_sdk-0.1.8/cognite_robotics/rest/models.py
+-rw-r--r--   0        0        0       58 2023-06-07 07:10:51.053380 cognite_robotics_sdk-0.1.8/cognite_robotics/utils/__init__.py
+-rw-r--r--   0        0        0      645 2023-06-07 07:10:51.053380 cognite_robotics_sdk-0.1.8/cognite_robotics/utils/env_utils.py
+-rw-r--r--   0        0        0     3016 2023-06-07 07:10:51.053380 cognite_robotics_sdk-0.1.8/cognite_robotics/utils/token.py
+-rw-r--r--   0        0        0     3865 2023-06-07 07:10:51.053380 cognite_robotics_sdk-0.1.8/cognite_robotics/utils/utils.py
+-rw-r--r--   0        0        0     1464 2023-06-07 07:10:51.054380 cognite_robotics_sdk-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 cognite_robotics_sdk-0.1.8/PKG-INFO
```

### Comparing `cognite_robotics_sdk-0.1.7/README.md` & `cognite_robotics_sdk-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/config/config.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/config/config.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/data_classes.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/data_classes.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/data_uploader/data_classes.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,41 +45,42 @@
 
     @property
     def error_data_path(self) -> str:
         """Return the error data path."""
         return self._error_data_path
 
 
+class UploadError(BaseModel):
+    """Upload error dataclass."""
+
+    message: str
+    exception: Optional[str] = None
+
+
 class BaseUploadRequest(BaseModel):
     """Upload request base dataclass."""
 
-    name: str
     mission_run_id: str
-    mission_id: str
     action_run_id: str
-    timestamp_ms: int
+    mission_id: Optional[str] = None
+    action_id: Optional[str] = None
+    timestamp_ms: Optional[int] = None
     data_set_id: Optional[int] = None
-    upload_instructions: Optional[JSONRPCRequest] = None
     data_postprocessing_input: Optional[JSONRPCRequest] = None
     asset_ids: Optional[List[int]] = None
-    cdf_metadata: Optional[Dict[str, Any]] = None
-    upload_succeeded: Optional[bool] = None
-    upload_error: Optional[str] = None
-
-    def update_file_metadata(self, metadata: Dict[str, Any]) -> None:
-        """Update the file metadata."""
-        metadata = self.cdf_metadata or {}
-        self.cdf_metadata = metadata.update(metadata)
+    asset_external_ids: Optional[List[str]] = None
+    error: Optional[UploadError] = None
 
 
 class FileUploadRequest(BaseUploadRequest):
     """File upload request dataclass."""
 
     file_path: str
     external_id: str
+    file_metadata: Optional[Dict[str, Any]] = None
 
 
 class Datapoint(BaseModel):
     """Data point dataclass, mirrors the Cognite datapoint."""
 
     timestamp: int
     value: Union[float, str]
@@ -87,18 +88,14 @@
 
 class DatapointsUploadRequest(BaseUploadRequest):
     """Data point upload request dataclass."""
 
     datapoints: List[Datapoint]
     timeseries_external_id: str
 
-    def update_datapoints(self, new_datapoints: Datapoint) -> None:
-        """Update datapoints."""
-        self.datapoints.append(new_datapoints)
-
 
 class UploadRequestParseError(Exception):
     """Upload request parse error."""
 
     def __init__(self, json_data: Dict[str, Any]) -> None:
         """Initialize the upload request parse error."""
         super().__init__(f"Error parsing upload request: {json_data}")
```

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/data_uploader.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/data_uploader/data_uploader.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import aiofiles
 import aiofiles.os
 import grpc
 from cognite.client import CogniteClient
 from cognite.client.exceptions import CogniteConnectionError
 
-from cognite_robotics.data_uploader.data_classes import DatapointsUploadRequest, DataUploaderConfig, FileUploadRequest
+from cognite_robotics.data_uploader.data_classes import DatapointsUploadRequest, DataUploaderConfig, FileUploadRequest, UploadError
 from cognite_robotics.data_uploader.helpers import (
     cleanup_upload_data_folder,
     create_data_upload_error_message,
     create_data_upload_event_message,
     flatten_dict,
     get_upload_request_from_json,
     move_files,
@@ -40,58 +40,58 @@
     data_upload_event_queue: "asyncio.Queue[data_pb2.DataUploadEvent]",
     cognite_client: CogniteClient,
     data_set_id: int,
     config: DataUploaderConfig,
     loop_time_step_s: float = 1.0,
 ) -> None:
     """Upload data to CDF and notify Robotics Services."""
+    data_error_path = config.error_data_path
+    if not os.path.exists(data_error_path):
+        os.makedirs(data_error_path, exist_ok=True)
+    data_upload_path = config.upload_data_path
+    if not os.path.exists(data_upload_path):
+        logger.warning(f"Data upload path does not exist, creating: `{data_upload_path}`.")
+        os.makedirs(data_upload_path, exist_ok=True)
+
     while not stop_task_trigger.is_set():
         logger.info("Starting data uploader.")
         try:
-            data_error_path = config.error_data_path
-            if not os.path.exists(data_error_path):
-                os.makedirs(data_error_path, exist_ok=True)
-            data_upload_path = config.upload_data_path
-            if not os.path.exists(data_upload_path):
-                logger.warning(f"Data upload path does not exist, creating: `{data_upload_path}`.")
-                os.makedirs(data_upload_path, exist_ok=True)
-
             logger.debug("Cleaning up upload data folder.")
             await cleanup_upload_data_folder(config.upload_data_path)
 
             while not stop_task_trigger.is_set():
                 loop_start_time = time.perf_counter_ns()
                 for json_file in glob.glob(os.path.join(config.upload_data_path, "*.json")):
                     if stop_task_trigger.is_set():
                         break
 
-                    file_basename, _ = os.path.splitext(os.path.basename(json_file))
-                    all_files_same_name = glob.glob(os.path.join(config.upload_data_path, f"{file_basename}.*"))
+                    file_root_name, _ = os.path.splitext(os.path.basename(json_file))
+                    all_files_same_name = glob.glob(os.path.join(config.upload_data_path, f"{file_root_name}.*"))
 
-                    logger.info(f"Upload request, file basename: `{file_basename}`.")
+                    logger.info(f"Upload request, file root name: `{file_root_name}`.")
                     try:
                         upload_request = await get_upload_request_from_json(json_file)
                     except Exception as e:
-                        logger.error(f"Error reading upload request file, skipping upload, files: `{file_basename}`.", exc_info=e)
+                        logger.error(f"Error reading upload request file, skipping upload, files: `{file_root_name}`.", exc_info=e)
                         await move_files(all_files_same_name, data_error_path)
                         continue
 
                     logger.info(
                         f"Uploading data to CDF, mission run: `{upload_request.mission_run_id}`, action: `{upload_request.action_run_id}`."
                     )
                     try:
                         data_upload_message = None
                         if isinstance(upload_request, FileUploadRequest):
-                            data_upload_message = await handle_upload_file(
+                            data_upload_message = await handle_file_upload_request(
                                 cognite_client=cognite_client,
                                 upload_request=upload_request,
                                 data_set_id=data_set_id,
                             )
                         elif isinstance(upload_request, DatapointsUploadRequest):
-                            data_upload_message = await handle_upload_timeseries(
+                            data_upload_message = await handle_datapoint_upload_request(
                                 cognite_client=cognite_client,
                                 upload_request=upload_request,
                             )
                     except (ConnectionError, CogniteConnectionError) as e:
                         logger.error(
                             f"Retrying upload in {config.retry_upload_interval_s} seconds.",
                             exc_info=e,
@@ -137,15 +137,15 @@
             await robot_interface_client.send_data_upload_event(data_upload_event)
         except grpc.RpcError as e:
             await handle_grpc_error(e, invoker="send_data_upload_event")
         except Exception as e:
             raise Exception("An unknown error occurred when sending data_upload_event, shutting down handler") from e
 
 
-async def handle_upload_file(
+async def handle_file_upload_request(
     cognite_client: CogniteClient,
     data_set_id: int,
     upload_request: FileUploadRequest,
 ) -> Optional[data_pb2.DataUploadEvent]:
     """Upload file to CDF."""
     file_path = upload_request.file_path
     if not os.path.exists(file_path):
@@ -163,33 +163,30 @@
             # await create_robot_log(
             #     message=message,
             #     severity=INFO,
             #     robot_status_queue=robot_status_queue,
             # )
             return None
 
-    cdf_metadata = upload_request.cdf_metadata
-    if cdf_metadata is not None:
-        cdf_metadata = flatten_dict(cdf_metadata)
-        cdf_metadata = {key: str(value) for key, value in cdf_metadata.items() if value not in (None, "", "None")}
+    file_metadata = upload_request.file_metadata
+    if file_metadata is not None:
+        file_metadata = flatten_dict(file_metadata)
+        file_metadata = {key: str(value) for key, value in file_metadata.items() if value not in (None, "", "None")}
     else:
-        cdf_metadata = {}
-
-    name = upload_request.name
-    external_id = upload_request.external_id
+        file_metadata = {}
 
     (mime_type, _) = mimetypes.guess_type(file_path)
 
     result = await asyncio.shield(
         to_thread(
             cognite_client.files.upload,
             file_path,
-            name=name,
-            external_id=external_id,
-            metadata=cdf_metadata,
+            name=os.path.basename(file_path),
+            external_id=upload_request.external_id,
+            metadata=file_metadata,
             data_set_id=data_set_id,
             mime_type=mime_type,  # type: ignore
         )
     )
 
     file_id = int(result.id)
     file_upload_message = data_pb2.FileUpload(file_id=file_id)
@@ -202,42 +199,41 @@
     #     message=f"File upload successful, file external_id: `{external_id}`.",
     #     severity=INFO,
     #     robot_status_queue=robot_status_queue,
     # )
     return data_upload_message
 
 
-async def handle_upload_timeseries(
+async def handle_datapoint_upload_request(
     cognite_client: CogniteClient,
     upload_request: DatapointsUploadRequest,
 ) -> data_pb2.DataUploadEvent:
     """Upload data to a timeseries."""
     timeseries_external_id = upload_request.timeseries_external_id
 
     def check_timeseries_exists() -> bool:
         return cognite_client.time_series.retrieve(external_id=timeseries_external_id) is None
 
     if not await to_thread(check_timeseries_exists):
         raise Exception(f"Timeseries does not exist, external_id: `{timeseries_external_id}`.")
 
     data_points = [datapoint.dict() for datapoint in upload_request.datapoints]
-    await asyncio.shield(
-        to_thread(cognite_client.time_series.data.insert, datapoints=data_points, external_id=timeseries_external_id)
-    )
+    await asyncio.shield(to_thread(cognite_client.time_series.data.insert, datapoints=data_points, external_id=timeseries_external_id))
     message = f"Datapoints upload successful, timeseries_external_id: `{timeseries_external_id}`."
     logger.info(message)
     # TODO: implement robot log client
     # await create_robot_log(
     #     message=message,
     #     severity=INFO,
     #     robot_status_queue=robot_status_queue,
     # )
     data_upload_message: data_pb2.DataUploadEvent = create_data_upload_event_message(upload_request)
     datapoint_upload_message = data_pb2.DataPointUpload(
-        timeseries_external_id=timeseries_external_id, timestamp=upload_request.timestamp_ms
+        timeseries_external_id=timeseries_external_id,
+        timestamp=upload_request.timestamp_ms if upload_request.timestamp_ms is not None else int(time.time() * 1000),
     )
     data_upload_message.data_point_upload.CopyFrom(datapoint_upload_message)
     return data_upload_message
 
 
 async def handle_failed_upload(
     json_file_path: str,
@@ -246,16 +242,15 @@
     error: Exception,
     data_error_path: str,
 ) -> data_pb2.DataUploadEvent:
     """Handle failed upload."""
     try:
         try:
             upload_request.mission_run_id
-            upload_request.upload_succeeded = False
-            upload_request.upload_error = str(error)
+            upload_request.error = UploadError(message="Failed data upload", exception=str(error))
             async with aiofiles.open(json_file_path, mode="w") as f:
                 await f.write(json.dumps(upload_request.dict()))
 
             if json_file_path not in all_files:
                 all_files.append(json_file_path)
         finally:
             try:
```

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/data_uploader_task.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/data_uploader/data_uploader_task.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/helpers.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/data_uploader/helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,180 +3,244 @@
 import asyncio
 import glob
 import json
 import logging
 import os
 import re
 import shutil
+import time
+import uuid
 from collections import defaultdict
 from typing import Any, Dict, List, MutableMapping, Optional, Union
 
 import aiofiles
 import aiofiles.os
 import pydantic
 
 from cognite_robotics.data_classes import JSONRPCRequest
 from cognite_robotics.data_uploader.data_classes import (
     Datapoint,
     DatapointsUploadRequest,
     DataUploaderConfig,
     FileUploadRequest,
+    UploadError,
     UploadRequestParseError,
 )
 from cognite_robotics.protos.messages import common_pb2, data_pb2
 from cognite_robotics.utils.utils import to_thread
 
 logger = logging.getLogger(__name__)
 
 
 async def create_file_upload_request(
     file_path: str,
-    data_type: str,
-    mission_id: str,
     mission_run_id: str,
     action_run_id: str,
-    data_capture_time: int,
-    filename_prefix: Optional[str],
     config: DataUploaderConfig,
-    data_set_id: int,
-    cdf_metadata: Dict[str, Any] = {},
+    mission_id: Optional[str] = None,
+    action_id: Optional[str] = None,
+    data_set_id: Optional[int] = None,
+    file_metadata: Optional[Dict[str, Any]] = None,
     asset_ids: Optional[List[int]] = None,
-    upload_instructions: Optional[JSONRPCRequest] = None,
+    asset_external_ids: Optional[List[str]] = None,
+    data_capture_time: Optional[int] = None,
     data_postprocessing_input: Optional[JSONRPCRequest] = None,
 ) -> None:
-    """Parse data for file upload."""
+    """Create a file upload request.
+
+    This is a helper function to create a file upload request. It copies the file to the upload data path and create a JSON metadata file.
+
+    Args:
+        file_path (str): Path to the file you wish to upload. The filename will be used as the external ID for the file in CDF, so make
+                sure it is unique (e.g., by adding a timestamp to the filename, data type). Preferably use an absolute path.
+        mission_run_id (str): ID for the specific run of the mission with `mission_id`. A typical example is: `mission_id`_`timestamp`.
+        action_run_id (str): ID for the specific execution of an action. For example, `infrared_image_capture_1234567910`.
+        mission_id (Optional[str]): External ID of the mission that is executed. Defaults to None.
+        action_id (Optional[str]): External ID of the action that the data is a result of (e.g., data capture) that is executed.
+                Defaults to None.
+        config (DataUploaderConfig): DataUploaderConfig object, containing the upload data path. Needs to be the same as the one
+                used in the DataUploader.
+        data_set_id (Optional[int], optional): ID of the CDF data set to which the data belongs to. Defaults to None.
+        file_metadata (Optional[Dict[str, Any]], optional): Metadata added to the uploaded file in CDF. Defaults to None.
+        asset_ids (Optional[List[int]], optional): List of asset ids. Defaults to None.
+        asset_external_ids (Optional[List[str]], optional): List of asset external ids. Defaults to None.
+        data_capture_time (Optional[int], optional): Data capture time. Elapsed time in milliseconds since January 1, 1970, 00:00:00 UTC.
+                Defaults to None.
+        data_postprocessing_input (Optional[JSONRPCRequest], optional): Instructions on how to postprocess the data after upload to CDF.
+                Defaults to None.
+
+    Raises:
+        FileNotFoundError: The file path does not exist.
+        IOError: You can only create upload requests per one file at a time.
+        exc_copy: Error copying the file to the upload data path.
+        exc_create_json: Error creating the JSON metadata file.
+    """
     if not os.path.exists(file_path):
         raise FileNotFoundError(f"File path does not exist: `{file_path}`.")
+    if not os.path.isfile(file_path):
+        raise IOError(f"File path is not a file: `{file_path}`.")
 
-    name = _create_cdf_filename(
-        filename_prefix=filename_prefix,
-        mission_run_id=mission_run_id,
-        action_run_id=action_run_id,
-        data_type=data_type,
-        timestamp=data_capture_time,
-    )
+    if data_capture_time is None:
+        data_capture_time = int(time.time() * 1000)
 
-    external_id = name
+    file_root_name, file_extension = os.path.splitext(os.path.basename(file_path))
+    if file_extension.lower() == ".jpeg":
+        os.rename(file_path, file_path.replace(".jpeg", ".jpg"))
+        file_extension = ".jpg"
 
     upload_data_path = config.upload_data_path
     if not os.path.exists(upload_data_path):
         os.makedirs(upload_data_path, exist_ok=True)
 
-    file_extension = os.path.splitext(file_path)[1]
-    if file_extension.lower() == ".jpeg":
-        os.rename(file_path, file_path.replace(".jpeg", ".jpg"))
-
-    upload_file_path = os.path.join(upload_data_path, name + file_extension)
-
-    cdf_metadata.update(
-        {
-            "mission_id": mission_id,
-            "mission_run_id": mission_run_id,
-            "action_run_id": action_run_id,
-        }
-    )
+    upload_file_path = os.path.join(upload_data_path, file_root_name + file_extension)
 
-    asset_id = asset_ids[0] if asset_ids is not None and len(asset_ids) > 0 else None
-    if asset_id is not None:
-        cdf_metadata.update({"asset_id": asset_id})
+    # add file metadata, used for data postprocessing and contextualization
+    if file_metadata is None:
+        file_metadata = {}
+    updates = {
+        "mission_id": mission_id,
+        "mission_run_id": mission_run_id,
+        "action_run_id": action_run_id,
+        "action_id": action_id,
+        "asset_id": asset_ids[0] if asset_ids is not None and len(asset_ids) > 0 else None,
+        "asset_external_id": asset_external_ids[0] if asset_external_ids is not None and len(asset_external_ids) > 0 else None,
+    }
+    for key, value in updates.items():
+        if value is not None:
+            file_metadata[key] = value
 
     upload_request = FileUploadRequest(
-        name=name,
+        external_id=file_root_name,
+        file_path=os.path.abspath(upload_file_path),
         mission_run_id=mission_run_id,
         mission_id=mission_id,
         action_run_id=action_run_id,
+        action_id=action_id,
         timestamp_ms=data_capture_time,
         data_set_id=data_set_id,
-        upload_instructions=upload_instructions,
         data_postprocessing_input=data_postprocessing_input,
         asset_ids=asset_ids,
-        cdf_metadata=cdf_metadata,
-        file_path=os.path.abspath(upload_file_path),
-        external_id=external_id,
+        asset_external_ids=asset_external_ids,
+        file_metadata=file_metadata,
     )
 
     try:
         await asyncio.shield(aiofiles.os.rename(file_path, upload_file_path))
-    except Exception as e:
-        logger.info("Failed to copy file to upload data path.")
-        # clean up of data file (if exists)
-        await remove_files([upload_file_path])
-        raise e
+    except Exception as exc_copy:
+        message = "Failed to copy file to upload data path."
+        logger.error(message)
+        try:
+            upload_request.error = UploadError(message=message, exception=str(exc_copy))
+            await move_files([upload_file_path], config.error_data_path)
+        except Exception as exc:
+            logger.error(f"Failed to move file to error data path. {exc}")
+        else:
+            await remove_files([upload_file_path])
+        raise exc_copy
 
     try:
-        await _create_upload_request_json(upload_request=upload_request, config=config)
-    except Exception as e:
-        logger.info("Failed to create upload request json.")
-        # clean up of both json and associated data files (if exists)
-        await remove_files(glob.glob(os.path.join(config.upload_data_path, f"{name}.*")))
-        raise e
+        await _create_upload_request_json(
+            upload_request=upload_request, raw_data_path=config.raw_data_path, upload_data_path=upload_data_path
+        )
+    except Exception as exc_create_json:
+        message = "Failed to create upload request JSON."
+        logger.error(message)
+        try:
+            upload_request.error = UploadError(message=message, exception=str(exc_create_json))
+            await move_files([upload_file_path], config.error_data_path)
+        except Exception as e:
+            logger.error(f"{message}: {e}")
+        finally:
+            # clean up of both json and associated data files (if exists)
+            await remove_files(glob.glob(os.path.join(config.upload_data_path, f"{file_root_name}.*")))
+        raise exc_create_json
 
 
 async def create_datapoints_upload_request(
-    measurements: List[Union[str, float]],
     timestamps: List[int],
-    data_type: str,
+    measurements: List[Union[str, float]],
     timeseries_external_id: str,
     mission_id: str,
     mission_run_id: str,
     action_run_id: str,
     config: DataUploaderConfig,
-    data_set_id: int,
-    cdf_metadata: Optional[Dict[str, Any]] = None,
+    data_set_id: Optional[int] = None,
     asset_ids: Optional[List[int]] = None,
-    upload_instructions: Optional[JSONRPCRequest] = None,
     data_postprocessing_input: Optional[JSONRPCRequest] = None,
 ) -> None:
-    """Process a measurement (float or string)."""
+    """Upload data points to a time series to Cognite Data Fusion.
+
+    Args:
+        timestamps (List[int]): List of measurement timestamps in milliseconds.
+                Elapsed time in milliseconds since January 1, 1970, 00:00:00 UTC
+        measurements (List[Union[str, float]]): List of measurement values. Must be either a float or a string.
+        timeseries_external_id (str): External ID of the time series in CDF.
+        mission_id (str): External ID of the mission that is executed.
+        mission_run_id (str): ID for the specific run of the mission with `mission_id`.
+        action_run_id (str): ID for the action execution.
+        config (DataUploaderConfig): DataUploaderConfig object, containing the upload data path. Needs to be the same as the one
+                used in the DataUploader.
+        data_set_id (Optional[int], optional): ID of the data set. Defaults to None.
+        cdf_metadata (Optional[Dict[str, Any]], optional): Metadata added to the timeseries in CDF. Defaults to None.
+        asset_ids (Optional[List[int]], optional): List of asset ids. Defaults to None.
+        data_postprocessing_input (Optional[JSONRPCRequest], optional): Instructions on how to postprocess the
+                data after upload to CDF. Defaults to None.
+
+    Raises:
+        ValueError: Number of measurements needs to be equal to number of timestamps.
+    """
     if len(measurements) == 0:
-        logger.info("No measurements to upload.")
+        logger.warn("No measurements to upload.")
         return
     if len(timestamps) == 1:
         timestamps = [timestamps[0]] * len(measurements)
     elif len(measurements) != len(timestamps):
         raise ValueError(f"Number of measurements ({len(measurements)}) and timestamps ({len(timestamps)}) must be equal.")
 
-    datapoints = [Datapoint(timestamp=timestamp, value=measurement) for timestamp, measurement in zip(timestamps, measurements)]
-
-    name = _create_cdf_filename(mission_run_id=mission_run_id, action_run_id=action_run_id, data_type=data_type, timestamp=timestamps[0])
+    datapoints = [Datapoint(timestamp=ts, value=value) for ts, value in zip(timestamps, measurements)]
 
     upload_request = DatapointsUploadRequest(
-        name=name,
         mission_id=mission_id,
         mission_run_id=mission_run_id,
         action_run_id=action_run_id,
         timestamp_ms=timestamps[0],
         data_set_id=data_set_id,
-        upload_instructions=upload_instructions,
         data_postprocessing_input=data_postprocessing_input,
         asset_ids=asset_ids,
-        cdf_metadata=cdf_metadata,
         datapoints=datapoints,
         timeseries_external_id=timeseries_external_id,
     )
 
-    await _create_upload_request_json(upload_request=upload_request, config=config)
+    try:
+        await _create_upload_request_json(
+            upload_request=upload_request, raw_data_path=config.raw_data_path, upload_data_path=config.upload_data_path
+        )
+    except Exception as exc_create_json:
+        logger.error(f"Failed to create upload request JSON. {exc_create_json}")
 
 
 async def _create_upload_request_json(
-    upload_request: Union[FileUploadRequest, DatapointsUploadRequest], config: DataUploaderConfig
+    upload_request: Union[FileUploadRequest, DatapointsUploadRequest], raw_data_path: str, upload_data_path: str
 ) -> None:
     """Create a JSON file containing the upload request data."""
 
     async def _create() -> None:
-        filename_json = upload_request.name + ".json"
-        file_path_raw = os.path.join(config.raw_data_path, filename_json)
+        if isinstance(upload_request, DatapointsUploadRequest):
+            filename_json = f"datapoint_upload_{uuid.uuid4()}.json"
+        else:
+            filename_json = f"{os.path.splitext(os.path.basename(upload_request.file_path))[0]}.json"
+        file_path_raw = os.path.join(raw_data_path, filename_json)
 
         try:
             async with aiofiles.open(file_path_raw, mode="w") as f:
                 await f.write(json.dumps(upload_request.dict(), indent=4))
         except Exception as e:
             raise e
 
-        os.rename(file_path_raw, os.path.join(config.upload_data_path, filename_json))
+        os.rename(file_path_raw, os.path.join(upload_data_path, filename_json))
 
     await asyncio.shield(_create())
 
 
 async def get_upload_request_from_json(upload_request_json_filename: str) -> Union[FileUploadRequest, DatapointsUploadRequest]:
     """Create UploadInfo from JSON file."""
     async with aiofiles.open(upload_request_json_filename) as json_file:
@@ -192,15 +256,15 @@
 
 
 def create_data_upload_event_message(upload_request: Union[FileUploadRequest, DatapointsUploadRequest]) -> data_pb2.DataUploadEvent:
     """Create data upload event message."""
     data_upload_message = data_pb2.DataUploadEvent(
         mission_report_id=upload_request.mission_run_id,
         action_report_id=upload_request.action_run_id,
-        data_capture_time=upload_request.timestamp_ms,
+        data_capture_time=upload_request.timestamp_ms if upload_request.timestamp_ms is not None else int(time.time() * 1000),
         data_postprocessing_input=json.dumps(upload_request.data_postprocessing_input.dict())
         if upload_request.data_postprocessing_input is not None
         else "",
     )
     if upload_request.asset_ids is not None:
         data_upload_message.asset_ids.extend(upload_request.asset_ids)
     return data_upload_message
@@ -214,27 +278,30 @@
     data_upload_message = create_data_upload_event_message(upload_request=upload_request)
     error_message = common_pb2.ErrorMessage(message=str(error))
     data_upload_message.error_message.CopyFrom(error_message)
     return data_upload_message
 
 
 def _create_cdf_filename(
-    mission_run_id: str, action_run_id: str, data_type: str, timestamp: int, filename_prefix: Optional[str] = None
+    mission_run_id: str, action_run_id: str, timestamp: int, filename_prefix: Optional[str] = None, data_type: Optional[str] = None
 ) -> str:
     """Create a name for the file to be uploaded."""
     if filename_prefix is not None:
-        name = "_".join([filename_prefix, data_type, mission_run_id, action_run_id])
+        name = "__".join([filename_prefix, mission_run_id, action_run_id])
     else:
-        name = "_".join([data_type, mission_run_id, action_run_id])
+        name = "__".join([mission_run_id, action_run_id])
+
+    if data_type is not None:
+        name = "__".join([name, data_type])
 
     # to avoid duplicate file names, append the data capture time to the end of the file name (if not already present)
     if re.search(r"\d+$", name) is None:
-        name = f"{name}_{timestamp}"
+        name = f"{name}__{timestamp}"
 
-    name = name.replace(".", "_")
+    name = name.replace(".", "__")
 
     return name
 
 
 async def remove_files(files: List[str]) -> None:
     """Remove files."""
```

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/clients/robot_interface_client.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/grpc/clients/robot_interface_client.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/clients/web_interface_client.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/grpc/clients/web_interface_client.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/bearer_token_auth.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/grpc/helpers/bearer_token_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/channel.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/grpc/helpers/channel.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/messages.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/grpc/helpers/messages.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/common_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/common_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/common_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/connectivity_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/connectivity_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/connectivity_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/connectivity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/control_authority_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/control_authority_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/control_authority_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/control_authority_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/data_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/data_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/data_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/geometry_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/geometry_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/geometry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/joint_state_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/joint_state_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/joint_state_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/joint_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_event_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/mission_event_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_event_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/mission_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_log_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/mission_log_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_log_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/mission_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/mission_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/mission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/payloads_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/payloads_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/payloads_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_control_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/robot_control_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_control_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/robot_control_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_registration_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/robot_registration_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_registration_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/robot_registration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_state_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/robot_state_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_state_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/robot_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/video_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/video_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14messages/video.proto\x12\x14\x63om.cognite.robotics\"\"\n\x10VideoComposition\x12\x0e\n\x06screen\x18\x01 \x01(\t\"8\n\x0e\x43\x61meraControls\x12\x11\n\tptz_go_to\x18\x01 \x01(\x08\x12\x13\n\x0bnavigate_to\x18\x02 \x01(\x08\"\xe4\x01\n\x12VideoConfiguration\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x11\n\tstream_id\x18\x02 \x01(\x03\x12\x0f\n\x07room_id\x18\x03 \x01(\x03\x12L\n\x1c\x61vailable_video_compositions\x18\x04 \x03(\x0b\x32&.com.cognite.robotics.VideoComposition\x12G\n\x19\x61vailable_camera_controls\x18\x05 \x01(\x0b\x32$.com.cognite.robotics.CameraControls\"\\\n\x0fLocalMediaTrack\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0c\n\x04kind\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x10\n\x08priority\x18\x05 \x01(\t\"\\\n\x10LocalMediaTracks\x12;\n\x0clocal_tracks\x18\x01 \x03(\x0b\x32%.com.cognite.robotics.LocalMediaTrack\x12\x0b\n\x03sdp\x18\x02 \x01(\t\"\x11\n\x0fMediaDisconnect\"\xb0\x01\n\x0eMediaPublisher\x12>\n\x0clocal_tracks\x18\x01 \x01(\x0b\x32&.com.cognite.robotics.LocalMediaTracksH\x00\x12\x13\n\theartbeat\x18\x02 \x01(\x03H\x00\x12\x41\n\x10media_disconnect\x18\x03 \x01(\x0b\x32%.com.cognite.robotics.MediaDisconnectH\x00\x42\x06\n\x04kind\"\x11\n\x0fMediaRenewToken\"\x86\x01\n\x0fMediaSubscriber\x12\x19\n\x11robot_data_set_id\x18\x01 \x01(\x03\x12\x13\n\theartbeat\x18\x02 \x01(\x03H\x00\x12;\n\nrenewToken\x18\x03 \x01(\x0b\x32%.com.cognite.robotics.MediaRenewTokenH\x00\x42\x06\n\x04kind\"\x8e\x01\n\x0cVideoRequest\x12\x39\n\tpublisher\x18\x01 \x01(\x0b\x32$.com.cognite.robotics.MediaPublisherH\x00\x12;\n\nsubscriber\x18\x02 \x01(\x0b\x32%.com.cognite.robotics.MediaSubscriberH\x00\x42\x06\n\x04kind\"<\n\x18TwilioConnectCredentials\x12\r\n\x05token\x18\x01 \x01(\t\x12\x11\n\troom_name\x18\x02 \x01(\t\"?\n\tIceServer\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x12\n\ncredential\x18\x03 \x01(\t\">\n\nIceServers\x12\x30\n\x07servers\x18\x01 \x03(\x0b\x32\x1f.com.cognite.robotics.IceServer\"\xca\x01\n\rVideoResponse\x12\x37\n\x0bice_servers\x18\x01 \x01(\x0b\x32 .com.cognite.robotics.IceServersH\x00\x12\r\n\x03sdp\x18\x02 \x01(\tH\x00\x12T\n\x1atwilio_connect_credentials\x18\x03 \x01(\x0b\x32..com.cognite.robotics.TwilioConnectCredentialsH\x00\x12\x13\n\theartbeat\x18\x04 \x01(\x03H\x00\x42\x06\n\x04kindB^Z\\github.com/cognite/robotics-services/integrations/go-webrtc-controller/pkg/robotics/messagesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14messages/video.proto\x12\x14\x63om.cognite.robotics\"\"\n\x10VideoComposition\x12\x0e\n\x06screen\x18\x01 \x01(\t\"8\n\x0e\x43\x61meraControls\x12\x11\n\tptz_go_to\x18\x01 \x01(\x08\x12\x13\n\x0bnavigate_to\x18\x02 \x01(\x08\"\xe4\x01\n\x12VideoConfiguration\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x11\n\tstream_id\x18\x02 \x01(\x03\x12\x0f\n\x07room_id\x18\x03 \x01(\x03\x12L\n\x1c\x61vailable_video_compositions\x18\x04 \x03(\x0b\x32&.com.cognite.robotics.VideoComposition\x12G\n\x19\x61vailable_camera_controls\x18\x05 \x01(\x0b\x32$.com.cognite.robotics.CameraControls\"\\\n\x0fLocalMediaTrack\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0c\n\x04kind\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x10\n\x08priority\x18\x05 \x01(\t\"\\\n\x10LocalMediaTracks\x12;\n\x0clocal_tracks\x18\x01 \x03(\x0b\x32%.com.cognite.robotics.LocalMediaTrack\x12\x0b\n\x03sdp\x18\x02 \x01(\t\"\x11\n\x0fMediaDisconnect\"\xb0\x01\n\x0eMediaPublisher\x12>\n\x0clocal_tracks\x18\x01 \x01(\x0b\x32&.com.cognite.robotics.LocalMediaTracksH\x00\x12\x13\n\theartbeat\x18\x02 \x01(\x03H\x00\x12\x41\n\x10media_disconnect\x18\x03 \x01(\x0b\x32%.com.cognite.robotics.MediaDisconnectH\x00\x42\x06\n\x04kind\",\n\x0fMediaSubscriber\x12\x19\n\x11robot_data_set_id\x18\x01 \x01(\x03\"\x8e\x01\n\x0cVideoRequest\x12\x39\n\tpublisher\x18\x01 \x01(\x0b\x32$.com.cognite.robotics.MediaPublisherH\x00\x12;\n\nsubscriber\x18\x02 \x01(\x0b\x32%.com.cognite.robotics.MediaSubscriberH\x00\x42\x06\n\x04kind\")\n\x18TwilioConnectCredentials\x12\r\n\x05token\x18\x01 \x01(\t\"?\n\tIceServer\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x12\n\ncredential\x18\x03 \x01(\t\">\n\nIceServers\x12\x30\n\x07servers\x18\x01 \x03(\x0b\x32\x1f.com.cognite.robotics.IceServer\"\xca\x01\n\rVideoResponse\x12\x37\n\x0bice_servers\x18\x01 \x01(\x0b\x32 .com.cognite.robotics.IceServersH\x00\x12\r\n\x03sdp\x18\x02 \x01(\tH\x00\x12T\n\x1atwilio_connect_credentials\x18\x03 \x01(\x0b\x32..com.cognite.robotics.TwilioConnectCredentialsH\x00\x12\x13\n\theartbeat\x18\x04 \x01(\x03H\x00\x42\x06\n\x04kindB^Z\\github.com/cognite/robotics-services/integrations/go-webrtc-controller/pkg/robotics/messagesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'messages.video_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\\github.com/cognite/robotics-services/integrations/go-webrtc-controller/pkg/robotics/messages'
@@ -31,22 +31,20 @@
   _LOCALMEDIATRACK._serialized_end=463
   _LOCALMEDIATRACKS._serialized_start=465
   _LOCALMEDIATRACKS._serialized_end=557
   _MEDIADISCONNECT._serialized_start=559
   _MEDIADISCONNECT._serialized_end=576
   _MEDIAPUBLISHER._serialized_start=579
   _MEDIAPUBLISHER._serialized_end=755
-  _MEDIARENEWTOKEN._serialized_start=757
-  _MEDIARENEWTOKEN._serialized_end=774
-  _MEDIASUBSCRIBER._serialized_start=777
-  _MEDIASUBSCRIBER._serialized_end=911
-  _VIDEOREQUEST._serialized_start=914
-  _VIDEOREQUEST._serialized_end=1056
-  _TWILIOCONNECTCREDENTIALS._serialized_start=1058
-  _TWILIOCONNECTCREDENTIALS._serialized_end=1118
-  _ICESERVER._serialized_start=1120
-  _ICESERVER._serialized_end=1183
-  _ICESERVERS._serialized_start=1185
-  _ICESERVERS._serialized_end=1247
-  _VIDEORESPONSE._serialized_start=1250
-  _VIDEORESPONSE._serialized_end=1452
+  _MEDIASUBSCRIBER._serialized_start=757
+  _MEDIASUBSCRIBER._serialized_end=801
+  _VIDEOREQUEST._serialized_start=804
+  _VIDEOREQUEST._serialized_end=946
+  _TWILIOCONNECTCREDENTIALS._serialized_start=948
+  _TWILIOCONNECTCREDENTIALS._serialized_end=989
+  _ICESERVER._serialized_start=991
+  _ICESERVER._serialized_end=1054
+  _ICESERVERS._serialized_start=1056
+  _ICESERVERS._serialized_end=1118
+  _VIDEORESPONSE._serialized_start=1121
+  _VIDEORESPONSE._serialized_end=1323
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/video_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/video_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -193,51 +193,28 @@
     def HasField(self, field_name: typing_extensions.Literal["heartbeat", b"heartbeat", "kind", b"kind", "local_tracks", b"local_tracks", "media_disconnect", b"media_disconnect"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["heartbeat", b"heartbeat", "kind", b"kind", "local_tracks", b"local_tracks", "media_disconnect", b"media_disconnect"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["kind", b"kind"]) -> typing_extensions.Literal["local_tracks", "heartbeat", "media_disconnect"] | None: ...
 
 global___MediaPublisher = MediaPublisher
 
 @typing_extensions.final
-class MediaRenewToken(google.protobuf.message.Message):
-    """/ Request a new access token from Twilio"""
-
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    def __init__(
-        self,
-    ) -> None: ...
-
-global___MediaRenewToken = MediaRenewToken
-
-@typing_extensions.final
 class MediaSubscriber(google.protobuf.message.Message):
     """/ Specify which robot media stream to subscribe to"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ROBOT_DATA_SET_ID_FIELD_NUMBER: builtins.int
-    HEARTBEAT_FIELD_NUMBER: builtins.int
-    RENEWTOKEN_FIELD_NUMBER: builtins.int
     robot_data_set_id: builtins.int
     """/ Robot dataset id of the robot we want to connect to"""
-    heartbeat: builtins.int
-    """Heartbeat forwarded to robot, keeps the video stream up"""
-    @property
-    def renewToken(self) -> global___MediaRenewToken:
-        """Request a twilio access token"""
     def __init__(
         self,
         *,
         robot_data_set_id: builtins.int = ...,
-        heartbeat: builtins.int = ...,
-        renewToken: global___MediaRenewToken | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["heartbeat", b"heartbeat", "kind", b"kind", "renewToken", b"renewToken"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["heartbeat", b"heartbeat", "kind", b"kind", "renewToken", b"renewToken", "robot_data_set_id", b"robot_data_set_id"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind", b"kind"]) -> typing_extensions.Literal["heartbeat", "renewToken"] | None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["robot_data_set_id", b"robot_data_set_id"]) -> None: ...
 
 global___MediaSubscriber = MediaSubscriber
 
 @typing_extensions.final
 class VideoRequest(google.protobuf.message.Message):
     """/ Specify your webrtc offer"""
 
@@ -268,26 +245,22 @@
     """/ If using the twilio-video.js sdk, the necessary session description
     / is deduced from the token and room name by the Twilio API
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOKEN_FIELD_NUMBER: builtins.int
-    ROOM_NAME_FIELD_NUMBER: builtins.int
     token: builtins.str
     """/ jwt auth token issued by the Cognite gRPC signaling service"""
-    room_name: builtins.str
-    """/ room name"""
     def __init__(
         self,
         *,
         token: builtins.str = ...,
-        room_name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["room_name", b"room_name", "token", b"token"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["token", b"token"]) -> None: ...
 
 global___TwilioConnectCredentials = TwilioConnectCredentials
 
 @typing_extensions.final
 class IceServer(google.protobuf.message.Message):
     """/ A media traversal candidate, i.e a potential network path between peers"""
```

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/web_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/web_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/web_pb2.pyi` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/messages/web_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/robot_interface_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/services/robot_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/robot_interface_pb2_grpc.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/services/robot_interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/web_interface_pb2.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/services/web_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/web_interface_pb2_grpc.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/protos/services/web_interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/rest/base_model.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/rest/base_model.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/rest/models.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/rest/models.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/utils/env_utils.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/utils/token.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/utils/token.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/cognite_robotics/utils/utils.py` & `cognite_robotics_sdk-0.1.8/cognite_robotics/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.7/pyproject.toml` & `cognite_robotics_sdk-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,42 +3,42 @@
 description = "Cognite Robotics SDK"
 name = "cognite-robotics-sdk"
 packages = [
     { include = "cognite_robotics", from = "." },
     { include = "protos", from = "cognite_robotics" },
 ]
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 aiofiles = ">=23.1.0"
 cognite-sdk = ">=6.0.0"
 grpcio = ">=1.54.0"
-protobuf = ">=4.22.3"
-pydantic = "1.10.7"
+protobuf = ">=4.23.0"
+pydantic = ">=1.10.7"
 python = "^3.8"
 python-dotenv = ">=0.21.1"
 
 [tool.poetry.dev-dependencies]
 black = "23.3.0"
 datamodel-code-generator = "0.19.0"
 mypy = "1.3.0"
 pre-commit = "3.3.2"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
-types-aiofiles = "23.1.0.1"
+types-aiofiles = "23.1.0.3"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.black]
 include = '\.py$'
 line-length = 140
-target_version = ['py39']
+target_version = ['py38']
 
 [tool.ruff]
 exclude = [
     ".git",
     ".mypy_cache",
     ".ruff_cache",
     "cognite_robotics/protos/",
```

### Comparing `cognite_robotics_sdk-0.1.7/PKG-INFO` & `cognite_robotics_sdk-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cognite-robotics-sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: Cognite Robotics SDK
 Author: Cognite Robotics
 Author-email: robotics-team@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0)
 Requires-Dist: cognite-sdk (>=6.0.0)
 Requires-Dist: grpcio (>=1.54.0)
-Requires-Dist: protobuf (>=4.22.3)
-Requires-Dist: pydantic (==1.10.7)
+Requires-Dist: protobuf (>=4.23.0)
+Requires-Dist: pydantic (>=1.10.7)
 Requires-Dist: python-dotenv (>=0.21.1)
 Description-Content-Type: text/markdown
 
 # Cognite Robotics SDK
 
 [![PyPI version](https://badge.fury.io/py/cognite-robotics-sdk.svg)](https://pypi.org/project/cognite-robotics-sdk/)
 [![mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
```

